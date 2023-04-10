# Comparing `tmp/balance-0.6.0.tar.gz` & `tmp/balance-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balance-0.6.0.tar", last modified: Wed Apr  5 12:48:14 2023, max compression
+gzip compressed data, was "balance-0.7.0.tar", last modified: Mon Apr 10 08:02:05 2023, max compression
```

## Comparing `balance-0.6.0.tar` & `balance-0.7.0.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.664798 balance-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-05 12:46:56.000000 balance-0.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.644798 balance-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.648798 balance-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-05 12:46:56.000000 balance-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-05 12:46:56.000000 balance-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.648798 balance-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-05 12:46:56.000000 balance-0.6.0/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-05 12:46:56.000000 balance-0.6.0/.github/workflows/deploy-website.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-05 12:46:56.000000 balance-0.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-05 12:46:56.000000 balance-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-04-05 12:46:56.000000 balance-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-05 12:46:56.000000 balance-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-05 12:46:56.000000 balance-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-04-05 12:46:56.000000 balance-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-04-05 12:46:56.000000 balance-0.6.0/LICENSE-DOCUMENTATION
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-05 12:48:14.664798 balance-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-05 12:46:56.000000 balance-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.648798 balance-0.6.0/balance/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-05 12:46:56.000000 balance-0.6.0/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-04-05 12:46:56.000000 balance-0.6.0/balance/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)    77610 2023-04-05 12:46:56.000000 balance-0.6.0/balance/balancedf_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    26001 2023-04-05 12:46:56.000000 balance-0.6.0/balance/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.652798 balance-0.6.0/balance/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-04-05 12:46:56.000000 balance-0.6.0/balance/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-05 12:46:56.000000 balance-0.6.0/balance/datasets/sim_data_cbps.R
--rw-r--r--   0 runner    (1001) docker     (123)    55895 2023-04-05 12:46:56.000000 balance-0.6.0/balance/datasets/sim_data_cbps.csv
--rw-r--r--   0 runner    (1001) docker     (123)    51298 2023-04-05 12:46:56.000000 balance-0.6.0/balance/sample_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.652798 balance-0.6.0/balance/stats_and_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-05 12:46:56.000000 balance-0.6.0/balance/stats_and_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-05 12:46:56.000000 balance-0.6.0/balance/stats_and_plots/general_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    50208 2023-04-05 12:46:56.000000 balance-0.6.0/balance/stats_and_plots/weighted_comparisons_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-04-05 12:46:56.000000 balance-0.6.0/balance/stats_and_plots/weighted_comparisons_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    26952 2023-04-05 12:46:56.000000 balance-0.6.0/balance/stats_and_plots/weighted_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-05 12:46:56.000000 balance-0.6.0/balance/stats_and_plots/weights_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-05 12:46:56.000000 balance-0.6.0/balance/testutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-05 12:46:56.000000 balance-0.6.0/balance/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-04-05 12:46:56.000000 balance-0.6.0/balance/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.652798 balance-0.6.0/balance/weighting_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-05 12:46:56.000000 balance-0.6.0/balance/weighting_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-05 12:46:56.000000 balance-0.6.0/balance/weighting_methods/adjust_null.py
--rw-r--r--   0 runner    (1001) docker     (123)    29253 2023-04-05 12:46:56.000000 balance-0.6.0/balance/weighting_methods/cbps.py
--rw-r--r--   0 runner    (1001) docker     (123)    26508 2023-04-05 12:46:56.000000 balance-0.6.0/balance/weighting_methods/ipw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-05 12:46:56.000000 balance-0.6.0/balance/weighting_methods/poststratify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.648798 balance-0.6.0/balance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-05 12:48:14.000000 balance-0.6.0/balance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-05 12:48:14.000000 balance-0.6.0/balance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 12:48:14.000000 balance-0.6.0/balance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-05 12:48:14.000000 balance-0.6.0/balance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 12:48:14.000000 balance-0.6.0/balance.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.652798 balance-0.6.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3373 2023-04-05 12:46:56.000000 balance-0.6.0/scripts/make_docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 12:48:14.664798 balance-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-05 12:46:56.000000 balance-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.652798 balance-0.6.0/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-05 12:46:56.000000 balance-0.6.0/sphinx/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.644798 balance-0.6.0/sphinx/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.652798 balance-0.6.0/sphinx/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-05 12:46:56.000000 balance-0.6.0/sphinx/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.644798 balance-0.6.0/sphinx/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.652798 balance-0.6.0/sphinx/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-05 12:46:56.000000 balance-0.6.0/sphinx/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-05 12:46:56.000000 balance-0.6.0/sphinx/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-05 12:46:56.000000 balance-0.6.0/sphinx/balance.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-05 12:46:56.000000 balance-0.6.0/sphinx/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-05 12:46:56.000000 balance-0.6.0/sphinx/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-05 12:46:56.000000 balance-0.6.0/sphinx/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.652798 balance-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_adjust_null.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)    43626 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_balancedf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19922 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_cbps.py
--rw-r--r--   0 runner    (1001) docker     (123)    38390 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_ipw.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_poststratify.py
--rw-r--r--   0 runner    (1001) docker     (123)    39114 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    32798 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_stats_and_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_testutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    48401 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-04-05 12:46:56.000000 balance-0.6.0/tests/test_weighted_comparisons_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.656798 balance-0.6.0/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-04-05 12:46:56.000000 balance-0.6.0/tutorials/balance_quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   590297 2023-04-05 12:46:56.000000 balance-0.6.0/tutorials/balance_quickstart_cbps.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31499 2023-04-05 12:46:56.000000 balance-0.6.0/tutorials/balance_transformations_and_formulas.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-05 12:46:56.000000 balance-0.6.0/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.656798 balance-0.6.0/website/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 12:46:56.000000 balance-0.6.0/website/.npmrc
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-05 12:46:56.000000 balance-0.6.0/website/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-05 12:46:56.000000 balance-0.6.0/website/babel.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.644798 balance-0.6.0/website/blog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.644798 balance-0.6.0/website/blog/2023/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.644798 balance-0.6.0/website/blog/2023/01/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.656798 balance-0.6.0/website/blog/2023/01/09/
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-05 12:46:56.000000 balance-0.6.0/website/blog/2023/01/09/bringing-balance-to-your-data.md
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-04-05 12:46:56.000000 balance-0.6.0/website/blog/2023/01/09/sample_vs_target_bar_chart.webp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.644798 balance-0.6.0/website/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.656798 balance-0.6.0/website/docs/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/api_reference/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.656798 balance-0.6.0/website/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.656798 balance-0.6.0/website/docs/docs/general_framework/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/general_framework/adjusting_sample_to_population.md
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/general_framework/evaluation_of_results.md
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/general_framework/general_framework.md
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/general_framework/pre_adjustment_diagnostics.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.660798 balance-0.6.0/website/docs/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    48494 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/fig_01_qqplot_income_before.png
--rw-r--r--   0 runner    (1001) docker     (123)    41572 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/fig_02_barplot_age_before.png
--rw-r--r--   0 runner    (1001) docker     (123)    38449 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/fig_03_barplot_gender_before.png
--rw-r--r--   0 runner    (1001) docker     (123)    61834 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/fig_04_qqplot_income_after.png
--rw-r--r--   0 runner    (1001) docker     (123)    45979 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/fig_05_barplot_age_after.png
--rw-r--r--   0 runner    (1001) docker     (123)    41950 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/fig_06_barplot_gender_after.png
--rw-r--r--   0 runner    (1001) docker     (123)    41877 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/fig_07_seaborn_after.png
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/fig_08_weights_kde.png
--rw-r--r--   0 runner    (1001) docker     (123)    28925 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/fig_09_seaborn_outcome_kde_after.png
--rw-r--r--   0 runner    (1001) docker     (123)   468436 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/total_survey_error_flow_v02.png
--rw-r--r--   0 runner    (1001) docker     (123)    26229 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/total_survey_error_flow_v02.svg
--rw-r--r--   0 runner    (1001) docker     (123)    68569 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/total_survey_error_image.png
--rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/img/total_survey_error_image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.660798 balance-0.6.0/website/docs/docs/statistical_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/statistical_methods/cbps.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/statistical_methods/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/statistical_methods/ipw.md
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/docs/statistical_methods/poststratify.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.660798 balance-0.6.0/website/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/tutorials/balance_transformations_and_formulas.mdx
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.mdx
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/tutorials/index.mdx
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/tutorials/quickstart.mdx
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-05 12:46:56.000000 balance-0.6.0/website/docs/tutorials/quickstart_cbps.mdx
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-04-05 12:46:56.000000 balance-0.6.0/website/docusaurus.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-05 12:46:56.000000 balance-0.6.0/website/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-05 12:46:56.000000 balance-0.6.0/website/sidebars.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.648798 balance-0.6.0/website/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.660798 balance-0.6.0/website/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-05 12:46:56.000000 balance-0.6.0/website/src/components/HTMLLoader.js
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-05 12:46:56.000000 balance-0.6.0/website/src/components/HomepageFeatures.js
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-05 12:46:56.000000 balance-0.6.0/website/src/components/HomepageFeatures.module.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.660798 balance-0.6.0/website/src/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-05 12:46:56.000000 balance-0.6.0/website/src/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.660798 balance-0.6.0/website/src/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-05 12:46:56.000000 balance-0.6.0/website/src/pages/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-05 12:46:56.000000 balance-0.6.0/website/src/pages/index.module.css
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-05 12:46:56.000000 balance-0.6.0/website/src/pages/markdown-page.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.660798 balance-0.6.0/website/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.660798 balance-0.6.0/website/static/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.660798 balance-0.6.0/website/static/img/balance_logo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.664798 balance-0.6.0/website/static/img/balance_logo/AI/
--rw-r--r--   0 runner    (1001) docker     (123)   460628 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/AI/balance_Logo_FINAL.ai
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.648798 balance-0.6.0/website/static/img/balance_logo/PNG/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.664798 balance-0.6.0/website/static/img/balance_logo/PNG/Horizontal/
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_Black_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_White_RGB.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.664798 balance-0.6.0/website/static/img/balance_logo/PNG/Icon/
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_Black_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_FullColor_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_White_RGB.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.664798 balance-0.6.0/website/static/img/balance_logo/PNG/Vertical/
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_Black_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_FullColor_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_White_RGB.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.648798 balance-0.6.0/website/static/img/balance_logo/SVG/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.664798 balance-0.6.0/website/static/img/balance_logo/SVG/Horizontal/
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_Black_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_White_RGB.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.664798 balance-0.6.0/website/static/img/balance_logo/SVG/Icon/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_Black_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_FullColor_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_White_RGB.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.664798 balance-0.6.0/website/static/img/balance_logo/SVG/Vertical/
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_Black_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_FullColor_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_White_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/vertical.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/balance_logo/vertical_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/docusaurus.png
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.664798 balance-0.6.0/website/static/img/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/fontawesome/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/fontawesome/layer-group.svg
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/fontawesome/users.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14679 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/meta_opensource_logo_negative.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:14.664798 balance-0.6.0/website/static/img/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/tutorial/docsVersionDropdown.png
--rw-r--r--   0 runner    (1001) docker     (123)    30020 2023-04-05 12:46:56.000000 balance-0.6.0/website/static/img/tutorial/localeDropdown.png
--rw-r--r--   0 runner    (1001) docker     (123)   537599 2023-04-05 12:46:56.000000 balance-0.6.0/website/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 08:00:29.000000 balance-0.7.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.188347 balance-0.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-10 08:00:29.000000 balance-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-10 08:00:29.000000 balance-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.188347 balance-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-10 08:00:29.000000 balance-0.7.0/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-10 08:00:29.000000 balance-0.7.0/.github/workflows/deploy-website.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-10 08:00:29.000000 balance-0.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-10 08:00:29.000000 balance-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-10 08:00:29.000000 balance-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-10 08:00:29.000000 balance-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-10 08:00:29.000000 balance-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-04-10 08:00:29.000000 balance-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-04-10 08:00:29.000000 balance-0.7.0/LICENSE-DOCUMENTATION
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-10 08:02:05.216347 balance-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-10 08:00:29.000000 balance-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.192347 balance-0.7.0/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-10 08:00:29.000000 balance-0.7.0/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-04-10 08:00:29.000000 balance-0.7.0/balance/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77711 2023-04-10 08:00:29.000000 balance-0.7.0/balance/balancedf_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26001 2023-04-10 08:00:29.000000 balance-0.7.0/balance/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.192347 balance-0.7.0/balance/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-04-10 08:00:29.000000 balance-0.7.0/balance/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-10 08:00:29.000000 balance-0.7.0/balance/datasets/sim_data_cbps.R
+-rw-r--r--   0 runner    (1001) docker     (123)    55895 2023-04-10 08:00:29.000000 balance-0.7.0/balance/datasets/sim_data_cbps.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    52104 2023-04-10 08:00:29.000000 balance-0.7.0/balance/sample_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.192347 balance-0.7.0/balance/stats_and_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/general_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59199 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/weighted_comparisons_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/weighted_comparisons_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26952 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/weighted_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/weights_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-10 08:00:29.000000 balance-0.7.0/balance/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-10 08:00:29.000000 balance-0.7.0/balance/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78678 2023-04-10 08:00:29.000000 balance-0.7.0/balance/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.196347 balance-0.7.0/balance/weighting_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 08:00:29.000000 balance-0.7.0/balance/weighting_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-10 08:00:29.000000 balance-0.7.0/balance/weighting_methods/adjust_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29249 2023-04-10 08:00:29.000000 balance-0.7.0/balance/weighting_methods/cbps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26505 2023-04-10 08:00:29.000000 balance-0.7.0/balance/weighting_methods/ipw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-10 08:00:29.000000 balance-0.7.0/balance/weighting_methods/poststratify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.192347 balance-0.7.0/balance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-10 08:02:04.000000 balance-0.7.0/balance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-10 08:02:05.000000 balance-0.7.0/balance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:02:04.000000 balance-0.7.0/balance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 08:02:04.000000 balance-0.7.0/balance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 08:02:04.000000 balance-0.7.0/balance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.196347 balance-0.7.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3373 2023-04-10 08:00:29.000000 balance-0.7.0/scripts/make_docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:02:05.216347 balance-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-10 08:00:29.000000 balance-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.196347 balance-0.7.0/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/sphinx/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.196347 balance-0.7.0/sphinx/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/sphinx/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.196347 balance-0.7.0/sphinx/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/balance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.200347 balance-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_adjust_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43626 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_balancedf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_cbps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38390 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_ipw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_poststratify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39114 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32798 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_stats_and_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49276 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_weighted_comparisons_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.200347 balance-0.7.0/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    22555 2023-04-10 08:00:29.000000 balance-0.7.0/tutorials/balance_quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   590306 2023-04-10 08:00:29.000000 balance-0.7.0/tutorials/balance_quickstart_cbps.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31499 2023-04-10 08:00:29.000000 balance-0.7.0/tutorials/balance_transformations_and_formulas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-10 08:00:29.000000 balance-0.7.0/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.200347 balance-0.7.0/website/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 08:00:29.000000 balance-0.7.0/website/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-10 08:00:29.000000 balance-0.7.0/website/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 08:00:29.000000 balance-0.7.0/website/babel.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/blog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/blog/2023/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/blog/2023/01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.200347 balance-0.7.0/website/blog/2023/01/09/
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-10 08:00:29.000000 balance-0.7.0/website/blog/2023/01/09/bringing-balance-to-your-data.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-04-10 08:00:29.000000 balance-0.7.0/website/blog/2023/01/09/sample_vs_target_bar_chart.webp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.204347 balance-0.7.0/website/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/api_reference/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.204347 balance-0.7.0/website/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.204347 balance-0.7.0/website/docs/docs/general_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/general_framework/adjusting_sample_to_population.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/general_framework/evaluation_of_results.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/general_framework/general_framework.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/general_framework/pre_adjustment_diagnostics.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/docs/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    48494 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_01_qqplot_income_before.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41572 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_02_barplot_age_before.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38449 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_03_barplot_gender_before.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61834 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_04_qqplot_income_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45979 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_05_barplot_age_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41950 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_06_barplot_gender_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41877 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_07_seaborn_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_08_weights_kde.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28925 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_09_seaborn_outcome_kde_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)   468436 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/total_survey_error_flow_v02.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26229 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/total_survey_error_flow_v02.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    68569 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/total_survey_error_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/total_survey_error_image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/docs/docs/statistical_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/statistical_methods/cbps.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/statistical_methods/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/statistical_methods/ipw.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/statistical_methods/poststratify.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/tutorials/balance_transformations_and_formulas.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/tutorials/index.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/tutorials/quickstart.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/tutorials/quickstart_cbps.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-04-10 08:00:29.000000 balance-0.7.0/website/docusaurus.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-10 08:00:29.000000 balance-0.7.0/website/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-10 08:00:29.000000 balance-0.7.0/website/sidebars.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/components/HTMLLoader.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/components/HomepageFeatures.js
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/components/HomepageFeatures.module.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/src/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/src/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/pages/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/pages/index.module.css
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/pages/markdown-page.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/img/balance_logo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/img/balance_logo/AI/
+-rw-r--r--   0 runner    (1001) docker     (123)   460628 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/AI/balance_Logo_FINAL.ai
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/static/img/balance_logo/PNG/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_Black_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_White_RGB.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/img/balance_logo/PNG/Icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_Black_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_FullColor_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_White_RGB.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_Black_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_FullColor_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_White_RGB.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/static/img/balance_logo/SVG/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_Black_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_White_RGB.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/balance_logo/SVG/Icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_Black_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_FullColor_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_White_RGB.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_Black_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_FullColor_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_White_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/vertical_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/docusaurus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/fontawesome/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/fontawesome/layer-group.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/fontawesome/users.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14679 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/meta_opensource_logo_negative.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/tutorial/docsVersionDropdown.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30020 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/tutorial/localeDropdown.png
+-rw-r--r--   0 runner    (1001) docker     (123)   537599 2023-04-10 08:00:29.000000 balance-0.7.0/website/yarn.lock
```

### Comparing `balance-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `balance-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `balance-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/.github/workflows/build-and-test.yml` & `balance-0.7.0/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/.github/workflows/deploy-website.yml` & `balance-0.7.0/.github/workflows/deploy-website.yml`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/.github/workflows/release.yml` & `balance-0.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/.gitignore` & `balance-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/CHANGELOG.md` & `balance-0.7.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+0.7.0 (2023-04-10)
+==================
+### New Features
+- Add `plotly_plot_density` function: Plots interactive density plots of the given variables using kernel density estimation.
+- Modified `plotly_plot_dist` and `plot_dist` to also support 'kde' plots. Also, these are now the default options. This automatically percolates to `BalanceDF.plot()` methods.
+- `Sample.from_frame` can now guess that a column called "weights" is a weight column (instead of only guessing so if the column is called "weight").
+
+### Bug Fixes
+- Fix `rm_mutual_nas`: it now remembers the index of pandas.Series that were used as input. This fixed erroneous plots produced by seaborn functions which uses rm_mutual_nas.
+- Fix `plot_hist_kde` to work when dist_type = "ecdf"
+- Fix `plot_hist_kde` and `plot_bar` when having an input only with "self" and "target", by fixing `_return_sample_palette`.
+
+## Misc
+- All plotting functions moved internally to expect weight column to be called `weight`, instead of `weights`.
+- All adjust (ipw, cbps, poststratify, null) functions now export a dict with a key called `weight` instead of `weights`.
+
+
 0.6.0 (2023-04-05)
 ==================
 ### New Features
 - Variance of the weighted mean
     - Add the `var_of_weighted_mean` function (from balance.stats_and_plots.weighted_stats import var_of_weighted_mean):
         Computes the variance of the weighted average (pi estimator for ratio-mean) of a list of values and their corresponding weights.
         - Added the `var_of_mean` option to stat in the `descriptive_stats` function (based on `var_of_weighted_mean`)
```

### Comparing `balance-0.6.0/CODE_OF_CONDUCT.md` & `balance-0.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/CONTRIBUTING.md` & `balance-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/LICENSE` & `balance-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/LICENSE-DOCUMENTATION` & `balance-0.7.0/LICENSE-DOCUMENTATION`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/PKG-INFO` & `balance-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balance
-Version: 0.6.0
+Version: 0.7.0
 Summary: balance is a Python package offering a simple workflow and methods for dealing with biased data samples when looking to infer from them to some target population of interest.
 Home-page: https://github.com/facebookresearch/balance
 Author: Facebook, Inc.
 License: GPLv2
 Description: [![balance_logo_horizontal](https://raw.githubusercontent.com/facebookresearch/balance/main/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png)](https://import-balance.org/)
```

### Comparing `balance-0.6.0/README.md` & `balance-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/__init__.py` & `balance-0.7.0/balance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from balance.sample_class import Sample  # noqa
 from balance.util import TruncationFormatter  # noqa
 
 # TODO: which objects do we want to explicitly externalize?
 # TODO: verify this works.
 
 global __version__
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 
 def setup_logging(
     logger_name: Optional[str] = __package__,
     level: str = "INFO",
     removeHandler: bool = True,
 ) -> logging.Logger:
```

### Comparing `balance-0.6.0/balance/adjustment.py` & `balance-0.7.0/balance/adjustment.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/balancedf_class.py` & `balance-0.7.0/balance/balancedf_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,25 +599,28 @@
 
                 s3_null.covars().plot()
                 s3_null.covars().plot(library = "seaborn")
 
                 # Controlling the limits of the y axis using lim:
                 s3_null.covars().plot(ylim = (0,1))
                 s3_null.covars().plot(library = "seaborn",ylim = (0,1), dist_type = "hist")
+
+                # Returning plotly qq plots:
+                s3_null.covars().plot(dist_type = "qq")
         """
         if on_linked_samples:
             dfs_to_add = self._BalanceDF_child_from_linked_samples()
         else:
             dfs_to_add = {"self": self}
 
         # Create a list of dicts, each dict representing a dataframe and weights
         # Notice that we skip cases in which there is no data (i.e.: v is None)
         # None values are skipped in both dfs and names
         dfs = [
-            {"df": v.df, "weights": v._weights}
+            {"df": v.df, "weight": v._weights}
             for k, v in dfs_to_add.items()
             if (v is not None)
         ]
         names = [k for k, v in dfs_to_add.items() if (v is not None)]
 
         # re-order dfs and names
         # NOTE: "target", if exists, is placed at the end of the dict so that comparative plotting functions,
@@ -1654,15 +1657,15 @@
 
     # TODO: once we have hist/kde methods for plotly, consider changing the defaults here to use plotly instead of seaborn.
     def plot(
         self: "BalanceOutcomesDF", on_linked_samples: bool = True, **kwargs
     ) -> Union[Union[List, np.ndarray], Dict[str, go.Figure], None]:
         """Plots histogram of covariates in a BalanceOutcomesDF object using seaborn (as default).
 
-        It's possible to use other plots using dist_type with arguments such as "hist" (default), "kde", "qq", and "ecdf".
+        It's possible to use other plots using dist_type with arguments such as "hist", "kde" (default), "qq", and "ecdf".
         Look at :func:`plot_dist` for more details.
 
         Args:
             self (BalanceOutcomesDF): a BalanceOutcomesDF object, with a set of variables.
             on_linked_samples (bool, optional): Determines if the linked samples should be included in the plot.
                 Defaults to True.
 
@@ -1777,15 +1780,15 @@
 
     # TODO: maybe add better control if there are no weights for unadjusted or target (the current default shows them in the legend, but not in the figure)
     def plot(
         self: "BalanceWeightsDF", on_linked_samples: bool = True, **kwargs
     ) -> Union[Union[List, np.ndarray], Dict[str, go.Figure], None]:
         """Plots kde (kernal density estimation) of the weights in a BalanceWeightsDF object using seaborn (as default).
 
-        It's possible to use other plots using dist_type with arguments such as "hist" (default), "kde", "qq", and "ecdf".
+        It's possible to use other plots using dist_type with arguments such as "hist", "kde" (default), "qq", and "ecdf".
         Look at :func:`plot_dist` for more details.
 
         Args:
             self (BalanceWeightsDF): a BalanceOutcomesDF object, with a set of variables.
             on_linked_samples (bool, optional): Determines if the linked samples should be included in the plot.
                 Defaults to True.
```

### Comparing `balance-0.6.0/balance/cli.py` & `balance-0.7.0/balance/cli.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/datasets/__init__.py` & `balance-0.7.0/balance/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/datasets/sim_data_cbps.R` & `balance-0.7.0/balance/datasets/sim_data_cbps.R`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/datasets/sim_data_cbps.csv` & `balance-0.7.0/balance/datasets/sim_data_cbps.csv`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/sample_class.py` & `balance-0.7.0/balance/sample_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,16 @@
         id_column: Optional[str] = None,
         outcome_columns: Optional[Union[list, tuple, str]] = None,
         weight_column: Optional[str] = None,
         check_id_uniqueness: bool = True,
         standardize_types: bool = True,
         use_deepcopy: bool = True,
     ) -> "Sample":
-        """Create a new Sample object.
+        """
+        Create a new Sample object.
 
         NOTE that all integer columns will be converted by defaults into floats. This behavior can be turned off
         by setting standardize_types argument to False.
         The reason this is done by default is because of missing value handling combined with balance current lack of support
         for pandas Integer types:
             1. Native numpy integers do not support missing values (NA), while pandas Integers do,
             as well numpy floats. Also,
@@ -147,15 +148,15 @@
 
         Args:
             df (pd.DataFrame): containing the sample's data
             id_column (Optional, Optional[str]): the column of the df which contains the respondent's id
             (should be unique). Defaults to None.
             outcome_columns (Optional, Optional[Union[list, tuple, str]]): names of columns to treat as outcome
             weight_column (Optional, Optional[str]): name of column to treat as weight. If not specified, will
-                be guessed. If not found, will be filled with 1.0.
+                be guessed (either "weight" or "weights"). If not found, a new column will be created ("weight") and filled with 1.0.
             check_id_uniqueness (Optional, bool): Whether to check if ids are unique. Defaults to True.
             standardize_types (Optional, bool): Whether to standardize types. Defaults to True.
                 Int64/int64 -> float64
                 Int32/int32 -> float64
                 string -> object
                 pandas.NA -> numpy.nan (within each cell)
                 This is slightly memory intensive (since it copies the data twice),
@@ -241,21 +242,31 @@
                 "df",
                 "sample._df",
             )
 
         # weight column
         if weight_column is None:
             if "weight" in sample._df.columns:
-                logger.warning(f"Guessing weight column '{'weight'}'")
+                logger.warning("Guessing weight column is 'weight'")
+                weight_column = "weight"
+            elif "weights" in sample._df.columns:
+                logger.warning("Guessing weight column is 'weights'")
+                weight_column = "weights"
             else:
-                logger.warning("No weights passed, setting all weights to 1")
-                sample._df.loc[:, "weight"] = 1
-            sample.weight_column = sample._df["weight"]
-        else:
-            sample.weight_column = sample._df[weight_column]
+                # TODO: The current default when weights are not available is "weight", while the method in balanceDF is called "weights",
+                #       and the subclass is called BalanceWeightsDF (with and 's' at the end)
+                #       In the future, it would be better to be more consistent and use the same name for all variations (e.g.: "weight").
+                #       Unless, we move to use more weights columns, and this method could be used to get all of them.
+                logger.warning(
+                    "No weights passed. Adding a 'weight' column and setting all values to 1"
+                )
+                weight_column = "weight"
+                sample._df.loc[:, weight_column] = 1
+
+        sample.weight_column = sample._df[weight_column]
 
         # outcome columns
         if outcome_columns is None:
             sample._outcome_columns = None
         else:
             if isinstance(outcome_columns, str):
                 outcome_columns = [outcome_columns]
@@ -417,15 +428,15 @@
             sample_df=self.covars().df,
             sample_weights=self.weight_column,
             target_df=target.covars().df,
             target_weights=target.weight_column,
             *args,
             **kwargs,
         )
-        new_sample.set_weights(adjusted["weights"])
+        new_sample.set_weights(adjusted["weight"])
         new_sample._adjustment_model = adjusted["model"]
         new_sample._links["unadjusted"] = self
         new_sample._links["target"] = target
 
         return new_sample
 
     def set_weights(self, weights: Optional[Union[pd.Series, float]]) -> None:
```

### Comparing `balance-0.6.0/balance/stats_and_plots/general_stats.py` & `balance-0.7.0/balance/stats_and_plots/general_stats.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/stats_and_plots/weighted_comparisons_plots.py` & `balance-0.7.0/balance/stats_and_plots/weighted_comparisons_plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     col_target = rgb2hex((158 / 255, 202 / 255, 225 / 255, 0.8), keep_alpha=True)
 
     if set(names) == {"self", "target"}:
         sample_palette = {
             "self": col_unadjusted,
             "target": col_target,
         }
-    if set(names) == {"self", "unadjusted"}:
+    elif set(names) == {"self", "unadjusted"}:
         sample_palette = {
             "self": col_adjusted,
             "unadjusted": col_unadjusted,
         }
     elif set(names) == {"self", "unadjusted", "target"}:
         sample_palette = {
             "self": col_adjusted,
@@ -75,14 +75,54 @@
             "target": col_target,
         }
     else:
         sample_palette = "muted"
     return sample_palette
 
 
+def _plotly_marker_color(
+    name: Literal["sample", "unadjusted", "self", "adjusted"],
+    only_self_and_target: bool,
+    color_type: Literal["color", "line"],
+) -> str:
+    """
+    Returns a color string for a marker in a plotly plot based on the given parameters.
+
+    Args:
+        name (Literal["sample", "unadjusted", "self", "adjusted"]): Name of the marker.
+        only_self_and_target (bool): Determines if only self and target groups are available, or if it's self, unadjusted and target.
+        color_type (Literal["color", "line"]): The type of color, either "color" or "line".
+
+    Returns:
+        str: A string representing the color in RGBA format.
+
+    Raises:
+        ValueError: If the color_type is not one of the accepted options.
+    """
+    if color_type == "color":
+        col1 = 0.8
+        col2 = 0.5
+    elif color_type == "line":
+        col1 = 1
+        col2 = 1
+    else:
+        raise ValueError(
+            "Invalid value for 'tycolor_typepe'. Must be either 'color' or 'line'."
+        )
+
+    if name.lower() in ["sample", "unadjusted"] or (
+        name.lower() == "self" and only_self_and_target
+    ):
+        return f"rgba(222,45,38,{col1})"
+    elif name.lower() in ["self", "adjusted"]:
+        return f"rgba(52,165,48,{col2})"
+    else:
+        return f"rgb(158,202,225,{col1})"
+
+
 def plot_bar(
     dfs: List[Dict[str, Union[pd.DataFrame, pd.Series]]],
     names: List[str],
     column: str,
     axis: Optional[plt.Axes] = None,
     weighted: bool = True,
     title: Optional[str] = None,
@@ -93,19 +133,19 @@
 
     If weighted is True, then mutual NA values are removed using :func:`rm_mutual_nas`.
 
     Args:
         dfs (List[Dict[str, Union[pd.DataFrame, pd.Series]]]): a list (of length 1 or more) of dictionaries which describe the DataFrames and weights
             The structure is as follows:
             [
-                {'df': pd.DataFrame(...), 'weights': pd.Series(...)},
+                {'df': pd.DataFrame(...), "weight": pd.Series(...)},
                 ...
             ]
             The 'df' is a DataFrame which includes the column name that was supplied through 'column'.
-            The 'weights' is a pd.Series of weights that are used when aggregating the variable using :func:`relative_frequency_table`.
+            The "weight" is a pd.Series of weights that are used when aggregating the variable using :func:`relative_frequency_table`.
         names (List[str]): a list of the names of the DataFrames that are plotted. E.g.: ['adjusted', 'unadjusted', 'target']
         column (str): The column to be used to aggregate using :func:`relative_frequency_table`.
         axis (Optional[plt.Axes], optional): matplotlib Axes object to draw the plot onto, otherwise uses the current Axes. Defaults to None.
         weighted (bool, optional): If to pass the weights from the dicts inside dfs. Defaults to True.
         title (str, optional): Title of the plot. Defaults to "barplot of covar '{column}'".
         ylim (Optional[Tuple[float, float]], optional): A tuple with two float values representing the lower and upper limits of the y-axis.
             If not provided, the y-axis range is determined automatically. Defaults to None.
@@ -119,41 +159,41 @@
 
             df = pd.DataFrame({
                 'group': ('a', 'b', 'c', 'c'),
                 'v1': (1, 2, 3, 4),
             })
 
             plot_bar(
-                [{"df": df, "weights": pd.Series((1, 1, 1, 1))}, {"df": df, "weights": pd.Series((2, 1, 1, 1))}],
+                [{"df": df, "weight": pd.Series((1, 1, 1, 1))}, {"df": df, "weight": pd.Series((2, 1, 1, 1))}],
                 names = ["self", "target"],
                 column = "group",
                 axis = None,
                 weighted = True)
 
             # The same as above just with ylim set to (0, 1).
             plot_bar(
-                [{"df": df, "weights": pd.Series((1, 1, 1, 1))}, {"df": df, "weights": pd.Series((2, 1, 1, 1))}],
+                [{"df": df, "weight": pd.Series((1, 1, 1, 1))}, {"df": df, "weight": pd.Series((2, 1, 1, 1))}],
                 names = ["self", "target"],
                 column = "group",
                 axis = None,
                 weighted = True,
                 ylim = (0, 1))
 
             # Also deals with np.nan weights
             a = plot_bar(
-                [{"df": df, "weights": pd.Series((1, 1, 1, np.nan))}, {"df": df, "weights": pd.Series((2, 1, 1, np.nan))}],
+                [{"df": df, "weight": pd.Series((1, 1, 1, np.nan))}, {"df": df, "weight": pd.Series((2, 1, 1, np.nan))}],
                 names = ["self", "target"],
                 column = "group",
                 axis = None,
                 weighted = True)
     """
     plot_data = []
     for ii, i in enumerate(dfs):
         a_series = i["df"][column]
-        _w = i["weights"]
+        _w = i["weight"]
         if weighted:
             a_series, _w = rm_mutual_nas(a_series, _w)
             a_series.name = column  # rm_mutual_nas removes name, so we set it back
 
         df_plot_data = relative_frequency_table(a_series, w=_w if weighted else None)
         df_plot_data["dataset"] = names[ii]  # a recycled column for barplot's hue.
 
@@ -193,19 +233,19 @@
 
     Options include histogram (hist), kernel density estimate (kde), and empirical cumulative density function (ecdf).
 
     Args:
         dfs (List[Dict[str, Union[pd.DataFrame, pd.Series]]]): a list (of length 1 or more) of dictionaries which describe the DataFrames and weights
             The structure is as follows:
             [
-                {'df': pd.DataFrame(...), 'weights': pd.Series(...)},
+                {'df': pd.DataFrame(...), "weight": pd.Series(...)},
                 ...
             ]
             The 'df' is a DataFrame which includes the column name that was supplied through 'column'.
-            The 'weights' is a pd.Series of weights that are used when aggregating the variable using :func:`relative_frequency_table`.
+            The "weight" is a pd.Series of weights that are used when aggregating the variable using :func:`relative_frequency_table`.
         names (List[str]): a list of the names of the DataFrames that are plotted. E.g.: ['adjusted', 'unadjusted', 'target']
         column (str): The column to be used to aggregate using :func:`relative_frequency_table`.
         axis (Optional[plt.Axes], optional): matplotlib Axes object to draw the plot onto, otherwise uses the current Axes. Defaults to None.
         weighted (bool, optional): If to pass the weights from the dicts inside dfs. Defaults to True.
         dist_type (Literal["hist", "kde", "ecdf"], optional): The type of plot to draw. Defaults to "hist".
         title (str, optional): Title of the plot. Defaults to "distribution plot of covar '{column}'".
 
@@ -219,15 +259,15 @@
             import matplotlib.pyplot as plt
 
             df = pd.DataFrame({
                 'group': ('a', 'b', 'c', 'c'),
                 'v1': (1, 2, 3, 4),
             })
 
-            dfs1 = [{"df": pd.DataFrame(pd.Series([1,2,2,2,3,4,5,5,7,8,9,9,9,9,5,2,5,4,4,4], name = "v1")), "weights": None}, {"df": df, "weights": pd.Series((200, 1, 0, 20))}]
+            dfs1 = [{"df": pd.DataFrame(pd.Series([1,2,2,2,3,4,5,5,7,8,9,9,9,9,5,2,5,4,4,4], name = "v1")), "weight": None}, {"df": df, "weight": pd.Series((200, 1, 0, 20))}]
 
             plt.figure(1)
 
             # kde: no weights
             plot_hist_kde(
                 dfs1,
                 names = ["self", "target"],
@@ -289,43 +329,47 @@
     dist_function = possible_dist_function[dist_type]
     # NOTE: the reason we don't use sns.displot directly is that it doesn't accept an ax= kwarg.
     # see also here: https://stackoverflow.com/a/63895570/256662
 
     plot_data = []
     for ii, i in enumerate(dfs):
         a_series = i["df"][column]
-        _w = i["weights"]
+        _w = i["weight"]
         if _w is None:
             _w = pd.Series(np.ones(len(a_series)), index=a_series.index)
         if weighted:
             a_series, _w = rm_mutual_nas(a_series, _w)
             a_series.name = column  # rm_mutual_nas removes name, so we set it back
+            # TODO: verify if this normalization to sum to 1 is needed (if so, how come we don't do it when _w is None)?
+            _w = _w / np.sum(_w)
 
         df_plot_data = pd.DataFrame({column: a_series, "_w": _w})
         df_plot_data["dataset"] = names[ii]  # a recycled column for barplot's hue.
 
         plot_data.append(df_plot_data)
 
     plot_data = pd.concat(plot_data)
-    _w = plot_data["_w"]
 
     sample_palette = _return_sample_palette(names)
     if title is None:
         title = f"distribution plot of covar '{column}'"
 
-    ax = dist_function(
-        data=plot_data,
-        x=column,
-        hue="dataset",
-        ax=axis,
-        weights=_w / np.sum(_w) if weighted else None,
-        common_norm=False,
-        palette=sample_palette,
-        linewidth=2,
-    )
+    kwargs_for_dist_function = {
+        "data": plot_data,
+        "x": column,
+        "hue": "dataset",
+        "ax": axis,
+        "weights": plot_data["_w"] if weighted else None,
+        # common_norm:False,
+        "palette": sample_palette,
+        "linewidth": 2,
+    }
+    if dist_type != "ecdf":
+        kwargs_for_dist_function["common_norm"] = False
+    ax = dist_function(**kwargs_for_dist_function)
     ax.set_title(title)
 
 
 def plot_qq(
     dfs: List[Dict[str, Union[pd.DataFrame, pd.Series]]],
     names: List[str],
     column: str,
@@ -336,19 +380,19 @@
 
     See: https://en.wikipedia.org/wiki/Q-Q_plot
 
     Args:
         dfs (List[Dict[str, Union[pd.DataFrame, pd.Series]]]): a list (of length 1 or more) of dictionaries which describe the DataFrames and weights
             The structure is as follows:
             [
-                {'df': pd.DataFrame(...), 'weights': pd.Series(...)},
+                {'df': pd.DataFrame(...), "weight": pd.Series(...)},
                 ...
             ]
             The 'df' is a DataFrame which includes the column name that was supplied through 'column'.
-            The 'weights' is a pd.Series of weights that are used when aggregating the variable using :func:`weighted_quantile`.
+            The "weight" is a pd.Series of weights that are used when aggregating the variable using :func:`weighted_quantile`.
             Uses the last df item in the list as the target.
         names (List[str]): a list of the names of the DataFrames that are plotted. E.g.: ['adjusted', 'unadjusted', 'target']
         column (str): The column to be used to aggregate using :func:`weighted_quantile`.
         axis (Optional[plt.Axes], optional): matplotlib Axes object to draw the plot onto, otherwise uses the current Axes. Defaults to None.
         weighted (bool, optional): If to pass the weights from the dicts inside dfs. Defaults to True.
 
     Examples:
@@ -360,39 +404,39 @@
             from numpy import random
 
             df = pd.DataFrame({
                 'v1': random.uniform(size=100),
             }).sort_values(by=['v1'])
 
             dfs1 = [
-                {"df": df, "weights": pd.Series(np.ones(100))},
-                {"df": df, "weights": pd.Series(range(100))},
-                {"df": df, "weights": pd.Series(np.ones(100))},
+                {"df": df, "weight": pd.Series(np.ones(100))},
+                {"df": df, "weight": pd.Series(range(100))},
+                {"df": df, "weight": pd.Series(np.ones(100))},
             ]
 
             # plot_qq(dfs1, names=["self", "unadjusted", "target"], column="v1", axis=None, weighted=False)
             plot_qq(dfs1, names=["self", "unadjusted", "target"], column="v1", axis=None, weighted=True)
     """
     target = dfs[-1]  # assumes the last item is target
     dfs = dfs[:-1]  # assumes the non-last item are dfs to be compared to target
 
     for ii, i in enumerate(dfs):
         d = i["df"]
-        _w = i["weights"]
+        _w = i["weight"]
 
         target_q = weighted_quantile(
             target["df"][column],
             np.arange(0, 1, 0.001),
             # pyre-fixme[6]: TODO:
             # This is because of using:
             # dfs: List[Dict[str, Union[pd.DataFrame, pd.Series]]],
             # When in fact we want to be clear that the first element is called
-            # "df" and the second "weights", and that the first is a pd.DataFrame and
+            # "df" and the second "weight", and that the first is a pd.DataFrame and
             # the second pd.Series. Until this is not clear - the following line will raise an error.
-            target["weights"] if weighted else None,
+            target["weight"] if weighted else None,
         )
         sample_q = weighted_quantile(
             d.loc[:, column],
             np.arange(0, 1, 0.001),
             # pyre-fixme[6]
             _w if weighted else None,
         )
@@ -424,19 +468,19 @@
 
     X-axis is the sample (adjusted, unadjusted) and Y-axis is the target.
 
     Args:
         dfs (List[Dict[str, Union[pd.DataFrame, pd.Series]]]): a list (of length 1 or more) of dictionaries which describe the DataFrames and weights
             The structure is as follows:
             [
-                {'df': pd.DataFrame(...), 'weights': pd.Series(...)},
+                {'df': pd.DataFrame(...), "weight": pd.Series(...)},
                 ...
             ]
             The 'df' is a DataFrame which includes the column name that was supplied through 'column'.
-            The 'weights' is a pd.Series of weights that are used when aggregating the variable using :func:`weighted_quantile`.
+            The "weight" is a pd.Series of weights that are used when aggregating the variable using :func:`weighted_quantile`.
             Uses the last df item in the list as the target.
         names (List[str]): a list of the names of the DataFrames that are plotted. E.g.: ['adjusted', 'unadjusted', 'target']
         column (str): The column to be used to aggregate using :func:`relative_frequency_table`.
         axis (Optional[plt.Axes], optional): matplotlib Axes object to draw the plot onto, otherwise uses the current Axes. Defaults to None.
         weighted (bool, optional): If to pass the weights from the dicts inside dfs. Defaults to True.
         label_threshold (int, optional): All labels that are larger from the threshold will be omitted from the scatter plot (so to reduce clutter). Defaults to 30.
 
@@ -449,17 +493,17 @@
             from numpy import random
 
             df = pd.DataFrame({
                 'v1': random.random_integers(11111, 11114, size=100),
             }).sort_values(by=['v1'])
 
             dfs1 = [
-                {"df": df, "weights": pd.Series(np.ones(100))},
-                {"df": df, "weights": pd.Series(np.ones(99).tolist() + [1000])},
-                {"df": df, "weights": pd.Series(np.ones(100))},
+                {"df": df, "weight": pd.Series(np.ones(100))},
+                {"df": df, "weight": pd.Series(np.ones(99).tolist() + [1000])},
+                {"df": df, "weight": pd.Series(np.ones(100))},
             ]
 
             import matplotlib.pyplot as plt
 
             plt.rcParams["figure.figsize"] = (20, 6) # (w, h)
 
             fig, axs = plt.subplots(1,3)
@@ -468,23 +512,23 @@
             plot_qq_categorical(dfs1, names=["self", "unadjusted", "target"], column="v1", axis=axs[0], weighted=False)
             # With weights
             plot_qq_categorical(dfs1, names=["self", "unadjusted", "target"], column="v1", axis=axs[1], weighted=True)
             # With label trimming if the text is longer than 3.
             plot_qq_categorical(dfs1, names=["self", "unadjusted", "target"], column="v1", axis=axs[2], weighted=True, label_threshold=3)
     """
     target = dfs[-1]["df"]
-    target_weights = dfs[-1]["weights"]
+    target_weights = dfs[-1]["weight"]
     dfs = dfs[:-1]
 
     # pyre-fixme[6]
     target_plot_data = relative_frequency_table(target, column, target_weights)
 
     for ii, i in enumerate(dfs):
         d = i["df"]
-        _w = i["weights"] if weighted else None
+        _w = i["weight"] if weighted else None
 
         # pyre-fixme[6]
         sample_plot_data = relative_frequency_table(d, column, _w)
         plot_data = pd.merge(
             sample_plot_data,
             target_plot_data,
             on=column,
@@ -527,19 +571,19 @@
 
     Uses: :func:`plot_qq_categorical`, :func:`plot_qq`, :func:`plot_hist_kde`, :func:`plot_bar`.
 
     Args:
         dfs (List[Dict[str, Union[pd.DataFrame, pd.Series]]]): a list (of length 1 or more) of dictionaries which describe the DataFrames and weights
             The structure is as follows:
             [
-                {'df': pd.DataFrame(...), 'weights': pd.Series(...)},
+                {'df': pd.DataFrame(...), "weight": pd.Series(...)},
                 ...
             ]
             The 'df' is a DataFrame which includes the column name that was supplied through 'column'.
-            The 'weights' is a pd.Series of weights that are used when aggregating by the column variable.
+            The "weight" is a pd.Series of weights that are used when aggregating by the column variable.
         names (List[str]): a list of the names of the DataFrames that are plotted. E.g.: ['adjusted', 'unadjusted', 'target']
         variables (Optional[List], optional): The list of variables to use, by default (None) will plot all of them.
         numeric_n_values_threshold (int, optional): How many unique values (or less) should be in a column so that it is considered to be a "category"? Defaults to 15.
             This is compared against the maximum number of distinct values (for each of the variables) across all DataFrames.
             Setting this value to 0 will disable this check.
         weighted (bool, optional): If to pass the weights from the dicts inside dfs. Defaults to True.
         dist_type (Optional[str], optional): can be "hist", "kde", or "qq". Defaults to None.
@@ -566,17 +610,17 @@
             df = pd.DataFrame({
                 'v1': random.random_integers(11111, 11114, size=100).astype(str),
                 'v2': random.normal(size = 100),
                 'v3': random.uniform(size = 100),
             }).sort_values(by=['v2'])
 
             dfs1 = [
-                {"df": df, "weights": pd.Series(np.ones(100))},
-                {"df": df, "weights": pd.Series(np.ones(99).tolist() + [1000])},
-                {"df": df, "weights": pd.Series(np.random.uniform(size=100))},
+                {"df": df, "weight": pd.Series(np.ones(100))},
+                {"df": df, "weight": pd.Series(np.ones(99).tolist() + [1000])},
+                {"df": df, "weight": pd.Series(np.random.uniform(size=100))},
             ]
 
             seaborn_plot_dist(dfs1, names=["self", "unadjusted", "target"], dist_type = "qq")  # default
             seaborn_plot_dist(dfs1, names=["self", "unadjusted", "target"], dist_type = "hist")
             seaborn_plot_dist(dfs1, names=["self", "unadjusted", "target"], dist_type = "kde")
             seaborn_plot_dist(dfs1, names=["self", "unadjusted", "target"], dist_type = "ecdf")
 
@@ -667,15 +711,16 @@
 
 def plotly_plot_qq(
     dict_of_dfs: Dict[str, pd.DataFrame],
     variables: List[str],
     plot_it: bool = True,
     return_dict_of_figures: bool = False,
 ) -> Optional[Dict[str, go.Figure]]:
-    """Plots interactive QQ plot of the given variables.
+    """
+    Plots interactive QQ plot of the given variables.
 
     Creates a plotly qq plot of the given variables from multiple DataFrames.
     This ASSUMES there is a df with key 'target'.
 
 
     Args:
         dict_of_dfs (Dict[str, pd.DataFrame]): The key is the name of the DataFrame (E.g.: self, unadjusted, target),
@@ -752,22 +797,20 @@
                             np.arange(0, 1, 0.001),
                             dict_of_dfs[name]["weight"]
                             if "weight" in dict_of_dfs[name].columns
                             else None,
                         )["col1"]
                     ),
                     marker={
-                        "color": "rgba(222,45,38,0.8)"
-                        if (
-                            (name.lower() in ["sample", "unadjusted"])
-                            or (name.lower() == "self" and only_self_and_target)
+                        "color": _plotly_marker_color(
+                            # pyre-ignore[6]: it cannot get to this point if name=="target".
+                            name,
+                            only_self_and_target,
+                            "color",
                         )
-                        else "rgba(52,165,48,0.5)"
-                        if name.lower() in ["self", "adjusted"]
-                        else "rgb(158,202,225,.8)"
                     },
                     mode="markers",
                     name=naming_legend(name, list(dict_of_dfs.keys())),
                     opacity=0.6,
                 )
 
         data = [variable_specific_dict_of_plots[name] for name in dict_of_dfs]
@@ -787,14 +830,170 @@
         dict_of_qqs[variable] = fig
         if plot_it:
             offline.iplot(fig)
     if return_dict_of_figures:
         return dict_of_qqs
 
 
+def plotly_plot_density(
+    dict_of_dfs: Dict[str, pd.DataFrame],
+    variables: List[str],
+    plot_it: bool = True,
+    return_dict_of_figures: bool = False,
+    plot_width: int = 800,
+) -> Optional[Dict[str, go.Figure]]:
+    """
+    Plots interactive density plots of the given variables using kernel density estimation.
+
+    Creates a plotly plot of the kernel density estimate for each variable in the given list
+    across multiple DataFrames. The function assumes there is a DataFrame with the key 'target'.
+    The density plot shows the distribution of the variable for each DataFrame in the dictionary.
+    It looks for a `weights` column and uses it to normalize the data. If no weight column is found, it assumes all weights are equal to 1.
+    It relies on the seaborn library to create the KDE (`sns.kdeplot`).
+
+    Args:
+        dict_of_dfs (Dict[str, pd.DataFrame]): A dictionary where each key is a name for the DataFrame
+            and the value is the DataFrame that contains the variables to plot.
+        variables (List[str]): A list of variables to plot.
+        plot_it (bool, optional): Whether to plot the figures interactively using plotly. Defaults to True.
+        return_dict_of_figures (bool, optional): Whether to return a dictionary of plotly figures.
+            Defaults to False.
+        plot_width (int, optional): The width of the plot in pixels. Defaults to 800.
+
+    Returns:
+        Optional[Dict[str, go.Figure]]: A dictionary containing plotly figures for each variable
+        in the given list if `return_dict_of_figures` is True. Otherwise, returns None.
+
+    Examples:
+        ::
+            import numpy as np
+            import pandas as pd
+            from numpy import random
+            from balance.stats_and_plots.weighted_comparisons_plots import plotly_plot_density, plot_dist
+
+            random.seed(96483)
+
+            df = pd.DataFrame({
+                'v1': random.random_integers(11111, 11114, size=100).astype(str),
+                'v2': random.normal(size = 100),
+                'v3': random.uniform(size = 100),
+            }).sort_values(by=['v2'])
+
+            dict_of_dfs = {
+                "self": pd.concat([df, pd.Series(random.random(size = 100) + 0.5, name = "weight")], axis = 1),
+                "unadjusted": pd.concat([df, pd.Series(np.ones(99).tolist() + [1000], name = "weight")], axis = 1),
+                "target": pd.concat([df, pd.Series(np.ones(100), name = "weight")], axis = 1),
+            }
+
+            # It won't work with "v1" since it is not numeric.
+            plotly_plot_density(dict_of_dfs, variables= ["v2", "v3"], plot_width = 550)
+
+
+            # The above gives the same results as:
+            dfs1 = [
+                {"df": df, "weight": dict_of_dfs['self']["weight"]},
+                {"df": df, "weight": dict_of_dfs['unadjusted']["weight"]},
+                {"df": df, "weight": dict_of_dfs['target']["weight"]},
+            ]
+            plot_dist(dfs1, names=["self", "unadjusted", "target"], library="seaborn", dist_type = "kde", variables= ["v2", "v3"])
+
+
+            # This gives the same shape of plots (notice how we must have the column "weight" for the plots to work)
+            df = pd.DataFrame({
+                'group': ('a', 'b', 'c', 'c'),
+                'v1': (1, 2, 3, 4),
+            })
+
+            dfs1 = [{"df": pd.DataFrame(pd.Series([1,2,2,2,3,4,5,5,7,8,9,9,9,9,5,2,5,4,4,4], name = "v1")), "weight": None}, {"df": df, "weight": pd.Series((200, 1, 0, 200000))}]
+            # dfs1[1]{'df'}
+
+            dict_of_dfs = {
+                "self": dfs1[0]['df'], # pd.concat([df, pd.Series(random.random(size = 100) + 0.5, name = "weight")], axis = 1),
+                "target": pd.concat([dfs1[1]['df'], pd.Series(dfs1[1]["weight"], name = "weight")], axis = 1),
+            }
+
+            plotly_plot_density(dict_of_dfs, variables= ["v1"], plot_width = 550)
+
+            plot_dist(dfs1, names=["self", "target"], library="seaborn", dist_type = "kde", variables= ["v1"],numeric_n_values_threshold = 1)
+
+    """
+    dict_of_density_plots = {}
+
+    for variable in variables:
+        data = []
+
+        # Indicate if we have only self and target (without unadjusted)
+        # since in this case the color of self should be red, since it's likely unadjusted.
+        only_self_and_target = set(dict_of_dfs.keys()) == {"self", "target"}
+
+        for name, df in dict_of_dfs.items():
+            if "weight" in df.columns:
+                weights = df["weight"]
+                # TODO: verify if this normalization to sum to 1 is needed (if so, how come we don't do it when _w is None)?
+                weights = weights / weights.sum()  # normalize weights by sum of weights
+            else:
+                weights = np.ones(len(df))
+
+            # Convert the data to long format
+            long_df = pd.DataFrame({"value": df[variable], "weight": weights})
+
+            # Replace KDE calculation with sns.kdeplot
+            with plt.xkcd():
+                plt.figure()
+                ax = sns.kdeplot(
+                    data=long_df, x="value", weights="weight", common_norm=False
+                )
+                x = ax.get_lines()[-1].get_xdata()
+                y = ax.get_lines()[-1].get_ydata()
+                # print(name)
+                # print(x)
+                # print(y)
+                plt.close()
+
+            trace = go.Scatter(
+                x=x,
+                y=y,
+                mode="lines",
+                name=naming_legend(name, list(dict_of_dfs.keys())),
+                line={
+                    # pyre-ignore[6]: it cannot get to this point if name=="target".
+                    "color": _plotly_marker_color(name, only_self_and_target, "line"),
+                    "width": 1.5,
+                },
+            )
+            data.append(trace)
+
+        layout = {
+            "title": f"Density Plots of '{variable}'",
+            "paper_bgcolor": "rgb(255, 255, 255)",
+            "plot_bgcolor": "rgb(255, 255, 255)",
+            "width": plot_width,
+            "xaxis": {
+                "title": variable,
+                "gridcolor": "rgba(128, 128, 128, 0.5)",
+                "gridwidth": 1,
+                "showgrid": True,
+            },
+            "yaxis": {
+                "title": "Density",
+                "gridcolor": "rgba(128, 128, 128, 0.5)",
+                "gridwidth": 1,
+                "showgrid": True,
+            },
+        }
+        fig = go.Figure(data=data, layout=layout)
+        dict_of_density_plots[variable] = fig
+
+        if plot_it:
+            offline.iplot(fig)
+
+    if return_dict_of_figures:
+        return dict_of_density_plots
+
+
 def plotly_plot_bar(
     dict_of_dfs: Dict[str, pd.DataFrame],
     variables: List[str],
     plot_it: bool = True,
     return_dict_of_figures: bool = False,
     ylim: Optional[Tuple[float, float]] = None,
 ) -> Optional[Dict[str, go.Figure]]:
@@ -861,31 +1060,23 @@
                 else None,
             )
 
             variable_specific_dict_of_plots[name] = go.Bar(
                 x=list(df_plot_data[variable]),
                 y=list(df_plot_data["prop"]),
                 marker={
-                    "color": "rgba(222,45,38,0.8)"
-                    if (
-                        (name.lower() in ["sample", "unadjusted"])
-                        or (name.lower() == "self" and only_self_and_target)
-                    )
-                    else "rgba(52,165,48,0.5)"
-                    if name.lower() in ["self", "adjusted"]
-                    else "rgb(158,202,225,.8)",
+                    # pyre-ignore[6]: it cannot get to this point if name=="target".
+                    "color": _plotly_marker_color(name, only_self_and_target, "color"),
                     "line": {
-                        "color": "rgba(222,45,38,1)"
-                        if (
-                            (name.lower() in ["sample", "unadjusted"])
-                            or (name.lower() == "self" and only_self_and_target)
-                        )
-                        else "rgba(52,165,48,1)"
-                        if name.lower() in ["self", "adjusted"]
-                        else "rgb(158,202,225,1)",
+                        "color": _plotly_marker_color(
+                            # pyre-ignore[6]: it cannot get to this point if name=="target".
+                            name,
+                            only_self_and_target,
+                            "line",
+                        ),
                         "width": 1.5,
                     },
                 },
                 opacity=0.6,
                 name=naming_legend(name, list(dict_of_dfs.keys())),
                 visible=True,
             )
@@ -906,38 +1097,43 @@
         dict_of_bars[variable] = fig
         if plot_it:
             offline.iplot(fig)
     if return_dict_of_figures:
         return dict_of_bars
 
 
-# TODO: add more plots other than qq for numeric (e.g.: density/kde, hist, ecdf,)
+# TODO: add more plots other than qq for numeric (e.g.: hist, ecdf,)
 # see https://plotly.com/python/distplot/
+# Notice that these plots do not support the 'weight' column, so it requires a different approach.
+# See the plotly_plot_density solution that uses seaborn's output
 def plotly_plot_dist(
     dict_of_dfs: Dict[str, pd.DataFrame],
     variables: Optional[List[str]] = None,
     numeric_n_values_threshold: int = 15,
     weighted: bool = True,
+    dist_type: Optional[Literal["kde", "qq"]] = None,
     plot_it: bool = True,
     return_dict_of_figures: bool = False,
     ylim: Optional[Tuple[float, float]] = None,
 ) -> Optional[Dict[str, go.Figure]]:
-    """Plots interactive distribution plots (qq and bar plots) of the given variables.
+    """
+    Plots interactive distribution plots (qq and bar plots) of the given variables.
 
     The plots compare the weighted distributions of an arbitrary number
     of variables from an arbitrary number of DataFrames.
-    Numeric variables are plotted as qq's using :func:`plotly_plot_qq`,
+    Numeric variables are plotted as either qq's using :func:`plotly_plot_qq`, or as kde desnity plots using :func:`plotly_plot_density`.
     categorical variables as barplots using :func:`plotly_plot_bar`.
 
     Args:
         dict_of_dfs (Dict[str, pd.DataFrame]): The key is the name of the DataFrame (E.g.: self, unadjusted, target),
             and the value is the DataFrame that contains the variables that we want to plot.
         variables (Optional[List[str]], optional): a list of variables to use for plotting. Defaults (i.e.: if None) is to use the list of all variables.
         numeric_n_values_threshold (int, optional): How many numbers should be in a column so that it is considered to be a "category"? Defaults to 15.
         weighted (bool, optional): If to use the weights with the plots. Defaults to True.
+        dist_type (Optional[Literal["kde", "qq"]], optional): The type of plot to draw (relevant only for numerical variables). Defaults to None (which fallbacks to "kde").
         plot_it (bool, optional): If to plot the plots interactively instead of returning a dictionary. Defaults to True.
         return_dict_of_figures (bool, optional): If to return the dictionary containing the plots rather than just returning None. Defaults to False.
             If returned - the dictionary is of plots.
             Keys in this dictionary are the variable names for each plot.
             Values are plotly plot objects plotted like:
                 offline.iplot(dict_of_all_plots['age'])
             Or simply:
@@ -971,14 +1167,17 @@
                 "target": pd.concat([df, pd.Series(np.ones(100), name = "weight")], axis = 1),
             }
 
             plotly_plot_dist(dict_of_dfs)
 
             # Make sure the bar plot is plotted with y in the range of 0 to 1.
             plotly_plot_dist(dict_of_dfs, ylim = (0,1))
+
+            # See the qqplots version
+            plotly_plot_dist(dict_of_dfs, dist_type="qq")
     """
     dict_of_all_plots = {}
     #  Choose set of variables to plot
     variables = choose_variables(
         *(dict_of_dfs[name] for name in dict_of_dfs), variables=variables
     )
 
@@ -1019,21 +1218,32 @@
 
             continue
 
         #  Plot categorical variables as histogram
         categorical = (o not in numeric_variables) or (
             n_values < numeric_n_values_threshold
         )
+
+        if (dist_type is None) or dist_type == "kde":
+            plotly_numeric_plot = plotly_plot_density
+        elif dist_type == "qq":
+            plotly_numeric_plot = plotly_plot_qq
+        else:
+            raise NotImplementedError(
+                f"dist_type of type {dist_type} is not implemented."
+            )
+
         # the below functions will create plotly plots
         if categorical:
             dict_of_plot = plotly_plot_bar(
                 dict_of_dfs, [o], plot_it, return_dict_of_figures, ylim=ylim
             )
         else:
-            dict_of_plot = plotly_plot_qq(
+            # plotly_plot_density
+            dict_of_plot = plotly_numeric_plot(
                 dict_of_dfs, [o], plot_it, return_dict_of_figures
             )
         # the below functions will add the plotly dict outputs
         # to the dictionary 'dict_of_all_plots' (if return_dict_of_figures is True).
         if dict_of_plot is not None and return_dict_of_figures:
             dict_of_all_plots.update(dict_of_plot)
 
@@ -1085,39 +1295,40 @@
 
 def plot_dist(
     dfs: List[Dict[str, Union[pd.DataFrame, pd.Series]]],
     names: Optional[List[str]] = None,
     variables: Optional[List[str]] = None,
     numeric_n_values_threshold: int = 15,
     weighted: bool = True,
-    dist_type: Optional[Literal["qq", "hist", "kde", "ecdf"]] = None,
+    dist_type: Optional[Literal["kde", "hist", "qq", "ecdf"]] = None,
     library: Literal["plotly", "seaborn"] = "plotly",
     ylim: Optional[Tuple[float, float]] = None,
     **kwargs,
 ) -> Union[Union[List, np.ndarray], Dict[str, go.Figure], None]:
     """Plots the variables of a DataFrame by using either seaborn or plotly.
 
-    If using plotly then using qq plots for numeric variables and bar plots for categorical variables. Uses :func:`plotly_plot_dist`.
+    If using plotly then using kde (or qq) plots for numeric variables and bar plots for categorical variables. Uses :func:`plotly_plot_dist`.
     If using seaborn then various types of plots are possible for the variables (see dist_type for details). Uses :func:`seaborn_plot_dist`
 
     Args:
         dfs (List[Dict[str, Union[pd.DataFrame, pd.Series]]]): a list (of length 1 or more) of dictionaries which describe the DataFrames and weights
             The structure is as follows:
             [
-                {'df': pd.DataFrame(...), 'weights': pd.Series(...)},
+                {'df': pd.DataFrame(...), "weight": pd.Series(...)},
                 ...
             ]
             The 'df' is a DataFrame which includes the column name that was supplied through 'column'.
-            The 'weights' is a pd.Series of weights that are used when aggregating the variable using :func:`relative_frequency_table`.
+            The "weight" is a pd.Series of weights that are used when aggregating the variable using :func:`relative_frequency_table`.
         names (List[str]): a list of the names of the DataFrames that are plotted. E.g.: ['adjusted', 'unadjusted', 'target']
             If None, then all DataFrames will be plotted, but only if library == "seaborn". (TODO: to remove this restriction)
         variables (Optional[List[str]], optional): a list of variables to use for plotting. Default (i.e.: if None) is to use the list of all variables.
         numeric_n_values_threshold (int, optional): How many numbers should be in a column so that it is considered to be a "category"? Defaults to 15.
         weighted (bool, optional): If to use the weights with the plots. Defaults to True.
-        dist_type (Literal["qq", "hist", "kde", "ecdf"], optional): The type of plot to draw. Relevant only if using library="seaborn". Defaults to "hist".
+        dist_type (Literal["kde", "hist", "qq", "ecdf"], optional): The type of plot to draw. The 'qq' and 'kde' options are available for library="plotly",
+            While all options are available if using library="seaborn". Defaults to "kde".
         library (Literal["plotly", "seaborn"], optional): Whichever library to use for the plot. Defaults to "plotly".
         ylim (Optional[Tuple[float, float]], optional): A tuple with two float values representing the lower and upper limits of the y-axis.
             If not provided, the y-axis range is determined automatically. Defaults to None.
             passed to bar plots only.
 
     Raises:
         ValueError: if library is not in ("plotly", "seaborn").
@@ -1140,71 +1351,73 @@
             df = pd.DataFrame({
                 'v1': random.random_integers(11111, 11114, size=100).astype(str),
                 'v2': random.normal(size = 100),
                 'v3': random.uniform(size = 100),
             }).sort_values(by=['v2'])
 
             dfs1 = [
-                {"df": df, "weights": pd.Series(random.random(size = 100) + 0.5)},
-                {"df": df, "weights": pd.Series(np.ones(99).tolist() + [1000])},
-                {"df": df, "weights": pd.Series(np.ones(100))},
+                {"df": df, "weight": pd.Series(random.random(size = 100) + 0.5)},
+                {"df": df, "weight": pd.Series(np.ones(99).tolist() + [1000])},
+                {"df": df, "weight": pd.Series(np.ones(100))},
             ]
 
 
             from balance.stats_and_plots.weighted_comparisons_plots import plot_dist
 
             # defaults to plotly with bar and qq plots. Returns None.
             plot_dist(dfs1, names=["self", "unadjusted", "target"])
 
-            # Using seaborn, deafults to qq plots
-            plot_dist(dfs1, names=["self", "unadjusted", "target"], library="seaborn") # like using dist_type = "qq"
+            # Using seaborn, deafults to kde plots
+            plot_dist(dfs1, names=["self", "unadjusted", "target"], library="seaborn") # like using dist_type = "kde"
             plot_dist(dfs1, names=["self", "unadjusted", "target"], library="seaborn", dist_type = "hist")
-            plot_dist(dfs1, names=["self", "unadjusted", "target"], library="seaborn", dist_type = "kde")
+            plot_dist(dfs1, names=["self", "unadjusted", "target"], library="seaborn", dist_type = "qq")
             plot_dist(dfs1, names=["self", "unadjusted", "target"], library="seaborn", dist_type = "ecdf")
 
             plot_dist(dfs1, names=["self", "unadjusted", "target"], ylim = (0,1))
-            plot_dist(dfs1, names=["self", "unadjusted", "target"], library="seaborn", dist_type = "kde", ylim = (0,1))
+            plot_dist(dfs1, names=["self", "unadjusted", "target"], library="seaborn", dist_type = "qq", ylim = (0,1))
     """
     if library not in ("plotly", "seaborn"):
         raise ValueError(f"library must be either 'plotly' or 'seaborn', is {library}")
 
     #  Set default names for samples
     # TODO: this will work only with seaborn. Will need to change to something that also works for plotly.
     if names is None:
         names = [f"sample {i}" for i in range(1, len(dfs) + 1)]
 
     if library == "seaborn":
         return seaborn_plot_dist(
-            dfs,
-            names,
-            variables,
-            numeric_n_values_threshold,
-            weighted,
-            dist_type,
+            dfs=dfs,
+            names=names,
+            variables=variables,
+            numeric_n_values_threshold=numeric_n_values_threshold,
+            weighted=weighted,
+            dist_type=dist_type,
             ylim=ylim,
             **kwargs,
         )
     elif library == "plotly":
         dict_of_dfs = dict(
             zip(
                 names,
                 (
-                    pd.concat((d["df"], pd.Series(d["weights"], name="weight")), axis=1)
+                    pd.concat((d["df"], pd.Series(d["weight"], name="weight")), axis=1)
                     for d in dfs
                 ),
             )
         )
 
         if dist_type is not None:
             logger.warning("plotly plots ignore dist_type. Consider library='seaborn'")
 
         return plotly_plot_dist(
             dict_of_dfs,
             variables,
             numeric_n_values_threshold,
             weighted,
+            # pyre-ignore[6]: plotly_plot_dist will raise a NotImplemented error if dist_type is not None, 'kde', or 'qq'
+            dist_type=dist_type,
             ylim=ylim,
             **kwargs,
         )
 
 
 # TODO: add plots to compare ASMD
```

### Comparing `balance-0.6.0/balance/stats_and_plots/weighted_comparisons_stats.py` & `balance-0.7.0/balance/stats_and_plots/weighted_comparisons_stats.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/stats_and_plots/weighted_stats.py` & `balance-0.7.0/balance/stats_and_plots/weighted_stats.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/stats_and_plots/weights_stats.py` & `balance-0.7.0/balance/stats_and_plots/weights_stats.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/testutil.py` & `balance-0.7.0/balance/testutil.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/balance/util.py` & `balance-0.7.0/balance/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1051,28 +1051,27 @@
         or isinstance(o, pd.arrays.BooleanArray)
         or "pandas.core.arrays" in str(type(o))  # support any pandas array type.
         or (isinstance(o, collections.abc.Sequence) and not isinstance(o, str))
     )
 
 
 def rm_mutual_nas(*args) -> List:
-    """Remove entries in a position which is na or infinite in any of the arguments
+    """
+    Remove entries in a position which is na or infinite in any of the arguments.
 
-    Ignores args which are None
+    Ignores args which are None.
 
-    can accept array-like or single arraylike argument. Including pandas and numpy arrays.
+    Can accept multiple array-like arguments or a single array-like argument. Handles pandas and numpy arrays.
 
     Raises:
-        ValueError: If args are not array like (see: :func:`_is_arraylike`)
-        ValueError: If args include arrays of different lengths.
+        ValueError: If any argument is not array-like. (see: :func:`_is_arraylike`)
+        ValueError: If arguments include arrays of different lengths.
 
     Returns:
-        List: A list with all the original vectors, after removing from them the
-            elements for which there was a missing value in the same position as
-            any of the other arrays.
+        List: A list containing the original input arrays, after removing elements that have a missing or infinite value in the same position as any of the other arrays.
 
     Examples:
         ::
 
             import pandas as pd
             import numpy as np
 
@@ -1120,14 +1119,35 @@
                 #  Length: 2, dtype: object,
                 #  <StringArray>
                 #  ['1.1', '2']
                 #  Length: 2, dtype: string,
                 #  array([1., 2.]),
                 #  array(['1', '2'], dtype='<U32'),
                 #  [1, 2]]
+
+                # Preserve the index values in the resulting pd.Series:
+                x1 = pd.Series([1, 2, 3, 4])
+                x2 = pd.Series([np.nan, 2, 3, 4])
+                x3 = np.array([1, 2, 3, 4])
+                print(rm_mutual_nas(x1, x2)[0])
+                print(rm_mutual_nas(x1.sort_values(ascending=False), x2)[0])
+                print(rm_mutual_nas(x1, x3)[0])
+                    # 1    2
+                    # 2    3
+                    # 3    4
+                    # dtype: int64
+                    # 3    4
+                    # 2    3
+                    # 1    2
+                    # dtype: int64
+                    # 0    1
+                    # 1    2
+                    # 2    3
+                    # 3    4
+                    # dtype: int64
     """
     if any(not (a is None or _is_arraylike(a)) for a in args):
         raise ValueError("All arguments must be arraylike")
     # create a set of lengths of all arrays, and see if there are is more than
     # one array length: (we shouldn't, since we expect all arrays to have the same length)
     if len({len(a) for a in args if a is not None}) > 1:
         raise ValueError("All arrays must be of same length")
@@ -1153,14 +1173,23 @@
         else:
             return type(x)
 
     #  Need to convert each argument to a type that can be indexed and then
     #  convert back
     original_types = [_return_type_creation_function(x) for x in args]
     r = [pd.Series(x)[nonmissing_mask].tolist() if x is not None else x for x in args]
+
+    # Reapply the index for pd.Series
+    r = [
+        pd.Series(data, index=pd.Series(orig_data)[nonmissing_mask].index)
+        if isinstance(orig_data, pd.Series)
+        else data
+        for data, orig_data in zip(r, args)
+    ]
+
     # reproduce the type of each array in the result
     r = [(t(x) if x is not None else x) for t, x in zip(original_types, r)]
     if len(args) == 1:
         r = r[0]
     return r
```

### Comparing `balance-0.6.0/balance/weighting_methods/adjust_null.py` & `balance-0.7.0/balance/weighting_methods/adjust_null.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,12 +32,12 @@
         target_weights (pd.Series): design weights for target
 
     Returns:
         Dict[str, Union[Dict[str, str], pd.Series]]: Dict of weights (original sample weights) and model (with method = null_adjustment)
     """
 
     return {
-        "weights": sample_weights,
+        "weight": sample_weights,
         "model": {
             "method": "null_adjustment",
         },
     }
```

### Comparing `balance-0.6.0/balance/weighting_methods/cbps.py` & `balance-0.7.0/balance/weighting_methods/cbps.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
         Exception: _description_
         Exception: _description_
         Exception: _description_
         Exception: _description_
 
     Returns:
         Dict[str, Union[pd.Series, Dict]]: A dictionary includes:
-        "weights" --- The weights for the sample.
+        "weight" --- The weights for the sample.
         "model" -- dictionary with details about the fitted model:
             X_matrix_columns, deviance, beta_optimal, balance_optimize_result,
             gmm_optimize_result_glm_init, gmm_optimize_result_bal_init
             It has the following shape:
             "model": {
                 "method": "cbps",
                 "X_matrix_columns": X_matrix_columns_names,
@@ -678,15 +678,15 @@
     )
     # normalize to target size
     original_sum_weights = np.sum(weights)
     logger.debug(f"original sum of weights for sample: {original_sum_weights}")
     weights = weights / original_sum_weights * np.sum(target_weights)
 
     # set index to sample_df
-    weights = pd.DataFrame({"weights": weights}).set_index(sample_index)["weights"]
+    weights = pd.DataFrame({"weight": weights}).set_index(sample_index)["weight"]
 
     if np.unique(weights).shape[0] == 1 or weights.describe()["std"] < 1e-4:
         # All weights are the same
         logger.warning(
             "All weights are identical (or almost identical). The estimates will not be adjusted"
         )
 
@@ -697,15 +697,15 @@
         s,
         Vh,
         model_matrix_standardized["model_matrix_mean"],
         model_matrix_standardized["model_matrix_std"],
     )
 
     out = {
-        "weights": weights,
+        "weight": weights,
         "model": {
             "method": "cbps",
             "X_matrix_columns": X_matrix_columns_names,
             "deviance": deviance,
             "original_sum_weights": original_sum_weights,  # This can be used to reconstruct the propensity probablities
             "beta_optimal": beta_opt,
             "beta_init_glm": beta_0,  # The initial estimator by glm
```

### Comparing `balance-0.6.0/balance/weighting_methods/ipw.py` & `balance-0.7.0/balance/weighting_methods/ipw.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,20 +405,20 @@
 
     Raises:
         Exception: f"Sample indicator only has value {_n_unique}. This can happen when your sample or target are empty from unknown reason"
         NotImplementedError: if model is not "glmnet"
 
     Returns:
         Dict[str, Any]: A dictionary includes:
-            "weights" --- The weights for the sample.
+            "weight" --- The weights for the sample.
             "model" --- parameters of the model:fit, performance, X_matrix_columns, lambda,
                         weight_trimming_mean_ratio
             Shape of the Dict:
             {
-                "weights": weights,
+                "weight": weights,
                 "model": {
                     "method": "ipw",
                     "X_matrix_columns": X_matrix_columns_names,
                     "fit": fit,
                     "perf": performance,
                     "lambda": best_s,
                     "weight_trimming_mean_ratio": weight_trimming_mean_ratio,
@@ -617,15 +617,15 @@
     if dev < 0.10:
         logger.warning(
             "The propensity model has low fraction null deviance explained "
             f"({dev}). Results may not be accurate"
         )
 
     out = {
-        "weights": weights,
+        "weight": weights,
         "model": {
             "method": "ipw",
             "X_matrix_columns": X_matrix_columns_names,
             "fit": fit,
             "perf": performance,
             "lambda": best_s,
             "weight_trimming_mean_ratio": weight_trimming_mean_ratio,
```

### Comparing `balance-0.6.0/balance/weighting_methods/poststratify.py` & `balance-0.7.0/balance/weighting_methods/poststratify.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,20 +45,20 @@
             Default is True.
     Raises:
         ValueError: _description_
         ValueError: _description_
 
     Returns:
         Dict[str, Union[pd.Series, Dict[str, str]]]:
-            weights (pd.Series): final weights (sum up to target's sum of weights)
+            weight (pd.Series): final weights (sum up to target's sum of weights)
             model (dict): method of adjustment
 
             Dict shape:
             {
-                "weights": w,
+                "weight": w,
                 "model": {"method": "poststratify"},
             }
     """
     balance_util._check_weighting_methods_input(sample_df, sample_weights, "sample")
     balance_util._check_weighting_methods_input(target_df, target_weights, "target")
 
     if ("weight" in sample_df.columns.values) or ("weight" in target_df.columns.values):
@@ -99,10 +99,10 @@
         raise ValueError("all combinations of cells in sample_df must be in target_df")
 
     combined["weight"] = combined["weight"] / combined["design_weight"]
     sample_df = sample_df.join(combined["weight"], on=variables)
     w = sample_df.weight * sample_df.design_weight
 
     return {
-        "weights": w,
+        "weight": w,
         "model": {"method": "poststratify"},
     }
```

### Comparing `balance-0.6.0/balance.egg-info/PKG-INFO` & `balance-0.7.0/balance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balance
-Version: 0.6.0
+Version: 0.7.0
 Summary: balance is a Python package offering a simple workflow and methods for dealing with biased data samples when looking to infer from them to some target population of interest.
 Home-page: https://github.com/facebookresearch/balance
 Author: Facebook, Inc.
 License: GPLv2
 Description: [![balance_logo_horizontal](https://raw.githubusercontent.com/facebookresearch/balance/main/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png)](https://import-balance.org/)
```

### Comparing `balance-0.6.0/balance.egg-info/SOURCES.txt` & `balance-0.7.0/balance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/scripts/make_docs.sh` & `balance-0.7.0/scripts/make_docs.sh`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/setup.py` & `balance-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/sphinx/Makefile` & `balance-0.7.0/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/sphinx/_templates/autosummary/class.rst` & `balance-0.7.0/sphinx/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/sphinx/conf.py` & `balance-0.7.0/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/sphinx/make.bat` & `balance-0.7.0/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/tests/test_adjust_null.py` & `balance-0.7.0/tests/test_adjust_null.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,12 +49,12 @@
     def test_adjust_null(self):
         res = balance_adjust_null.adjust_null(
             pd.DataFrame({"a": [1, 2, 3]}),
             pd.Series([4, 5, 6]),
             pd.DataFrame({"a": [7, 8, 9]}),
             pd.Series([10, 11, 12]),
         )
-        self.assertEqual(res["weights"], pd.Series([4, 5, 6]))
+        self.assertEqual(res["weight"], pd.Series([4, 5, 6]))
         self.assertEqual(res["model"]["method"], "null_adjustment")
 
         result = sample.adjust(target, method="null")
         self.assertEqual(sample.weights().df, result.weights().df)
```

### Comparing `balance-0.6.0/tests/test_adjustment.py` & `balance-0.7.0/tests/test_adjustment.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/tests/test_balancedf.py` & `balance-0.7.0/tests/test_balancedf.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/tests/test_cbps.py` & `balance-0.7.0/tests/test_cbps.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         target_df = pd.DataFrame({"a": (1, 2, 3, 4, 5, 6, 7, 8, 9, 9)})
         sample_weights = pd.Series((1,) * 10)
         target_weights = pd.Series((1,) * 10)
         result_cbps = balance_cbps.cbps(
             sample_df, sample_weights, target_df, target_weights, transformations=None
         )
         self.assertEqual(
-            result_adjust.df["weight"], result_cbps["weights"].rename("weight")
+            result_adjust.df["weight"], result_cbps["weight"].rename("weight")
         )
 
     def test_logit_truncated(self):
         X = np.array([[1, 2, 3], [4, 5, 6], [0, 0, -100]])
         beta = np.array([1, 0.5, 1])
         result = balance_cbps.logit_truncated(X, beta)
         self.assertEqual(
@@ -265,21 +265,21 @@
 
         res = balance_cbps.cbps(sample_df, sample_weights, target_df, target_weights)
 
         # Compare output weights (examples and distribution)
         # TODO: The results are not 100% reproducible due to rounding issues in SVD that produce slightly different U:
         # http://numpy-discussion.10968.n7.nabble.com/strange-behavior-of-numpy-random-multivariate-normal-ticket-1842-td31547.html
         # This results in slightly different optimizations solutions (that might have some randomness in them too).
-        # self.assertEqual(round(res["weights"][4],4), 4.3932)
-        # self.assertEqual(round(res["weights"][997],4), 0.7617)
-        # self.assertEqual(np.around(res["weights"].describe().values,4),
+        # self.assertEqual(round(res["weight"][4],4), 4.3932)
+        # self.assertEqual(round(res["weight"][997],4), 0.7617)
+        # self.assertEqual(np.around(res["weight"].describe().values,4),
         #                np.array([1.0000e+03, 1.0167e+00, 1.1340e+00, 3.0000e-04,
         #                          3.3410e-01, 6.8400e-01, 1.2317e+00, 7.4006e+00]))
         self.assertTrue(
-            res["weights"][995] < res["weights"][999]
+            res["weight"][995] < res["weight"][999]
         )  # these are obs with different a value
 
     # Test cbps constraints
     def test_cbps_constraints(self):
         sample_df = pd.DataFrame({"a": [-20] + [1] * 13 + [10] * 1})
         sample_weights = pd.Series((1,) * 15)
         target_df = pd.DataFrame({"a": [10] * 10 + [11] * 5})
@@ -292,57 +292,53 @@
             target_weights,
             transformations=None,
             max_de=None,
             weight_trimming_mean_ratio=None,
         )
 
         # Ensure that example df would produce DE > 1.5 if unconstrained
-        self.assertTrue(design_effect(unconconstrained_result["weights"]) > 1.5)
+        self.assertTrue(design_effect(unconconstrained_result["weight"]) > 1.5)
 
         # Same data but now with constraint produces desired design effect - for cbps_method = "over"
         de_constrained_result = balance_cbps.cbps(
             sample_df,
             sample_weights,
             target_df,
             target_weights,
             transformations=None,
             max_de=1.5,
             weight_trimming_mean_ratio=None,
         )
-        self.assertTrue(
-            round(design_effect(de_constrained_result["weights"]), 5) <= 1.5
-        )
+        self.assertTrue(round(design_effect(de_constrained_result["weight"]), 5) <= 1.5)
         # Same data but now with constraint produces desired design effect - for cbps_method = "exact"
         de_constrained_result = balance_cbps.cbps(
             sample_df,
             sample_weights,
             target_df,
             target_weights,
             transformations=None,
             max_de=1.5,
             weight_trimming_mean_ratio=None,
             cbps_method="exact",
         )
-        self.assertTrue(
-            round(design_effect(de_constrained_result["weights"]), 5) <= 1.5
-        )
+        self.assertTrue(round(design_effect(de_constrained_result["weight"]), 5) <= 1.5)
 
     def test_cbps_weights_order(self):
         sample = pd.DataFrame({"a": (1, 2, 3, 4, 5, 6, 7, 9, 1)})
         target = pd.DataFrame({"a": (1, 2, 3, 4, 5, 6, 7, 9, 9)})
 
         result = balance_cbps.cbps(
             sample_df=sample,
             sample_weights=pd.Series((1,) * 9),
             target_df=target,
             target_weights=pd.Series((1,) * 9),
             transformations=None,
         )
 
-        w = result["weights"].values
+        w = result["weight"].values
         self.assertEqual(round(w[0], 10), round(w[8], 10))
         self.assertTrue(w[0] < w[1])
         self.assertTrue(w[0] < w[7])
 
     def test_cbps_all_weight_identical(self):
         #  Test the check for identical weights
         np.random.seed(1)
@@ -350,15 +346,15 @@
         sample_df = pd.DataFrame({"a": np.random.normal(0, 1, n).reshape((n,))})
         sample_weights = pd.Series((1,) * n)
         target_df = sample_df
         target_weights = sample_weights
         result = balance_cbps.cbps(
             sample_df, sample_weights, target_df, target_weights, transformations=None
         )
-        self.assertTrue(np.var(result["weights"]) < 1e-10)
+        self.assertTrue(np.var(result["weight"]) < 1e-10)
 
         sample = Sample.from_frame(
             df=pd.DataFrame(
                 {"a": np.random.normal(0, 1, n).reshape((n,)), "id": range(0, n)}
             ),
             id_column="id",
         )
```

### Comparing `balance-0.6.0/tests/test_cli.py` & `balance-0.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/tests/test_datasets.py` & `balance-0.7.0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/tests/test_ipw.py` & `balance-0.7.0/tests/test_ipw.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             sample_df=sample,
             sample_weights=pd.Series((1,) * 9),
             target_df=target,
             target_weights=pd.Series((1,) * 9),
             transformations=None,
         )
 
-        w = result["weights"].values
+        w = result["weight"].values
 
         self.assertEqual(w[0], w[8])
         self.assertTrue(w[0] < w[1])
         self.assertTrue(w[0] < w[7])
 
     def test_ipw_sample_indicator(self):
         # TODO: verify this behavior of balance is sensible
@@ -362,18 +362,18 @@
 
         sample_weights = pd.Series(np.random.uniform(0, 1, size=n_sample))
         target_weights = pd.Series(np.random.uniform(0, 1, size=n_target))
 
         res = balance_ipw.ipw(sample_df, sample_weights, target_df, target_weights)
 
         # Compare output weights (examples and distribution)
-        self.assertEqual(round(res["weights"][15], 4), 0.0886)
-        self.assertEqual(round(res["weights"][995], 4), 0.2363)
+        self.assertEqual(round(res["weight"][15], 4), 0.0886)
+        self.assertEqual(round(res["weight"][995], 4), 0.2363)
         self.assertEqual(
-            np.around(res["weights"].describe().values, 4),
+            np.around(res["weight"].describe().values, 4),
             np.array([1000, 1.0167, 0.7108, 0.0001, 0.2349, 1.2151, 1.7077, 1.7077]),
         )
 
         # Compare properties of output model
         self.assertEqual(np.around(res["model"]["fit"]["lambda_1se"], 5), 0.00474)
         self.assertEqual(
             np.around(res["model"]["perf"]["prop_dev_explained"], 5), 0.77107
```

### Comparing `balance-0.6.0/tests/test_logging.py` & `balance-0.7.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/tests/test_poststratify.py` & `balance-0.7.0/tests/test_poststratify.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,41 +24,41 @@
             },
         )
         s_weights = pd.Series([4, 2, 1, 1])
         t = s
         t_weights = pd.Series([4, 2, 2, 8])
         result = poststratify(
             sample_df=s, sample_weights=s_weights, target_df=t, target_weights=t_weights
-        )["weights"]
+        )["weight"]
         self.assertEqual(result, t_weights.astype("float64"))
 
         # same example when dataframe of elements are all related to weights of one
         s = pd.DataFrame(
             {
                 "a": (0, 0, 0, 0, 1, 1, 0, 1),
                 "c": ("a", "a", "a", "a", "a", "a", "b", "b"),
             },
         )
         s_weights = pd.Series([1, 1, 1, 1, 1, 1, 1, 1])
         result = poststratify(
             sample_df=s, sample_weights=s_weights, target_df=t, target_weights=t_weights
-        )["weights"]
+        )["weight"]
         self.assertEqual(result, pd.Series((1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 2.0, 8.0)))
 
         # same example with normalized weights
         s = pd.DataFrame(
             {
                 "a": (0, 1, 0, 1),
                 "c": ("a", "a", "b", "b"),
             },
         )
         s_weights = pd.Series([1 / 2, 1 / 4, 1 / 8, 1 / 8])
         result = poststratify(
             sample_df=s, sample_weights=s_weights, target_df=t, target_weights=t_weights
-        )["weights"]
+        )["weight"]
         self.assertEqual(result, t_weights.astype("float64"))
 
         # test through adjustment
         # TODO: test the previous example through adjustment as well
         sample = Sample.from_frame(
             df=pd.DataFrame(
                 {
@@ -110,15 +110,15 @@
         t_weights = pd.Series([4, 2, 2, 8])
         result = poststratify(
             sample_df=s,
             sample_weights=s_weights,
             target_df=t,
             target_weights=t_weights,
             variables=["a"],
-        )["weights"]
+        )["weight"]
         self.assertEqual(result, pd.Series([4.0, 4.0, 2.0, 6.0]))
 
     def test_poststratify_transformations(self):
         # for numeric
         size = 10000
         s = pd.DataFrame({"age": np.random.uniform(0, 1, size)})
         tmp = int(size * 0.2)
@@ -133,15 +133,15 @@
             }
         )
         result = poststratify(
             sample_df=s,
             sample_weights=pd.Series([1] * size),
             target_df=t,
             target_weights=pd.Series([1] * size),
-        )["weights"]
+        )["weight"]
 
         # age>0.4 has 4 times as many people than age <0.4 in the target
         # Check that the weights come out as 0.2 and 0.8
         eps = 0.05
         self.assertTrue(abs(result[s.age < 0.4].sum() / size - 0.2) < eps)
         self.assertTrue(abs(result[s.age >= 0.4].sum() / size - 0.8) < eps)
 
@@ -154,15 +154,15 @@
             {"x": np.random.choice(("a", "b", "c"), size, p=(0.95, 0.015, 0.035))}
         )
         result = poststratify(
             sample_df=s,
             sample_weights=pd.Series([1] * size),
             target_df=t,
             target_weights=pd.Series([1] * size),
-        )["weights"]
+        )["weight"]
 
         # Output weights should ignore the difference between values 'b' and 'c'
         # since these are combined in default transformations (into '_lumped_other').
         # Hence their frequency would be as in sample
         eps = 0.05
         self.assertTrue(abs(result[s.x == "a"].sum() / size - 0.95) < eps)
         self.assertTrue(abs(result[s.x == "b"].sum() / size - 0.035) < eps)
```

### Comparing `balance-0.6.0/tests/test_sample.py` & `balance-0.7.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/tests/test_stats_and_plots.py` & `balance-0.7.0/tests/test_stats_and_plots.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/tests/test_testutil.py` & `balance-0.7.0/tests/test_testutil.py`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/tests/test_util.py` & `balance-0.7.0/tests/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -889,14 +889,32 @@
         #  PandasDtype('object'),
         #  PandasDtype('float64'),
         #  PandasDtype('object'),
         #  StringDtype,
         #  dtype('float64'),
         #  dtype('<U32')]
 
+        # Preserve index in pd.Series input
+        x1 = pd.Series([1, 2, 3, 4])
+        x2 = pd.Series([np.nan, 2, 3, 4])
+        x3 = np.array([1, 2, 3, 4])
+        # When there is nothing to remove, the original pd.Series will be returned with proper index:
+        self.assertEqual(rm_mutual_nas(x1, x3)[0].to_dict(), {0: 1, 1: 2, 2: 3, 3: 4})
+        self.assertEqual(
+            rm_mutual_nas(x1.sort_values(ascending=False), x3)[0].to_dict(),
+            {3: 4, 2: 3, 1: 2, 0: 1},
+        )
+        # Index is not changed also when na values are omitted:
+        self.assertEqual(rm_mutual_nas(x1, x2)[0].to_dict(), {1: 2, 2: 3, 3: 4})
+        # The order of the Series can be is changed, but the indexes remain the same
+        self.assertEqual(
+            rm_mutual_nas(x1.sort_values(ascending=False), x2)[0].to_dict(),
+            {3: 4, 2: 3, 1: 2},
+        )
+
     def test_choose_variables(self):
         from balance.util import choose_variables
 
         # For one dataframe
         self.assertEqual(
             choose_variables(pd.DataFrame({"a": [1], "b": [2]})),
             ["a", "b"],
```

### Comparing `balance-0.6.0/tests/test_weighted_comparisons_plots.py` & `balance-0.7.0/tests/test_weighted_comparisons_plots.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,14 +46,75 @@
 )
 
 
 # TODO: split out the weighted_stats.relative_frequency_table function.
 class Test_weighted_comparisons_plots(
     balance.testutil.BalanceTestCase,
 ):
+    def test_plot__return_sample_palette(self):
+        from balance.stats_and_plots.weighted_comparisons_plots import (
+            _return_sample_palette,
+        )
+
+        self.assertEqual(
+            _return_sample_palette(["self", "target"]),
+            {"self": "#de2d26cc", "target": "#9ecae1cc"},
+        )
+        self.assertEqual(
+            _return_sample_palette(["self", "unadjusted"]),
+            {"self": "#34a53080", "unadjusted": "#de2d26cc"},
+        )
+        self.assertEqual(
+            _return_sample_palette(["self", "unadjusted", "target"]),
+            {"self": "#34a53080", "unadjusted": "#de2d26cc", "target": "#9ecae1cc"},
+        )
+        self.assertEqual(
+            _return_sample_palette(["adjusted", "unadjusted", "target"]),
+            {"adjusted": "#34a53080", "unadjusted": "#de2d26cc", "target": "#9ecae1cc"},
+        )
+        self.assertEqual(_return_sample_palette(["cat", "dog"]), "muted")
+
+    def test_plot__plotly_marker_color(self):
+        from balance.stats_and_plots.weighted_comparisons_plots import (
+            _plotly_marker_color,
+        )
+
+        self.assertEqual(
+            _plotly_marker_color("self", True, "color"), "rgba(222,45,38,0.8)"
+        )
+        self.assertEqual(
+            _plotly_marker_color("self", False, "color"), "rgba(52,165,48,0.5)"
+        )
+        self.assertEqual(
+            _plotly_marker_color("self", True, "line"), "rgba(222,45,38,1)"
+        )
+        self.assertEqual(
+            _plotly_marker_color("self", False, "line"), "rgba(52,165,48,1)"
+        )
+
+        self.assertEqual(
+            _plotly_marker_color("target", True, "color"), "rgb(158,202,225,0.8)"
+        )
+        self.assertEqual(
+            _plotly_marker_color("target", False, "color"), "rgb(158,202,225,0.8)"
+        )
+        self.assertEqual(
+            _plotly_marker_color("target", True, "line"), "rgb(158,202,225,1)"
+        )
+        self.assertEqual(
+            _plotly_marker_color("target", False, "line"), "rgb(158,202,225,1)"
+        )
+
+        self.assertEqual(
+            _plotly_marker_color("adjusted", False, "color"), "rgba(52,165,48,0.5)"
+        )
+        self.assertEqual(
+            _plotly_marker_color("adjusted", False, "line"), "rgba(52,165,48,1)"
+        )
+
     def test_plot_bar(self):
         import matplotlib.pyplot as plt
         from balance.stats_and_plots.weighted_comparisons_plots import plot_bar
 
         df = pd.DataFrame(
             {
                 "group": ("a", "b", "c", "c"),
@@ -62,31 +123,31 @@
         )
 
         plt.figure(1)
         fig, ax = plt.subplots(1, 1, figsize=(7.2, 7.2))
 
         plot_bar(
             [
-                {"df": df, "weights": pd.Series((1, 1, 1, 1))},
-                {"df": df, "weights": pd.Series((2, 1, 1, 1))},
+                {"df": df, "weight": pd.Series((1, 1, 1, 1))},
+                {"df": df, "weight": pd.Series((2, 1, 1, 1))},
             ],
             names=["self", "target"],
             column="group",
             axis=ax,
             weighted=True,
         )
 
         self.assertIn("barplot of covar ", ax.get_title())
 
     def test_plot_dist_weighted_kde_error(self):
         df4 = {
             "df": pd.DataFrame(
                 {"numeric_5": pd.Series([0, 0, 0, 0, 0, 1, 1, 2, 3, 4])}
             ),
-            "weights": pd.Series([0, 0, 0, 0, 0, 0, 0, 0, 0, 5]),
+            "weight": pd.Series([0, 0, 0, 0, 0, 0, 0, 0, 0, 5]),
         }
 
         plot_dist_type = type(
             weighted_comparisons_plots.plot_dist(
                 (df4,),
                 dist_type="kde",
                 numeric_n_values_threshold=0,
@@ -172,15 +233,15 @@
         )
 
     def test_seaborn_plot_dist(self):
         df4 = {
             "df": pd.DataFrame(
                 {"numeric_5": pd.Series([0, 0, 0, 0, 0, 1, 1, 2, 3, 4])}
             ),
-            "weights": pd.Series([0, 0, 0, 0, 0, 0, 0, 0, 0, 5]),
+            "weight": pd.Series([0, 0, 0, 0, 0, 0, 0, 0, 0, 5]),
         }
 
         # Check that we get a list of matplotlib axes
         out = []
         for dist_type in ("hist", "kde", "qq", "ecdf"):
             out.append(
                 type(
@@ -213,17 +274,17 @@
                 "v1": random.random_integers(11111, 11114, size=100).astype(str),
                 "v2": random.normal(size=100),
                 "v3": random.uniform(size=100),
             }
         ).sort_values(by=["v2"])
 
         dfs1 = [
-            {"df": df, "weights": pd.Series(np.ones(100))},
-            {"df": df, "weights": pd.Series(np.ones(99).tolist() + [1000])},
-            {"df": df, "weights": pd.Series(np.ones(100))},
+            {"df": df, "weight": pd.Series(np.ones(100))},
+            {"df": df, "weight": pd.Series(np.ones(99).tolist() + [1000])},
+            {"df": df, "weight": pd.Series(np.ones(100))},
         ]
 
         # If plot_it=False and
         self.assertTrue(
             plot_dist(
                 dfs1,
                 names=["self", "unadjusted", "target"],
```

### Comparing `balance-0.6.0/tutorials/balance_quickstart.ipynb` & `balance-0.7.0/tutorials/balance_quickstart.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999069940476191%*

 * *Differences: {"'cells'": "{23: {'source': {insert: [(0, 'We can use `.covars()` and then followup with "*

 * *            '`.mean()` and `.plot()` (barplots and kde density plots) to get some basic '*

 * *            "diagnostics on what we got.\\n')], delete: [0]}}}"}*

```diff
@@ -342,15 +342,15 @@
         {
             "cell_type": "markdown",
             "metadata": {
                 "originalKey": "debd7a86-d3bc-4555-ab29-eb5380b90119",
                 "showInput": false
             },
             "source": [
-                "We can use `.covars()` and then followup with `.mean()` and `.plot()` (barplots and qqplots) to get some basic diagnostics on what we got.\n",
+                "We can use `.covars()` and then followup with `.mean()` and `.plot()` (barplots and kde density plots) to get some basic diagnostics on what we got.\n",
                 "\n",
                 "We can see how:\n",
                 "- The proportion of missing values in gender is similar in sample and target.\n",
                 "- We have younger people in the sample as compared to the target.\n",
                 "- We have more females than males in the sample, as compared to around 50-50 split for the (non NA) target.\n",
                 "- Income is more right skewed in the target as compared to the sample."
             ]
```

### Comparing `balance-0.6.0/tutorials/balance_quickstart_cbps.ipynb` & `balance-0.7.0/tutorials/balance_quickstart_cbps.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999799061214%*

 * *Differences: {"'cells'": "{27: {'outputs': {2: {'data': {'application/vnd.plotly.v1+json': {'layout': {'title': "*

 * *            "{'text': 'KDE density Plots of income'}}}}}}}}"}*

```diff
@@ -7223,15 +7223,15 @@
                                             },
                                             "zerolinecolor": "white",
                                             "zerolinewidth": 2
                                         }
                                     }
                                 },
                                 "title": {
-                                    "text": "QQ Plots of income"
+                                    "text": "KDE density Plots of income"
                                 },
                                 "xaxis": {
                                     "autorange": true,
                                     "linewidth": 1,
                                     "mirror": true,
                                     "range": [
                                         -4.857309021410357,
```

### Comparing `balance-0.6.0/tutorials/balance_transformations_and_formulas.ipynb` & `balance-0.7.0/tutorials/balance_transformations_and_formulas.ipynb`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.ipynb` & `balance-0.7.0/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.ipynb`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/README.md` & `balance-0.7.0/website/README.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/blog/2023/01/09/bringing-balance-to-your-data.md` & `balance-0.7.0/website/blog/2023/01/09/bringing-balance-to-your-data.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/blog/2023/01/09/sample_vs_target_bar_chart.webp` & `balance-0.7.0/website/blog/2023/01/09/sample_vs_target_bar_chart.webp`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/general_framework/adjusting_sample_to_population.md` & `balance-0.7.0/website/docs/docs/general_framework/adjusting_sample_to_population.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/general_framework/evaluation_of_results.md` & `balance-0.7.0/website/docs/docs/general_framework/evaluation_of_results.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/general_framework/general_framework.md` & `balance-0.7.0/website/docs/docs/general_framework/general_framework.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/general_framework/pre_adjustment_diagnostics.md` & `balance-0.7.0/website/docs/docs/general_framework/pre_adjustment_diagnostics.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/fig_01_qqplot_income_before.png` & `balance-0.7.0/website/docs/docs/img/fig_01_qqplot_income_before.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/fig_02_barplot_age_before.png` & `balance-0.7.0/website/docs/docs/img/fig_02_barplot_age_before.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/fig_03_barplot_gender_before.png` & `balance-0.7.0/website/docs/docs/img/fig_03_barplot_gender_before.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/fig_04_qqplot_income_after.png` & `balance-0.7.0/website/docs/docs/img/fig_04_qqplot_income_after.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/fig_05_barplot_age_after.png` & `balance-0.7.0/website/docs/docs/img/fig_05_barplot_age_after.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/fig_06_barplot_gender_after.png` & `balance-0.7.0/website/docs/docs/img/fig_06_barplot_gender_after.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/fig_07_seaborn_after.png` & `balance-0.7.0/website/docs/docs/img/fig_07_seaborn_after.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/fig_08_weights_kde.png` & `balance-0.7.0/website/docs/docs/img/fig_08_weights_kde.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/fig_09_seaborn_outcome_kde_after.png` & `balance-0.7.0/website/docs/docs/img/fig_09_seaborn_outcome_kde_after.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/total_survey_error_flow_v02.png` & `balance-0.7.0/website/docs/docs/img/total_survey_error_flow_v02.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/total_survey_error_flow_v02.svg` & `balance-0.7.0/website/docs/docs/img/total_survey_error_flow_v02.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/total_survey_error_image.png` & `balance-0.7.0/website/docs/docs/img/total_survey_error_image.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/img/total_survey_error_image.svg` & `balance-0.7.0/website/docs/docs/img/total_survey_error_image.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/statistical_methods/cbps.md` & `balance-0.7.0/website/docs/docs/statistical_methods/cbps.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/statistical_methods/ipw.md` & `balance-0.7.0/website/docs/docs/statistical_methods/ipw.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/docs/statistical_methods/poststratify.md` & `balance-0.7.0/website/docs/docs/statistical_methods/poststratify.md`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.mdx` & `balance-0.7.0/website/docs/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.mdx`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docs/tutorials/index.mdx` & `balance-0.7.0/website/docs/tutorials/index.mdx`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/docusaurus.config.js` & `balance-0.7.0/website/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/package.json` & `balance-0.7.0/website/package.json`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/sidebars.js` & `balance-0.7.0/website/sidebars.js`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/src/components/HTMLLoader.js` & `balance-0.7.0/website/src/components/HTMLLoader.js`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/src/components/HomepageFeatures.js` & `balance-0.7.0/website/src/components/HomepageFeatures.js`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/src/css/custom.css` & `balance-0.7.0/website/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/src/pages/index.js` & `balance-0.7.0/website/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/src/pages/index.module.css` & `balance-0.7.0/website/src/pages/index.module.css`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/AI/balance_Logo_FINAL.ai` & `balance-0.7.0/website/static/img/balance_logo/AI/balance_Logo_FINAL.ai`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_Black_RGB.png` & `balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_Black_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png` & `balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_White_RGB.png` & `balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_White_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_Black_RGB.png` & `balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_Black_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_FullColor_RGB.png` & `balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_FullColor_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_White_RGB.png` & `balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_White_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_Black_RGB.png` & `balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_Black_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_FullColor_RGB.png` & `balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_FullColor_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_White_RGB.png` & `balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_White_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_Black_RGB.svg` & `balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_Black_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.svg` & `balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_White_RGB.svg` & `balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_White_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_Black_RGB.svg` & `balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_Black_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_FullColor_RGB.svg` & `balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_FullColor_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_White_RGB.svg` & `balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_White_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_Black_RGB.svg` & `balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_Black_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_FullColor_RGB.svg` & `balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_FullColor_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_White_RGB.svg` & `balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_White_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/icon.png` & `balance-0.7.0/website/static/img/balance_logo/icon.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/icon.svg` & `balance-0.7.0/website/static/img/balance_logo/icon.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/vertical.svg` & `balance-0.7.0/website/static/img/balance_logo/vertical.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/balance_logo/vertical_white.svg` & `balance-0.7.0/website/static/img/balance_logo/vertical_white.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/docusaurus.png` & `balance-0.7.0/website/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/favicon.ico` & `balance-0.7.0/website/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/fontawesome/code.svg` & `balance-0.7.0/website/static/img/fontawesome/code.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/fontawesome/layer-group.svg` & `balance-0.7.0/website/static/img/fontawesome/layer-group.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/fontawesome/users.svg` & `balance-0.7.0/website/static/img/fontawesome/users.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/logo.svg` & `balance-0.7.0/website/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/meta_opensource_logo_negative.svg` & `balance-0.7.0/website/static/img/meta_opensource_logo_negative.svg`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/tutorial/docsVersionDropdown.png` & `balance-0.7.0/website/static/img/tutorial/docsVersionDropdown.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/static/img/tutorial/localeDropdown.png` & `balance-0.7.0/website/static/img/tutorial/localeDropdown.png`

 * *Files identical despite different names*

### Comparing `balance-0.6.0/website/yarn.lock` & `balance-0.7.0/website/yarn.lock`

 * *Files identical despite different names*


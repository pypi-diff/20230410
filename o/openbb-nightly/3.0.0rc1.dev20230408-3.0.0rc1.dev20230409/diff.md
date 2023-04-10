# Comparing `tmp/openbb_nightly-3.0.0rc1.dev20230408.tar.gz` & `tmp/openbb_nightly-3.0.0rc1.dev20230409.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-3.0.0rc1.dev20230408.tar", max compression
+gzip compressed data, was "openbb_nightly-3.0.0rc1.dev20230409.tar", max compression
```

## Comparing `openbb_nightly-3.0.0rc1.dev20230408.tar` & `openbb_nightly-3.0.0rc1.dev20230409.tar`

### file list

```diff
@@ -1,954 +1,964 @@
--rw-r--r--   0        0        0     1073 2023-04-08 00:08:53.724399 openbb_nightly-3.0.0rc1.dev20230408/LICENSE
--rw-r--r--   0        0        0    18588 2023-04-08 00:08:53.880403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/SDK_README.md
--rw-r--r--   0        0        0      243 2023-04-08 00:08:53.880403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/__init__.py
--rw-r--r--   0        0        0    20243 2023-04-08 00:08:53.880403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/account/account_controller.py
--rw-r--r--   0        0        0     3480 2023-04-08 00:08:53.880403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/account/account_model.py
--rw-r--r--   0        0        0      612 2023-04-08 00:08:53.880403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/account/account_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.880403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/__init__.py
--rw-r--r--   0        0        0     3131 2023-04-08 00:08:53.880403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/alt_controller.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.880403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/covid/__init__.py
--rw-r--r--   0        0        0     1881 2023-04-08 00:08:53.880403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/covid/countries.txt
--rw-r--r--   0        0        0     9347 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/covid/covid_controller.py
--rw-r--r--   0        0        0     5387 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/covid/covid_model.py
--rw-r--r--   0        0        0     8586 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/covid/covid_view.py
--rw-r--r--   0        0        0     1070 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/hackernews_model.py
--rw-r--r--   0        0        0     1087 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/hackernews_view.py
--rw-r--r--   0        0        0     6752 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/oss/github_model.py
--rw-r--r--   0        0        0     3968 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/oss/github_view.py
--rw-r--r--   0        0        0     8656 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/oss/oss_controller.py
--rw-r--r--   0        0        0     4437 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/oss/runa_model.py
--rw-r--r--   0        0        0     4018 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/oss/runa_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/realestate/__init__.py
--rw-r--r--   0        0        0     9030 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/realestate/landRegistry_model.py
--rw-r--r--   0        0        0     3309 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/realestate/landRegistry_view.py
--rw-r--r--   0        0        0     8108 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/realestate/realestate_controller.py
--rw-r--r--   0        0        0     2718 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/base_helpers.py
--rw-r--r--   0        0        0       93 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/finbrain_model.py
--rw-r--r--   0        0        0     4394 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/finbrain_view.py
--rw-r--r--   0        0        0     1335 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/finnhub_model.py
--rw-r--r--   0        0        0     1861 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/finnhub_view.py
--rw-r--r--   0        0        0     3329 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/google_model.py
--rw-r--r--   0        0        0     7118 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/google_view.py
--rw-r--r--   0        0        0     5524 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/reddit_helpers.py
--rw-r--r--   0        0        0    18297 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/reddit_model.py
--rw-r--r--   0        0        0    10206 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/reddit_view.py
--rw-r--r--   0        0        0     3239 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/stocktwits_model.py
--rw-r--r--   0        0        0     2898 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/stocktwits_view.py
--rw-r--r--   0        0        0     6160 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/twitter_model.py
--rw-r--r--   0        0        0     5870 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/twitter_view.py
--rw-r--r--   0        0        0     4142 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/common_model.py
--rw-r--r--   0        0        0     3634 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/feedparser_model.py
--rw-r--r--   0        0        0     1242 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/feedparser_view.py
--rw-r--r--   0        0        0     2639 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/newsapi_model.py
--rw-r--r--   0        0        0     1465 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/newsapi_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    19923 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/quantitative_analysis/qa_model.py
--rw-r--r--   0        0        0    32308 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/quantitative_analysis/qa_view.py
--rw-r--r--   0        0        0     3226 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/quantitative_analysis/rolling_model.py
--rw-r--r--   0        0        0    10790 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/quantitative_analysis/rolling_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/__init__.py
--rw-r--r--   0        0        0     2977 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/custom_indicators_model.py
--rw-r--r--   0        0        0     4272 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/custom_indicators_view.py
--rw-r--r--   0        0        0     6427 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/momentum_model.py
--rw-r--r--   0        0        0    10556 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/momentum_view.py
--rw-r--r--   0        0        0     4179 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/overlap_model.py
--rw-r--r--   0        0        0     4361 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/overlap_view.py
--rw-r--r--   0        0        0     1453 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/ta_helpers.py
--rw-r--r--   0        0        0     1819 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/trend_indicators_model.py
--rw-r--r--   0        0        0     2621 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/trend_indicators_view.py
--rw-r--r--   0        0        0    19962 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/volatility_model.py
--rw-r--r--   0        0        0    10008 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/volatility_view.py
--rw-r--r--   0        0        0     2614 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/volume_model.py
--rw-r--r--   0        0        0     3806 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/volume_view.py
--rw-r--r--   0        0        0     5424 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/ultima_newsmonitor_model.py
--rw-r--r--   0        0        0     3885 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/ultima_newsmonitor_view.py
--rw-r--r--   0        0        0     2634 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/config_terminal.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/__init__.py
--rw-r--r--   0        0        0     9829 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/completer/choices.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/config/__init__.py
--rw-r--r--   0        0        0      860 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/config/paths.py
--rw-r--r--   0        0        0     2650 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/config/paths_helper.py
--rw-r--r--   0        0        0     9162 2023-04-08 00:08:53.884403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/integration_tests/README.md
--rw-r--r--   0        0        0    21758 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/integration_tests/integration_controller.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/collection/__init__.py
--rw-r--r--   0        0        0     3848 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/collection/log_sender.py
--rw-r--r--   0        0        0     3744 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/collection/logging_clock.py
--rw-r--r--   0        0        0     3495 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/collection/s3_sender.py
--rw-r--r--   0        0        0      166 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/constants.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/__init__.py
--rw-r--r--   0        0        0      524 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/common.py
--rw-r--r--   0        0        0      525 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/custom_logger.py
--rw-r--r--   0        0        0      979 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/directories.py
--rw-r--r--   0        0        0      841 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/expired_files.py
--rw-r--r--   0        0        0     4896 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/formatter_with_exceptions.py
--rw-r--r--   0        0        0     6058 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4166 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/settings.py
--rw-r--r--   0        0        0     1621 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/settings_logger.py
--rw-r--r--   0        0        0      396 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/user_logger.py
--rw-r--r--   0        0        0      627 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/__init__.py
--rw-r--r--   0        0        0     1221 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/base_model.py
--rw-r--r--   0        0        0      818 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/credentials_model.py
--rw-r--r--   0        0        0     4154 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/preferences_model.py
--rw-r--r--   0        0        0     1817 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/profile_model.py
--rw-r--r--   0        0        0     1113 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/sources_model.py
--rw-r--r--   0        0        0     1753 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/system_model.py
--rw-r--r--   0        0        0      562 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/user_model.py
--rw-r--r--   0        0        0      200 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/__init__.py
--rw-r--r--   0        0        0   418780 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/assets/Terminal_icon.png
--rw-r--r--   0        0        0      727 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/assets/icon.png
--rw-r--r--   0        0        0    14854 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/backend.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/config/__init__.py
--rw-r--r--   0        0        0     7156 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/config/openbb_styles.py
--rw-r--r--   0        0        0     3073 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/no_import.py
--rw-r--r--   0        0        0     1261 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/old_table.html
--rw-r--r--   0        0        0     7732 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly.html
--rw-r--r--   0        0        0    62668 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_helper.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/__init__.py
--rw-r--r--   0        0        0     6724 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/base.py
--rw-r--r--   0        0        0    11358 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/data_classes.py
--rw-r--r--   0        0        0     8016 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    15173 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3361 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5683 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6868 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3429 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    20644 2023-04-08 00:08:53.888403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/ta_class.py
--rw-r--r--   0        0        0   704570 2023-04-08 00:08:53.892403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/table.html
--rw-r--r--   0        0        0    11182 2023-04-08 00:08:53.892403 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/bar_menus.js
--rw-r--r--   0        0        0   289624 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf
--rw-r--r--   0        0        0   286320 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf
--rw-r--r--   0        0        0    25188 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/css/style.css
--rw-r--r--   0        0        0      151 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/css/table.css
--rw-r--r--   0        0        0    16611 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/helpers.js
--rw-r--r--   0        0        0    12724 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/main.js
--rw-r--r--   0        0        0     3255 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/main_table.js
--rw-r--r--   0        0        0    24525 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/popups.js
--rw-r--r--   0        0        0     7747 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/scripts/sdk_audit.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/__init__.py
--rw-r--r--   0        0        0      450 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/__init__.py
--rw-r--r--   0        0        0     2660 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py
--rw-r--r--   0        0        0    24088 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py
--rw-r--r--   0        0        0     1513 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py
--rw-r--r--   0        0        0     2365 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py
--rw-r--r--   0        0        0     5128 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py
--rw-r--r--   0        0        0    18676 2023-04-08 00:08:53.896404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py
--rw-r--r--   0        0        0      761 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/__init__.py
--rw-r--r--   0        0        0     4308 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/alt_sdk_model.py
--rw-r--r--   0        0        0    42910 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/crypto_sdk_model.py
--rw-r--r--   0        0        0     4497 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/econometrics_sdk_model.py
--rw-r--r--   0        0        0     7975 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/economy_sdk_model.py
--rw-r--r--   0        0        0     2496 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/etf_sdk_model.py
--rw-r--r--   0        0        0     3515 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py
--rw-r--r--   0        0        0     8550 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/forecast_sdk_model.py
--rw-r--r--   0        0        0     4386 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/forex_sdk_model.py
--rw-r--r--   0        0        0     1530 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/funds_sdk_model.py
--rw-r--r--   0        0        0     1067 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/futures_sdk_model.py
--rw-r--r--   0        0        0     3662 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/keys_sdk_model.py
--rw-r--r--   0        0        0    10046 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/portfolio_sdk_model.py
--rw-r--r--   0        0        0     4603 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/qa_sdk_model.py
--rw-r--r--   0        0        0    33128 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/stocks_sdk_model.py
--rw-r--r--   0        0        0     7229 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/ta_sdk_model.py
--rw-r--r--   0        0        0    11508 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/sdk_helpers.py
--rw-r--r--   0        0        0    20021 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/sdk_init.py
--rw-r--r--   0        0        0    44206 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/trail_map.csv
--rw-r--r--   0        0        0     2801 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/trail_map_forecasting.csv
--rw-r--r--   0        0        0     1301 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/trail_map_optimization.csv
--rw-r--r--   0        0        0     7118 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/trailmap.py
--rw-r--r--   0        0        0     1017 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/banner.txt
--rw-r--r--   0        0        0      485 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/constants.py
--rw-r--r--   0        0        0     1000 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/current_system.py
--rw-r--r--   0        0        0     4179 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/current_user.py
--rw-r--r--   0        0        0     1147 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/env_handler.py
--rw-r--r--   0        0        0    20476 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/hub_model.py
--rw-r--r--   0        0        0     7856 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/local_model.py
--rw-r--r--   0        0        0     3123 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/sdk_session.py
--rw-r--r--   0        0        0     2913 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/session_controller.py
--rw-r--r--   0        0        0     3960 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/session_model.py
--rw-r--r--   0        0        0     1065 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/sources_handler.py
--rw-r--r--   0        0        0     1268 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/utils.py
--rw-r--r--   0        0        0     3011 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sources/utils.py
--rw-r--r--   0        0        0      199 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/README.md
--rw-r--r--   0        0        0       84 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/__init__.py
--rw-r--r--   0        0        0     5303 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/coinbase_helpers.py
--rw-r--r--   0        0        0     2147 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/coinpaprika_helpers.py
--rw-r--r--   0        0        0    19275 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/crypto_controller.py
--rw-r--r--   0        0        0     4481 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/crypto_models.py
--rw-r--r--   0        0        0     1785 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/crypto_views.py
--rw-r--r--   0        0        0    30339 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py
--rw-r--r--   0        0        0      949 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/README.md
--rw-r--r--   0        0        0     7341 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/binance_gecko_map.json
--rw-r--r--   0        0        0     2436 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json
--rw-r--r--   0        0        0     4813 2023-04-08 00:08:53.900404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/coingecko_categories.json
--rw-r--r--   0        0        0   954385 2023-04-08 00:08:53.904404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/coingecko_coins.json
--rw-r--r--   0        0        0  2245016 2023-04-08 00:08:53.912404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json
--rw-r--r--   0        0        0    31307 2023-04-08 00:08:53.912404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/defillama_dapps.json
--rw-r--r--   0        0        0   107203 2023-04-08 00:08:53.912404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/erc20_coins.json
--rw-r--r--   0        0        0     7255 2023-04-08 00:08:53.912404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/finbrain_coins.json
--rw-r--r--   0        0        0   222978 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/santiment_slugs.json
--rw-r--r--   0        0        0   300253 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json
--rw-r--r--   0        0        0     4951 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/dataframe_helpers.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/__init__.py
--rw-r--r--   0        0        0     4537 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/coindix_model.py
--rw-r--r--   0        0        0     2720 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/coindix_view.py
--rw-r--r--   0        0        0     2483 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py
--rw-r--r--   0        0        0     1994 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py
--rw-r--r--   0        0        0    31284 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/defi_controller.py
--rw-r--r--   0        0        0     8918 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/graph_model.py
--rw-r--r--   0        0        0     7165 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/graph_view.py
--rw-r--r--   0        0        0     5005 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/llama_model.py
--rw-r--r--   0        0        0     5827 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/llama_view.py
--rw-r--r--   0        0        0     1808 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/smartstake_model.py
--rw-r--r--   0        0        0     3110 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/smartstake_view.py
--rw-r--r--   0        0        0     2882 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/substack_model.py
--rw-r--r--   0        0        0     1090 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/substack_view.py
--rw-r--r--   0        0        0     1947 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/terraengineer_model.py
--rw-r--r--   0        0        0     2699 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/terraengineer_view.py
--rw-r--r--   0        0        0     9734 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py
--rw-r--r--   0        0        0     8022 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/__init__.py
--rw-r--r--   0        0        0     2317 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py
--rw-r--r--   0        0        0     1620 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py
--rw-r--r--   0        0        0     2116 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py
--rw-r--r--   0        0        0     1936 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py
--rw-r--r--   0        0        0     7614 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/dappradar_model.py
--rw-r--r--   0        0        0     5045 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/dappradar_view.py
--rw-r--r--   0        0        0    21019 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/discovery_controller.py
--rw-r--r--   0        0        0    10833 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py
--rw-r--r--   0        0        0     6352 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py
--rw-r--r--   0        0        0     1095 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/__init__.py
--rw-r--r--   0        0        0     7483 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/binance_model.py
--rw-r--r--   0        0        0     3009 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/binance_view.py
--rw-r--r--   0        0        0     3188 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py
--rw-r--r--   0        0        0     2840 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py
--rw-r--r--   0        0        0     6439 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py
--rw-r--r--   0        0        0     4134 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py
--rw-r--r--   0        0        0     6587 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py
--rw-r--r--   0        0        0     6638 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py
--rw-r--r--   0        0        0    15062 2023-04-08 00:08:53.916404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py
--rw-r--r--   0        0        0     9133 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py
--rw-r--r--   0        0        0     2332 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py
--rw-r--r--   0        0        0    64101 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py
--rw-r--r--   0        0        0     1850 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py
--rw-r--r--   0        0        0     4333 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py
--rw-r--r--   0        0        0    15044 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py
--rw-r--r--   0        0        0    11237 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py
--rw-r--r--   0        0        0    24480 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/messari_model.py
--rw-r--r--   0        0        0    22260 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/messari_view.py
--rw-r--r--   0        0        0    25887 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py
--rw-r--r--   0        0        0     8762 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py
--rw-r--r--   0        0        0     3076 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py
--rw-r--r--   0        0        0     2070 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py
--rw-r--r--   0        0        0     2508 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py
--rw-r--r--   0        0        0     6001 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py
--rw-r--r--   0        0        0     3474 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/__init__.py
--rw-r--r--   0        0        0     5562 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/nft_controller.py
--rw-r--r--   0        0        0     1664 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py
--rw-r--r--   0        0        0     4495 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py
--rw-r--r--   0        0        0     2895 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/opensea_model.py
--rw-r--r--   0        0        0     1289 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/opensea_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/__init__.py
--rw-r--r--   0        0        0    21848 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/bitquery_model.py
--rw-r--r--   0        0        0    11444 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/bitquery_view.py
--rw-r--r--   0        0        0     3393 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/blockchain_model.py
--rw-r--r--   0        0        0     4733 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/blockchain_view.py
--rw-r--r--   0        0        0     1840 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py
--rw-r--r--   0        0        0     1266 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py
--rw-r--r--   0        0        0    15974 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py
--rw-r--r--   0        0        0    10572 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py
--rw-r--r--   0        0        0    53494 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/onchain_controller.py
--rw-r--r--   0        0        0     5938 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/shroom_model.py
--rw-r--r--   0        0        0     5144 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/shroom_view.py
--rw-r--r--   0        0        0     4772 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py
--rw-r--r--   0        0        0     2088 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/__init__.py
--rw-r--r--   0        0        0     2274 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py
--rw-r--r--   0        0        0     2664 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py
--rw-r--r--   0        0        0     1464 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/coinbase_model.py
--rw-r--r--   0        0        0     1342 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/coinbase_view.py
--rw-r--r--   0        0        0    11841 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py
--rw-r--r--   0        0        0     9646 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py
--rw-r--r--   0        0        0     6776 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py
--rw-r--r--   0        0        0     2278 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py
--rw-r--r--   0        0        0     1100 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/glassnode_model.py
--rw-r--r--   0        0        0     4677 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/glassnode_view.py
--rw-r--r--   0        0        0     5936 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/loanscan_model.py
--rw-r--r--   0        0        0     3279 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/loanscan_view.py
--rw-r--r--   0        0        0    55381 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/overview_controller.py
--rw-r--r--   0        0        0    13641 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py
--rw-r--r--   0        0        0    21320 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py
--rw-r--r--   0        0        0     5346 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/rekt_model.py
--rw-r--r--   0        0        0     2253 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/rekt_view.py
--rw-r--r--   0        0        0     2042 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/sdk_helpers.py
--rw-r--r--   0        0        0     7167 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py
--rw-r--r--   0        0        0     3126 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py
--rw-r--r--   0        0        0     6708 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py
--rw-r--r--   0        0        0     3480 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py
--rw-r--r--   0        0        0     7635 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/pycoingecko_helpers.py
--rw-r--r--   0        0        0     5693 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/pyth_model.py
--rw-r--r--   0        0        0      973 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/pyth_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    26081 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.920404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/technical_analysis/__init__.py
--rw-r--r--   0        0        0    54572 2023-04-08 00:08:53.924404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.924404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/tools/__init__.py
--rw-r--r--   0        0        0     6219 2023-04-08 00:08:53.924404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/tools/tools_controller.py
--rw-r--r--   0        0        0     1357 2023-04-08 00:08:53.924404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/tools/tools_helpers.py
--rw-r--r--   0        0        0     3447 2023-04-08 00:08:53.924404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/tools/tools_model.py
--rw-r--r--   0        0        0     2772 2023-04-08 00:08:53.924404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/tools/tools_view.py
--rw-r--r--   0        0        0    16936 2023-04-08 00:08:53.924404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_prompt_toolkit.py
--rw-r--r--   0        0        0    55138 2023-04-08 00:08:53.924404 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/coin_highs.png
--rw-r--r--   0        0        0  2879534 2023-04-08 00:08:53.940405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/luna_crash.html
--rw-r--r--   0        0        0   350260 2023-04-08 00:08:53.944405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/luna_supply.png
--rw-r--r--   0        0        0   607642 2023-04-08 00:08:53.948405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/luna_terra.png
--rw-r--r--   0        0        0    11988 2023-04-08 00:08:53.948405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb
--rw-r--r--   0        0        0   667206 2023-04-08 00:08:53.948405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/tvl.png
--rw-r--r--   0        0        0   465754 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/ust_terra.png
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/__init__.py
--rw-r--r--   0        0        0    15437 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/dashboards_controller.py
--rw-r--r--   0        0        0    15983 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/stream/Forecasting.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/stream/__init__.py
--rw-r--r--   0        0        0    16808 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/stream/pages/Indicators.py
--rw-r--r--   0        0        0     5481 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/chains.ipynb
--rw-r--r--   0        0        0     6789 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/correlation.ipynb
--rw-r--r--   0        0        0    13852 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/forecast.ipynb
--rw-r--r--   0        0        0    10953 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/futures.ipynb
--rw-r--r--   0        0        0     9421 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/shortdata.ipynb
--rw-r--r--   0        0        0    15315 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/stocks.ipynb
--rw-r--r--   0        0        0     5091 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/decorators.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/__init__.py
--rw-r--r--   0        0        0    73682 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/econometrics_controller.py
--rw-r--r--   0        0        0     2973 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/econometrics_helpers.py
--rw-r--r--   0        0        0    13544 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/econometrics_model.py
--rw-r--r--   0        0        0    16620 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/econometrics_view.py
--rw-r--r--   0        0        0    20449 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/regression_model.py
--rw-r--r--   0        0        0     6739 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/regression_view.py
--rw-r--r--   0        0        0       77 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/README.md
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/__init__.py
--rw-r--r--   0        0        0    10230 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/alphavantage_model.py
--rw-r--r--   0        0        0    12075 2023-04-08 00:08:53.952405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/alphavantage_view.py
--rw-r--r--   0        0        0     1614 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/commodity_model.py
--rw-r--r--   0        0        0     1561 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/commodity_view.py
--rw-r--r--   0        0        0      909 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv
--rw-r--r--   0        0        0    21218 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/datasets/cpi.csv
--rw-r--r--   0        0        0    10355 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/datasets/harmonized_cpi.csv
--rw-r--r--   0        0        0    28404 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/econdb_model.py
--rw-r--r--   0        0        0     8013 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/econdb_view.py
--rw-r--r--   0        0        0    91589 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/economy_controller.py
--rw-r--r--   0        0        0     3436 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/economy_helpers.py
--rw-r--r--   0        0        0     1298 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/finnhub_model.py
--rw-r--r--   0        0        0     2581 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/finnhub_view.py
--rw-r--r--   0        0        0     7966 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/finviz_model.py
--rw-r--r--   0        0        0     4600 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/finviz_view.py
--rw-r--r--   0        0        0     9940 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/fred_model.py
--rw-r--r--   0        0        0     9117 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/fred_view.py
--rw-r--r--   0        0        0     6972 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/nasdaq_model.py
--rw-r--r--   0        0        0     3286 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/nasdaq_view.py
--rw-r--r--   0        0        0    38418 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/oecd_model.py
--rw-r--r--   0        0        0    26364 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/oecd_view.py
--rw-r--r--   0        0        0     3768 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/plot_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    28433 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0     1218 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/sdk_helpers.py
--rw-r--r--   0        0        0    12870 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/wsj_model.py
--rw-r--r--   0        0        0     4673 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/wsj_view.py
--rw-r--r--   0        0        0    30415 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/yfinance_model.py
--rw-r--r--   0        0        0     5055 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/yfinance_view.py
--rw-r--r--   0        0        0      106 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/README.md
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/__init__.py
--rw-r--r--   0        0        0     4023 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/discovery/disc_controller.py
--rw-r--r--   0        0        0     2804 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/discovery/wsj_model.py
--rw-r--r--   0        0        0     1320 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/discovery/wsj_view.py
--rw-r--r--   0        0        0    21045 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/etf_controller.py
--rw-r--r--   0        0        0      450 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/etf_helper.py
--rw-r--r--   0        0        0   188615 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/etfs.csv
--rw-r--r--   0        0        0     2608 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/financedatabase_model.py
--rw-r--r--   0        0        0     3864 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/financedatabase_view.py
--rw-r--r--   0        0        0     1417 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/fmp_model.py
--rw-r--r--   0        0        0     3152 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/fmp_view.py
--rw-r--r--   0        0        0     4172 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/stockanalysis_model.py
--rw-r--r--   0        0        0     3941 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/stockanalysis_view.py
--rw-r--r--   0        0        0    51458 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0     8025 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/featflags_controller.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/__init__.py
--rw-r--r--   0        0        0    58622 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2023-04-08 00:08:53.956405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/corporate_spot_rates.csv
--rw-r--r--   0        0        0     9217 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/ecb_model.py
--rw-r--r--   0        0        0     7096 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/ecb_view.py
--rw-r--r--   0        0        0     5811 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/econdb_model.py
--rw-r--r--   0        0        0     7831 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/econdb_view.py
--rw-r--r--   0        0        0    56207 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/fixedincome_controller.py
--rw-r--r--   0        0        0    37985 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/fred_model.py
--rw-r--r--   0        0        0    51962 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/fred_view.py
--rw-r--r--   0        0        0   227110 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/ice_bofa_indices.csv
--rw-r--r--   0        0        0    10963 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/oecd_model.py
--rw-r--r--   0        0        0     3997 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/oecd_view.py
--rw-r--r--   0        0        0     2174 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/yfinance_model.py
--rw-r--r--   0        0        0     1702 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/yfinance_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/anom_model.py
--rw-r--r--   0        0        0     2962 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/anom_view.py
--rw-r--r--   0        0        0     4629 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoarima_model.py
--rw-r--r--   0        0        0     3933 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoarima_view.py
--rw-r--r--   0        0        0     4658 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoces_model.py
--rw-r--r--   0        0        0     3970 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoces_view.py
--rw-r--r--   0        0        0     4694 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoets_model.py
--rw-r--r--   0        0        0     3972 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoets_view.py
--rw-r--r--   0        0        0     7272 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoselect_model.py
--rw-r--r--   0        0        0     3938 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoselect_view.py
--rw-r--r--   0        0        0     5874 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/brnn_model.py
--rw-r--r--   0        0        0     6577 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/brnn_view.py
--rw-r--r--   0        0        0     5562 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/expo_model.py
--rw-r--r--   0        0        0     5038 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/expo_view.py
--rw-r--r--   0        0        0     2053 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/forecast.ipynb
--rw-r--r--   0        0        0   121785 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/forecast_controller.py
--rw-r--r--   0        0        0    15471 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/forecast_model.py
--rw-r--r--   0        0        0     9034 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/forecast_view.py
--rw-r--r--   0        0        0    47334 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/helpers.py
--rw-r--r--   0        0        0     3405 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/linregr_model.py
--rw-r--r--   0        0        0     4760 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/linregr_view.py
--rw-r--r--   0        0        0     5013 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/mstl_model.py
--rw-r--r--   0        0        0     3861 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/mstl_view.py
--rw-r--r--   0        0        0     5896 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/nbeats_model.py
--rw-r--r--   0        0        0     6396 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/nbeats_view.py
--rw-r--r--   0        0        0     7561 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/nhits_model.py
--rw-r--r--   0        0        0     7952 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/nhits_view.py
--rw-r--r--   0        0        0     3007 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/regr_model.py
--rw-r--r--   0        0        0     4521 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/regr_view.py
--rw-r--r--   0        0        0     5030 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/rnn_model.py
--rw-r--r--   0        0        0     5533 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/rnn_view.py
--rw-r--r--   0        0        0     4340 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/rwd_model.py
--rw-r--r--   0        0        0     3643 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/rwd_view.py
--rw-r--r--   0        0        0     4709 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/seasonalnaive_model.py
--rw-r--r--   0        0        0     3879 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/seasonalnaive_view.py
--rw-r--r--   0        0        0     5790 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/tcn_model.py
--rw-r--r--   0        0        0     6289 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/tcn_view.py
--rw-r--r--   0        0        0     7249 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/tft_model.py
--rw-r--r--   0        0        0     6520 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/tft_view.py
--rw-r--r--   0        0        0     4928 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/theta_model.py
--rw-r--r--   0        0        0     4379 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/theta_view.py
--rw-r--r--   0        0        0     6321 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/trans_model.py
--rw-r--r--   0        0        0     6765 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/trans_view.py
--rw-r--r--   0        0        0    12580 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/whisper_model.py
--rw-r--r--   0        0        0     2935 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/whisper_utils.py
--rw-r--r--   0        0        0      122 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/README.md
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/__init__.py
--rw-r--r--   0        0        0     5077 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/av_model.py
--rw-r--r--   0        0        0     1458 2023-04-08 00:08:53.960405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/av_view.py
--rw-r--r--   0        0        0     3281 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/data/av_forex_currencies.csv
--rw-r--r--   0        0        0     7847 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/data/polygon_tickers.csv
--rw-r--r--   0        0        0   419838 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/data/yahoofinance_forex.json
--rw-r--r--   0        0        0    16492 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/forex_controller.py
--rw-r--r--   0        0        0     8211 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/forex_helper.py
--rw-r--r--   0        0        0      931 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/fxempire_model.py
--rw-r--r--   0        0        0     1471 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/fxempire_view.py
--rw-r--r--   0        0        0    17162 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/oanda/oanda_controller.py
--rw-r--r--   0        0        0    22592 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/oanda/oanda_model.py
--rw-r--r--   0        0        0    12856 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/oanda/oanda_view.py
--rw-r--r--   0        0        0     2349 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/polygon_model.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    26168 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0     1446 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/sdk_helpers.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/technical_analysis/__init__.py
--rw-r--r--   0        0        0    35136 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/__init__.py
--rw-r--r--   0        0        0     2218 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/databento_view.py
--rw-r--r--   0        0        0     8903 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/futures_controller.py
--rw-r--r--   0        0        0      358 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/futures_helper.py
--rw-r--r--   0        0        0      964 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/sdk_helper.py
--rw-r--r--   0        0        0     4989 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/yfinance_model.py
--rw-r--r--   0        0        0     7379 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/yfinance_view.py
--rw-r--r--   0        0        0    13288 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/helper_classes.py
--rw-r--r--   0        0        0    67647 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/helper_funcs.py
--rw-r--r--   0        0        0     3212 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/helpers_denomination.py
--rw-r--r--   0        0        0     9052 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/intro.json
--rw-r--r--   0        0        0    42583 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/keys_controller.py
--rw-r--r--   0        0        0    80429 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/keys_model.py
--rw-r--r--   0        0        0     1148 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/keys_view.py
--rw-r--r--   0        0        0     5984 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/loggers.py
--rw-r--r--   0        0        0     1722 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/menu.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/alternative/covid/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/common/behavioural_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/common/prediction_techniques/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/common/quantitative_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/common/technical_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/custom/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/econometrics/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/economy/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/etf/movers/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/etf/screeners/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/mutual_funds/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/portfolio/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/portfolio/views/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.964405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/backtesting/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/behavioural_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/comparison_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/dark_pool_shorts/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/discovery/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/due_diligence/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/fundamental_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/government/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/insider/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/options/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/prediction_techniques/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/quantitative_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/raw_data/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/sector_industry_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/exports/stocks/technical_analysis/.gitkeep
--rw-r--r--   0        0        0     8528 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/futures/futures.csv
--rw-r--r--   0        0        0    60860 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/i18n/en.yml
--rw-r--r--   0        0        0     5831 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/i18n/help_translation.ipynb
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/.gitkeep
--rw-r--r--   0        0        0       64 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/account/test_account.openbb
--rw-r--r--   0        0        0       87 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_covid.openbb
--rw-r--r--   0        0        0      153 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_oss.openbb
--rw-r--r--   0        0        0      119 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_realestate.openbb
--rw-r--r--   0        0        0      856 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb
--rw-r--r--   0        0        0      802 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb
--rw-r--r--   0        0        0     1192 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb
--rw-r--r--   0        0        0      374 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_disc.openbb
--rw-r--r--   0        0        0      168 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_nft.openbb
--rw-r--r--   0        0        0     1229 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb
--rw-r--r--   0        0        0     1533 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb
--rw-r--r--   0        0        0      561 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb
--rw-r--r--   0        0        0       87 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_shroom.openbb
--rw-r--r--   0        0        0      768 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb
--rw-r--r--   0        0        0      154 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_tools.openbb
--rw-r--r--   0        0        0      120 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/dashboards/test_dashboards_base.openbb
--rw-r--r--   0        0        0     1333 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb
--rw-r--r--   0        0        0     2082 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb
--rw-r--r--   0        0        0      155 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf.openbb
--rw-r--r--   0        0        0       33 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ca.openbb
--rw-r--r--   0        0        0       38 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_disc.openbb
--rw-r--r--   0        0        0      878 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb
--rw-r--r--   0        0        0      749 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb
--rw-r--r--   0        0        0      301 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast.openbb
--rw-r--r--   0        0        0      176 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast_advanced.openbb
--rw-r--r--   0        0        0      241 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_base.openbb
--rw-r--r--   0        0        0      108 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_load.openbb
--rw-r--r--   0        0        0      745 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb
--rw-r--r--   0        0        0       62 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda_base.openbb
--rw-r--r--   0        0        0      630 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb
--rw-r--r--   0        0        0      611 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb
--rw-r--r--   0        0        0      173 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/futures/test_futures.openbb
--rw-r--r--   0        0        0     1275 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb
--rw-r--r--   0        0        0     1826 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb
--rw-r--r--   0        0        0       98 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_boolean_args.openbb
--rw-r--r--   0        0        0      683 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb
--rw-r--r--   0        0        0       67 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_base.openbb
--rw-r--r--   0        0        0       65 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_crypto.openbb
--rw-r--r--   0        0        0      151 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_economy.openbb
--rw-r--r--   0        0        0       83 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_equity.openbb
--rw-r--r--   0        0        0      113 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_etf.openbb
--rw-r--r--   0        0        0      174 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forecast.openbb
--rw-r--r--   0        0        0      158 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forex.openbb
--rw-r--r--   0        0        0      132 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_portfolio.openbb
--rw-r--r--   0        0        0      102 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_run.openbb
--rw-r--r--   0        0        0      258 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks.openbb
--rw-r--r--   0        0        0      255 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ba.openbb
--rw-r--r--   0        0        0     1513 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb
--rw-r--r--   0        0        0      422 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ca.openbb
--rw-r--r--   0        0        0      251 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_disc.openbb
--rw-r--r--   0        0        0      145 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_dps.openbb
--rw-r--r--   0        0        0     1874 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb
--rw-r--r--   0        0        0       44 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_base.openbb
--rw-r--r--   0        0        0       31 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_epsfc.openbb
--rw-r--r--   0        0        0       31 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_revfc.openbb
--rw-r--r--   0        0        0      470 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_gov.openbb
--rw-r--r--   0        0        0      276 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ins.openbb
--rw-r--r--   0        0        0      340 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options.openbb
--rw-r--r--   0        0        0       91 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_payoff.openbb
--rw-r--r--   0        0        0      121 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_pricing.openbb
--rw-r--r--   0        0        0       82 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_screen.openbb
--rw-r--r--   0        0        0      644 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb
--rw-r--r--   0        0        0      170 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_scr.openbb
--rw-r--r--   0        0        0      347 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_sia.openbb
--rw-r--r--   0        0        0      717 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb
--rw-r--r--   0        0        0       82 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_th.openbb
--rw-r--r--   0        0        0       65 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/test_jupyter_base.openbb
--rw-r--r--   0        0        0       16 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/test_keys_.openbb
--rw-r--r--   0        0        0       46 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/test_news.openbb
--rw-r--r--   0        0        0     1080 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/models/hub_credentials.json
--rw-r--r--   0        0        0      380 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/models/local_credentials.json
--rw-r--r--   0        0        0    17970 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx
--rw-r--r--   0        0        0    29757 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx
--rw-r--r--   0        0        0      310 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/routines/routine_example.openbb
--rw-r--r--   0        0        0    22732 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/sources/openbb_default.json
--rw-r--r--   0        0        0     2332 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini
--rw-r--r--   0        0        0     2354 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini
--rw-r--r--   0        0        0     2341 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini
--rw-r--r--   0        0        0     2316 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini
--rw-r--r--   0        0        0     2316 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Banks.ini
--rw-r--r--   0        0        0     2346 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini
--rw-r--r--   0        0        0     2336 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini
--rw-r--r--   0        0        0     2346 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini
--rw-r--r--   0        0        0     2307 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini
--rw-r--r--   0        0        0     2309 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Construction.ini
--rw-r--r--   0        0        0     2329 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini
--rw-r--r--   0        0        0     2353 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini
--rw-r--r--   0        0        0     2360 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini
--rw-r--r--   0        0        0     2320 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini
--rw-r--r--   0        0        0     2344 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini
--rw-r--r--   0        0        0     2315 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini
--rw-r--r--   0        0        0     2346 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini
--rw-r--r--   0        0        0     2376 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini
--rw-r--r--   0        0        0     2326 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Health.ini
--rw-r--r--   0        0        0     2307 2023-04-08 00:08:53.968405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini
--rw-r--r--   0        0        0     2320 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini
--rw-r--r--   0        0        0     2324 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini
--rw-r--r--   0        0        0     2334 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini
--rw-r--r--   0        0        0     2324 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Legal.ini
--rw-r--r--   0        0        0     2313 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini
--rw-r--r--   0        0        0     2341 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini
--rw-r--r--   0        0        0     2296 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Mining.ini
--rw-r--r--   0        0        0     2367 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini
--rw-r--r--   0        0        0     2342 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini
--rw-r--r--   0        0        0     2361 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini
--rw-r--r--   0        0        0     2351 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini
--rw-r--r--   0        0        0     2336 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini
--rw-r--r--   0        0        0     2322 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini
--rw-r--r--   0        0        0     2310 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini
--rw-r--r--   0        0        0     2326 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini
--rw-r--r--   0        0        0     2341 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini
--rw-r--r--   0        0        0     2299 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini
--rw-r--r--   0        0        0     2316 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini
--rw-r--r--   0        0        0     2342 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini
--rw-r--r--   0        0        0     2381 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini
--rw-r--r--   0        0        0     2314 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini
--rw-r--r--   0        0        0    34473 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/template.ini
--rw-r--r--   0        0        0    34519 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/whales.ini
--rw-r--r--   0        0        0     2688 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/README.md
--rw-r--r--   0        0        0     4195 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/high_iv.ini
--rw-r--r--   0        0        0     4210 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini
--rw-r--r--   0        0        0     3925 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini
--rw-r--r--   0        0        0     4202 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini
--rw-r--r--   0        0        0     4079 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/template.ini
--rwxr-xr-x   0        0        0      282 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/5pct_above_low.ini
--rwxr-xr-x   0        0        0      315 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/analyst_strong_buy.ini
--rwxr-xr-x   0        0        0      464 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/break_out_stocks.ini
--rw-r--r--   0        0        0      413 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/buffett_like.ini
--rwxr-xr-x   0        0        0      184 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/bull_runs_over_10pct.ini
--rwxr-xr-x   0        0        0      364 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/channel_up_and_low_debt_and_sma_50and200.ini
--rw-r--r--   0        0        0      326 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/cheap_bottom_dividend.ini
--rw-r--r--   0        0        0      193 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/cheap_dividend.ini
--rw-r--r--   0        0        0      241 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/cheap_oversold.ini
--rwxr-xr-x   0        0        0      335 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/continued_momentum_scan.ini
--rw-r--r--   0        0        0      286 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/death_cross.ini
--rw-r--r--   0        0        0      221 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/golden_cross.ini
--rwxr-xr-x   0        0        0      255 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/golden_cross_penny.ini
--rwxr-xr-x   0        0        0      518 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini
--rw-r--r--   0        0        0      302 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/heavy_inst_ins.ini
--rwxr-xr-x   0        0        0      279 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/high_vol_and_low_debt.ini
--rw-r--r--   0        0        0      316 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/modified_dreman.ini
--rw-r--r--   0        0        0      349 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/modified_neff.ini
--rwxr-xr-x   0        0        0      295 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/news_scanner.ini
--rwxr-xr-x   0        0        0      274 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/oversold.ini
--rwxr-xr-x   0        0        0      328 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/oversold_under_3dol.ini
--rwxr-xr-x   0        0        0      301 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/oversold_under_5dol.ini
--rwxr-xr-x   0        0        0      212 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/potential_reversals.ini
--rwxr-xr-x   0        0        0      295 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/recent_growth_and_support.ini
--rw-r--r--   0        0        0      337 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/rosenwald.ini
--rw-r--r--   0        0        0      280 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/rosenwald_gtfo.ini
--rw-r--r--   0        0        0      360 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/sexy_year.ini
--rwxr-xr-x   0        0        0      222 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/short_squeeze_scan.ini
--rwxr-xr-x   0        0        0      260 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/simplistic_momentum_scanner_under_7dol.ini
--rwxr-xr-x   0        0        0      276 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/stocks_strong_support_levels.ini
--rwxr-xr-x   0        0        0      272 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/top_performers_all.ini
--rwxr-xr-x   0        0        0      299 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/top_performers_healthcare.ini
--rwxr-xr-x   0        0        0      293 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/top_performers_tech.ini
--rwxr-xr-x   0        0        0      286 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/under_15dol_stocks.ini
--rw-r--r--   0        0        0      209 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/undervalue.ini
--rwxr-xr-x   0        0        0      272 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/unusual_volume.ini
--rwxr-xr-x   0        0        0      675 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini
--rwxr-xr-x   0        0        0      315 2023-04-08 00:08:53.972405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/weak_support_and_top_performers.ini
--rw-r--r--   0        0        0   358460 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/Consolas.ttf
--rw-r--r--   0        0        0      972 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json
--rw-r--r--   0        0        0      182 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/dark.mplrc.json
--rw-r--r--   0        0        0     2086 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/dark.mplstyle
--rw-r--r--   0        0        0     2750 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0      203 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/dark.richstyle.json
--rw-r--r--   0        0        0      970 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json
--rw-r--r--   0        0        0      182 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/light.mplrc.json
--rw-r--r--   0        0        0     2035 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/light.mplstyle
--rw-r--r--   0        0        0    24077 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0      202 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/light.richstyle.json
--rw-r--r--   0        0        0     2607 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0      186 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/user/openbb.richstyle.json
--rw-r--r--   0        0        0      144 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/README.md
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/__init__.py
--rw-r--r--   0        0        0    81373 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/avanza_fund_ID.csv
--rw-r--r--   0        0        0      834 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/avanza_model.py
--rw-r--r--   0        0        0     3941 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/avanza_view.py
--rw-r--r--   0        0        0     6535 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/mstarpy_model.py
--rw-r--r--   0        0        0     7883 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/mstarpy_view.py
--rw-r--r--   0        0        0    15141 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/mutual_fund_controller.py
--rw-r--r--   0        0        0     6040 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/mutual_funds_utils.py
--rw-r--r--   0        0        0    51025 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/parent_classes.py
--rw-r--r--   0        0        0       61 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/__init__.py
--rw-r--r--   0        0        0    15080 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/allocation_model.py
--rw-r--r--   0        0        0    12944 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/attribution_model.py
--rw-r--r--   0        0        0      417 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/README.md
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/bro_controller.py
--rw-r--r--   0        0        0     1121 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/brokers_helpers.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/coinbase/__init__.py
--rw-r--r--   0        0        0     8211 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py
--rw-r--r--   0        0        0     9561 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py
--rw-r--r--   0        0        0     4495 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py
--rw-r--r--   0        0        0     4666 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/degiro/README.md
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/degiro/__init__.py
--rw-r--r--   0        0        0    12789 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py
--rw-r--r--   0        0        0    15571 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/degiro/degiro_model.py
--rw-r--r--   0        0        0    15670 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/degiro/degiro_view.py
--rw-r--r--   0        0        0     3894 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py
--rw-r--r--   0        0        0     3002 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py
--rw-r--r--   0        0        0     2482 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py
--rw-r--r--   0        0        0    30861 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/metrics_model.py
--rw-r--r--   0        0        0    54979 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_controller.py
--rw-r--r--   0        0        0    39188 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_engine.py
--rw-r--r--   0        0        0     9643 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_helper.py
--rw-r--r--   0        0        0    60205 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_model.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/__init__.py
--rw-r--r--   0        0        0     5255 2023-04-08 00:08:53.976405 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/excel_model.py
--rw-r--r--   0        0        0     2106 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py
--rw-r--r--   0        0        0   120571 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py
--rw-r--r--   0        0        0   155050 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py
--rw-r--r--   0        0        0     2773 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py
--rw-r--r--   0        0        0    13116 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py
--rw-r--r--   0        0        0     5965 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py
--rw-r--r--   0        0        0     5346 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py
--rw-r--r--   0        0        0     4427 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py
--rw-r--r--   0        0        0   138034 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/po_controller.py
--rw-r--r--   0        0        0     8587 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/po_engine.py
--rw-r--r--   0        0        0   103568 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/po_model.py
--rw-r--r--   0        0        0    24186 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/po_view.py
--rw-r--r--   0        0        0    11390 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/statics.py
--rw-r--r--   0        0        0    12009 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py
--rw-r--r--   0        0        0    54944 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_view.py
--rw-r--r--   0        0        0     8433 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/statics.py
--rw-r--r--   0        0        0     2877 2023-04-08 00:08:53.980406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reporting.md
--rw-r--r--   0        0        0  1028287 2023-04-08 00:08:53.984406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html
--rw-r--r--   0        0        0     2839 2023-04-08 00:08:53.984406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/README.md
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.984406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/__init__.py
--rw-r--r--   0        0        0      443 2023-04-08 00:08:53.984406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/data/crypto_tickers.csv
--rw-r--r--   0        0        0      437 2023-04-08 00:08:53.984406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/data/etf_tickers.csv
--rw-r--r--   0        0        0      222 2023-04-08 00:08:53.984406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/data/stocks_tickers.csv
--rw-r--r--   0        0        0     9716 2023-04-08 00:08:53.984406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/reports_controller.py
--rw-r--r--   0        0        0    12275 2023-04-08 00:08:53.984406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/reports_model.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.984406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/stored/.gitkeep
--rw-r--r--   0        0        0  1076317 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html
--rw-r--r--   0        0        0     5214 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/OpenBB_reports_logo.png
--rw-r--r--   0        0        0    32298 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/crypto.ipynb
--rw-r--r--   0        0        0    22724 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/economy.ipynb
--rw-r--r--   0        0        0    39716 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/equity.ipynb
--rw-r--r--   0        0        0     9851 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/etf.ipynb
--rw-r--r--   0        0        0     2782 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/floppy-disc.png
--rw-r--r--   0        0        0     8557 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/forecast.ipynb
--rw-r--r--   0        0        0    17576 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/forex.ipynb
--rw-r--r--   0        0        0    14912 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/portfolio.ipynb
--rw-r--r--   0        0        0    11247 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/widget_helpers.py
--rw-r--r--   0        0        0      205 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/widgets/card.j2
--rw-r--r--   0        0        0     3556 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/widgets/report.css
--rw-r--r--   0        0        0      474 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/widgets/report.j2
--rw-r--r--   0        0        0      119 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/widgets/row.j2
--rw-r--r--   0        0        0      896 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/widgets/style.css
--rw-r--r--   0        0        0     9972 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/rich_config.py
--rw-r--r--   0        0        0    30909 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/sdk.py
--rw-r--r--   0        0        0    28128 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/settings_controller.py
--rw-r--r--   0        0        0     6595 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/sources_controller.py
--rw-r--r--   0        0        0      357 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/README.md
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/backtesting/__init__.py
--rw-r--r--   0        0        0    10448 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/backtesting/bt_controller.py
--rw-r--r--   0        0        0     8126 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/backtesting/bt_model.py
--rw-r--r--   0        0        0     9046 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/backtesting/bt_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/behavioural_analysis/__init__.py
--rw-r--r--   0        0        0    29872 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/behavioural_analysis/ba_controller.py
--rw-r--r--   0        0        0     3541 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py
--rw-r--r--   0        0        0     3761 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py
--rw-r--r--   0        0        0     1931 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/cboe_model.py
--rw-r--r--   0        0        0      969 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/cboe_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.992406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/__init__.py
--rw-r--r--   0        0        0    37655 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/ca_controller.py
--rw-r--r--   0        0        0     4871 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/finbrain_model.py
--rw-r--r--   0        0        0     5785 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/finbrain_view.py
--rw-r--r--   0        0        0     1328 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/finnhub_model.py
--rw-r--r--   0        0        0     2679 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py
--rw-r--r--   0        0        0     1539 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py
--rw-r--r--   0        0        0    12381 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py
--rw-r--r--   0        0        0     5757 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py
--rw-r--r--   0        0        0     1690 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/polygon_model.py
--rw-r--r--   0        0        0     1379 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py
--rw-r--r--   0        0        0     8073 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py
--rw-r--r--   0        0        0    10157 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/__init__.py
--rw-r--r--   0        0        0    20377 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py
--rw-r--r--   0        0        0    10009 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/finra_model.py
--rw-r--r--   0        0        0     7203 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/finra_view.py
--rw-r--r--   0        0        0     1093 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py
--rw-r--r--   0        0        0     1200 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py
--rw-r--r--   0        0        0     1387 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py
--rw-r--r--   0        0        0     4648 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py
--rw-r--r--   0        0        0     6836 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/sec_model.py
--rw-r--r--   0        0        0     3470 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/sec_view.py
--rw-r--r--   0        0        0     1882 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py
--rw-r--r--   0        0        0     1385 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py
--rw-r--r--   0        0        0     5053 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py
--rw-r--r--   0        0        0     9997 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py
--rw-r--r--   0        0        0     1166 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py
--rw-r--r--   0        0        0     3613 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py
--rw-r--r--   0        0        0      668 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py
--rw-r--r--   0        0        0     1271 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py
--rw-r--r--   0        0        0     5740 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/databento_model.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/__init__.py
--rw-r--r--   0        0        0     4169 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/ark_model.py
--rw-r--r--   0        0        0     2589 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/ark_view.py
--rw-r--r--   0        0        0    31510 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/disc_controller.py
--rw-r--r--   0        0        0      483 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/disc_helpers.py
--rw-r--r--   0        0        0     2696 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/fidelity_model.py
--rw-r--r--   0        0        0     2680 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/fidelity_view.py
--rw-r--r--   0        0        0     4164 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/finnhub_model.py
--rw-r--r--   0        0        0     2510 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/finnhub_view.py
--rw-r--r--   0        0        0     1731 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/finviz_model.py
--rw-r--r--   0        0        0     3084 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/finviz_view.py
--rw-r--r--   0        0        0     2562 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/fmp_view.py
--rw-r--r--   0        0        0     3051 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/nasdaq_model.py
--rw-r--r--   0        0        0     3406 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/nasdaq_view.py
--rw-r--r--   0        0        0     7080 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/seeking_alpha_model.py
--rw-r--r--   0        0        0     4803 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/seeking_alpha_view.py
--rw-r--r--   0        0        0     1120 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/shortinterest_model.py
--rw-r--r--   0        0        0     2566 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/shortinterest_view.py
--rw-r--r--   0        0        0     4113 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/yahoofinance_model.py
--rw-r--r--   0        0        0     5871 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/yahoofinance_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/__init__.py
--rw-r--r--   0        0        0    24082 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/av_model.py
--rw-r--r--   0        0        0    14910 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/av_view.py
--rw-r--r--   0        0        0    10834 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py
--rw-r--r--   0        0        0     7680 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py
--rw-r--r--   0        0        0     1833 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py
--rw-r--r--   0        0        0     2347 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py
--rw-r--r--   0        0        0    14888 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/dcf_model.py
--rw-r--r--   0        0        0     4279 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/dcf_static.py
--rw-r--r--   0        0        0    44464 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/dcf_view.py
--rw-r--r--   0        0        0     1532 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py
--rw-r--r--   0        0        0     1205 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py
--rw-r--r--   0        0        0     2396 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py
--rw-r--r--   0        0        0     4904 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py
--rw-r--r--   0        0        0    81236 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/fa_controller.py
--rw-r--r--   0        0        0      266 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/fa_helper.py
--rw-r--r--   0        0        0     1389 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py
--rw-r--r--   0        0        0     3518 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py
--rw-r--r--   0        0        0     3419 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/finviz_model.py
--rw-r--r--   0        0        0     2484 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/finviz_view.py
--rw-r--r--   0        0        0    22210 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/fmp_model.py
--rw-r--r--   0        0        0    25688 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/fmp_view.py
--rw-r--r--   0        0        0     6417 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt
--rw-r--r--   0        0        0    11855 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/market_watch_model.py
--rw-r--r--   0        0        0     1509 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/market_watch_view.py
--rw-r--r--   0        0        0     2217 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py
--rw-r--r--   0        0        0     1259 2023-04-08 00:08:53.996406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py
--rw-r--r--   0        0        0     5391 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/polygon_model.py
--rw-r--r--   0        0        0     4361 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/polygon_view.py
--rw-r--r--   0        0        0     7593 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py
--rw-r--r--   0        0        0    11162 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py
--rw-r--r--   0        0        0     2059 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py
--rw-r--r--   0        0        0    11829 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py
--rw-r--r--   0        0        0    14679 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/government/__init__.py
--rw-r--r--   0        0        0    18461 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/government/gov_controller.py
--rw-r--r--   0        0        0    15719 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/government/quiverquant_model.py
--rw-r--r--   0        0        0    21407 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/government/quiverquant_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/__init__.py
--rw-r--r--   0        0        0     2062 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/businessinsider_model.py
--rw-r--r--   0        0        0     5102 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/businessinsider_view.py
--rw-r--r--   0        0        0     1125 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/finviz_model.py
--rw-r--r--   0        0        0     1171 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/finviz_view.py
--rw-r--r--   0        0        0    32744 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/insider_controller.py
--rw-r--r--   0        0        0    87496 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/openinsider_model.py
--rw-r--r--   0        0        0     7695 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/openinsider_view.py
--rw-r--r--   0        0        0     4909 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/sdk_helper.py
--rw-r--r--   0        0        0    76085 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/mappings/Mic_Codes.csv
--rw-r--r--   0        0        0        0 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/__init__.py
--rw-r--r--   0        0        0     1757 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/alphaquery_model.py
--rw-r--r--   0        0        0     1713 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/alphaquery_view.py
--rw-r--r--   0        0        0     1161 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/barchart_model.py
--rw-r--r--   0        0        0     1137 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/barchart_view.py
--rw-r--r--   0        0        0     1526 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/calculator_model.py
--rw-r--r--   0        0        0     2416 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/calculator_view.py
--rw-r--r--   0        0        0     2777 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/chartexchange_model.py
--rw-r--r--   0        0        0     3211 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/chartexchange_view.py
--rw-r--r--   0        0        0     2433 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/fdscanner_model.py
--rw-r--r--   0        0        0     1672 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/fdscanner_view.py
--rw-r--r--   0        0        0    21092 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/hedge/hedge_controller.py
--rw-r--r--   0        0        0     9884 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/hedge/hedge_model.py
--rw-r--r--   0        0        0     3968 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/hedge/hedge_view.py
--rw-r--r--   0        0        0    10030 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/intrinio_model.py
--rw-r--r--   0        0        0     6101 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/intrinio_view.py
--rw-r--r--   0        0        0     7097 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/nasdaq_model.py
--rw-r--r--   0        0        0    22486 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/op_helpers.py
--rw-r--r--   0        0        0    52192 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/options_controller.py
--rw-r--r--   0        0        0    10568 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/options_sdk_helper.py
--rw-r--r--   0        0        0    14169 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/options_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/screen/__init__.py
--rw-r--r--   0        0        0     5686 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/screen/screener_controller.py
--rw-r--r--   0        0        0     9556 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/screen/syncretism_model.py
--rw-r--r--   0        0        0     5566 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/screen/syncretism_view.py
--rw-r--r--   0        0        0     8295 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/tradier_model.py
--rw-r--r--   0        0        0     2561 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/tradier_view.py
--rw-r--r--   0        0        0     7674 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/yfinance_model.py
--rw-r--r--   0        0        0    11615 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/yfinance_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0     2260 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/beta_model.py
--rw-r--r--   0        0        0     2798 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/beta_view.py
--rw-r--r--   0        0        0     3187 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/factors_model.py
--rw-r--r--   0        0        0      687 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/factors_view.py
--rw-r--r--   0        0        0    38741 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0      447 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/qa_model.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/research/__init__.py
--rw-r--r--   0        0        0     6218 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/research/res_controller.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:54.000406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/__init__.py
--rw-r--r--   0        0        0     2055 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/ark_model.py
--rw-r--r--   0        0        0     1846 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/ark_view.py
--rw-r--r--   0        0        0    46491 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/finviz_model.py
--rw-r--r--   0        0        0     6858 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/finviz_view.py
--rw-r--r--   0        0        0    25607 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/screener_controller.py
--rw-r--r--   0        0        0      944 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/screener_helper.py
--rw-r--r--   0        0        0     2562 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/screener_view.py
--rw-r--r--   0        0        0     5200 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/yahoofinance_model.py
--rw-r--r--   0        0        0     2797 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/yahoofinance_view.py
--rw-r--r--   0        0        0    27077 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/stock_statics.py
--rw-r--r--   0        0        0    27310 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/stocks_controller.py
--rw-r--r--   0        0        0    33057 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/stocks_helper.py
--rw-r--r--   0        0        0    10576 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/stocks_model.py
--rw-r--r--   0        0        0     1241 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/stocks_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/__init__.py
--rw-r--r--   0        0        0     1004 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/finbrain_model.py
--rw-r--r--   0        0        0      644 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/finbrain_view.py
--rw-r--r--   0        0        0      761 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/finviz_model.py
--rw-r--r--   0        0        0     1229 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/finviz_view.py
--rw-r--r--   0        0        0     1532 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/rsp_model.py
--rw-r--r--   0        0        0     2386 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/rsp_view.py
--rw-r--r--   0        0        0    63334 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0     3260 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/tradingview_model.py
--rw-r--r--   0        0        0     1985 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/tradingview_view.py
--rw-r--r--   0        0        0      334 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/README.md
--rw-r--r--   0        0        0        0 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/__init__.py
--rw-r--r--   0        0        0     5328 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/bursa_model.py
--rw-r--r--   0        0        0     2202 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/bursa_view.py
--rw-r--r--   0        0        0        0 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/data/__init__.py
--rw-r--r--   0        0        0    28098 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json
--rw-r--r--   0        0        0     1466 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py
--rw-r--r--   0        0        0     1378 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py
--rw-r--r--   0        0        0    10137 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/tradinghours_controller.py
--rw-r--r--   0        0        0      614 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/tradinghours_helper.py
--rw-r--r--   0        0        0    43410 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/terminal_controller.py
--rw-r--r--   0        0        0    13888 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/terminal_helper.py
--rw-r--r--   0        0        0     3848 2023-04-08 00:08:54.004406 openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/thought_of_the_day.py
--rw-r--r--   0        0        0     5787 2023-04-08 00:08:55.684447 openbb_nightly-3.0.0rc1.dev20230408/pyproject.toml
--rw-r--r--   0        0        0      945 2023-04-08 00:08:54.008406 openbb_nightly-3.0.0rc1.dev20230408/terminal.py
--rw-r--r--   0        0        0     2304 2023-04-08 00:08:55.688447 openbb_nightly-3.0.0rc1.dev20230408/website/pypi.md
--rw-r--r--   0        0        0     7861 1970-01-01 00:00:00.000000 openbb_nightly-3.0.0rc1.dev20230408/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-09 00:10:01.777439 openbb_nightly-3.0.0rc1.dev20230409/LICENSE
+-rw-r--r--   0        0        0    18588 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/SDK_README.md
+-rw-r--r--   0        0        0      243 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/__init__.py
+-rw-r--r--   0        0        0    19834 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/account/account_controller.py
+-rw-r--r--   0        0        0     3382 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/account/account_model.py
+-rw-r--r--   0        0        0      612 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/account/account_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/__init__.py
+-rw-r--r--   0        0        0     3131 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/alt_controller.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/covid/__init__.py
+-rw-r--r--   0        0        0     1881 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/covid/countries.txt
+-rw-r--r--   0        0        0     9347 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/covid/covid_controller.py
+-rw-r--r--   0        0        0     5387 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/covid/covid_model.py
+-rw-r--r--   0        0        0     8586 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/covid/covid_view.py
+-rw-r--r--   0        0        0     1070 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/hackernews_model.py
+-rw-r--r--   0        0        0     1087 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/hackernews_view.py
+-rw-r--r--   0        0        0     6752 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/oss/github_model.py
+-rw-r--r--   0        0        0     3968 2023-04-09 00:10:01.981452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/oss/github_view.py
+-rw-r--r--   0        0        0     8656 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/oss/oss_controller.py
+-rw-r--r--   0        0        0     4437 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/oss/runa_model.py
+-rw-r--r--   0        0        0     4018 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/oss/runa_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/realestate/__init__.py
+-rw-r--r--   0        0        0     9030 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/realestate/landRegistry_model.py
+-rw-r--r--   0        0        0     3309 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/realestate/landRegistry_view.py
+-rw-r--r--   0        0        0     8108 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/realestate/realestate_controller.py
+-rw-r--r--   0        0        0     2718 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/base_helpers.py
+-rw-r--r--   0        0        0       93 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/__init__.py
+-rw-r--r--   0        0        0     1198 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/finbrain_model.py
+-rw-r--r--   0        0        0     4394 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/finbrain_view.py
+-rw-r--r--   0        0        0     1335 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     1861 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     3329 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/google_model.py
+-rw-r--r--   0        0        0     7118 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/google_view.py
+-rw-r--r--   0        0        0     5524 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/reddit_helpers.py
+-rw-r--r--   0        0        0    18297 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/reddit_model.py
+-rw-r--r--   0        0        0    10206 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/reddit_view.py
+-rw-r--r--   0        0        0     3239 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/stocktwits_model.py
+-rw-r--r--   0        0        0     2898 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/stocktwits_view.py
+-rw-r--r--   0        0        0     6160 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/twitter_model.py
+-rw-r--r--   0        0        0     5870 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/twitter_view.py
+-rw-r--r--   0        0        0     4142 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/common_model.py
+-rw-r--r--   0        0        0     3634 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/feedparser_model.py
+-rw-r--r--   0        0        0     1242 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/feedparser_view.py
+-rw-r--r--   0        0        0     2639 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/newsapi_model.py
+-rw-r--r--   0        0        0     1465 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/newsapi_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    19923 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/quantitative_analysis/qa_model.py
+-rw-r--r--   0        0        0    32308 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/quantitative_analysis/qa_view.py
+-rw-r--r--   0        0        0     3226 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/quantitative_analysis/rolling_model.py
+-rw-r--r--   0        0        0    10790 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/quantitative_analysis/rolling_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/__init__.py
+-rw-r--r--   0        0        0     2977 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/custom_indicators_model.py
+-rw-r--r--   0        0        0     4272 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/custom_indicators_view.py
+-rw-r--r--   0        0        0     6427 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/momentum_model.py
+-rw-r--r--   0        0        0    10556 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/momentum_view.py
+-rw-r--r--   0        0        0     4179 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/overlap_model.py
+-rw-r--r--   0        0        0     4361 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/overlap_view.py
+-rw-r--r--   0        0        0     1453 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/ta_helpers.py
+-rw-r--r--   0        0        0     1819 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/trend_indicators_model.py
+-rw-r--r--   0        0        0     2621 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/trend_indicators_view.py
+-rw-r--r--   0        0        0    19962 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/volatility_model.py
+-rw-r--r--   0        0        0    10008 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/volatility_view.py
+-rw-r--r--   0        0        0     2614 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/volume_model.py
+-rw-r--r--   0        0        0     3806 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/volume_view.py
+-rw-r--r--   0        0        0     5813 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/ultima_newsmonitor_model.py
+-rw-r--r--   0        0        0     3886 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/ultima_newsmonitor_view.py
+-rw-r--r--   0        0        0     2634 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/config_terminal.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/__init__.py
+-rw-r--r--   0        0        0     9829 2023-04-09 00:10:01.985452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/completer/choices.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/config/__init__.py
+-rw-r--r--   0        0        0      927 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/config/paths.py
+-rw-r--r--   0        0        0     2650 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/config/paths_helper.py
+-rw-r--r--   0        0        0     9162 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/integration_tests/README.md
+-rw-r--r--   0        0        0    21758 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/integration_tests/integration_controller.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/collection/__init__.py
+-rw-r--r--   0        0        0     3848 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/collection/log_sender.py
+-rw-r--r--   0        0        0     3744 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/collection/logging_clock.py
+-rw-r--r--   0        0        0     3495 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/collection/s3_sender.py
+-rw-r--r--   0        0        0      166 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/constants.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/__init__.py
+-rw-r--r--   0        0        0      524 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/common.py
+-rw-r--r--   0        0        0      525 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/custom_logger.py
+-rw-r--r--   0        0        0      979 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/directories.py
+-rw-r--r--   0        0        0      841 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/expired_files.py
+-rw-r--r--   0        0        0     4896 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     6058 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4166 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/settings.py
+-rw-r--r--   0        0        0     1621 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/settings_logger.py
+-rw-r--r--   0        0        0      396 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/user_logger.py
+-rw-r--r--   0        0        0      627 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/__init__.py
+-rw-r--r--   0        0        0     1221 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/base_model.py
+-rw-r--r--   0        0        0      818 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/credentials_model.py
+-rw-r--r--   0        0        0     4154 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/preferences_model.py
+-rw-r--r--   0        0        0     1817 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/profile_model.py
+-rw-r--r--   0        0        0     1113 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/sources_model.py
+-rw-r--r--   0        0        0     1753 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/system_model.py
+-rw-r--r--   0        0        0      562 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/user_model.py
+-rw-r--r--   0        0        0      200 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/__init__.py
+-rw-r--r--   0        0        0   418780 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/assets/Terminal_icon.png
+-rw-r--r--   0        0        0      727 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/assets/icon.png
+-rw-r--r--   0        0        0    14854 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/backend.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/config/__init__.py
+-rw-r--r--   0        0        0     7156 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/config/openbb_styles.py
+-rw-r--r--   0        0        0     3073 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/no_import.py
+-rw-r--r--   0        0        0     1261 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/old_table.html
+-rw-r--r--   0        0        0     7732 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly.html
+-rw-r--r--   0        0        0    62668 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_helper.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     6724 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/base.py
+-rw-r--r--   0        0        0    11358 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0     8016 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    15173 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3361 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5683 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6868 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3429 2023-04-09 00:10:01.989452 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    20644 2023-04-09 00:10:01.993453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0   704570 2023-04-09 00:10:01.997453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/table.html
+-rw-r--r--   0        0        0    11182 2023-04-09 00:10:01.997453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/bar_menus.js
+-rw-r--r--   0        0        0   289624 2023-04-09 00:10:01.997453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf
+-rw-r--r--   0        0        0   286320 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf
+-rw-r--r--   0        0        0    25188 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/css/style.css
+-rw-r--r--   0        0        0      151 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/css/table.css
+-rw-r--r--   0        0        0    16611 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/helpers.js
+-rw-r--r--   0        0        0    12724 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/main.js
+-rw-r--r--   0        0        0     3255 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/main_table.js
+-rw-r--r--   0        0        0    24525 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/popups.js
+-rw-r--r--   0        0        0     7747 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/scripts/sdk_audit.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/__init__.py
+-rw-r--r--   0        0        0      450 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/__init__.py
+-rw-r--r--   0        0        0     2660 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py
+-rw-r--r--   0        0        0    24088 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py
+-rw-r--r--   0        0        0     1513 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py
+-rw-r--r--   0        0        0     2365 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py
+-rw-r--r--   0        0        0     5128 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py
+-rw-r--r--   0        0        0    18447 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py
+-rw-r--r--   0        0        0      761 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/__init__.py
+-rw-r--r--   0        0        0     4308 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/alt_sdk_model.py
+-rw-r--r--   0        0        0    42910 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/crypto_sdk_model.py
+-rw-r--r--   0        0        0     4497 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/econometrics_sdk_model.py
+-rw-r--r--   0        0        0     7975 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/economy_sdk_model.py
+-rw-r--r--   0        0        0     2496 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/etf_sdk_model.py
+-rw-r--r--   0        0        0     3515 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py
+-rw-r--r--   0        0        0     8550 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/forecast_sdk_model.py
+-rw-r--r--   0        0        0     4386 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/forex_sdk_model.py
+-rw-r--r--   0        0        0     1530 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/funds_sdk_model.py
+-rw-r--r--   0        0        0     1067 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/futures_sdk_model.py
+-rw-r--r--   0        0        0     3638 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/keys_sdk_model.py
+-rw-r--r--   0        0        0    10046 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/portfolio_sdk_model.py
+-rw-r--r--   0        0        0     4603 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/qa_sdk_model.py
+-rw-r--r--   0        0        0    32674 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/stocks_sdk_model.py
+-rw-r--r--   0        0        0     7229 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/ta_sdk_model.py
+-rw-r--r--   0        0        0    11508 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/sdk_helpers.py
+-rw-r--r--   0        0        0    19813 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/sdk_init.py
+-rw-r--r--   0        0        0    43994 2023-04-09 00:10:02.001453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/trail_map.csv
+-rw-r--r--   0        0        0     2801 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/trail_map_forecasting.csv
+-rw-r--r--   0        0        0     1301 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/trail_map_optimization.csv
+-rw-r--r--   0        0        0     7118 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/trailmap.py
+-rw-r--r--   0        0        0     1017 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/banner.txt
+-rw-r--r--   0        0        0      485 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/constants.py
+-rw-r--r--   0        0        0     1000 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/current_system.py
+-rw-r--r--   0        0        0     4179 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/current_user.py
+-rw-r--r--   0        0        0     1147 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/env_handler.py
+-rw-r--r--   0        0        0    20476 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/hub_model.py
+-rw-r--r--   0        0        0     5244 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/local_model.py
+-rw-r--r--   0        0        0     3097 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/sdk_session.py
+-rw-r--r--   0        0        0     2913 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/session_controller.py
+-rw-r--r--   0        0        0     4016 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/session_model.py
+-rw-r--r--   0        0        0     1065 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/sources_handler.py
+-rw-r--r--   0        0        0     1268 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/utils.py
+-rw-r--r--   0        0        0     3011 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sources/utils.py
+-rw-r--r--   0        0        0      199 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/README.md
+-rw-r--r--   0        0        0       84 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/__init__.py
+-rw-r--r--   0        0        0     5303 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/coinbase_helpers.py
+-rw-r--r--   0        0        0     2147 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/coinpaprika_helpers.py
+-rw-r--r--   0        0        0    19275 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/crypto_controller.py
+-rw-r--r--   0        0        0     4481 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/crypto_models.py
+-rw-r--r--   0        0        0     1785 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/crypto_views.py
+-rw-r--r--   0        0        0    30339 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py
+-rw-r--r--   0        0        0      949 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/README.md
+-rw-r--r--   0        0        0     7341 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/binance_gecko_map.json
+-rw-r--r--   0        0        0     2436 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json
+-rw-r--r--   0        0        0     4813 2023-04-09 00:10:02.005453 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/coingecko_categories.json
+-rw-r--r--   0        0        0   954385 2023-04-09 00:10:02.009454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/coingecko_coins.json
+-rw-r--r--   0        0        0  2245016 2023-04-09 00:10:02.017454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json
+-rw-r--r--   0        0        0    31307 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/defillama_dapps.json
+-rw-r--r--   0        0        0   107203 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/erc20_coins.json
+-rw-r--r--   0        0        0     7255 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/finbrain_coins.json
+-rw-r--r--   0        0        0   222978 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/santiment_slugs.json
+-rw-r--r--   0        0        0   300253 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json
+-rw-r--r--   0        0        0     4951 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/dataframe_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/__init__.py
+-rw-r--r--   0        0        0     4537 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/coindix_model.py
+-rw-r--r--   0        0        0     2720 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/coindix_view.py
+-rw-r--r--   0        0        0     2483 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py
+-rw-r--r--   0        0        0     1994 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py
+-rw-r--r--   0        0        0    31284 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/defi_controller.py
+-rw-r--r--   0        0        0     8918 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/graph_model.py
+-rw-r--r--   0        0        0     7165 2023-04-09 00:10:02.021454 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/graph_view.py
+-rw-r--r--   0        0        0     5005 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/llama_model.py
+-rw-r--r--   0        0        0     5827 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/llama_view.py
+-rw-r--r--   0        0        0     1808 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/smartstake_model.py
+-rw-r--r--   0        0        0     3110 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/smartstake_view.py
+-rw-r--r--   0        0        0     2882 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/substack_model.py
+-rw-r--r--   0        0        0     1090 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/substack_view.py
+-rw-r--r--   0        0        0     1947 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/terraengineer_model.py
+-rw-r--r--   0        0        0     2699 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/terraengineer_view.py
+-rw-r--r--   0        0        0     9734 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py
+-rw-r--r--   0        0        0     8022 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/__init__.py
+-rw-r--r--   0        0        0     2317 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py
+-rw-r--r--   0        0        0     1620 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py
+-rw-r--r--   0        0        0     2116 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py
+-rw-r--r--   0        0        0     1936 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py
+-rw-r--r--   0        0        0     7614 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/dappradar_model.py
+-rw-r--r--   0        0        0     5045 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/dappradar_view.py
+-rw-r--r--   0        0        0    21019 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/discovery_controller.py
+-rw-r--r--   0        0        0    10833 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py
+-rw-r--r--   0        0        0     6352 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py
+-rw-r--r--   0        0        0     1095 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/__init__.py
+-rw-r--r--   0        0        0     7483 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/binance_model.py
+-rw-r--r--   0        0        0     3009 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/binance_view.py
+-rw-r--r--   0        0        0     3188 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py
+-rw-r--r--   0        0        0     2840 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py
+-rw-r--r--   0        0        0     6439 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py
+-rw-r--r--   0        0        0     4134 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py
+-rw-r--r--   0        0        0     6587 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py
+-rw-r--r--   0        0        0     6638 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py
+-rw-r--r--   0        0        0    15062 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py
+-rw-r--r--   0        0        0     9133 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py
+-rw-r--r--   0        0        0     2332 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py
+-rw-r--r--   0        0        0    64101 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py
+-rw-r--r--   0        0        0     1850 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py
+-rw-r--r--   0        0        0     4333 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py
+-rw-r--r--   0        0        0    15044 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py
+-rw-r--r--   0        0        0    11237 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py
+-rw-r--r--   0        0        0    24480 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/messari_model.py
+-rw-r--r--   0        0        0    22260 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/messari_view.py
+-rw-r--r--   0        0        0    25887 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py
+-rw-r--r--   0        0        0     8762 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py
+-rw-r--r--   0        0        0     3076 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py
+-rw-r--r--   0        0        0     2070 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py
+-rw-r--r--   0        0        0     2508 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py
+-rw-r--r--   0        0        0     6001 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py
+-rw-r--r--   0        0        0     3474 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/__init__.py
+-rw-r--r--   0        0        0     5562 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/nft_controller.py
+-rw-r--r--   0        0        0     1664 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py
+-rw-r--r--   0        0        0     4495 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py
+-rw-r--r--   0        0        0     2895 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/opensea_model.py
+-rw-r--r--   0        0        0     1289 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/opensea_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/__init__.py
+-rw-r--r--   0        0        0    21848 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/bitquery_model.py
+-rw-r--r--   0        0        0    11444 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/bitquery_view.py
+-rw-r--r--   0        0        0     3393 2023-04-09 00:10:02.025455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/blockchain_model.py
+-rw-r--r--   0        0        0     4733 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/blockchain_view.py
+-rw-r--r--   0        0        0     1840 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py
+-rw-r--r--   0        0        0     1266 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py
+-rw-r--r--   0        0        0    15974 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py
+-rw-r--r--   0        0        0    10572 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py
+-rw-r--r--   0        0        0    53494 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/onchain_controller.py
+-rw-r--r--   0        0        0     5938 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/shroom_model.py
+-rw-r--r--   0        0        0     5144 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/shroom_view.py
+-rw-r--r--   0        0        0     4772 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py
+-rw-r--r--   0        0        0     2088 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/__init__.py
+-rw-r--r--   0        0        0     2274 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py
+-rw-r--r--   0        0        0     2664 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py
+-rw-r--r--   0        0        0     1464 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/coinbase_model.py
+-rw-r--r--   0        0        0     1342 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/coinbase_view.py
+-rw-r--r--   0        0        0    11841 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py
+-rw-r--r--   0        0        0     9646 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py
+-rw-r--r--   0        0        0     6776 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py
+-rw-r--r--   0        0        0     2278 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py
+-rw-r--r--   0        0        0     1100 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/glassnode_model.py
+-rw-r--r--   0        0        0     4677 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/glassnode_view.py
+-rw-r--r--   0        0        0     5936 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/loanscan_model.py
+-rw-r--r--   0        0        0     3279 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/loanscan_view.py
+-rw-r--r--   0        0        0    55381 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/overview_controller.py
+-rw-r--r--   0        0        0    13641 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py
+-rw-r--r--   0        0        0    21320 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py
+-rw-r--r--   0        0        0     5346 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/rekt_model.py
+-rw-r--r--   0        0        0     2253 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/rekt_view.py
+-rw-r--r--   0        0        0     2042 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/sdk_helpers.py
+-rw-r--r--   0        0        0     7167 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py
+-rw-r--r--   0        0        0     3126 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py
+-rw-r--r--   0        0        0     6708 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py
+-rw-r--r--   0        0        0     3480 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py
+-rw-r--r--   0        0        0     7635 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/pycoingecko_helpers.py
+-rw-r--r--   0        0        0     5693 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/pyth_model.py
+-rw-r--r--   0        0        0      973 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/pyth_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    26081 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/technical_analysis/__init__.py
+-rw-r--r--   0        0        0    54572 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/tools/__init__.py
+-rw-r--r--   0        0        0     6219 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/tools/tools_controller.py
+-rw-r--r--   0        0        0     1357 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/tools/tools_helpers.py
+-rw-r--r--   0        0        0     3447 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/tools/tools_model.py
+-rw-r--r--   0        0        0     2772 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/tools/tools_view.py
+-rw-r--r--   0        0        0    16935 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_prompt_toolkit.py
+-rw-r--r--   0        0        0    55138 2023-04-09 00:10:02.029455 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/coin_highs.png
+-rw-r--r--   0        0        0  2879534 2023-04-09 00:10:02.053456 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/luna_crash.html
+-rw-r--r--   0        0        0   350260 2023-04-09 00:10:02.053456 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/luna_supply.png
+-rw-r--r--   0        0        0   607642 2023-04-09 00:10:02.057457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/luna_terra.png
+-rw-r--r--   0        0        0    11988 2023-04-09 00:10:02.057457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb
+-rw-r--r--   0        0        0   667206 2023-04-09 00:10:02.061457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/tvl.png
+-rw-r--r--   0        0        0   465754 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/ust_terra.png
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/__init__.py
+-rw-r--r--   0        0        0    15437 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/dashboards_controller.py
+-rw-r--r--   0        0        0    15983 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/stream/Forecasting.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/stream/__init__.py
+-rw-r--r--   0        0        0    16808 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/stream/pages/Indicators.py
+-rw-r--r--   0        0        0     5481 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/chains.ipynb
+-rw-r--r--   0        0        0     6789 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/correlation.ipynb
+-rw-r--r--   0        0        0    13852 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/forecast.ipynb
+-rw-r--r--   0        0        0    10953 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/futures.ipynb
+-rw-r--r--   0        0        0     9421 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/shortdata.ipynb
+-rw-r--r--   0        0        0    15315 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/stocks.ipynb
+-rw-r--r--   0        0        0     5091 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/__init__.py
+-rw-r--r--   0        0        0    73682 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/econometrics_controller.py
+-rw-r--r--   0        0        0     2973 2023-04-09 00:10:02.065457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/econometrics_helpers.py
+-rw-r--r--   0        0        0    13544 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/econometrics_model.py
+-rw-r--r--   0        0        0    16620 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/econometrics_view.py
+-rw-r--r--   0        0        0    20449 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/regression_model.py
+-rw-r--r--   0        0        0     6739 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/regression_view.py
+-rw-r--r--   0        0        0       77 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/__init__.py
+-rw-r--r--   0        0        0    10230 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/alphavantage_model.py
+-rw-r--r--   0        0        0    12075 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/alphavantage_view.py
+-rw-r--r--   0        0        0     1614 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/commodity_model.py
+-rw-r--r--   0        0        0     1561 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/commodity_view.py
+-rw-r--r--   0        0        0      909 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv
+-rw-r--r--   0        0        0    21218 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/datasets/cpi.csv
+-rw-r--r--   0        0        0    10355 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/datasets/harmonized_cpi.csv
+-rw-r--r--   0        0        0    28404 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/econdb_model.py
+-rw-r--r--   0        0        0     8013 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/econdb_view.py
+-rw-r--r--   0        0        0    91589 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/economy_controller.py
+-rw-r--r--   0        0        0     3436 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/economy_helpers.py
+-rw-r--r--   0        0        0     1298 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/finnhub_model.py
+-rw-r--r--   0        0        0     2581 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/finnhub_view.py
+-rw-r--r--   0        0        0     7966 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/finviz_model.py
+-rw-r--r--   0        0        0     4600 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/finviz_view.py
+-rw-r--r--   0        0        0     9940 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/fred_model.py
+-rw-r--r--   0        0        0     9117 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/fred_view.py
+-rw-r--r--   0        0        0     6972 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/nasdaq_model.py
+-rw-r--r--   0        0        0     3286 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/nasdaq_view.py
+-rw-r--r--   0        0        0    38418 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/oecd_model.py
+-rw-r--r--   0        0        0    26364 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/oecd_view.py
+-rw-r--r--   0        0        0     3768 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/plot_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    28433 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0     1218 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/sdk_helpers.py
+-rw-r--r--   0        0        0    12870 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/wsj_model.py
+-rw-r--r--   0        0        0     4673 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/wsj_view.py
+-rw-r--r--   0        0        0    30415 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/yfinance_model.py
+-rw-r--r--   0        0        0     5055 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/yfinance_view.py
+-rw-r--r--   0        0        0      106 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/__init__.py
+-rw-r--r--   0        0        0     4023 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/discovery/disc_controller.py
+-rw-r--r--   0        0        0     2804 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/discovery/wsj_model.py
+-rw-r--r--   0        0        0     1320 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/discovery/wsj_view.py
+-rw-r--r--   0        0        0    21045 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/etf_controller.py
+-rw-r--r--   0        0        0      450 2023-04-09 00:10:02.069457 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/etf_helper.py
+-rw-r--r--   0        0        0   188615 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/etfs.csv
+-rw-r--r--   0        0        0     2608 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/financedatabase_model.py
+-rw-r--r--   0        0        0     3864 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/financedatabase_view.py
+-rw-r--r--   0        0        0     1417 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/fmp_model.py
+-rw-r--r--   0        0        0     3152 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/fmp_view.py
+-rw-r--r--   0        0        0     4172 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/stockanalysis_model.py
+-rw-r--r--   0        0        0     3941 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/stockanalysis_view.py
+-rw-r--r--   0        0        0    51458 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0     8025 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/featflags_controller.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/__init__.py
+-rw-r--r--   0        0        0    58622 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/corporate_spot_rates.csv
+-rw-r--r--   0        0        0     9217 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/ecb_model.py
+-rw-r--r--   0        0        0     7096 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/ecb_view.py
+-rw-r--r--   0        0        0     5811 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/econdb_model.py
+-rw-r--r--   0        0        0     7831 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/econdb_view.py
+-rw-r--r--   0        0        0    56207 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/fixedincome_controller.py
+-rw-r--r--   0        0        0    37985 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/fred_model.py
+-rw-r--r--   0        0        0    51962 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/fred_view.py
+-rw-r--r--   0        0        0   227110 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/ice_bofa_indices.csv
+-rw-r--r--   0        0        0    10963 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/oecd_model.py
+-rw-r--r--   0        0        0     3997 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/oecd_view.py
+-rw-r--r--   0        0        0     2174 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/yfinance_model.py
+-rw-r--r--   0        0        0     1702 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/yfinance_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/__init__.py
+-rw-r--r--   0        0        0     1547 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/anom_model.py
+-rw-r--r--   0        0        0     2962 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/anom_view.py
+-rw-r--r--   0        0        0     4629 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoarima_model.py
+-rw-r--r--   0        0        0     3933 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoarima_view.py
+-rw-r--r--   0        0        0     4658 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoces_model.py
+-rw-r--r--   0        0        0     3970 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoces_view.py
+-rw-r--r--   0        0        0     4694 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoets_model.py
+-rw-r--r--   0        0        0     3972 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoets_view.py
+-rw-r--r--   0        0        0     7272 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoselect_model.py
+-rw-r--r--   0        0        0     3938 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoselect_view.py
+-rw-r--r--   0        0        0     5874 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/brnn_model.py
+-rw-r--r--   0        0        0     6577 2023-04-09 00:10:02.073458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/brnn_view.py
+-rw-r--r--   0        0        0     5562 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/expo_model.py
+-rw-r--r--   0        0        0     5038 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/expo_view.py
+-rw-r--r--   0        0        0     2053 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/forecast.ipynb
+-rw-r--r--   0        0        0   121785 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/forecast_controller.py
+-rw-r--r--   0        0        0    15471 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/forecast_model.py
+-rw-r--r--   0        0        0     9034 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/forecast_view.py
+-rw-r--r--   0        0        0    47334 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/helpers.py
+-rw-r--r--   0        0        0     3405 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/linregr_model.py
+-rw-r--r--   0        0        0     4760 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/linregr_view.py
+-rw-r--r--   0        0        0     5013 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/mstl_model.py
+-rw-r--r--   0        0        0     3861 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/mstl_view.py
+-rw-r--r--   0        0        0     5896 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/nbeats_model.py
+-rw-r--r--   0        0        0     6396 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/nbeats_view.py
+-rw-r--r--   0        0        0     7561 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/nhits_model.py
+-rw-r--r--   0        0        0     7952 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/nhits_view.py
+-rw-r--r--   0        0        0     3007 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/regr_model.py
+-rw-r--r--   0        0        0     4521 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/regr_view.py
+-rw-r--r--   0        0        0     5030 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/rnn_model.py
+-rw-r--r--   0        0        0     5533 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/rnn_view.py
+-rw-r--r--   0        0        0     4340 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/rwd_model.py
+-rw-r--r--   0        0        0     3643 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/rwd_view.py
+-rw-r--r--   0        0        0     4709 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/seasonalnaive_model.py
+-rw-r--r--   0        0        0     3879 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/seasonalnaive_view.py
+-rw-r--r--   0        0        0     5790 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/tcn_model.py
+-rw-r--r--   0        0        0     6289 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/tcn_view.py
+-rw-r--r--   0        0        0     7249 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/tft_model.py
+-rw-r--r--   0        0        0     6520 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/tft_view.py
+-rw-r--r--   0        0        0     4928 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/theta_model.py
+-rw-r--r--   0        0        0     4379 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/theta_view.py
+-rw-r--r--   0        0        0     6321 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/trans_model.py
+-rw-r--r--   0        0        0     6765 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/trans_view.py
+-rw-r--r--   0        0        0    12580 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/whisper_model.py
+-rw-r--r--   0        0        0     2935 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/whisper_utils.py
+-rw-r--r--   0        0        0      122 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/__init__.py
+-rw-r--r--   0        0        0     5077 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/av_model.py
+-rw-r--r--   0        0        0     1458 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/av_view.py
+-rw-r--r--   0        0        0     3281 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/data/av_forex_currencies.csv
+-rw-r--r--   0        0        0     7847 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/data/polygon_tickers.csv
+-rw-r--r--   0        0        0   419838 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/data/yahoofinance_forex.json
+-rw-r--r--   0        0        0    16492 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/forex_controller.py
+-rw-r--r--   0        0        0     8211 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/forex_helper.py
+-rw-r--r--   0        0        0      931 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/fxempire_model.py
+-rw-r--r--   0        0        0     1471 2023-04-09 00:10:02.077458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/fxempire_view.py
+-rw-r--r--   0        0        0    17162 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/oanda/oanda_controller.py
+-rw-r--r--   0        0        0    22592 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/oanda/oanda_model.py
+-rw-r--r--   0        0        0    12856 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/oanda/oanda_view.py
+-rw-r--r--   0        0        0     2349 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/polygon_model.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    26168 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0     1446 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/sdk_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/technical_analysis/__init__.py
+-rw-r--r--   0        0        0    35136 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/__init__.py
+-rw-r--r--   0        0        0     2218 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/databento_view.py
+-rw-r--r--   0        0        0     8903 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/futures_controller.py
+-rw-r--r--   0        0        0      358 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/futures_helper.py
+-rw-r--r--   0        0        0      964 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/sdk_helper.py
+-rw-r--r--   0        0        0     4989 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/yfinance_model.py
+-rw-r--r--   0        0        0     7379 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/yfinance_view.py
+-rw-r--r--   0        0        0    13288 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/helper_classes.py
+-rw-r--r--   0        0        0    67647 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/helper_funcs.py
+-rw-r--r--   0        0        0     3212 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/helpers_denomination.py
+-rw-r--r--   0        0        0     9052 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/intro.json
+-rw-r--r--   0        0        0    42551 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/keys_controller.py
+-rw-r--r--   0        0        0    80350 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/keys_model.py
+-rw-r--r--   0        0        0     1148 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/keys_view.py
+-rw-r--r--   0        0        0     5984 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/loggers.py
+-rw-r--r--   0        0        0     1722 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/menu.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/alternative/covid/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/common/behavioural_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/common/prediction_techniques/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/common/quantitative_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/common/technical_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/custom/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/econometrics/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/economy/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/etf/movers/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/etf/screeners/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/mutual_funds/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/portfolio/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/portfolio/views/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/backtesting/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/behavioural_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/comparison_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/dark_pool_shorts/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/discovery/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/due_diligence/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/fundamental_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/government/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/insider/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/options/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/prediction_techniques/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/quantitative_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/raw_data/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/sector_industry_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/exports/stocks/technical_analysis/.gitkeep
+-rw-r--r--   0        0        0     8528 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/futures/futures.csv
+-rw-r--r--   0        0        0    60770 2023-04-09 00:10:02.081458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/i18n/en.yml
+-rw-r--r--   0        0        0     5831 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/i18n/help_translation.ipynb
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/.gitkeep
+-rw-r--r--   0        0        0       64 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/account/test_account.openbb
+-rw-r--r--   0        0        0       87 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_covid.openbb
+-rw-r--r--   0        0        0      153 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_oss.openbb
+-rw-r--r--   0        0        0      119 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_realestate.openbb
+-rw-r--r--   0        0        0      856 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb
+-rw-r--r--   0        0        0      802 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb
+-rw-r--r--   0        0        0     1192 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb
+-rw-r--r--   0        0        0      374 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_disc.openbb
+-rw-r--r--   0        0        0      168 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_nft.openbb
+-rw-r--r--   0        0        0     1229 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb
+-rw-r--r--   0        0        0     1533 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb
+-rw-r--r--   0        0        0      561 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb
+-rw-r--r--   0        0        0       87 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_shroom.openbb
+-rw-r--r--   0        0        0      768 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb
+-rw-r--r--   0        0        0      154 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_tools.openbb
+-rw-r--r--   0        0        0      120 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/dashboards/test_dashboards_base.openbb
+-rw-r--r--   0        0        0     1333 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb
+-rw-r--r--   0        0        0     2082 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb
+-rw-r--r--   0        0        0      155 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf.openbb
+-rw-r--r--   0        0        0       33 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ca.openbb
+-rw-r--r--   0        0        0       38 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_disc.openbb
+-rw-r--r--   0        0        0      878 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb
+-rw-r--r--   0        0        0      749 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb
+-rw-r--r--   0        0        0      301 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast.openbb
+-rw-r--r--   0        0        0      176 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast_advanced.openbb
+-rw-r--r--   0        0        0      241 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_base.openbb
+-rw-r--r--   0        0        0      108 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_load.openbb
+-rw-r--r--   0        0        0      745 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb
+-rw-r--r--   0        0        0       62 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda_base.openbb
+-rw-r--r--   0        0        0      630 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb
+-rw-r--r--   0        0        0      611 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb
+-rw-r--r--   0        0        0      173 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/futures/test_futures.openbb
+-rw-r--r--   0        0        0     1275 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb
+-rw-r--r--   0        0        0     1826 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb
+-rw-r--r--   0        0        0       98 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_boolean_args.openbb
+-rw-r--r--   0        0        0      683 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb
+-rw-r--r--   0        0        0       67 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_base.openbb
+-rw-r--r--   0        0        0       65 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_crypto.openbb
+-rw-r--r--   0        0        0      151 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_economy.openbb
+-rw-r--r--   0        0        0       83 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_equity.openbb
+-rw-r--r--   0        0        0      113 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_etf.openbb
+-rw-r--r--   0        0        0      174 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forecast.openbb
+-rw-r--r--   0        0        0      158 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forex.openbb
+-rw-r--r--   0        0        0      132 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_portfolio.openbb
+-rw-r--r--   0        0        0      102 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_run.openbb
+-rw-r--r--   0        0        0      258 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks.openbb
+-rw-r--r--   0        0        0      255 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ba.openbb
+-rw-r--r--   0        0        0     1513 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb
+-rw-r--r--   0        0        0      422 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ca.openbb
+-rw-r--r--   0        0        0      251 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_disc.openbb
+-rw-r--r--   0        0        0      145 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_dps.openbb
+-rw-r--r--   0        0        0     1874 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb
+-rw-r--r--   0        0        0       44 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_base.openbb
+-rw-r--r--   0        0        0       31 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_epsfc.openbb
+-rw-r--r--   0        0        0       31 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_revfc.openbb
+-rw-r--r--   0        0        0      470 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_gov.openbb
+-rw-r--r--   0        0        0      276 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ins.openbb
+-rw-r--r--   0        0        0      340 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options.openbb
+-rw-r--r--   0        0        0       91 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_payoff.openbb
+-rw-r--r--   0        0        0      121 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_pricing.openbb
+-rw-r--r--   0        0        0       82 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_screen.openbb
+-rw-r--r--   0        0        0      644 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb
+-rw-r--r--   0        0        0      170 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_scr.openbb
+-rw-r--r--   0        0        0      347 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_sia.openbb
+-rw-r--r--   0        0        0      717 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb
+-rw-r--r--   0        0        0       82 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_th.openbb
+-rw-r--r--   0        0        0       65 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/test_jupyter_base.openbb
+-rw-r--r--   0        0        0       16 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/test_keys_.openbb
+-rw-r--r--   0        0        0       46 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/test_news.openbb
+-rw-r--r--   0        0        0     1072 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/models/hub_credentials.json
+-rw-r--r--   0        0        0      380 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/models/local_credentials.json
+-rw-r--r--   0        0        0    17970 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx
+-rw-r--r--   0        0        0    29757 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx
+-rw-r--r--   0        0        0      310 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/routines/routine_example.openbb
+-rw-r--r--   0        0        0    22698 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/sources/openbb_default.json
+-rw-r--r--   0        0        0     2332 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini
+-rw-r--r--   0        0        0     2354 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini
+-rw-r--r--   0        0        0     2341 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini
+-rw-r--r--   0        0        0     2316 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini
+-rw-r--r--   0        0        0     2316 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Banks.ini
+-rw-r--r--   0        0        0     2346 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini
+-rw-r--r--   0        0        0     2336 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini
+-rw-r--r--   0        0        0     2346 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini
+-rw-r--r--   0        0        0     2307 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini
+-rw-r--r--   0        0        0     2309 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Construction.ini
+-rw-r--r--   0        0        0     2329 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini
+-rw-r--r--   0        0        0     2353 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini
+-rw-r--r--   0        0        0     2360 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini
+-rw-r--r--   0        0        0     2320 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini
+-rw-r--r--   0        0        0     2344 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini
+-rw-r--r--   0        0        0     2315 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini
+-rw-r--r--   0        0        0     2346 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini
+-rw-r--r--   0        0        0     2376 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini
+-rw-r--r--   0        0        0     2326 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Health.ini
+-rw-r--r--   0        0        0     2307 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini
+-rw-r--r--   0        0        0     2320 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini
+-rw-r--r--   0        0        0     2324 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini
+-rw-r--r--   0        0        0     2334 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini
+-rw-r--r--   0        0        0     2324 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Legal.ini
+-rw-r--r--   0        0        0     2313 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini
+-rw-r--r--   0        0        0     2341 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini
+-rw-r--r--   0        0        0     2296 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Mining.ini
+-rw-r--r--   0        0        0     2367 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini
+-rw-r--r--   0        0        0     2342 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini
+-rw-r--r--   0        0        0     2361 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini
+-rw-r--r--   0        0        0     2351 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini
+-rw-r--r--   0        0        0     2336 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini
+-rw-r--r--   0        0        0     2322 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini
+-rw-r--r--   0        0        0     2310 2023-04-09 00:10:02.085458 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini
+-rw-r--r--   0        0        0     2326 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini
+-rw-r--r--   0        0        0     2341 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini
+-rw-r--r--   0        0        0     2299 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini
+-rw-r--r--   0        0        0     2316 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini
+-rw-r--r--   0        0        0     2342 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini
+-rw-r--r--   0        0        0     2381 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini
+-rw-r--r--   0        0        0     2314 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini
+-rw-r--r--   0        0        0    34473 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/template.ini
+-rw-r--r--   0        0        0    34519 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/whales.ini
+-rw-r--r--   0        0        0     2688 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/README.md
+-rw-r--r--   0        0        0     4195 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/high_iv.ini
+-rw-r--r--   0        0        0     4210 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini
+-rw-r--r--   0        0        0     3925 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini
+-rw-r--r--   0        0        0     4202 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini
+-rw-r--r--   0        0        0     4079 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/template.ini
+-rwxr-xr-x   0        0        0      282 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/5pct_above_low.ini
+-rw-r--r--   0        0        0    21940 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt
+-rwxr-xr-x   0        0        0      315 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/analyst_strong_buy.ini
+-rwxr-xr-x   0        0        0      464 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/break_out_stocks.ini
+-rw-r--r--   0        0        0      413 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/buffett_like.ini
+-rwxr-xr-x   0        0        0      184 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/bull_runs_over_10pct.ini
+-rwxr-xr-x   0        0        0      364 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/channel_up_and_low_debt_and_sma_50and200.ini
+-rw-r--r--   0        0        0      326 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/cheap_bottom_dividend.ini
+-rw-r--r--   0        0        0      193 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/cheap_dividend.ini
+-rw-r--r--   0        0        0      241 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/cheap_oversold.ini
+-rwxr-xr-x   0        0        0      335 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/continued_momentum_scan.ini
+-rw-r--r--   0        0        0      286 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/death_cross.ini
+-rwxr-xr-x   0        0        0      167 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/djia_components.ini
+-rw-r--r--   0        0        0      221 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/golden_cross.ini
+-rwxr-xr-x   0        0        0      255 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/golden_cross_penny.ini
+-rwxr-xr-x   0        0        0      518 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini
+-rw-r--r--   0        0        0      302 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/heavy_inst_ins.ini
+-rwxr-xr-x   0        0        0      279 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/high_vol_and_low_debt.ini
+-rw-r--r--   0        0        0      316 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/modified_dreman.ini
+-rw-r--r--   0        0        0      349 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/modified_neff.ini
+-rwxr-xr-x   0        0        0      295 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/news_scanner.ini
+-rwxr-xr-x   0        0        0      274 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/oversold.ini
+-rwxr-xr-x   0        0        0      328 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/oversold_under_3dol.ini
+-rwxr-xr-x   0        0        0      301 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/oversold_under_5dol.ini
+-rwxr-xr-x   0        0        0      212 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/potential_reversals.ini
+-rwxr-xr-x   0        0        0      295 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/recent_growth_and_support.ini
+-rw-r--r--   0        0        0      337 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/rosenwald.ini
+-rw-r--r--   0        0        0      280 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/rosenwald_gtfo.ini
+-rw-r--r--   0        0        0      246 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sdk_guide_preset.ini
+-rw-r--r--   0        0        0      360 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sexy_year.ini
+-rwxr-xr-x   0        0        0      222 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/short_squeeze_scan.ini
+-rwxr-xr-x   0        0        0      260 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/simplistic_momentum_scanner_under_7dol.ini
+-rwxr-xr-x   0        0        0      197 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_basic_materials_sector.ini
+-rwxr-xr-x   0        0        0      211 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_communication_services_sector.ini
+-rwxr-xr-x   0        0        0      201 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_cyclical_sector.ini
+-rwxr-xr-x   0        0        0      203 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_defensive_sector.ini
+-rwxr-xr-x   0        0        0      179 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_energy_sector.ini
+-rwxr-xr-x   0        0        0      185 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_financial_sector.ini
+-rwxr-xr-x   0        0        0      187 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_healthcare_sector.ini
+-rwxr-xr-x   0        0        0      189 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_industrials_sector.ini
+-rwxr-xr-x   0        0        0      189 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_real_estate_sector.ini
+-rwxr-xr-x   0        0        0      187 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_technology_sector.ini
+-rwxr-xr-x   0        0        0      185 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/sp500_utilities_sector.ini
+-rwxr-xr-x   0        0        0      276 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/stocks_strong_support_levels.ini
+-rwxr-xr-x   0        0        0      272 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/top_performers_all.ini
+-rwxr-xr-x   0        0        0      299 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/top_performers_healthcare.ini
+-rwxr-xr-x   0        0        0      293 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/top_performers_tech.ini
+-rwxr-xr-x   0        0        0      286 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/under_15dol_stocks.ini
+-rw-r--r--   0        0        0      209 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/undervalue.ini
+-rwxr-xr-x   0        0        0      272 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/unusual_volume.ini
+-rwxr-xr-x   0        0        0      675 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini
+-rwxr-xr-x   0        0        0      315 2023-04-09 00:10:02.089459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/weak_support_and_top_performers.ini
+-rw-r--r--   0        0        0   358460 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/Consolas.ttf
+-rw-r--r--   0        0        0      972 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json
+-rw-r--r--   0        0        0      182 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/dark.mplrc.json
+-rw-r--r--   0        0        0     2086 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/dark.mplstyle
+-rw-r--r--   0        0        0     2750 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0      203 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/dark.richstyle.json
+-rw-r--r--   0        0        0      970 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json
+-rw-r--r--   0        0        0      182 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/light.mplrc.json
+-rw-r--r--   0        0        0     2035 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/light.mplstyle
+-rw-r--r--   0        0        0    24077 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0      202 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/light.richstyle.json
+-rw-r--r--   0        0        0     2607 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0      186 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/user/openbb.richstyle.json
+-rw-r--r--   0        0        0      144 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/__init__.py
+-rw-r--r--   0        0        0    81373 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/avanza_fund_ID.csv
+-rw-r--r--   0        0        0      834 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/avanza_model.py
+-rw-r--r--   0        0        0     3941 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/avanza_view.py
+-rw-r--r--   0        0        0     6535 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/mstarpy_model.py
+-rw-r--r--   0        0        0     7883 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/mstarpy_view.py
+-rw-r--r--   0        0        0    15141 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/mutual_fund_controller.py
+-rw-r--r--   0        0        0     6040 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/mutual_funds_utils.py
+-rw-r--r--   0        0        0    51025 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/parent_classes.py
+-rw-r--r--   0        0        0       61 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/__init__.py
+-rw-r--r--   0        0        0    15080 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/allocation_model.py
+-rw-r--r--   0        0        0    12944 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/attribution_model.py
+-rw-r--r--   0        0        0      417 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/bro_controller.py
+-rw-r--r--   0        0        0     1121 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/brokers_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.093459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/coinbase/__init__.py
+-rw-r--r--   0        0        0     8211 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py
+-rw-r--r--   0        0        0     9561 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py
+-rw-r--r--   0        0        0     4495 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py
+-rw-r--r--   0        0        0     4666 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/degiro/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/degiro/__init__.py
+-rw-r--r--   0        0        0    12789 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py
+-rw-r--r--   0        0        0    15571 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/degiro/degiro_model.py
+-rw-r--r--   0        0        0    15670 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/degiro/degiro_view.py
+-rw-r--r--   0        0        0     3894 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py
+-rw-r--r--   0        0        0     3002 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py
+-rw-r--r--   0        0        0     2482 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py
+-rw-r--r--   0        0        0    30861 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/metrics_model.py
+-rw-r--r--   0        0        0    54979 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_controller.py
+-rw-r--r--   0        0        0    39188 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_engine.py
+-rw-r--r--   0        0        0     9643 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_helper.py
+-rw-r--r--   0        0        0    60205 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_model.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/__init__.py
+-rw-r--r--   0        0        0     5255 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/excel_model.py
+-rw-r--r--   0        0        0     2106 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py
+-rw-r--r--   0        0        0   120571 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py
+-rw-r--r--   0        0        0   155050 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py
+-rw-r--r--   0        0        0     2773 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py
+-rw-r--r--   0        0        0    13116 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py
+-rw-r--r--   0        0        0     5965 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py
+-rw-r--r--   0        0        0     5346 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py
+-rw-r--r--   0        0        0     4427 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py
+-rw-r--r--   0        0        0   138034 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/po_controller.py
+-rw-r--r--   0        0        0     8587 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/po_engine.py
+-rw-r--r--   0        0        0   103568 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/po_model.py
+-rw-r--r--   0        0        0    24186 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/po_view.py
+-rw-r--r--   0        0        0    11390 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/statics.py
+-rw-r--r--   0        0        0    12009 2023-04-09 00:10:02.097459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py
+-rw-r--r--   0        0        0    54944 2023-04-09 00:10:02.101459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_view.py
+-rw-r--r--   0        0        0     8433 2023-04-09 00:10:02.101459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/statics.py
+-rw-r--r--   0        0        0     2877 2023-04-09 00:10:02.101459 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reporting.md
+-rw-r--r--   0        0        0  1028287 2023-04-09 00:10:02.105460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html
+-rw-r--r--   0        0        0     2839 2023-04-09 00:10:02.105460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.105460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/__init__.py
+-rw-r--r--   0        0        0      443 2023-04-09 00:10:02.105460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/data/crypto_tickers.csv
+-rw-r--r--   0        0        0      437 2023-04-09 00:10:02.105460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/data/etf_tickers.csv
+-rw-r--r--   0        0        0      222 2023-04-09 00:10:02.105460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/data/stocks_tickers.csv
+-rw-r--r--   0        0        0     9716 2023-04-09 00:10:02.105460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/reports_controller.py
+-rw-r--r--   0        0        0    12275 2023-04-09 00:10:02.105460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/reports_model.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.105460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/stored/.gitkeep
+-rw-r--r--   0        0        0  1076317 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html
+-rw-r--r--   0        0        0     5214 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/OpenBB_reports_logo.png
+-rw-r--r--   0        0        0    32298 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/crypto.ipynb
+-rw-r--r--   0        0        0    22724 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/economy.ipynb
+-rw-r--r--   0        0        0    39716 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/equity.ipynb
+-rw-r--r--   0        0        0     9851 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/etf.ipynb
+-rw-r--r--   0        0        0     2782 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/floppy-disc.png
+-rw-r--r--   0        0        0     8557 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/forecast.ipynb
+-rw-r--r--   0        0        0    17576 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/forex.ipynb
+-rw-r--r--   0        0        0    14912 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/portfolio.ipynb
+-rw-r--r--   0        0        0    11247 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/widget_helpers.py
+-rw-r--r--   0        0        0      205 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/widgets/card.j2
+-rw-r--r--   0        0        0     3556 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/widgets/report.css
+-rw-r--r--   0        0        0      474 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/widgets/report.j2
+-rw-r--r--   0        0        0      119 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/widgets/row.j2
+-rw-r--r--   0        0        0      896 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/widgets/style.css
+-rw-r--r--   0        0        0     9972 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/rich_config.py
+-rw-r--r--   0        0        0    30901 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/sdk.py
+-rw-r--r--   0        0        0    28128 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/settings_controller.py
+-rw-r--r--   0        0        0     7180 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/sources_controller.py
+-rw-r--r--   0        0        0      357 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/backtesting/__init__.py
+-rw-r--r--   0        0        0    10448 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/backtesting/bt_controller.py
+-rw-r--r--   0        0        0     8126 2023-04-09 00:10:02.113460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/backtesting/bt_model.py
+-rw-r--r--   0        0        0     9046 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/backtesting/bt_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/behavioural_analysis/__init__.py
+-rw-r--r--   0        0        0    29872 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/behavioural_analysis/ba_controller.py
+-rw-r--r--   0        0        0     3541 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     3761 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     1931 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/cboe_model.py
+-rw-r--r--   0        0        0      969 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/cboe_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/__init__.py
+-rw-r--r--   0        0        0    37655 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/ca_controller.py
+-rw-r--r--   0        0        0     4871 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/finbrain_model.py
+-rw-r--r--   0        0        0     5785 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/finbrain_view.py
+-rw-r--r--   0        0        0     1328 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     2679 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py
+-rw-r--r--   0        0        0     1539 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py
+-rw-r--r--   0        0        0    12381 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py
+-rw-r--r--   0        0        0     5757 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py
+-rw-r--r--   0        0        0     1690 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/polygon_model.py
+-rw-r--r--   0        0        0     1379 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py
+-rw-r--r--   0        0        0     8073 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py
+-rw-r--r--   0        0        0    10157 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/__init__.py
+-rw-r--r--   0        0        0    20377 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py
+-rw-r--r--   0        0        0    10009 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/finra_model.py
+-rw-r--r--   0        0        0     7203 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/finra_view.py
+-rw-r--r--   0        0        0     1093 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py
+-rw-r--r--   0        0        0     1200 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py
+-rw-r--r--   0        0        0     1387 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py
+-rw-r--r--   0        0        0     4648 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py
+-rw-r--r--   0        0        0     6836 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/sec_model.py
+-rw-r--r--   0        0        0     3470 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/sec_view.py
+-rw-r--r--   0        0        0     1882 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py
+-rw-r--r--   0        0        0     1385 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py
+-rw-r--r--   0        0        0     5053 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py
+-rw-r--r--   0        0        0     9997 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py
+-rw-r--r--   0        0        0     1166 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py
+-rw-r--r--   0        0        0     3613 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py
+-rw-r--r--   0        0        0      668 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py
+-rw-r--r--   0        0        0     1271 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py
+-rw-r--r--   0        0        0     5740 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/databento_model.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/__init__.py
+-rw-r--r--   0        0        0     4169 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/ark_model.py
+-rw-r--r--   0        0        0     2589 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/ark_view.py
+-rw-r--r--   0        0        0    31510 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/disc_controller.py
+-rw-r--r--   0        0        0      483 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/disc_helpers.py
+-rw-r--r--   0        0        0     2696 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/fidelity_model.py
+-rw-r--r--   0        0        0     2680 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/fidelity_view.py
+-rw-r--r--   0        0        0     4164 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/finnhub_model.py
+-rw-r--r--   0        0        0     2510 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/finnhub_view.py
+-rw-r--r--   0        0        0     1731 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/finviz_model.py
+-rw-r--r--   0        0        0     3084 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/finviz_view.py
+-rw-r--r--   0        0        0     2562 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/fmp_view.py
+-rw-r--r--   0        0        0     3051 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/nasdaq_model.py
+-rw-r--r--   0        0        0     3406 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/nasdaq_view.py
+-rw-r--r--   0        0        0     7080 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/seeking_alpha_model.py
+-rw-r--r--   0        0        0     4803 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/seeking_alpha_view.py
+-rw-r--r--   0        0        0     1120 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/shortinterest_model.py
+-rw-r--r--   0        0        0     2566 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/shortinterest_view.py
+-rw-r--r--   0        0        0     4113 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/yahoofinance_model.py
+-rw-r--r--   0        0        0     5871 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/yahoofinance_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/__init__.py
+-rw-r--r--   0        0        0    24082 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/av_model.py
+-rw-r--r--   0        0        0    14910 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/av_view.py
+-rw-r--r--   0        0        0    10834 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py
+-rw-r--r--   0        0        0     7680 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py
+-rw-r--r--   0        0        0     1833 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py
+-rw-r--r--   0        0        0     2347 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py
+-rw-r--r--   0        0        0    14888 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/dcf_model.py
+-rw-r--r--   0        0        0     4279 2023-04-09 00:10:02.117460 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/dcf_static.py
+-rw-r--r--   0        0        0    44464 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/dcf_view.py
+-rw-r--r--   0        0        0     1532 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py
+-rw-r--r--   0        0        0     1205 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py
+-rw-r--r--   0        0        0     2396 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py
+-rw-r--r--   0        0        0     4904 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py
+-rw-r--r--   0        0        0    81236 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/fa_controller.py
+-rw-r--r--   0        0        0      266 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/fa_helper.py
+-rw-r--r--   0        0        0     1389 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     3518 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     3419 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/finviz_model.py
+-rw-r--r--   0        0        0     2484 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/finviz_view.py
+-rw-r--r--   0        0        0    22210 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/fmp_model.py
+-rw-r--r--   0        0        0    25688 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/fmp_view.py
+-rw-r--r--   0        0        0     6417 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt
+-rw-r--r--   0        0        0    11855 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/market_watch_model.py
+-rw-r--r--   0        0        0     1509 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/market_watch_view.py
+-rw-r--r--   0        0        0     2217 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py
+-rw-r--r--   0        0        0     1259 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py
+-rw-r--r--   0        0        0     5391 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/polygon_model.py
+-rw-r--r--   0        0        0     4361 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/polygon_view.py
+-rw-r--r--   0        0        0     7593 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py
+-rw-r--r--   0        0        0    11162 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py
+-rw-r--r--   0        0        0     2059 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py
+-rw-r--r--   0        0        0    11829 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py
+-rw-r--r--   0        0        0    14679 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/government/__init__.py
+-rw-r--r--   0        0        0    18461 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/government/gov_controller.py
+-rw-r--r--   0        0        0    15719 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/government/quiverquant_model.py
+-rw-r--r--   0        0        0    21407 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/government/quiverquant_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/__init__.py
+-rw-r--r--   0        0        0     2062 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/businessinsider_model.py
+-rw-r--r--   0        0        0     5102 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/businessinsider_view.py
+-rw-r--r--   0        0        0     1125 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/finviz_model.py
+-rw-r--r--   0        0        0     1171 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/finviz_view.py
+-rw-r--r--   0        0        0    32744 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/insider_controller.py
+-rw-r--r--   0        0        0    87496 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/openinsider_model.py
+-rw-r--r--   0        0        0     7695 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/openinsider_view.py
+-rw-r--r--   0        0        0     4909 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/sdk_helper.py
+-rw-r--r--   0        0        0    76085 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/mappings/Mic_Codes.csv
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/alphaquery_model.py
+-rw-r--r--   0        0        0     1713 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/alphaquery_view.py
+-rw-r--r--   0        0        0     1161 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/barchart_model.py
+-rw-r--r--   0        0        0     1137 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/barchart_view.py
+-rw-r--r--   0        0        0     1526 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/calculator_model.py
+-rw-r--r--   0        0        0     2416 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/calculator_view.py
+-rw-r--r--   0        0        0     2777 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/chartexchange_model.py
+-rw-r--r--   0        0        0     3211 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/chartexchange_view.py
+-rw-r--r--   0        0        0     2433 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/fdscanner_model.py
+-rw-r--r--   0        0        0     1672 2023-04-09 00:10:02.121461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/fdscanner_view.py
+-rw-r--r--   0        0        0    21092 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/hedge/hedge_controller.py
+-rw-r--r--   0        0        0     9884 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/hedge/hedge_model.py
+-rw-r--r--   0        0        0     3968 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/hedge/hedge_view.py
+-rw-r--r--   0        0        0    10030 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/intrinio_model.py
+-rw-r--r--   0        0        0     6101 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/intrinio_view.py
+-rw-r--r--   0        0        0     7097 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/nasdaq_model.py
+-rw-r--r--   0        0        0    22486 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/op_helpers.py
+-rw-r--r--   0        0        0    52192 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/options_controller.py
+-rw-r--r--   0        0        0    10568 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/options_sdk_helper.py
+-rw-r--r--   0        0        0    14169 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/options_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/screen/__init__.py
+-rw-r--r--   0        0        0     5686 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/screen/screener_controller.py
+-rw-r--r--   0        0        0     9556 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/screen/syncretism_model.py
+-rw-r--r--   0        0        0     5566 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/screen/syncretism_view.py
+-rw-r--r--   0        0        0     8295 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/tradier_model.py
+-rw-r--r--   0        0        0     2561 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/tradier_view.py
+-rw-r--r--   0        0        0     7674 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/yfinance_model.py
+-rw-r--r--   0        0        0    11615 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/yfinance_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0     2260 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/beta_model.py
+-rw-r--r--   0        0        0     2798 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/beta_view.py
+-rw-r--r--   0        0        0     3187 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/factors_model.py
+-rw-r--r--   0        0        0      687 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/factors_view.py
+-rw-r--r--   0        0        0    38741 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0      447 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/qa_model.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/research/__init__.py
+-rw-r--r--   0        0        0     6218 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/research/res_controller.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/__init__.py
+-rw-r--r--   0        0        0    46491 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/finviz_model.py
+-rw-r--r--   0        0        0     6981 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/finviz_view.py
+-rw-r--r--   0        0        0    21493 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/screener_controller.py
+-rw-r--r--   0        0        0      944 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/screener_helper.py
+-rw-r--r--   0        0        0     2562 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/screener_view.py
+-rw-r--r--   0        0        0    27077 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/stock_statics.py
+-rw-r--r--   0        0        0    27315 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/stocks_controller.py
+-rw-r--r--   0        0        0    33068 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/stocks_helper.py
+-rw-r--r--   0        0        0    10576 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/stocks_model.py
+-rw-r--r--   0        0        0     1241 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/stocks_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/__init__.py
+-rw-r--r--   0        0        0     1004 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/finbrain_model.py
+-rw-r--r--   0        0        0      644 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/finbrain_view.py
+-rw-r--r--   0        0        0      761 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/finviz_model.py
+-rw-r--r--   0        0        0     1229 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/finviz_view.py
+-rw-r--r--   0        0        0     1532 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/rsp_model.py
+-rw-r--r--   0        0        0     2386 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/rsp_view.py
+-rw-r--r--   0        0        0    63334 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0     3260 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/tradingview_model.py
+-rw-r--r--   0        0        0     1985 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/tradingview_view.py
+-rw-r--r--   0        0        0      334 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/__init__.py
+-rw-r--r--   0        0        0     5328 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/bursa_model.py
+-rw-r--r--   0        0        0     2202 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/bursa_view.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/data/__init__.py
+-rw-r--r--   0        0        0    28098 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json
+-rw-r--r--   0        0        0     1466 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py
+-rw-r--r--   0        0        0     1378 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py
+-rw-r--r--   0        0        0    10137 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/tradinghours_controller.py
+-rw-r--r--   0        0        0      614 2023-04-09 00:10:02.125461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/tradinghours_helper.py
+-rw-r--r--   0        0        0    42825 2023-04-09 00:10:02.129461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/terminal_controller.py
+-rw-r--r--   0        0        0    13888 2023-04-09 00:10:02.129461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/terminal_helper.py
+-rw-r--r--   0        0        0     3848 2023-04-09 00:10:02.129461 openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/thought_of_the_day.py
+-rw-r--r--   0        0        0     5787 2023-04-09 00:10:04.169590 openbb_nightly-3.0.0rc1.dev20230409/pyproject.toml
+-rw-r--r--   0        0        0      945 2023-04-09 00:10:02.133461 openbb_nightly-3.0.0rc1.dev20230409/terminal.py
+-rw-r--r--   0        0        0     2293 2023-04-09 00:10:04.177591 openbb_nightly-3.0.0rc1.dev20230409/website/pypi.md
+-rw-r--r--   0        0        0     7850 1970-01-01 00:00:00.000000 openbb_nightly-3.0.0rc1.dev20230409/PKG-INFO
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/LICENSE` & `openbb_nightly-3.0.0rc1.dev20230409/LICENSE`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/SDK_README.md` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/SDK_README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/account/account_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/account/account_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import argparse
 import logging
-import os
 from pathlib import Path
 from typing import Dict, List, Optional
 
 from openbb_terminal.account.account_model import (
     get_routines_info,
+    read_routine,
+    save_routine,
     set_login_called,
 )
 from openbb_terminal.account.account_view import display_routines_list
-from openbb_terminal.core.session import (
-    hub_model as Hub,
-    local_model as Local,
-)
+from openbb_terminal.core.session import hub_model as Hub
 from openbb_terminal.core.session.current_user import (
     get_current_user,
     is_local,
 )
 from openbb_terminal.core.session.session_model import logout
 from openbb_terminal.custom_prompt_toolkit import NestedCompleter
 from openbb_terminal.decorators import log_start_end
@@ -69,29 +67,20 @@
                 {c: {} for c in self.REMOTE_CHOICES}
             )
             self.completer = NestedCompleter.from_nested_dict(self.choices)
 
     def get_routines(self):
         """Get routines"""
         current_user = get_current_user()
-        routines = {
+        return {
             filepath.name: filepath
-            for filepath in current_user.preferences.USER_ROUTINES_DIRECTORY.glob(
+            for filepath in current_user.preferences.USER_ROUTINES_DIRECTORY.rglob(
                 "*.openbb"
             )
         }
-        user_folder = (
-            current_user.preferences.USER_ROUTINES_DIRECTORY
-            / get_current_user().profile.get_uuid()
-        )
-        if os.path.exists(user_folder):
-            routines.update(
-                {filepath.name: filepath for filepath in user_folder.rglob("*.openbb")}
-            )
-        return routines
 
     def print_help(self):
         """Print help"""
         mt = MenuText("account/", 100)
         mt.add_info("_info_")
         mt.add_cmd("clear")
         mt.add_raw("\n")
@@ -142,15 +131,14 @@
             print_guest_block_msg()
         else:
             if ns_parser:
                 current_user = get_current_user()
                 logout(
                     auth_header=current_user.profile.get_auth_header(),
                     token=current_user.profile.get_token(),
-                    guest=is_local(),
                     cls=True,
                 )
                 self.print_help()
 
     @log_start_end(log=logger)
     def call_clear(self, other_args: List[str]):
         """Clear data"""
@@ -260,15 +248,15 @@
             nargs="+",
         )
         ns_parser = self.parse_known_args_and_warn(parser, other_args)
         if is_local() and "-h" not in other_args and "--help" not in other_args:
             print_guest_block_msg()
         else:
             if ns_parser:
-                routine = Local.get_routine(file_name=" ".join(ns_parser.file))
+                routine = read_routine(file_name=" ".join(ns_parser.file))
                 if routine:
                     description = " ".join(ns_parser.description)
 
                     name = (
                         " ".join(ns_parser.name)
                         if ns_parser.name
                         else " ".join(ns_parser.file).split(sep=".openbb", maxsplit=-1)[
@@ -347,26 +335,26 @@
                         description = data.get("description", "")
                         if description:
                             console.print(f"[info]Description:[/info] {description}")
 
                         script = data.get("script", "")
                         if script:
                             file_name = f"{name}.openbb"
-                            file_path = Local.save_routine(
+                            file_path = save_routine(
                                 file_name=file_name,
                                 routine=script,
                             )
                             if file_path == "File already exists":
                                 i = console.input(
                                     "\nA file with the same name already exists, "
                                     "do you want to replace it? (y/n): "
                                 )
                                 console.print("")
                                 if i.lower() in ["y", "yes"]:
-                                    file_path = Local.save_routine(
+                                    file_path = save_routine(
                                         file_name=file_name,
                                         routine=script,
                                         force=True,
                                     )
                                     if file_path:
                                         console.print(
                                             f"[info]Location:[/info] {file_path}"
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/account/account_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/google_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,152 +1,134 @@
-from pathlib import Path
-from typing import Any, Dict, Tuple
+"""Google Model"""
+__docformat__ = "numpy"
+
+import logging
 
-import numpy as np
 import pandas as pd
+from pytrends.request import TrendReq
 
-from openbb_terminal.base_helpers import strtobool
-from openbb_terminal.core.session.current_user import get_current_user
+from openbb_terminal.decorators import log_start_end
 from openbb_terminal.rich_config import console
 
-__login_called = False
-
-
-def get_login_called():
-    """Get the login/logout called flag.
-
-    Returns
-    -------
-    bool
-        The login/logout called flag.
-    """
-    return __login_called
-
-
-def set_login_called(value: bool):
-    """Set the login/logout called flag.
-
-    Parameters
-    ----------
-    value : bool
-        The login/logout called flag.
-    """
-    global __login_called  # pylint: disable=global-statement
-    __login_called = value
+logger = logging.getLogger(__name__)
 
 
-def get_diff(configs: dict) -> dict:
-    """Show the diff between the local and remote configs.
+@log_start_end(log=logger)
+def get_mentions(symbol: str) -> pd.DataFrame:
+    """Get interest over time from google api [Source: google].
 
     Parameters
     ----------
-    configs : dict
-        The configs.
+    symbol: str
+        Stock ticker symbol
 
     Returns
     -------
-    dict
-        The diff.
+    pd.DataFrame
+        Dataframe of interest over time
     """
-    KEYS = "features_keys"
-    configs_diff: Dict[str, Dict[str, Any]] = {KEYS: {}}
-
-    diff_keys = get_diff_keys(configs.get(KEYS, {}))
-    if diff_keys:
-        console.print("[info]Keys:[/info]")
-        for k, v in diff_keys.items():
-            configs_diff[KEYS][k] = v[1]
-            console.print(f"  [menu]{k}[/menu]: {v[0]} -> {v[1]}")
-
-    if not configs_diff[KEYS]:
-        configs_diff.pop(KEYS)
-
-    return configs_diff
-
-
-def get_diff_keys(keys: dict) -> dict:
-    """Get the diff between the local and remote keys.
+    try:
+        pytrend = TrendReq()
+        pytrend.build_payload(kw_list=[symbol])
+        return pytrend.interest_over_time()
+
+    except Exception as e:
+        if pytrend.google_rl:
+            console.print(f"[red]Too many requests: {pytrend.google_rl}[/red]\n")
+        else:
+            console.print(f"[red]{str(e)}[/red]\n")
+
+        return pd.DataFrame()
+
+
+@log_start_end(log=logger)
+def get_regions(symbol: str) -> pd.DataFrame:
+    """Get interest by region from google api [Source: google].
 
     Parameters
     ----------
-    configs : dict
-        The configs.
+    symbol: str
+        Ticker symbol to look at
 
     Returns
     -------
-    dict
-        The diff.
+    pd.DataFrame
+        Dataframe of interest by region
     """
-    current_user = get_current_user()
-    diff = {}
-    if keys:
-        for k, v in sorted(keys.items()):
-            if hasattr(current_user.credentials, k):
-                old, new = get_var_diff(current_user.credentials, k, v)
-                if new is not None:
-                    diff[k] = (old, new)
 
-    return diff
+    try:
+        pytrend = TrendReq()
+        pytrend.build_payload(kw_list=[symbol])
+        return pytrend.interest_by_region().sort_values([symbol], ascending=False)
+
+    except Exception as e:
+        if pytrend.google_rl:
+            console.print(f"[red]Too many requests: {pytrend.google_rl}[/red]\n")
+        else:
+            console.print(f"[red]{str(e)}[/red]\n")
 
+        return pd.DataFrame()
 
-def get_var_diff(obj, name, value) -> Tuple[Any, Any]:
-    """Set attribute in object.
+
+@log_start_end(log=logger)
+def get_queries(symbol: str, limit: int = 10) -> pd.DataFrame:
+    """Get related queries from google api [Source: google].
 
     Parameters
     ----------
-    obj : object
-        The object.
-    name : str
-        The attribute name.
-    value : str
-        The attribute value.
+    symbol: str
+        Stock ticker symbol to compare
+    limit: int
+        Number of queries to show
 
     Returns
     -------
-    Tuple[Any, Any]
-        The old and new values.
+    pd.DataFrame
+        Dataframe of related queries
     """
-    current_value = getattr(obj, name)
-
-    if str(value).lower() in ["true", "false"]:
-        cast_value = strtobool(value)
-    elif isinstance(getattr(obj, name), int):
-        cast_value = int(value)
-    elif isinstance(getattr(obj, name), float):
-        cast_value = float(value)
-    elif isinstance(getattr(obj, name), Path):
-        cast_value = Path(value)
-    else:
-        cast_value = value
-
-    if current_value != cast_value:
-        return current_value, cast_value
-
-    return None, None
-
-
-def get_routines_info(response) -> Tuple[pd.DataFrame, int, int]:
-    """Get the routines list.
+    try:
+        pytrend = TrendReq()
+        pytrend.build_payload(kw_list=[symbol])
+        df = pytrend.related_queries()
+        df = df[symbol]["top"].head(limit)
+        df["value"] = df["value"].apply(lambda x: str(x) + "%")
+        return df
+
+    except Exception as e:
+        if pytrend.google_rl:
+            console.print(f"[red]Too many requests: {pytrend.google_rl}[/red]\n")
+        else:
+            console.print(f"[red]{str(e)}[/red]\n")
+
+        return pd.DataFrame()
+
+
+@log_start_end(log=logger)
+def get_rise(symbol: str, limit: int = 10) -> pd.DataFrame:
+    """Get top rising related queries with this stock's query [Source: google].
 
     Parameters
     ----------
-    response : requests.Response
-        The response.
+    symbol: str
+        Stock ticker symbol
+    limit: int
+        Number of queries to show
 
     Returns
     -------
-    Tuple[pd.DataFrame, int, int]
-        The routines list, the current page and the total number of pages.
+    pd.DataFrame
+        Dataframe containing rising related queries
     """
-    df = pd.DataFrame()
-    page = 1
-    pages = 1
-    if response and response.status_code == 200:
-        data = response.json()
-        page = data.get("page", 1)
-        pages = data.get("pages", 1)
-        items = data.get("items", [])
-        if items:
-            df = pd.DataFrame(items)
-            df.index = np.arange(1, len(df) + 1)
+    try:
+        pytrend = TrendReq()
+        pytrend.build_payload(kw_list=[symbol])
+        df = pytrend.related_queries()
+        df = df[symbol]["rising"].head(limit)
+        return df
+
+    except Exception as e:
+        if pytrend.google_rl:
+            console.print(f"[red]Too many requests: {pytrend.google_rl}[/red]\n")
+        else:
+            console.print(f"[red]{str(e)}[/red]\n")
 
-    return df, page, pages
+        return pd.DataFrame()
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/account/account_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/account/account_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/alt_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/alt_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/covid/countries.txt` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/covid/countries.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/covid/covid_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/covid/covid_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/covid/covid_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/covid/covid_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/covid/covid_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/covid/covid_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/hackernews_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/hackernews_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/hackernews_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/hackernews_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/oss/github_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/oss/github_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/oss/github_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/oss/github_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/oss/oss_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/oss/oss_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/oss/runa_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/oss/runa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/oss/runa_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/oss/runa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/realestate/landRegistry_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/realestate/landRegistry_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/realestate/landRegistry_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/realestate/landRegistry_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/alternative/realestate/realestate_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/alternative/realestate/realestate_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/base_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/base_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/finbrain_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/finbrain_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/finnhub_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/google_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/stocktwits_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,134 +1,118 @@
-"""Google Model"""
+"""Stocktwits Model"""
 __docformat__ = "numpy"
 
 import logging
+from typing import Any, Dict, List, Tuple
 
 import pandas as pd
-from pytrends.request import TrendReq
 
 from openbb_terminal.decorators import log_start_end
-from openbb_terminal.rich_config import console
+from openbb_terminal.helper_funcs import request
 
 logger = logging.getLogger(__name__)
 
 
 @log_start_end(log=logger)
-def get_mentions(symbol: str) -> pd.DataFrame:
-    """Get interest over time from google api [Source: google].
+def get_bullbear(symbol: str) -> Tuple[int, int, int, int]:
+    """Gets bullbear sentiment for ticker [Source: stocktwits].
 
     Parameters
     ----------
-    symbol: str
-        Stock ticker symbol
+    symbol : str
+        Ticker symbol to look at
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe of interest over time
+    Tuple[int, int, int, int]
+        Watchlist count,
+        Number of cases found for ticker,
+        Number of bullish statements,
+        Number of bearish statements,
     """
-    try:
-        pytrend = TrendReq()
-        pytrend.build_payload(kw_list=[symbol])
-        return pytrend.interest_over_time()
-
-    except Exception as e:
-        if pytrend.google_rl:
-            console.print(f"[red]Too many requests: {pytrend.google_rl}[/red]\n")
-        else:
-            console.print(f"[red]{str(e)}[/red]\n")
+    result = request(f"https://api.stocktwits.com/api/2/streams/symbol/{symbol}.json")
+    if result.status_code == 200:
+        result_json = result.json()
+        watchlist_count = result_json["symbol"]["watchlist_count"]
+        n_cases = 0
+        n_bull = 0
+        n_bear = 0
+        for message in result_json["messages"]:
+            if message["entities"]["sentiment"]:
+                n_cases += 1
+                n_bull += message["entities"]["sentiment"]["basic"] == "Bullish"
+                n_bear += message["entities"]["sentiment"]["basic"] == "Bearish"
 
-        return pd.DataFrame()
+        return watchlist_count, n_cases, n_bull, n_bear
+    return 0, 0, 0, 0
 
 
 @log_start_end(log=logger)
-def get_regions(symbol: str) -> pd.DataFrame:
-    """Get interest by region from google api [Source: google].
+def get_messages(symbol: str, limit: int = 30) -> pd.DataFrame:
+    """Get last messages for a given ticker [Source: stocktwits].
 
     Parameters
     ----------
-    symbol: str
-        Ticker symbol to look at
+    symbol : str
+        Stock ticker symbol
+    limit : int
+        Number of messages to get
 
     Returns
     -------
     pd.DataFrame
-        Dataframe of interest by region
+        Dataframe of messages
     """
+    result = request(f"https://api.stocktwits.com/api/2/streams/symbol/{symbol}.json")
+    if result.status_code == 200:
+        return pd.DataFrame(
+            [message["body"] for message in result.json()["messages"][:limit]]
+        )
 
-    try:
-        pytrend = TrendReq()
-        pytrend.build_payload(kw_list=[symbol])
-        return pytrend.interest_by_region().sort_values([symbol], ascending=False)
-
-    except Exception as e:
-        if pytrend.google_rl:
-            console.print(f"[red]Too many requests: {pytrend.google_rl}[/red]\n")
-        else:
-            console.print(f"[red]{str(e)}[/red]\n")
-
-        return pd.DataFrame()
+    return pd.DataFrame()
 
 
 @log_start_end(log=logger)
-def get_queries(symbol: str, limit: int = 10) -> pd.DataFrame:
-    """Get related queries from google api [Source: google].
-
-    Parameters
-    ----------
-    symbol: str
-        Stock ticker symbol to compare
-    limit: int
-        Number of queries to show
+def get_trending() -> pd.DataFrame:
+    """Get trending tickers from stocktwits [Source: stocktwits].
 
     Returns
     -------
     pd.DataFrame
-        Dataframe of related queries
+        Dataframe of trending tickers and watchlist count
     """
-    try:
-        pytrend = TrendReq()
-        pytrend.build_payload(kw_list=[symbol])
-        df = pytrend.related_queries()
-        df = df[symbol]["top"].head(limit)
-        df["value"] = df["value"].apply(lambda x: str(x) + "%")
-        return df
-
-    except Exception as e:
-        if pytrend.google_rl:
-            console.print(f"[red]Too many requests: {pytrend.google_rl}[/red]\n")
-        else:
-            console.print(f"[red]{str(e)}[/red]\n")
+    result = request("https://api.stocktwits.com/api/2/trending/symbols.json")
+    if result.status_code == 200:
+        l_symbols = [
+            [symbol["symbol"], symbol["watchlist_count"], symbol["title"]]
+            for symbol in result.json()["symbols"]
+        ]
+
+        df_trending = pd.DataFrame(
+            l_symbols, columns=["Ticker", "Watchlist Count", "Name"]
+        )
+        return df_trending
 
-        return pd.DataFrame()
+    return pd.DataFrame()
 
 
 @log_start_end(log=logger)
-def get_rise(symbol: str, limit: int = 10) -> pd.DataFrame:
-    """Get top rising related queries with this stock's query [Source: google].
+def get_stalker(user: str, limit: int = 30) -> List[Dict[str, Any]]:
+    """Gets messages from given user [Source: stocktwits].
 
     Parameters
     ----------
-    symbol: str
-        Stock ticker symbol
-    limit: int
-        Number of queries to show
+    user : str
+        User to get posts for
+    limit : int, optional
+        Number of posts to get, by default 30
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe containing rising related queries
+    List[Dict[str, Any]]
+        List of posts
     """
-    try:
-        pytrend = TrendReq()
-        pytrend.build_payload(kw_list=[symbol])
-        df = pytrend.related_queries()
-        df = df[symbol]["rising"].head(limit)
-        return df
-
-    except Exception as e:
-        if pytrend.google_rl:
-            console.print(f"[red]Too many requests: {pytrend.google_rl}[/red]\n")
-        else:
-            console.print(f"[red]{str(e)}[/red]\n")
+    result = request(f"https://api.stocktwits.com/api/2/streams/user/{user}.json")
+    if result.status_code == 200:
+        return list(result.json()["messages"][:limit])
 
-        return pd.DataFrame()
+    return []
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/google_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/google_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/reddit_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/reddit_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/reddit_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/reddit_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/reddit_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/reddit_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/stocktwits_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/finviz_view.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,118 +1,103 @@
-"""Stocktwits Model"""
+""" FinViz View """
 __docformat__ = "numpy"
 
 import logging
-from typing import Any, Dict, List, Tuple
-
-import pandas as pd
+import os
+from typing import Optional
 
+from openbb_terminal import rich_config
+from openbb_terminal.core.session.current_user import get_current_user
 from openbb_terminal.decorators import log_start_end
-from openbb_terminal.helper_funcs import request
+from openbb_terminal.helper_funcs import export_data, print_rich_table
+from openbb_terminal.rich_config import console
+from openbb_terminal.stocks.fundamental_analysis import finviz_model
 
 logger = logging.getLogger(__name__)
 
 
 @log_start_end(log=logger)
-def get_bullbear(symbol: str) -> Tuple[int, int, int, int]:
-    """Gets bullbear sentiment for ticker [Source: stocktwits].
+def display_screen_data(
+    symbol: str, export: str = "", sheet_name: Optional[str] = None
+):
+    """FinViz ticker screener
 
     Parameters
     ----------
     symbol : str
-        Ticker symbol to look at
-
-    Returns
-    -------
-    Tuple[int, int, int, int]
-        Watchlist count,
-        Number of cases found for ticker,
-        Number of bullish statements,
-        Number of bearish statements,
+        Stock ticker symbol
+    export : str
+        Format to export data
     """
-    result = request(f"https://api.stocktwits.com/api/2/streams/symbol/{symbol}.json")
-    if result.status_code == 200:
-        result_json = result.json()
-        watchlist_count = result_json["symbol"]["watchlist_count"]
-        n_cases = 0
-        n_bull = 0
-        n_bear = 0
-        for message in result_json["messages"]:
-            if message["entities"]["sentiment"]:
-                n_cases += 1
-                n_bull += message["entities"]["sentiment"]["basic"] == "Bullish"
-                n_bear += message["entities"]["sentiment"]["basic"] == "Bearish"
+    fund_data = finviz_model.get_data(symbol)
 
-        return watchlist_count, n_cases, n_bull, n_bear
-    return 0, 0, 0, 0
+    if fund_data.empty:
+        console.print(f"No data found for {symbol}", style="bold red")
+        return
+
+    print_rich_table(
+        fund_data, title="Ticker Screener", show_index=True, export=bool(export)
+    )
+
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        "data",
+        fund_data,
+        sheet_name,
+    )
 
 
-@log_start_end(log=logger)
-def get_messages(symbol: str, limit: int = 30) -> pd.DataFrame:
-    """Get last messages for a given ticker [Source: stocktwits].
+def lambda_category_color_red_green(val: str) -> str:
+    """Add color to analyst rating
 
     Parameters
     ----------
-    symbol : str
-        Stock ticker symbol
-    limit : int
-        Number of messages to get
+    val : str
+        Analyst rating - Upgrade/Downgrade
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe of messages
+    str
+        Analyst rating with color
     """
-    result = request(f"https://api.stocktwits.com/api/2/streams/symbol/{symbol}.json")
-    if result.status_code == 200:
-        return pd.DataFrame(
-            [message["body"] for message in result.json()["messages"][:limit]]
-        )
 
-    return pd.DataFrame()
+    if val == "Upgrade":
+        return f"[green]{val}[/green]"
+    if val == "Downgrade":
+        return f"[red]{val}[/red]"
+    if val == "Reiterated":
+        return f"[yellow]{val}[/yellow]"
+    return val
 
 
 @log_start_end(log=logger)
-def get_trending() -> pd.DataFrame:
-    """Get trending tickers from stocktwits [Source: stocktwits].
-
-    Returns
-    -------
-    pd.DataFrame
-        Dataframe of trending tickers and watchlist count
-    """
-    result = request("https://api.stocktwits.com/api/2/trending/symbols.json")
-    if result.status_code == 200:
-        l_symbols = [
-            [symbol["symbol"], symbol["watchlist_count"], symbol["title"]]
-            for symbol in result.json()["symbols"]
-        ]
-
-        df_trending = pd.DataFrame(
-            l_symbols, columns=["Ticker", "Watchlist Count", "Name"]
-        )
-        return df_trending
-
-    return pd.DataFrame()
-
-
-@log_start_end(log=logger)
-def get_stalker(user: str, limit: int = 30) -> List[Dict[str, Any]]:
-    """Gets messages from given user [Source: stocktwits].
+def analyst(symbol: str, export: str = "", sheet_name: Optional[str] = None):
+    """Display analyst ratings. [Source: Finviz]
 
     Parameters
     ----------
-    user : str
-        User to get posts for
-    limit : int, optional
-        Number of posts to get, by default 30
-
-    Returns
-    -------
-    List[Dict[str, Any]]
-        List of posts
+    symbol : str
+        Stock ticker
+    export : str
+        Export dataframe data to csv,json,xlsx file
     """
-    result = request(f"https://api.stocktwits.com/api/2/streams/user/{user}.json")
-    if result.status_code == 200:
-        return list(result.json()["messages"][:limit])
+    df = finviz_model.get_analyst_data(symbol)
+
+    if rich_config.USE_COLOR and not get_current_user().preferences.USE_INTERACTIVE_DF:
+        df["category"] = df["category"].apply(lambda_category_color_red_green)
 
-    return []
+    print_rich_table(
+        df,
+        headers=list(df.columns),
+        show_index=True,
+        title="Display Analyst Ratings",
+        export=bool(export),
+    )
+
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        "analyst",
+        df,
+        sheet_name,
+    )
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/stocktwits_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/stocktwits_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/twitter_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/twitter_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/behavioural_analysis/twitter_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/behavioural_analysis/twitter_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/common_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/common_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/feedparser_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/feedparser_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/feedparser_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/feedparser_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/newsapi_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/newsapi_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/newsapi_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/newsapi_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/quantitative_analysis/qa_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/quantitative_analysis/qa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/quantitative_analysis/qa_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/quantitative_analysis/qa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/quantitative_analysis/rolling_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/quantitative_analysis/rolling_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/quantitative_analysis/rolling_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/quantitative_analysis/rolling_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/custom_indicators_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/custom_indicators_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/custom_indicators_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/custom_indicators_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/momentum_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/momentum_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/momentum_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/momentum_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/overlap_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/overlap_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/overlap_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/overlap_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/ta_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/trend_indicators_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/trend_indicators_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/trend_indicators_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/trend_indicators_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/volatility_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/volatility_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/volatility_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/volatility_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/volume_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/volume_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/technical_analysis/volume_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/technical_analysis/volume_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/ultima_newsmonitor_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/ultima_newsmonitor_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-""" Ultima Insights News Monitor Model """
+""" Ultima News Monitor Model """
 __docformat__ = "numpy"
 
 import logging
 import os
 from urllib.parse import quote
 
 import certifi
 import pandas as pd
 
 from openbb_terminal.core.session.current_user import get_current_user
-from openbb_terminal.decorators import check_api_key, log_start_end
+from openbb_terminal.decorators import log_start_end
+
+# from openbb_terminal.decorators import check_api_key
 from openbb_terminal.helper_funcs import request
 from openbb_terminal.rich_config import console
 
 logger = logging.getLogger(__name__)
 
 
-base_url = "https://api.ultimainsights.ai/v1"
+BASE_URL = "https://api.ultimainsights.ai/v1"
+NO_API_KEY = "REPLACE_ME"
 
 
 @log_start_end(log=logger)
-@check_api_key(["API_ULTIMAINSIGHTS_KEY"])
+# @check_api_key(["API_ULTIMA_KEY"])
 def get_news(term: str = "", sort: str = "articlePublishedDate") -> pd.DataFrame:
     """Get news for a given term and source. [Source: Ultima Insights News Monitor]
 
     Parameters
     ----------
     term : str
         term to search on the news articles
@@ -44,30 +47,36 @@
     # Necessary for installer so that it can locate the correct certificates for
     # API calls and https
     # https://stackoverflow.com/questions/27835619/urllib-and-ssl-certificate-verify-failed-error/73270162#73270162
     os.environ["REQUESTS_CA_BUNDLE"] = certifi.where()
     os.environ["SSL_CERT_FILE"] = certifi.where()
 
     current_user = get_current_user()
-    auth_header = {
-        "Authorization": f"Bearer {current_user.credentials.API_ULTIMAINSIGHTS_KEY}"
-    }
+    if current_user.credentials.API_ULTIMA_KEY == NO_API_KEY:
+        auth_header = None
+    else:
+        auth_header = {
+            "Authorization": f"Bearer {current_user.credentials.API_ULTIMA_KEY}"
+        }
 
     have_data = False
     limit = 0
 
     while not have_data:
         if term:
             term = quote(term)
             term = term.upper()
             term = term.strip()
             if term in supported_terms():
-                data = request(
-                    f"{base_url}/getNewsArticles/{term}", headers=auth_header
-                )
+                if auth_header:
+                    data = request(
+                        f"{BASE_URL}/getNewsArticles/{term}", headers=auth_header
+                    )
+                else:
+                    data = request(f"{BASE_URL}/getNewsArticles/{term}")
             else:
                 console.print(
                     "[red]Ticker not supported. Unable to retrieve data\n[/red]"
                 )
                 return pd.DataFrame()
         else:
             console.print("[red]No term specified. Unable to retrieve data\n[/red]")
@@ -80,14 +89,21 @@
                 have_data = True
             elif limit == 60:  # Breaking if 60 successful requests return no data
                 console.print("[red]Timeout occurred. Please try again\n[/red]")
                 break
             limit = limit + 1
 
         elif (
+            hasattr(data, "status") and data.status_code == 429
+        ):  # If data request failed
+            console.print(
+                "[red]Too many requests. Please get an API Key from https://www.ultimainsights.ai/[/red]"
+            )
+            break
+        elif (
             hasattr(data, "status") and data.status_code != 200
         ):  # If data request failed
             console.print("[red]Status code not 200. Unable to retrieve data\n[/red]")
             break
         else:
             # console.print("[red]Could not retrieve data\n[/red]")
             break
@@ -114,35 +130,35 @@
     )
     df["articlePublishedDate"] = pd.to_datetime(df["articlePublishedDate"])
     df = df.sort_values(by=[sort], ascending=False)
     return df
 
 
 @log_start_end(log=logger)
+# @check_api_key(["API_ULTIMA_KEY"])
 def supported_terms() -> list:
-    """Get supported terms for news. [Source: Ultima Insights]
+    """Get supported terms for news. [Source: Ultima]
 
     Returns
     -------
     terms: list
         list of supported terms (tickers)
 
     """
 
     # Necessary for installer so that it can locate the correct certificates for
     # API calls and https
     # https://stackoverflow.com/questions/27835619/urllib-and-ssl-certificate-verify-failed-error/73270162#73270162
     os.environ["REQUESTS_CA_BUNDLE"] = certifi.where()
     os.environ["SSL_CERT_FILE"] = certifi.where()
-    data = request(f"{base_url}/supportedTickers")
+    data = request(f"{BASE_URL}/supportedTickers")
     return list(data.json())
 
 
 @log_start_end(log=logger)
-@check_api_key(["API_ULTIMAINSIGHTS_KEY"])
 def get_company_info(ticker: str) -> dict:
     """Get company info for a given ticker. [Source: Ultima Insights]
 
     Parameters
     ----------
     ticker : str
         ticker to search for company info
@@ -155,17 +171,12 @@
 
     # Necessary for installer so that it can locate the correct certificates for
     # API calls and https
     # https://stackoverflow.com/questions/27835619/urllib-and-ssl-certificate-verify-failed-error/73270162#73270162
     os.environ["REQUESTS_CA_BUNDLE"] = certifi.where()
     os.environ["SSL_CERT_FILE"] = certifi.where()
 
-    current_user = get_current_user()
-    auth_header = {
-        "Authorization": f"Bearer {current_user.credentials.API_ULTIMAINSIGHTS_KEY}"
-    }
-
     if ticker in supported_terms():
-        data = request(f"{base_url}/getCompanyInfo/{ticker}", headers=auth_header)
+        data = request(f"{BASE_URL}/getCompanyInfo/{ticker}")
         return data.json()
     console.print("[red]Ticker not supported. Unable to retrieve data\n[/red]")
     return {}
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/common/ultima_newsmonitor_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/common/ultima_newsmonitor_view.py`

 * *Files 15% similar despite different names*

```diff
@@ -73,26 +73,24 @@
             for _, row in breaking_news.head(limit).iterrows():
                 console.print(f"> {row['Date']} - {row['Description']}")
                 console.print(row["URL"] + "\n")
             console.print("------------------------")
 
     articles = ultima_newsmonitor_model.get_news(term, sort)
     articles = articles.head(limit).sort_values(by="relevancyScore", ascending=False)
-    # console.print(f"News Powered by [purple]ULTIMA INSIGHTS[/purple].\nFor more info: https://www.ultimainsights.ai\n")
+    # console.print(f"News Powered by [purple]Ultima Insights[/purple].\nFor more info: https://www.ultimainsights.ai\n")
     for _, row in articles.iterrows():
         console.print(
-            f"> {row['articlePublishedDate']} - {row['articleHeadline']} -> [green]{row['riskCategory']}[/green] "
-            f"(\x1B[3m{row['riskElaboratedDescription']}\x1B[0m) -> "
-            f"[purple]relevancy score: {round(row['relevancyScore'], 2) if row['relevancyScore'] < 5 else 5}"
-            f"/5 Stars[/purple]"
+            f"> {row['articlePublishedDate']} - {row['articleHeadline']}\n"
+            f"[purple]Relevancy score: {round(row['relevancyScore'], 2) if row['relevancyScore'] < 5 else 5}"
+            f"/5 Stars[/purple]\n[green]{row['riskCategory']}[/green] "
+            f"(\x1B[3m{row['riskElaboratedDescription']}\x1B[0m)"
         )
-        console.print(row["articleURL"] + "\n")
-    console.print(
-        "[red]To report any issues, please visit https://beta.ultimainsights.ai/my-account/support[/red]\n"
-    )
+        console.print(f"Read more: {row['articleURL']}\n")
+    # console.print("[purple]To report any issues, please visit https://beta.ultimainsights.ai/my-account/support[/purple]\n")
     console.print()
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         f"news_{'_'.join(term)}_{'_'.join(sources)}",
         articles,
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/config_terminal.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/config_terminal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/completer/choices.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/completer/choices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/config/paths.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/config/paths.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,7 +18,10 @@
 I18N_DICT_LOCATION = MISCELLANEOUS_DIRECTORY / "i18n"
 
 # styles
 STYLES_DIRECTORY_REPO = MISCELLANEOUS_DIRECTORY / "styles"
 
 # sources
 DATA_SOURCES_DEFAULT_FILE = MISCELLANEOUS_DIRECTORY / "sources" / "openbb_default.json"
+
+# session
+SESSION_FILE_PATH = SETTINGS_DIRECTORY / "session.json"
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/config/paths_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/config/paths_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/integration_tests/README.md` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/integration_tests/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/integration_tests/integration_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/integration_tests/integration_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/collection/log_sender.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/collection/log_sender.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/collection/logging_clock.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/collection/logging_clock.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/collection/s3_sender.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/collection/s3_sender.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/common.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/common.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/custom_logger.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/custom_logger.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/directories.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/directories.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/expired_files.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/formatter_with_exceptions.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/path_tracking_file_handler.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/settings.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/log/generation/settings_logger.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/log/generation/settings_logger.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/__init__.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/base_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/credentials_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/credentials_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/preferences_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/preferences_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/profile_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/profile_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/sources_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/sources_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/system_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/system_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/models/user_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/models/user_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/assets/Terminal_icon.png` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/assets/icon.png` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/assets/icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/backend.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/config/openbb_styles.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/no_import.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/no_import.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/old_table.html` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/old_table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly.html` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/base.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/data_classes.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/plotly_ta/ta_class.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/table.html` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/bar_menus.js` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/bar_menus.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/css/style.css` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/css/style.css`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/helpers.js` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/helpers.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/main.js` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/main.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/main_table.js` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/main_table.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/plots/web/popups.js` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/plots/web/popups.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/scripts/sdk_audit.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/scripts/sdk_audit.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,17 +306,14 @@
         return model.StocksQuantitativeAnalysis()
 
     @property
     def screener(self):
         """Stocks Screener Submodule
 
         Attributes:
-            `arktrades`: Gets a dataframe of ARK trades for ticker\n
-            `historical`: View historical price of stocks that meet preset\n
-            `historical_chart`: View historical price of stocks that meet preset\n
             `screener_data`: Screener Overview\n
             `screener_data_chart`: Screener one of the following: overview, valuation, financial, ownership, performance, technical.\n
         """
 
         return model.StocksScreener()
 
     @property
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/__init__.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/alt_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/alt_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/crypto_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/crypto_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/econometrics_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/econometrics_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/economy_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/economy_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/etf_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/etf_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/forecast_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/forecast_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/forex_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/forex_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/funds_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/funds_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/futures_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/futures_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/keys_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/keys_sdk_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         `set_keys`: Set API keys in bundle.\n
         `shroom`: Set Shroom key\n
         `smartstake`: Set Smartstake key.\n
         `stocksera`: Set Stocksera key.\n
         `tokenterminal`: Set Token Terminal key.\n
         `tradier`: Set Tradier key\n
         `twitter`: Set Twitter key\n
-        `ultimainsights`: Set Ultima Insights key\n
+        `ultima`: Set Ultima Insights key\n
         `walert`: Set Walert key\n
     """
 
     _location_path = "keys"
 
     def __init__(self):
         super().__init__()
@@ -79,9 +79,9 @@
         self.set_keys = lib.keys_model.set_keys
         self.shroom = lib.keys_model.set_shroom_key
         self.smartstake = lib.keys_model.set_smartstake_key
         self.stocksera = lib.keys_model.set_stocksera_key
         self.tokenterminal = lib.keys_model.set_tokenterminal_key
         self.tradier = lib.keys_model.set_tradier_key
         self.twitter = lib.keys_model.set_twitter_key
-        self.ultimainsights = lib.keys_model.set_ultimainsights_key
+        self.ultima = lib.keys_model.set_ultima_key
         self.walert = lib.keys_model.set_walert_key
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/portfolio_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/portfolio_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/qa_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/qa_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/stocks_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/stocks_sdk_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -534,28 +534,22 @@
         self.historical_5 = lib.stocks_qa_factors_model.get_historical_5
 
 
 class StocksScreener(Category):
     """Screener Module.
 
     Attributes:
-        `arktrades`: Gets a dataframe of ARK trades for ticker\n
-        `historical`: View historical price of stocks that meet preset\n
-        `historical_chart`: View historical price of stocks that meet preset\n
         `screener_data`: Screener Overview\n
         `screener_data_chart`: Screener one of the following: overview, valuation, financial, ownership, performance, technical.\n
     """
 
     _location_path = "stocks.screener"
 
     def __init__(self):
         super().__init__()
-        self.arktrades = lib.stocks_screener_ark_model.get_ark_trades_by_ticker
-        self.historical = lib.stocks_screener_yahoofinance_model.historical
-        self.historical_chart = lib.stocks_screener_yahoofinance_view.historical
         self.screener_data = lib.stocks_screener_finviz_model.get_screener_data
         self.screener_data_chart = lib.stocks_screener_finviz_view.screener
 
 
 class StocksTechnicalAnalysis(Category):
     """Technical Analysis Module.
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/models/ta_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/models/ta_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/sdk_init.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/sdk_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,18 +397,14 @@
     syncretism_view as stocks_options_screen_syncretism_view,
 )
 
 # Stocks - Screener
 from openbb_terminal.stocks.screener import (
     finviz_model as stocks_screener_finviz_model,
     finviz_view as stocks_screener_finviz_view,
-    yahoofinance_model as stocks_screener_yahoofinance_model,
-    yahoofinance_view as stocks_screener_yahoofinance_view,
-    ark_model as stocks_screener_ark_model,
-    ark_view as stocks_screener_ark_view,
 )
 
 # Stocks - Technical Analysis
 from openbb_terminal.stocks.technical_analysis import (
     finbrain_model as stocks_ta_finbrain_model,
     finbrain_view as stocks_ta_finbrain_view,
     finviz_model as stocks_ta_finviz_model,
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/trail_map.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/trail_map.csv`

 * *Files 2% similar despite different names*

```diff
@@ -306,15 +306,15 @@
 keys.set_keys,keys_model.set_keys,
 keys.shroom,keys_model.set_shroom_key,
 keys.smartstake,keys_model.set_smartstake_key,
 keys.stocksera,keys_model.set_stocksera_key,
 keys.tokenterminal,keys_model.set_tokenterminal_key,
 keys.tradier,keys_model.set_tradier_key,
 keys.twitter,keys_model.set_twitter_key,
-keys.ultimainsights,keys_model.set_ultimainsights_key,
+keys.ultima,keys_model.set_ultima_key,
 keys.walert,keys_model.set_walert_key,
 login,sdk_session.login,
 logout,sdk_session.logout,
 news,common_ultima_newsmonitor_model.get_news,
 portfolio.alloc.assets,portfolio_model.get_assets_allocation,
 portfolio.alloc.countries,portfolio_model.get_countries_allocation,
 portfolio.alloc.regions,portfolio_model.get_regions_allocation,
@@ -528,16 +528,14 @@
 stocks.news,common_ultima_newsmonitor_model.get_news,
 stocks.process_candle,stocks_helper.process_candle,
 stocks.qa.beta,stocks_qa_beta_model.beta_model,stocks_qa_beta_view.beta_view
 stocks.qa.capm,stocks_qa_factors_model.capm_information,
 stocks.qa.fama_raw,stocks_qa_factors_model.get_fama_raw,
 stocks.qa.historical_5,stocks_qa_factors_model.get_historical_5,
 stocks.quote,stocks_model.get_quote,
-stocks.screener.arktrades,stocks_screener_ark_model.get_ark_trades_by_ticker,
-stocks.screener.historical,stocks_screener_yahoofinance_model.historical,stocks_screener_yahoofinance_view.historical
 stocks.screener.screener_data,stocks_screener_finviz_model.get_screener_data,stocks_screener_finviz_view.screener
 stocks.search,stocks_helper.search,
 stocks.ta.recom,stocks_ta_tradingview_model.get_tradingview_recommendation,stocks_ta_tradingview_view.print_recommendation
 stocks.ta.rsp,stocks_ta_rsp_model.get_rsp,stocks_ta_rsp_view.display_rsp
 stocks.ta.summary,stocks_ta_finbrain_model.get_technical_summary_report,stocks_ta_finbrain_view.technical_summary_report
 stocks.ta.view,stocks_ta_finviz_model.get_finviz_image,stocks_ta_finviz_view.view
 stocks.th.all,stocks_th_bursa_model.get_all,stocks_th_bursa_view.display_all
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/trail_map_forecasting.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/trail_map_forecasting.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/trail_map_optimization.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/trail_map_optimization.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sdk/trailmap.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sdk/trailmap.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/banner.txt` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/banner.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/current_system.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/current_system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/current_user.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/current_user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/env_handler.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/env_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/hub_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/hub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/local_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/pycoingecko_helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,310 +1,284 @@
+"""CoinGecko helpers"""
+__docformat__ = "numpy"
+
+import datetime as dt
 import json
-import os
-from pathlib import Path
-from typing import List, Optional, Union
-
-from openbb_terminal.core.config.paths import (
-    HIST_FILE_PATH,
-    MISCELLANEOUS_DIRECTORY,
-    SETTINGS_DIRECTORY,
-)
-from openbb_terminal.core.session.current_user import (
-    get_current_user,
-    get_env_dict,
-    set_credential,
-    set_preference,
-    set_sources,
-)
+import logging
+import math
+import textwrap
+from datetime import timezone
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+
+import pandas as pd
+import requests
+from bs4 import BeautifulSoup
+from dateutil import parser
+from requests.adapters import HTTPAdapter, RetryError
+from urllib3.util.retry import Retry
+
+from openbb_terminal.helper_funcs import get_user_agent, request
 from openbb_terminal.rich_config import console
 
-SESSION_FILE_PATH = SETTINGS_DIRECTORY / "session.json"
+logger = logging.getLogger(__name__)
 
+GECKO_BASE_URL = "https://www.coingecko.com"
 
-def save_session(data: dict, file_path: Path = SESSION_FILE_PATH):
-    """Save the login info to a file.
+DENOMINATION = ("usd", "btc", "eth")
 
-    Parameters
-    ----------
-    data : dict
-        The data to write.
-    file_path : Path
-        The file path.
-    """
-    try:
-        with open(file_path, "w") as file:
-            file.write(json.dumps(data))
-    except Exception:
-        console.print("[red]Failed to save session info.[/red]")
 
+def millify(n: Union[float, int]) -> str:
+    millnames = ["", "K", "M", "B", "T"]
+    n = float(n)
+    millidx = max(
+        0,
+        min(
+            len(millnames) - 1, int(math.floor(0 if n == 0 else math.log10(abs(n)) / 3))
+        ),
+    )
 
-def get_session(file_path: Path = SESSION_FILE_PATH) -> dict:
-    """Get the session info from the file.
+    return f"{n / 10 ** (3 * millidx):.0f}{millnames[millidx]}"
 
-    Parameters
-    ----------
-    file_path : Path
-        The file path.
+
+def calc_change(current: Union[float, int], previous: Union[float, int]):
+    """Calculates change between two different values"""
+    if current == previous:
+        return 0
+    try:
+        return ((current - previous) / previous) * 100.0
+    except ZeroDivisionError:
+        return float("inf")
+
+
+def get_btc_price() -> float:
+    """Get BTC/USD price from CoinGecko API
 
     Returns
     -------
-    dict
-        The session info.
+    str
+        latest bitcoin price in usd.
     """
-    try:
-        if os.path.isfile(file_path):
-            with open(file_path) as file:
-                return json.load(file)
-    except Exception:
-        console.print("\n[red]Failed to get login info.[/red]")
-    return {}
 
+    req = request(
+        "https://api.coingecko.com/api/v3/simple/"
+        "price?ids=bitcoin&vs_currencies=usd&include_market_cap"
+        "=false&include_24hr_vol"
+        "=false&include_24hr_change=false&include_last_updated_at=false"
+    )
+    return req.json()["bitcoin"]["usd"]
+
+
+def _retry_session(
+    url: str, retries: int = 3, backoff_factor: float = 1.0
+) -> requests.Session:
+    """Helper methods that retries to make request to CoinGecko
 
-def remove_session_file(file_path: Path = SESSION_FILE_PATH) -> bool:
-    """Remove the session file.
 
     Parameters
     ----------
-    file_path : Path
-        The file path.
+    url: str
+        Url to mount a session
+    retries: int
+        How many retries
+    backoff_factor: float
+        Backoff schema - time periods between retry
 
     Returns
     -------
-    bool
-        The status of the removal.
+    requests.Session
+        Mounted session
     """
 
-    try:
-        if os.path.isfile(file_path):
-            os.remove(file_path)
-            return True
-        return True
-    except Exception:
-        console.print(
-            f"\n[bold red]Failed to remove {file_path}"
-            "\nPlease delete this file manually![/bold red]"
-        )
-        return False
+    session = requests.Session()
+    retry = Retry(
+        total=retries,
+        read=retries,
+        connect=retries,
+        status_forcelist=[500, 502, 503, 504],
+        backoff_factor=backoff_factor,
+    )
+    adapter = HTTPAdapter(max_retries=retry)
+    session.mount(url, adapter)
+    return session
 
 
-def remove_cli_history_file(file_path: Path = HIST_FILE_PATH) -> bool:
-    """Remove the cli history file.
+def scrape_gecko_data(url: str) -> BeautifulSoup:
+    """Helper method that scrape Coin Gecko site.
 
     Parameters
     ----------
-    file_path : Path
-        The file path.
+    url : str
+        coin gecko url to scrape e.g: "https://www.coingecko.com/en/discover"
 
     Returns
     -------
-    bool
-        The status of the removal.
+        BeautifulSoup object
     """
-
+    headers = {"User-Agent": get_user_agent()}
+    session = _retry_session("https://www.coingecko.com")
     try:
-        if os.path.isfile(file_path):
-            os.remove(file_path)
-            return True
-        return True
-    except Exception:
-        console.print(
-            f"\n[bold red]Failed to remove {file_path}"
-            "\nPlease delete this file manually![/bold red]"
+        req = session.get(url, headers=headers)
+    except Exception as error:
+        logger.exception(error)
+        console.print(error)
+        raise RetryError(
+            "Connection error. Couldn't connect to CoinGecko and scrape the data. "
+            "Please visit CoinGecko site, and check if it's not under maintenance"
+        ) from error
+
+    if req.status_code >= 400:
+        raise Exception(
+            f"Couldn't connect to {url}. Status code: {req.status_code}. Reason: {req.reason}"
         )
-        return False
-
 
-def update_flair():
-    """Update the flair."""
-    if "FLAIR" not in get_env_dict():
-        MAX_FLAIR_LEN = 20
-        flair = "[" + get_current_user().profile.username[:MAX_FLAIR_LEN] + "]" + " 🦋"
-        set_preference("FLAIR", flair)
+    return BeautifulSoup(req.text, features="lxml")
 
 
-def apply_configs(configs: dict):
-    """Apply configurations.
+def replace_underscores_to_newlines(cols: list, line: int = 13) -> list:
+    """Helper method that replace underscores to white space and breaks it to new line
 
     Parameters
     ----------
-    configs : dict
-        The configurations.
+    cols
+        - list of columns names
+    line
+        - line length
+    Returns
+    -------
+        list of column names with replaced underscores
     """
-    # Saving the RICH_STYLE state allows user to change from hub rich style to local
-    set_credentials_from_hub(configs)
-    set_preferences_from_hub(configs, fields=["RICH_STYLE"])
-    set_rich_style_from_hub(configs)
-    set_chart_table_style_from_hub(configs)
-    set_sources_from_hub(configs)
 
+    return [
+        textwrap.fill(c.replace("_", " "), line, break_long_words=False)
+        for c in list(cols)
+    ]
 
-def set_credentials_from_hub(configs: dict):
-    """Set credentials from hub.
 
-    Parameters
-    ----------
-    configs : dict
-        The configurations.
-    """
-    if configs:
-        credentials = configs.get("features_keys", {}) or {}
-        for k, v in credentials.items():
-            set_credential(k, v)
+def find_discord(item: Optional[List[Any]]) -> Union[str, Any]:
+    if isinstance(item, list) and len(item) > 0:
+        discord = [chat for chat in item if "discord" in chat]
+        if len(discord) > 0:
+            return discord[0]
+    return None
 
 
-def set_preferences_from_hub(configs: dict, fields: Optional[List[str]] = None):
-    """Set preferences from hub.
+def join_list_elements(elem):
+    if isinstance(elem, dict):
+        return ", ".join(k for k, v in elem.items())
+    if isinstance(elem, list):
+        return ", ".join(k for k in elem)
+    return None
 
-    Parameters
-    ----------
-    configs : dict
-        The configurations.
-    fields : Optional[List[str]]
-        The fields to set, if None, all fields will be set.
-    """
-    if configs:
-        preferences = configs.get("features_settings", {}) or {}
-        for k, v in preferences.items():
-            if not fields:
-                set_preference(k, v)
-            elif k in fields:
-                set_preference(k, v)
 
+def filter_list(lst: Optional[List[Any]]) -> Optional[List[Any]]:
+    if isinstance(lst, list) and len(lst) > 0:
+        return [i for i in lst if i != ""]
+    return lst
 
-def set_rich_style_from_hub(configs: dict):
-    """Set rich style from hub.
 
-    Parameters
-    ----------
-    configs : dict
-        The configurations.
-    """
-    if configs:
-        terminal_style = configs.get("features_terminal_style", {}) or {}
-        if terminal_style:
-            rich_style = terminal_style.get("theme", None)
-            if rich_style:
-                rich_style = {k: v.replace(" ", "") for k, v in rich_style.items()}
-                try:
-                    with open(
-                        MISCELLANEOUS_DIRECTORY
-                        / "styles"
-                        / "user"
-                        / "hub.richstyle.json",
-                        "w",
-                    ) as f:
-                        json.dump(rich_style, f)
-
-                    # Default to hub theme
-                    preferences = configs.get("features_settings", {}) or {}
-                    if "RICH_STYLE" not in preferences:
-                        set_preference("RICH_STYLE", "hub")
+def calculate_time_delta(date: dt.datetime) -> int:
+    now = dt.datetime.now(timezone.utc)
+    if not isinstance(date, dt.datetime):
+        date = parser.parse(date)
+    return (now - date).days
 
-                except Exception:
-                    console.print("[red]Failed to set rich style.[/red]")
 
+def get_eth_addresses_for_cg_coins(file) -> pd.DataFrame:  # pragma: no cover
+    with open(file, encoding="utf8") as f:
+        data = json.load(f)
+        df = pd.DataFrame(data)
+        df["ethereum"] = df["platforms"].apply(
+            lambda x: x.get("ethereum") if "ethereum" in x else None
+        )
+        return df
 
-def set_chart_table_style_from_hub(configs: dict):
-    """Set chart and table style from hub.
 
-    Parameters
-    ----------
-    configs : dict
-        The configurations.
-    """
-    if configs:
-        terminal_style = configs.get("features_terminal_style", {}) or {}
-        if terminal_style:
-            chart_table = terminal_style.get("chart_table", None)
-            if chart_table:
-                set_preference("THEME", chart_table)
+def clean_question_marks(dct: dict) -> None:
+    if isinstance(dct, dict):
+        for k, v in dct.items():
+            if v == "?":
+                dct[k] = None
 
 
-def set_sources_from_hub(configs: dict):
-    """Set sources from hub.
+def replace_qm(df: pd.DataFrame) -> pd.DataFrame:
+    df.replace({"?": None, " ?": None}, inplace=True)
+    return df
 
-    Parameters
-    ----------
-    configs : dict
-        The configurations.
-    """
-    if configs:
-        sources = configs.get("features_sources", {}) or {}
-        if sources:
-            set_sources(sources)
 
+def get_url(url: str, elem: BeautifulSoup):  # pragma: no cover
+    return url + elem.find("a")["href"]
 
-def get_routine(file_name: str, folder: Optional[Path] = None) -> Optional[str]:
-    """Get the routine.
 
+def clean_row(row: BeautifulSoup) -> list:
+    """Helper method that cleans whitespaces and newlines in text returned from BeautifulSoup
+    Parameters
+    ----------
+    row
+        text returned from BeautifulSoup find method
     Returns
     -------
-    file_name : str
-        The routine.
-    folder : Optional[Path]
-        The routines folder.
+        list of elements
     """
 
-    current_user = get_current_user()
-    if folder is None:
-        folder = current_user.preferences.USER_ROUTINES_DIRECTORY
-
-    try:
-        user_folder = folder / current_user.profile.get_uuid()
-        file_path = (
-            user_folder / file_name
-            if os.path.exists(user_folder / file_name)
-            else folder / file_name
-        )
-
-        with open(file_path) as f:
-            routine = "".join(f.readlines())
-        return routine
-    except Exception:
-        console.print("[red]Failed to find routine.[/red]")
-        return None
-
+    return [r for r in row.text.strip().split("\n") if r not in ["", " "]]
 
-def save_routine(
-    file_name: str,
-    routine: str,
-    folder: Optional[Path] = None,
-    force: bool = False,
-) -> Union[Optional[Path], str]:
-    """Save the routine.
 
-    Parameters
-    ----------
-    file_name : str
-        The routine.
-    routine : str
-        The routine.
-    folder : Path
-        The routines folder.
-    force : bool
-        Force the save.
-
-    Returns
-    -------
-    Optional[Path, str]
-        The path to the routine or None.
-    """
+def convert(word: str) -> str:
+    return "".join(x.capitalize() or "_" for x in word.split("_") if word.isalpha())
 
-    current_user = get_current_user()
-    if folder is None:
-        folder = current_user.preferences.USER_ROUTINES_DIRECTORY
 
+def collateral_auditors_parse(
+    args: Any,
+) -> Tuple[Any, Any]:  # pragma: no cover
     try:
-        uuid = current_user.profile.get_uuid()
-        user_folder = folder / uuid
-        if not os.path.exists(user_folder):
-            os.makedirs(user_folder)
-
-        file_path = user_folder / file_name
-        if os.path.exists(file_path) and not force:
-            return "File already exists"
-        with open(file_path, "w") as f:
-            f.write(routine)
-        return user_folder / file_name
-    except Exception:
-        console.print("[red]\nFailed to save routine.[/red]")
-        return None
+        if args and args[0] == "N/A":
+            collateral = args[1:]
+            auditors = []
+        else:
+            n_elem = int(args[0])
+            auditors = args[1 : n_elem + 1]  # noqa: E203
+            collateral = args[n_elem + 1 :]  # noqa: E203
+
+        return auditors, collateral
+    except ValueError:
+        return [], []
+
+
+def swap_columns(df: pd.DataFrame) -> pd.DataFrame:
+    cols = list(df.columns)
+    cols = [cols[-1]] + cols[:-1]
+    df = df[cols]
+    return df
+
+
+def changes_parser(changes: list) -> list:
+    if isinstance(changes, list) and len(changes) < 3:
+        for _ in range(3 - len(changes)):
+            changes.append(None)
+    else:
+        changes = [None for _ in range(3)]
+    return changes
+
+
+def remove_keys(entries: tuple, the_dict: Dict[Any, Any]) -> None:
+    for key in entries:
+        if key in the_dict:
+            del the_dict[key]
+
+
+def rename_columns_in_dct(dct: dict, mapper: dict) -> dict:
+    return {mapper.get(k, v): v for k, v in dct.items()}
+
+
+def create_dictionary_with_prefixes(
+    columns: Sequence[Any], dct: Dict[Any, Any], constrains: Optional[Tuple] = None
+):  # type: ignore
+    results = {}
+    for column in columns:
+        ath_data = dct.get(column, {})
+        for element in ath_data:  # type: ignore
+            if constrains:  # type: ignore
+                if element in constrains:  # type: ignore
+                    results[f"{column}_" + element] = ath_data.get(element)  # type: ignore
+            else:
+                results[f"{column}_" + element] = ath_data.get(element)  # type: ignore
+    return results
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/sdk_session.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/sdk_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
     >>> from openbb_terminal.sdk import openbb
     >>> openbb.logout()
     """
     current_user = get_current_user()
     session_model.logout(
         auth_header=current_user.profile.get_auth_header(),
         token=current_user.profile.token,
-        guest=is_local(),
     )
 
 
 @log_start_end(log=logger)
 def whoami():
     """
     Display user info.
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/session_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/session_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/session_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/session_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import matplotlib.pyplot as plt
 
 import openbb_terminal.core.session.hub_model as Hub
 import openbb_terminal.core.session.local_model as Local
 from openbb_terminal.base_helpers import (
     remove_log_handlers,
 )
+from openbb_terminal.core.config.paths import HIST_FILE_PATH, SESSION_FILE_PATH
 from openbb_terminal.core.models.user_model import (
     CredentialsModel,
     ProfileModel,
     SourcesModel,
     UserModel,
 )
 from openbb_terminal.core.session.current_user import (
@@ -105,47 +106,46 @@
         return LoginStatus.FAILED
     return LoginStatus.NO_RESPONSE
 
 
 def logout(
     auth_header: Optional[str] = None,
     token: Optional[str] = None,
-    guest: bool = True,
     cls: bool = False,
 ):
     """Logout and clear session.
 
     Parameters
     ----------
     auth_header : str, optional
         The authorization header, e.g. "Bearer <token>".
     token : str, optional
         The token to delete.
         In the terminal we want to delete the current session, so we use the user own token.
-    guest : bool
-        True if the user is guest, False otherwise.
     cls : bool
         Clear the screen.
     """
     if cls:
         system_clear()
 
+    if not auth_header or not token:
+        return
+
     success = True
-    if not guest:
-        if not auth_header or not token:
-            return
-
-        r = Hub.delete_session(auth_header, token)
-        if not r or r.status_code != 200:
-            success = False
+    r = Hub.delete_session(auth_header, token)
+    if not r or r.status_code != 200:
+        success = False
 
-        if not Local.remove_session_file():
-            success = False
+    if not Local.remove(SESSION_FILE_PATH):
+        success = False
+
+    if not Local.remove(HIST_FILE_PATH):
+        success = False
 
-    if not Local.remove_cli_history_file():
+    if not Local.remove(get_current_user().preferences.USER_ROUTINES_DIRECTORY / "hub"):
         success = False
 
     remove_log_handlers()
     set_default_user()
     setup_logging()
 
     plt.close("all")
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/sources_handler.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/sources_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/session/utils.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/session/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/core/sources/utils.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/core/sources/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/coinbase_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/coinbase_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/coinpaprika_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/coinpaprika_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/crypto_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/crypto_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/crypto_models.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/crypto_models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/crypto_views.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/crypto_views.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/README.md` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/binance_gecko_map.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/binance_gecko_map.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/coingecko_categories.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/coingecko_categories.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/coingecko_coins.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/coingecko_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/defillama_dapps.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/defillama_dapps.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/erc20_coins.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/erc20_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/finbrain_coins.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/finbrain_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/santiment_slugs.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/santiment_slugs.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/dataframe_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/dataframe_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/coindix_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/coindix_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/coindix_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/coindix_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/defi_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/defi_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/graph_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/graph_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/graph_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/graph_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/llama_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/llama_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/llama_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/llama_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/smartstake_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/smartstake_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/smartstake_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/smartstake_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/substack_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/substack_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/substack_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/substack_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/terraengineer_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/terraengineer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/terraengineer_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/terraengineer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/dappradar_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/dappradar_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/dappradar_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/dappradar_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/discovery_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/discovery_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/binance_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/binance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/binance_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/binance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/messari_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/messari_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/messari_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/messari_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/nft_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/nft_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/opensea_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/opensea_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/nft/opensea_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/nft/opensea_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/bitquery_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/bitquery_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/bitquery_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/bitquery_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/blockchain_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/blockchain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/blockchain_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/blockchain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/onchain_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/onchain_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/shroom_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/shroom_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/shroom_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/shroom_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/coinbase_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/coinbase_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/glassnode_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/glassnode_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/glassnode_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/glassnode_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/loanscan_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/loanscan_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/loanscan_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/loanscan_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/overview_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/overview_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/rekt_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/rekt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/rekt_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/rekt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/pyth_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/pyth_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/pyth_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/pyth_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/tools/tools_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/tools/tools_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/tools/tools_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/tools/tools_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/tools/tools_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/tools/tools_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/cryptocurrency/tools/tools_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/cryptocurrency/tools/tools_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_prompt_toolkit.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_prompt_toolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     def __init__(
         self,
         words: Union[List[str], Callable[[], List[str]]],
         ignore_case: bool = False,
         display_dict: Optional[Mapping[str, AnyFormattedText]] = None,
         meta_dict: Optional[Mapping[str, AnyFormattedText]] = None,
-        WORD: bool = False,
+        WORD: bool = True,
         sentence: bool = False,
         match_middle: bool = False,
         pattern: Optional[Pattern[str]] = None,
     ) -> None:
         assert not (WORD and sentence)  # noqa: S101
 
         self.words = words
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/coin_highs.png` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/coin_highs.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/luna_crash.html` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/luna_crash.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/luna_supply.png` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/luna_supply.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/luna_terra.png` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/luna_terra.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/tvl.png` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/tvl.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/custom_reports/lunar_crash/ust_terra.png` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/custom_reports/lunar_crash/ust_terra.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/dashboards_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/dashboards_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/stream/Forecasting.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/stream/Forecasting.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/stream/pages/Indicators.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/stream/pages/Indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/chains.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/chains.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/correlation.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/correlation.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/forecast.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/futures.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/futures.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/shortdata.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/shortdata.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/dashboards/voila/stocks.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/dashboards/voila/stocks.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/decorators.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/econometrics_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/econometrics_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/econometrics_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/econometrics_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/econometrics_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/econometrics_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/econometrics_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/econometrics_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/regression_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/regression_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/econometrics/regression_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/econometrics/regression_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/alphavantage_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/alphavantage_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/alphavantage_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/alphavantage_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/commodity_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/commodity_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/commodity_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/commodity_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/datasets/cpi.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/datasets/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/datasets/harmonized_cpi.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/datasets/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/econdb_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/econdb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/econdb_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/econdb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/economy_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/economy_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/economy_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/economy_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/finnhub_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/fred_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/fred_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/fred_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/fred_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/nasdaq_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/nasdaq_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/nasdaq_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/oecd_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/oecd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/oecd_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/oecd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/plot_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/plot_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/wsj_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/wsj_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/wsj_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/wsj_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/yfinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/economy/yfinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/economy/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/discovery/disc_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/discovery/disc_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/discovery/wsj_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/discovery/wsj_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/discovery/wsj_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/discovery/wsj_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/etf_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/etf_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/etfs.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/etfs.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/financedatabase_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/financedatabase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/financedatabase_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/financedatabase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/fmp_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/fmp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/fmp_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/stockanalysis_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/stockanalysis_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/stockanalysis_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/stockanalysis_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/etf/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/etf/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/featflags_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/featflags_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/commercial_paper.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/corporate_spot_rates.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/ecb_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/ecb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/ecb_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/ecb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/econdb_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/econdb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/econdb_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/econdb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/fixedincome_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/fixedincome_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/fred_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/fred_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/fred_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/fred_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/ice_bofa_indices.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/oecd_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/oecd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/oecd_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/oecd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/yfinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/fixedincome/yfinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/fixedincome/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/anom_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/anom_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/anom_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/anom_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoarima_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoarima_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoarima_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoarima_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoces_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoces_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoces_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoces_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoets_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoets_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoets_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoets_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoselect_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoselect_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/autoselect_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/autoselect_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/brnn_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/brnn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/brnn_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/brnn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/expo_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/expo_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/expo_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/expo_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/forecast.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/forecast_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/forecast_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/forecast_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/forecast_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/forecast_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/forecast_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/linregr_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/linregr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/linregr_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/linregr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/mstl_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/mstl_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/mstl_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/mstl_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/nbeats_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/nbeats_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/nbeats_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/nbeats_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/nhits_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/nhits_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/nhits_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/nhits_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/regr_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/regr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/regr_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/regr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/rnn_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/rnn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/rnn_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/rnn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/rwd_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/rwd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/rwd_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/rwd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/seasonalnaive_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/seasonalnaive_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/seasonalnaive_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/seasonalnaive_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/tcn_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/tcn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/tcn_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/tcn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/tft_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/tft_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/tft_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/tft_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/theta_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/theta_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/theta_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/theta_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/trans_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/trans_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/trans_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/trans_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/whisper_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/whisper_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forecast/whisper_utils.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forecast/whisper_utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/av_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/av_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/av_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/av_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/data/av_forex_currencies.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/data/av_forex_currencies.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/data/polygon_tickers.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/data/polygon_tickers.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/data/yahoofinance_forex.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/data/yahoofinance_forex.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/forex_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/forex_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/forex_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/forex_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/fxempire_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/fxempire_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/fxempire_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/fxempire_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/oanda/oanda_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/oanda/oanda_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/oanda/oanda_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/oanda/oanda_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/oanda/oanda_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/oanda/oanda_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/polygon_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/forex/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/forex/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/databento_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/databento_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/futures_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/futures_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/sdk_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/yfinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/futures/yfinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/futures/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/helper_classes.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/helper_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/helper_funcs.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/helpers_denomination.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/helpers_denomination.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/intro.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/intro.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/keys_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/keys_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1233,20 +1233,20 @@
         ns_parser = self.parse_simple_args(parser, other_args)
         if ns_parser:
             self.status_dict["databento"] = keys_model.set_databento_key(
                 key=ns_parser.key, persist=True, show_output=True
             )
 
     @log_start_end(log=logger)
-    def call_ultimainsights(self, other_args: List[str]):
+    def call_ultima(self, other_args: List[str]):
         """Process ultima command"""
         parser = argparse.ArgumentParser(
             add_help=False,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-            prog="ultimainsights",
+            prog="ultima",
             description="Set Ultima Insights API key.",
         )
         parser.add_argument(
             "-k",
             "--key",
             type=str,
             dest="key",
@@ -1256,10 +1256,10 @@
             console.print("For your API Key, https://ultimainsights.ai/")
             return
 
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-k")
         ns_parser = self.parse_simple_args(parser, other_args)
         if ns_parser:
-            self.status_dict["ultimainsights"] = keys_model.set_ultimainsights_key(
+            self.status_dict["ultima"] = keys_model.set_ultima_key(
                 key=ns_parser.key, persist=True, show_output=True
             )
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/keys_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/keys_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 API_DICT: Dict = {
     "av": "ALPHA_VANTAGE",
     "fmp": "FINANCIAL_MODELING_PREP",
     "quandl": "QUANDL",
     "polygon": "POLYGON",
     "intrinio": "INTRINIO",
     "databento": "DATABENTO",
-    "ultimainsights": "ULTIMAINSIGHTS",
+    "ultima": "ULTIMA",
     "fred": "FRED",
     "news": "NEWSAPI",
     "tradier": "TRADIER",
     "cmc": "COINMARKETCAP",
     "finnhub": "FINNHUB",
     "reddit": "REDDIT",
     "twitter": "TWITTER",
@@ -2783,17 +2783,15 @@
 
     if show_output:
         console.print(status.colorize())
 
     return str(status)
 
 
-def set_ultimainsights_key(
-    key: str, persist: bool = False, show_output: bool = False
-) -> str:
+def set_ultima_key(key: str, persist: bool = False, show_output: bool = False) -> str:
     """Set Ultima Insights key
 
     Parameters
     ----------
     key: str
         API key
     persist: bool, optional
@@ -2807,22 +2805,22 @@
     -------
     str
         Status of key set
 
     Examples
     --------
     >>> from openbb_terminal.sdk import openbb
-    >>> openbb.keys.ultima_insights(key="example_key")
+    >>> openbb.keys.ultima(key="example_key")
     """
 
-    handle_credential("API_ULTIMAINSIGHTS_KEY", key, persist)
-    return check_ultimainsights_key(show_output)
+    handle_credential("API_ULTIMA_KEY", key, persist)
+    return check_ultima_key(show_output)
 
 
-def check_ultimainsights_key(show_output: bool = False) -> str:
+def check_ultima_key(show_output: bool = False) -> str:
     """Check Ultima Insights key
 
     Parameters
     ----------
     show_output: bool
         Display status string or not. By default, False.
 
@@ -2830,22 +2828,22 @@
     -------
     str
         Status of key set
     """
 
     current_user = get_current_user()
 
-    if current_user.credentials.API_ULTIMAINSIGHTS_KEY == "REPLACE_ME":
+    if current_user.credentials.API_ULTIMA_KEY == "REPLACE_ME":
         logger.info("Ultima Insights key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = request(
             "https://api.ultimainsights.ai/v1/checkAPIKey",
             headers={
-                "Authorization": f"Bearer {current_user.credentials.API_ULTIMAINSIGHTS_KEY}"
+                "Authorization": f"Bearer {current_user.credentials.API_ULTIMA_KEY}"
             },
         )
         if r.status_code in [403, 401, 429]:
             logger.warning("Ultima Insights key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
             logger.info("Ultima Insights key defined, test passed")
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/keys_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/keys_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/loggers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/loggers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/menu.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/menu.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/futures/futures.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/futures/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/i18n/en.yml` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/i18n/en.yml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   account/revoke: Revoke the Personal Access Token
   account/_info_: Cloud storage of keys
   account/clear: Clear keys from cloud
   account/_routines_: Cloud storage of routines
   account/list: List available routines
   account/upload: Upload routine
   account/download: Download routine
-  account/delete: Delete routine
+  account/delete: Delete routine stored in cloud
   keys/_source: Source
   keys/_keys_: This menu allows you to set your own API keys. Type 'about' for more information
   keys/mykeys: get your defined keys
   keys/status: reevaluate keys status
   keys/_status_: Status
   defined, test passed: defined, test passed
   defined, test failed: defined, test failed
@@ -246,22 +246,20 @@
   stocks/dps/dpotc: dark pools (ATS) vs OTC data
   stocks/dps/ftd: fails-to-deliver data
   stocks/dps/spos: net short vs position
   stocks/dps/psi: price vs short interest volume
   stocks/scr/view: view available presets (defaults and customs)
   stocks/scr/set: set one of the available presets
   stocks/scr/_preset: Preset
-  stocks/scr/historical: view historical price
   stocks/scr/overview: overview (e.g. Sector, Industry, Market Cap, Volume)
   stocks/scr/valuation: valuation (e.g. P/E, PEG, P/S, P/B, EPS this Y)
   stocks/scr/financial: financial (e.g. Dividend, ROA, ROE, ROI, Earnings)
   stocks/scr/ownership: ownership (e.g. Float, Insider Own, Short Ratio)
   stocks/scr/performance: performance (e.g. Perf Week, Perf YTD, Volatility M)
   stocks/scr/technical: technical (e.g. Beta, SMA50, 52W Low, RSI, Change)
-  stocks/scr/arktrades: get ARK trades for a chosen ticker
   stocks/scr/_screened_tickers: Last screened tickers
   stocks/scr/ca: take these to comparison analysis menu
   stocks/ins/view: view available presets
   stocks/ins/set: set one of the available presets
   stocks/ins/_preset: Preset
   stocks/ins/filter: filter insiders based on preset
   stocks/ins/load: load a specific stock ticker for analysis
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/i18n/help_translation.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/i18n/help_translation.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/models/hub_credentials.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/models/hub_credentials.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9459459459459459%*

 * *Differences: {"'API_ULTIMA_KEY'": "''", 'delete': "['API_ULTIMAINSIGHTS_KEY']"}*

```diff
@@ -29,10 +29,10 @@
     "API_SMARTSTAKE_KEY": "",
     "API_SMARTSTAKE_TOKEN": "",
     "API_STOCKSERA_KEY": "",
     "API_TOKEN_TERMINAL_KEY": "",
     "API_TWITTER_BEARER_TOKEN": "",
     "API_TWITTER_KEY": "",
     "API_TWITTER_SECRET_KEY": "",
-    "API_ULTIMAINSIGHTS_KEY": "",
+    "API_ULTIMA_KEY": "",
     "API_WHALE_ALERT_KEY": ""
 }
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/sources/openbb_default.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/sources/openbb_default.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993882275132275%*

 * *Differences: {"'stocks'": "{'news': {insert: [(2, 'Ultima')], delete: [0]}, 'disc': {'cnews': {delete: [0]}}}"}*

```diff
@@ -868,15 +868,14 @@
             "arkord": [
                 "CathiesArk"
             ],
             "asc": [
                 "YahooFinance"
             ],
             "cnews": [
-                "UltimaInsights",
                 "SeekingAlpha"
             ],
             "divcal": [
                 "Nasdaq"
             ],
             "filings": [
                 "FinancialModelingPrep"
@@ -1207,17 +1206,17 @@
             "AlphaVantage",
             "Polygon",
             "EODHD",
             "Intrinio",
             "DataBento"
         ],
         "news": [
-            "UltimaInsights",
             "Feedparser",
-            "NewsApi"
+            "NewsApi",
+            "Ultima"
         ],
         "options": {
             "binom": [
                 "YahooFinance"
             ],
             "calc": [],
             "chains": [
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Banks.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Banks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Construction.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Construction.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Health.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Health.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Legal.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Legal.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Mining.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Mining.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/template.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/template.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/insider/whales.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/insider/whales.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/README.md` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/high_iv.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/high_iv.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/options/template.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/options/template.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/Consolas.ttf` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/Consolas.ttf`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/dark.mplstyle` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/dark.mplstyle`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/light.mplstyle` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/light.mplstyle`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/avanza_fund_ID.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/avanza_fund_ID.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/avanza_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/avanza_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/avanza_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/avanza_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/mstarpy_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/mstarpy_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/mstarpy_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/mstarpy_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/mutual_fund_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/mutual_fund_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/mutual_funds/mutual_funds_utils.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/mutual_funds/mutual_funds_utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/parent_classes.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/parent_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/allocation_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/allocation_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/attribution_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/attribution_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/bro_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/bro_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/brokers_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/brokers_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/degiro/README.md` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/degiro/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/degiro/degiro_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/degiro/degiro_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/degiro/degiro_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/degiro/degiro_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/metrics_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/metrics_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_engine.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_engine.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/excel_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/excel_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/po_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/po_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/po_engine.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/po_engine.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/po_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/po_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/po_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/po_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/statics.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/portfolio_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/portfolio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/portfolio/statics.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/portfolio/statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reporting.md` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reporting.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/README.md` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/reports_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/reports_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/reports_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/reports_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/OpenBB_reports_logo.png` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/OpenBB_reports_logo.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/crypto.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/crypto.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/economy.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/economy.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/equity.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/equity.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/etf.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/etf.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/floppy-disc.png` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/floppy-disc.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/forecast.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/forex.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/forex.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/templates/portfolio.ipynb` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/templates/portfolio.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/widget_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/widget_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/widgets/report.css` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/widgets/report.css`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/reports/widgets/style.css` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/reports/widgets/style.css`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/rich_config.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/rich_config.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/sdk.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
             `set_keys`: Set API keys in bundle.\n
             `shroom`: Set Shroom key\n
             `smartstake`: Set Smartstake key.\n
             `stocksera`: Set Stocksera key.\n
             `tokenterminal`: Set Token Terminal key.\n
             `tradier`: Set Tradier key\n
             `twitter`: Set Twitter key\n
-            `ultimainsights`: Set Ultima Insights key\n
+            `ultima`: Set Ultima Insights key\n
             `walert`: Set Walert key\n
         """
 
         return model.KeysRoot()
 
     @property
     def portfolio(self):
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/settings_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/settings_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/sources_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/sources_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Sources Controller Module"""
 __docformat__ = "numpy"
 
 # IMPORTATION STANDARD
 import argparse
 import logging
+import os
 from pathlib import Path
 from typing import List, Optional
 
 from openbb_terminal.core.session.constants import SOURCES_URL
 
 # IMPORTATION THIRDPARTY
 # IMPORTATION INTERNAL
@@ -37,42 +38,47 @@
     ]
     PATH = "/sources/"
     CHOICES_GENERATION = True
 
     def __init__(self, queue: Optional[List[str]] = None):
         """Constructor"""
         super().__init__(queue)
-
+        self.source = "default"
         if session and get_current_user().preferences.USE_PROMPT_TOOLKIT:
             self.choices: dict = self.choices_default
             self.completer = NestedCompleter.from_nested_dict(self.choices)
 
+    def update_print_help(self):
+        """Update print help"""
+        sources_file = get_current_user().preferences.USER_DATA_SOURCES_FILE
+        if is_local():
+            if Path(sources_file).exists() and os.stat(sources_file).st_size > 0:
+                self.source = sources_file
+        else:
+            self.source = SOURCES_URL
+
     def parse_input(self, an_input: str) -> List:
         """Parse controller input
 
         Overrides the parent class function to handle github org/repo path convention.
         See `BaseController.parse_input()` for details.
         """
-        cmd_filter = r"((set\ --cmd |set\ -c |get\ --cmd |get\ -c ).*?("
+        cmd_filter = r"((set\s+--cmd\s+|set\s+-c\s+|set\s+|get\s+--cmd\s+|get\s+-c\s+|get\s+).*?("
         for cmd in get_current_user().sources.sources_dict:
             cmd = cmd.replace("/", r"\/")
             cmd_filter += f"{cmd}|"
         cmd_filter += ")*)"
+
         commands = parse_and_split_input(an_input=an_input, custom_filters=[cmd_filter])
         return commands
 
     def print_help(self):
         """Print help"""
         mt = MenuText("sources/")
-        mt.add_param(
-            "_source",
-            get_current_user().preferences.USER_DATA_SOURCES_FILE
-            if is_local()
-            else SOURCES_URL,
-        )
+        mt.add_param("_source", self.source)
         mt.add_raw("\n")
         mt.add_info("_info_")
         mt.add_cmd("get")
         mt.add_cmd("set")
         console.print(text=mt.menu_text, menu="Data Sources")
 
     @log_start_end(log=logger)
@@ -86,15 +92,15 @@
         )
         parser.add_argument(
             "-c",
             "--cmd",
             action="store",
             dest="cmd",
             choices=list(get_current_user().sources.sources_dict.keys()),
-            required="-h" not in other_args,
+            required="-h" not in other_args and "--help" not in other_args,
             help="Command that we want to check the available data sources and the default one.",
             metavar="COMMAND",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-c")
         ns_parser = self.parse_simple_args(parser, other_args)
         if ns_parser:
@@ -105,14 +111,15 @@
             elif len(cmd_defaults) == 0:
                 console.print("This command has no data sources available.\n")
             else:
                 console.print(
                     f"[param]Default   :[/param] {cmd_defaults[0]}\n"
                     f"[param]Available :[/param] {', '.join(cmd_defaults)}"
                 )
+        self.update_print_help()
 
     @log_start_end(log=logger)
     def call_set(self, other_args):
         """Process set command"""
         parser = argparse.ArgumentParser(
             add_help=False,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -136,14 +143,23 @@
             dest="source",
             type=str,
             required="-h" not in other_args and "--help" not in other_args,
             help="Data source to use by default on specified command.",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-c")
+
+        if (
+            other_args
+            and len(other_args) >= 2
+            and "-s" not in other_args
+            and "--source" not in other_args
+        ):
+            other_args.insert(2, "-s")
+
         ns_parser = self.parse_simple_args(parser, other_args)
         if ns_parser:
             sources_dict = get_current_user().sources.sources_dict
             if ns_parser.source in sources_dict[ns_parser.cmd]:
                 sources_dict[ns_parser.cmd].remove(ns_parser.source)
                 sources_dict[ns_parser.cmd].insert(0, ns_parser.source)
                 set_sources(sources_dict)
@@ -168,7 +184,8 @@
                 )
             else:
                 console.print(
                     f"[red]'{ns_parser.source}' is not a valid data source for "
                     f"'{ns_parser.cmd}' command.[/red]\n"
                     f"[param]\nAvailable :[/param] {', '.join(sources_dict[ns_parser.cmd])}\n"
                 )
+        self.update_print_help()
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/backtesting/bt_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/backtesting/bt_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/backtesting/bt_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/backtesting/bt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/backtesting/bt_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/backtesting/bt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/behavioural_analysis/ba_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/behavioural_analysis/ba_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/cboe_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/cboe_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/cboe_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/cboe_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/ca_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/ca_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/finbrain_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/finbrain_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/polygon_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/finra_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/finra_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/finra_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/finra_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/sec_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/sec_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/sec_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/sec_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/databento_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/databento_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/ark_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/ark_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/ark_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/ark_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/disc_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/disc_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/fidelity_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/fidelity_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/fidelity_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/fidelity_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/finnhub_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/fmp_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/nasdaq_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/nasdaq_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/nasdaq_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/seeking_alpha_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/seeking_alpha_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/seeking_alpha_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/seeking_alpha_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/shortinterest_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/shortinterest_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/shortinterest_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/shortinterest_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/yahoofinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/yahoofinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/discovery/yahoofinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/discovery/yahoofinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/av_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/av_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/av_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/av_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/dcf_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/dcf_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/dcf_static.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/dcf_static.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/dcf_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/dcf_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/fa_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/fa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/rsp_view.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,77 @@
-""" FinViz View """
+""" Relative Strength Percentile View """
 __docformat__ = "numpy"
 
 import logging
 import os
 from typing import Optional
 
-from openbb_terminal import rich_config
-from openbb_terminal.core.session.current_user import get_current_user
+import pandas as pd
+
 from openbb_terminal.decorators import log_start_end
 from openbb_terminal.helper_funcs import export_data, print_rich_table
 from openbb_terminal.rich_config import console
-from openbb_terminal.stocks.fundamental_analysis import finviz_model
+from openbb_terminal.stocks.technical_analysis import rsp_model
 
 logger = logging.getLogger(__name__)
 
 
 @log_start_end(log=logger)
-def display_screen_data(
-    symbol: str, export: str = "", sheet_name: Optional[str] = None
+def display_rsp(
+    s_ticker: str = "",
+    export: str = "",
+    sheet_name: Optional[str] = None,
+    tickers_show: bool = False,
 ):
-    """FinViz ticker screener
-
-    Parameters
-    ----------
-    symbol : str
-        Stock ticker symbol
-    export : str
-        Format to export data
-    """
-    fund_data = finviz_model.get_data(symbol)
-
-    if fund_data.empty:
-        console.print(f"No data found for {symbol}", style="bold red")
-        return
-
-    print_rich_table(
-        fund_data, title="Ticker Screener", show_index=True, export=bool(export)
-    )
-
-    export_data(
-        export,
-        os.path.dirname(os.path.abspath(__file__)),
-        "data",
-        fund_data,
-        sheet_name,
-    )
-
-
-def lambda_category_color_red_green(val: str) -> str:
-    """Add color to analyst rating
+    """Display Relative Strength Percentile [Source: https://github.com/skyte/relative-strength]
 
     Parameters
     ----------
-    val : str
-        Analyst rating - Upgrade/Downgrade
-
-    Returns
-    -------
-    str
-        Analyst rating with color
-    """
-
-    if val == "Upgrade":
-        return f"[green]{val}[/green]"
-    if val == "Downgrade":
-        return f"[red]{val}[/red]"
-    if val == "Reiterated":
-        return f"[yellow]{val}[/yellow]"
-    return val
-
-
-@log_start_end(log=logger)
-def analyst(symbol: str, export: str = "", sheet_name: Optional[str] = None):
-    """Display analyst ratings. [Source: Finviz]
-
-    Parameters
-    ----------
-    symbol : str
+    s_ticker : str
         Stock ticker
     export : str
-        Export dataframe data to csv,json,xlsx file
+        Format of export file
+    tickers_show : bool
+        Boolean to check if tickers in the same industry as the stock should be shown
     """
-    df = finviz_model.get_analyst_data(symbol)
-
-    if rich_config.USE_COLOR and not get_current_user().preferences.USE_INTERACTIVE_DF:
-        df["category"] = df["category"].apply(lambda_category_color_red_green)
 
-    print_rich_table(
-        df,
-        headers=list(df.columns),
-        show_index=True,
-        title="Display Analyst Ratings",
-        export=bool(export),
-    )
-
-    export_data(
-        export,
-        os.path.dirname(os.path.abspath(__file__)),
-        "analyst",
-        df,
-        sheet_name,
-    )
+    rsp_stock, rsp_industry, df_stock_p, df_industries_p = rsp_model.get_rsp(s_ticker)
+    if rsp_stock.empty or rsp_industry.empty:
+        console.print(f"[red]Ticker '{s_ticker}' not found.\n[/red]")
+    else:
+        tickers = pd.DataFrame(rsp_industry["Tickers"])
+        del rsp_industry["Tickers"]
+        print_rich_table(
+            rsp_stock,
+            headers=list(rsp_stock.columns),
+            show_index=False,
+            title="Relative Strength Percentile of Stock (relative to SPY)",
+            export=bool(export),
+        )
+        print_rich_table(
+            rsp_industry,
+            headers=list(rsp_industry.columns),
+            show_index=False,
+            title="Relative Strength Percentile of Industry the ticker is part of",
+            export=bool(export),
+        )
+        if tickers_show:
+            print_rich_table(
+                tickers,
+                headers=list(tickers.columns),
+                show_index=False,
+                title="Tickers in same industry as chosen stock",
+            )
+        export_data(
+            export,
+            os.path.dirname(os.path.abspath(__file__)).replace("common", "stocks"),
+            "rsp_stock",
+            df_stock_p,
+            sheet_name,
+        )
+        export_data(
+            export,
+            os.path.dirname(os.path.abspath(__file__)).replace("common", "stocks"),
+            "rsp_industry",
+            df_industries_p,
+            sheet_name,
+        )
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/fmp_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/fmp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/fmp_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/market_watch_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/market_watch_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/market_watch_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/market_watch_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/polygon_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/polygon_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/polygon_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/government/gov_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/government/gov_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/government/quiverquant_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/government/quiverquant_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/government/quiverquant_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/government/quiverquant_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/businessinsider_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/businessinsider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/businessinsider_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/businessinsider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/insider_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/insider_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/openinsider_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/openinsider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/openinsider_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/openinsider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/insider/sdk_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/insider/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/mappings/Mic_Codes.csv` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/mappings/Mic_Codes.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/alphaquery_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/alphaquery_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/alphaquery_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/alphaquery_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/barchart_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/barchart_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/barchart_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/barchart_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/calculator_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/calculator_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/calculator_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/calculator_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/chartexchange_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/chartexchange_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/chartexchange_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/chartexchange_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/fdscanner_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/fdscanner_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/fdscanner_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/fdscanner_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/hedge/hedge_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/hedge/hedge_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/hedge/hedge_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/hedge/hedge_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/hedge/hedge_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/hedge/hedge_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/intrinio_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/intrinio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/intrinio_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/intrinio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/nasdaq_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/op_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/op_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/options_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/options_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/options_sdk_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/options_sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/options_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/options_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/screen/screener_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/screen/screener_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/screen/syncretism_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/screen/syncretism_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/screen/syncretism_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/screen/syncretism_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/tradier_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/tradier_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/tradier_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/tradier_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/yfinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/options/yfinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/options/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/beta_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/beta_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/beta_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/beta_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/factors_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/factors_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/factors_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/factors_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/research/res_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/research/res_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/ark_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/stocks_view.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,47 @@
-"""ARK View"""
-__docformat__ = "numpy"
-
 import logging
 import os
 from typing import Optional
 
-import pandas as pd
-
-from openbb_terminal.decorators import log_start_end
+from openbb_terminal.decorators import check_api_key, log_start_end
 from openbb_terminal.helper_funcs import export_data, print_rich_table
 from openbb_terminal.rich_config import console
-from openbb_terminal.stocks.screener import ark_model
+from openbb_terminal.stocks import stocks_model
 
 logger = logging.getLogger(__name__)
 
 
 @log_start_end(log=logger)
-def display_ark_trades(
-    symbol: str,
-    limit: int = 20,
-    show_symbol: bool = False,
-    export: str = "",
-    sheet_name: Optional[str] = None,
-):
-    """Display ARK trades for ticker
+@check_api_key(["API_KEY_FINANCIALMODELINGPREP"])
+def display_quote(symbol: str, export: str = "", sheet_name: Optional[str] = None):
+    """Financial Modeling Prep ticker quote
 
     Parameters
     ----------
-    symbol: str
-        Ticker to get trades for
-    limit: int
-        Number of rows to show
-    show_symbol: bool
-        Flag to show ticker in table
-    export: str, optional
+    symbol : str
+        Fundamental analysis ticker symbol
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    export: str
         Format to export data
     """
-    ark_holdings = ark_model.get_ark_trades_by_ticker(symbol)
 
-    if ark_holdings.empty:
-        console.print(
-            "Issue getting data from cathiesark.com.  Likely no trades found.\n"
-        )
+    quote = stocks_model.get_quote(symbol)
+    if quote.empty:
+        console.print("[red]Data not found[/red]\n")
         return
-
-    # Since this is for a given ticker, no need to show it
-    if not show_symbol:
-        ark_holdings = ark_holdings.drop(columns=["ticker"])
-    ark_holdings["Total"] = ark_holdings["Total"] / 1_000_000
-    ark_holdings.rename(
-        columns={"Close": "Close ($)", "Total": "Total ($1M)"}, inplace=True
-    )
-
-    ark_holdings.index = pd.Series(ark_holdings.index).apply(
-        lambda x: x.strftime("%Y-%m-%d")
-    )
     print_rich_table(
-        ark_holdings,
-        headers=list(ark_holdings.columns),
+        quote,
+        headers=["Value"],
+        title=f"{symbol.upper()} Quote",
+        index_name="Info",
         show_index=True,
-        title="ARK Trades",
         export=bool(export),
-        limit=limit,
     )
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
-        "arktrades",
-        ark_holdings,
+        "quote",
+        quote,
         sheet_name,
     )
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/finviz_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 }
 
 
 @log_start_end(log=logger)
 def get_screener_data(
     preset_loaded: str = "top_gainers",
     data_type: str = "overview",
-    limit: int = 10,
+    limit: int = -1,
     ascend: bool = False,
 ):
     """Screener Overview
 
     Parameters
     ----------
     preset_loaded : str
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/finviz_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 }
 
 
 @log_start_end(log=logger)
 def screener(
     loaded_preset: str = "top_gainers",
     data_type: str = "overview",
-    limit: int = 10,
+    limit: int = -1,
     ascend: bool = False,
     sortby: str = "",
     export: str = "",
     sheet_name: Optional[str] = None,
 ) -> List[str]:
     """Screener one of the following: overview, valuation, financial, ownership, performance, technical.
 
@@ -155,15 +155,15 @@
     List[str]
         List of stocks that meet preset criteria
     """
     with suppress_stdout():
         df_screen = get_screener_data(
             preset_loaded=loaded_preset,
             data_type=data_type,
-            limit=10,
+            limit=limit,
             ascend=ascend,
         )
 
     if isinstance(df_screen, pd.DataFrame):
         if df_screen.empty:
             return []
 
@@ -248,13 +248,15 @@
             export,
             os.path.dirname(os.path.abspath(__file__)),
             data_type,
             df_screen,
             sheet_name,
         )
 
-        return list(df_screen.head(n=limit)["Ticker"].values)
+        return list(df_screen["Ticker"].values)
 
     console.print(
-        "The preset selected did not return a sufficient number of tickers. Two or more tickers are needed."
+        "Error: The preset selected did not return results."
+        "This might be a temporary error that is resolved by running the command again."
+        "If no results continue to be returned, check the preset and expand the parameters."
     )
     return []
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/screener_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/screener_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 """ Screener Controller Module """
 __docformat__ = "numpy"
 
 import argparse
-import datetime
 import logging
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 from openbb_terminal.core.config.paths import (
     MISCELLANEOUS_DIRECTORY,
 )
 from openbb_terminal.core.session.current_user import get_current_user
 from openbb_terminal.custom_prompt_toolkit import NestedCompleter
 from openbb_terminal.decorators import log_start_end
 from openbb_terminal.helper_funcs import (
-    EXPORT_BOTH_RAW_DATA_AND_FIGURES,
     EXPORT_ONLY_RAW_DATA_ALLOWED,
-    check_positive,
     parse_and_split_input,
-    valid_date,
 )
 from openbb_terminal.menu import session
 from openbb_terminal.parent_classes import BaseController
 from openbb_terminal.rich_config import MenuText, console
 from openbb_terminal.stocks.comparison_analysis import ca_controller
 from openbb_terminal.stocks.screener import (
-    ark_view,
     finviz_model,
     finviz_view,
     screener_helper,
     screener_view,
-    yahoofinance_view,
 )
 
 logger = logging.getLogger(__name__)
 
 # pylint: disable=E1121
 
 
@@ -42,22 +36,20 @@
     """Screener Controller class"""
 
     CHOICES_MENUS = ["ca"]
 
     CHOICES_COMMANDS = [
         "view",
         "set",
-        "historical",
         "overview",
         "valuation",
         "financial",
         "ownership",
         "performance",
         "technical",
-        "arktrades",
     ]
     PRESETS_PATH = (
         get_current_user().preferences.USER_PRESETS_DIRECTORY / "stocks" / "screener"
     )
     PRESETS_PATH_DEFAULT = MISCELLANEOUS_DIRECTORY / "stocks" / "screener"
 
     preset_choices: Dict[str, Union[str, Path]] = {}
@@ -86,15 +78,15 @@
     PATH = "/stocks/scr/"
     CHOICES_GENERATION = True
 
     def __init__(self, queue: Optional[List[str]] = None):
         """Constructor"""
         super().__init__(queue)
 
-        self.preset = "top_gainers.ini"
+        self.preset = "top_gainers"
         self.screen_tickers: List = list()
 
         if session and get_current_user().preferences.USE_PROMPT_TOOLKIT:
             choices: dict = self.choices_default
             self.completer = NestedCompleter.from_nested_dict(choices)
 
     def parse_input(self, an_input: str) -> List:
@@ -120,22 +112,20 @@
         """Print help"""
         mt = MenuText("stocks/scr/")
         mt.add_cmd("view")
         mt.add_cmd("set")
         mt.add_raw("\n")
         mt.add_param("_preset", self.preset)
         mt.add_raw("\n")
-        mt.add_cmd("historical")
         mt.add_cmd("overview")
         mt.add_cmd("valuation")
         mt.add_cmd("financial")
         mt.add_cmd("ownership")
         mt.add_cmd("performance")
         mt.add_cmd("technical")
-        mt.add_cmd("arktrades")
         mt.add_raw("\n")
         mt.add_param("_screened_tickers", ", ".join(self.screen_tickers))
         mt.add_raw("\n")
         mt.add_menu("ca", self.screen_tickers)
         console.print(text=mt.menu_text, menu="Stocks - Screener")
 
     @log_start_end(log=logger)
@@ -157,19 +147,19 @@
             choices=self.preset_choices,
             metavar="Desired preset.",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-p")
         ns_parser = self.parse_known_args_and_warn(parser, other_args)
         if ns_parser:
-            if ns_parser.preset:
-                if ns_parser.preset in finviz_model.d_signals:
-                    console.print("This is a Finviz preset.\n")
-                    return
-                ns_parser.preset += ".ini"
+            if ns_parser.preset and ns_parser.preset in finviz_model.d_signals:
+                console.print(
+                    "This preset contains no parameters other than the signal.\n"
+                )
+                return
             screener_view.display_presets(ns_parser.preset)
 
     @log_start_end(log=logger)
     def call_set(self, other_args: List[str]):
         """Process set command"""
         parser = argparse.ArgumentParser(
             add_help=False,
@@ -187,80 +177,15 @@
             choices=self.preset_choices,
             metavar="Desired preset.",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-p")
         ns_parser = self.parse_known_args_and_warn(parser, other_args)
         if ns_parser:
-            self.preset = ns_parser.preset + ".ini"
-
-    @log_start_end(log=logger)
-    def call_historical(self, other_args: List[str]):
-        """Process historical command"""
-        parser = argparse.ArgumentParser(
-            add_help=False,
-            prog="historical",
-            description="""Historical price comparison between similar companies [Source: Yahoo Finance]
-            """,
-        )
-        parser.add_argument(
-            "-l",
-            "--limit",
-            action="store",
-            dest="limit",
-            type=check_positive,
-            default=10,
-            help="Limit of the most shorted stocks to retrieve.",
-        )
-        parser.add_argument(
-            "-n",
-            "--no-scale",
-            action="store_false",
-            dest="no_scale",
-            default=False,
-            help="Flag to not put all prices on same 0-1 scale",
-        )
-        parser.add_argument(
-            "-s",
-            "--start",
-            type=valid_date,
-            default=(
-                datetime.datetime.now() - datetime.timedelta(days=6 * 30)
-            ).strftime("%Y-%m-%d"),
-            dest="start",
-            help="The starting date (format YYYY-MM-DD) of the historical price to plot",
-        )
-        parser.add_argument(
-            "-t",
-            "--type",
-            action="store",
-            dest="type_candle",
-            choices=self.historical_candle_choices,
-            default="a",  # in case it's adjusted close
-            help="type of candles: o-open, h-high, l-low, c-close, a-adjusted close.",
-        )
-        if other_args and "-" not in other_args[0][0]:
-            other_args.insert(0, "-l")
-        ns_parser = self.parse_known_args_and_warn(
-            parser, other_args, EXPORT_BOTH_RAW_DATA_AND_FIGURES
-        )
-        if ns_parser:
-            preset = (
-                self.preset.strip(".ini")
-                if self.preset.strip(".ini") in finviz_model.d_signals
-                else self.preset
-            )
-            self.screen_tickers = yahoofinance_view.historical(
-                preset,
-                ns_parser.limit,
-                ns_parser.start,
-                ns_parser.type_candle,
-                not ns_parser.no_scale,
-                ns_parser.export,
-            )
+            self.preset = ns_parser.preset
 
     @log_start_end(log=logger)
     def call_overview(self, other_args: List[str]):
         """Process overview command"""
         parser = argparse.ArgumentParser(
             add_help=False,
             prog="overview",
@@ -280,16 +205,16 @@
             metavar="Desired preset.",
         )
         parser.add_argument(
             "-l",
             "--limit",
             action="store",
             dest="limit",
-            type=check_positive,
-            default=10,
+            type=int,
+            default=0,
             help="Limit of stocks to print",
         )
         parser.add_argument(
             "-r",
             "--reverse",
             action="store_true",
             dest="reverse",
@@ -303,15 +228,15 @@
         parser.add_argument(
             "-s",
             "--sort",
             choices=screener_helper.finviz_choices("overview"),
             type=str.lower,
             dest="sort",
             metavar="SORT",
-            default="Ticker",
+            default="marketcap",
             help="Sort elements of the table.",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-l")
         ns_parser = self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED
         )
@@ -358,16 +283,16 @@
             metavar="Desired preset.",
         )
         parser.add_argument(
             "-l",
             "--limit",
             action="store",
             dest="limit",
-            type=check_positive,
-            default=10,
+            type=int,
+            default=0,
             help="Limit of stocks to print",
         )
         parser.add_argument(
             "-r",
             "--reverse",
             action="store_true",
             dest="reverse",
@@ -378,15 +303,15 @@
                 "Only works when raw data is displayed."
             ),
         )
         parser.add_argument(
             "-s",
             "--sort",
             dest="sort",
-            default="Ticker",
+            default="marketcap",
             choices=screener_helper.finviz_choices("valuation"),
             type=str.lower,
             metavar="SORT",
             help="Sort elements of the table.",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-l")
@@ -435,16 +360,16 @@
             metavar="Desired preset.",
         )
         parser.add_argument(
             "-l",
             "--limit",
             action="store",
             dest="limit",
-            type=check_positive,
-            default=10,
+            type=int,
+            default=0,
             help="Limit of stocks to print",
         )
         parser.add_argument(
             "-r",
             "--reverse",
             action="store_true",
             dest="reverse",
@@ -458,15 +383,15 @@
         parser.add_argument(
             "-s",
             "--sort",
             choices=screener_helper.finviz_choices("financial"),
             type=str.lower,
             dest="sort",
             metavar="SORT",
-            default="Ticker",
+            default="marketcap",
             help="Sort elements of the table.",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-l")
         ns_parser = self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED
         )
@@ -512,16 +437,16 @@
             metavar="Desired preset.",
         )
         parser.add_argument(
             "-l",
             "--limit",
             action="store",
             dest="limit",
-            type=check_positive,
-            default=10,
+            type=int,
+            default=0,
             help="Limit of stocks to print",
         )
         parser.add_argument(
             "-r",
             "--reverse",
             action="store_true",
             dest="reverse",
@@ -533,15 +458,15 @@
             ),
         )
         parser.add_argument(
             "-s",
             "--sort",
             dest="sort",
             metavar="SORT",
-            default="Ticker",
+            default="marketcap",
             choices=screener_helper.finviz_choices("ownership"),
             type=str.lower,
             help="Sort elements of the table.",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-l")
         ns_parser = self.parse_known_args_and_warn(
@@ -589,16 +514,16 @@
             metavar="Desired preset.",
         )
         parser.add_argument(
             "-l",
             "--limit",
             action="store",
             dest="limit",
-            type=check_positive,
-            default=10,
+            type=int,
+            default=0,
             help="Limit of stocks to print",
         )
         parser.add_argument(
             "-r",
             "--reverse",
             action="store_true",
             dest="reverse",
@@ -611,15 +536,15 @@
         )
         parser.add_argument(
             "-s",
             "--sort",
             choices=screener_helper.finviz_choices("performance"),
             type=str.lower,
             dest="sort",
-            default="Ticker",
+            default="perfytd",
             metavar="SORTBY",
             help="Sort elements of the table.",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-l")
         ns_parser = self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED
@@ -666,16 +591,16 @@
             metavar="Desired preset.",
         )
         parser.add_argument(
             "-l",
             "--limit",
             action="store",
             dest="limit",
-            type=check_positive,
-            default=10,
+            type=int,
+            default=0,
             help="Limit of stocks to print",
         )
         parser.add_argument(
             "-r",
             "--reverse",
             action="store_true",
             dest="reverse",
@@ -688,15 +613,15 @@
         )
         parser.add_argument(
             "-s",
             "--sort",
             choices=screener_helper.finviz_choices("technical"),
             type=str.lower,
             dest="sort",
-            default="Ticker",
+            default="rsi",
             help="Sort elements of the table.",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-l")
         ns_parser = self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED
         )
@@ -730,56 +655,7 @@
                 self.queue,
             )
         else:
             console.print(
                 "Please select a screener using 'set' and then run 'historical' "
                 "before going to the CA menu.\n"
             )
-
-    @log_start_end(log=logger)
-    def call_arktrades(self, other_args):
-        """Process arktrades command"""
-        parser = argparse.ArgumentParser(
-            add_help=False,
-            prog="arktrades",
-            description="""
-                Get trades for ticker across all ARK funds.
-            """,
-        )
-        parser.add_argument(
-            "-t",
-            "--ticker",
-            help="The ticker to use for searching.",
-            dest="ticker",
-            required=True,
-        )
-        parser.add_argument(
-            "-l",
-            "--limit",
-            help="Limit of rows to show",
-            dest="limit",
-            default=10,
-            type=check_positive,
-        )
-        parser.add_argument(
-            "-s",
-            "--show_symbol",
-            action="store_true",
-            default=False,
-            help="Flag to show ticker in table",
-            dest="show_symbol",
-        )
-        if other_args and "-" not in other_args[0][0]:
-            other_args.insert(0, "-t")
-        ns_parser = self.parse_known_args_and_warn(
-            parser, other_args, export_allowed=EXPORT_ONLY_RAW_DATA_ALLOWED
-        )
-        if ns_parser:
-            ark_view.display_ark_trades(
-                symbol=ns_parser.ticker,
-                limit=ns_parser.limit,
-                show_symbol=ns_parser.show_symbol,
-                export=ns_parser.export,
-                sheet_name=" ".join(ns_parser.sheet_name)
-                if ns_parser.sheet_name
-                else None,
-            )
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/screener_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/screener_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/screener/screener_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/screener/screener_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/stock_statics.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/stock_statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/stocks_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/stocks_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,24 +543,32 @@
             "--sources",
             dest="sources",
             type=str,
             default="",
             help="Show news only from the sources specified (e.g bloomberg,reuters)",
         )
         if other_args and "-" not in other_args[0][0]:
-            other_args.insert(0, "-l")
+            other_args.insert(0, "-t")
         ns_parser = self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED, limit=10
         )
         if ns_parser:
             if ns_parser.ticker:
                 self.ticker = ns_parser.ticker
                 self.custom_load_wrapper([self.ticker])
             if self.ticker:
-                if ns_parser.source == "UltimaInsights":
+                if ns_parser.source == "NewsApi":
+                    newsapi_view.display_news(
+                        query=self.ticker,
+                        limit=ns_parser.limit,
+                        start_date=ns_parser.n_start_date.strftime("%Y-%m-%d"),
+                        show_newest=ns_parser.n_oldest,
+                        sources=ns_parser.sources,
+                    )
+                elif str(ns_parser.source).lower() == "ultima":
                     query = str(self.ticker).upper()
                     if query not in ultima_newsmonitor_view.supported_terms():
                         console.print(
                             "[red]Ticker not supported by Ultima Insights News Monitor[/red]"
                         )
                         feedparser_view.display_news(
                             term=query,
@@ -573,22 +581,14 @@
                         ultima_newsmonitor_view.display_news(
                             term=query,
                             sources=ns_parser.sources,
                             limit=ns_parser.limit,
                             export=ns_parser.export,
                             sheet_name=ns_parser.sheet_name,
                         )
-                elif ns_parser.source == "NewsApi":
-                    newsapi_view.display_news(
-                        query=self.ticker,
-                        limit=ns_parser.limit,
-                        start_date=ns_parser.n_start_date.strftime("%Y-%m-%d"),
-                        show_newest=ns_parser.n_oldest,
-                        sources=ns_parser.sources,
-                    )
                 elif ns_parser.source == "Feedparser":
                     feedparser_view.display_news(
                         term=self.ticker,
                         sources=ns_parser.sources,
                         limit=ns_parser.limit,
                         export=ns_parser.export,
                         sheet_name=" ".join(ns_parser.sheet_name)
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/stocks_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/stocks_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Main helper."""
 __docformat__ = "numpy"
-
-# pylint: disable=unsupported-assignment-operation,C0302
-# pylint: disable=no-member,too-many-branches,too-many-arguments
+# pylint: disable=too-many-lines, unsupported-assignment-operation
+# pylint: disable=no-member, too-many-branches, too-many-arguments
 # pylint: disable=inconsistent-return-statements
 # pylint: disable=consider-using-dict-items
 
 import logging
 import os
 from copy import deepcopy
 from datetime import datetime, timedelta
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/stocks_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/stocks_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/finbrain_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/finbrain_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/rsp_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/rsp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/rsp_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/tradingview_view.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,68 @@
-""" Relative Strength Percentile View """
+"""Tradingview view"""
 __docformat__ = "numpy"
 
 import logging
 import os
 from typing import Optional
 
 import pandas as pd
 
 from openbb_terminal.decorators import log_start_end
 from openbb_terminal.helper_funcs import export_data, print_rich_table
 from openbb_terminal.rich_config import console
-from openbb_terminal.stocks.technical_analysis import rsp_model
+from openbb_terminal.stocks.technical_analysis import tradingview_model
 
 logger = logging.getLogger(__name__)
 
 
 @log_start_end(log=logger)
-def display_rsp(
-    s_ticker: str = "",
+def print_recommendation(
+    symbol: str,
+    screener: str = "america",
+    exchange: str = "",
+    interval: str = "",
     export: str = "",
     sheet_name: Optional[str] = None,
-    tickers_show: bool = False,
 ):
-    """Display Relative Strength Percentile [Source: https://github.com/skyte/relative-strength]
+    """Print tradingview recommendation based on technical indicators
 
     Parameters
     ----------
-    s_ticker : str
-        Stock ticker
-    export : str
+    symbol : str
+        Ticker symbol to get tradingview recommendation based on technical indicators
+    screener : str
+        Screener based on tradingview docs https://python-tradingview-ta.readthedocs.io/en/latest/usage.html
+    exchange: str
+        Exchange based on tradingview docs https://python-tradingview-ta.readthedocs.io/en/latest/usage.html
+    interval: str
+        Interval time to check technical indicators and correspondent recommendation
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    export: str
         Format of export file
-    tickers_show : bool
-        Boolean to check if tickers in the same industry as the stock should be shown
     """
 
-    rsp_stock, rsp_industry, df_stock_p, df_industries_p = rsp_model.get_rsp(s_ticker)
-    if rsp_stock.empty or rsp_industry.empty:
-        console.print(f"[red]Ticker '{s_ticker}' not found.\n[/red]")
-    else:
-        tickers = pd.DataFrame(rsp_industry["Tickers"])
-        del rsp_industry["Tickers"]
-        print_rich_table(
-            rsp_stock,
-            headers=list(rsp_stock.columns),
-            show_index=False,
-            title="Relative Strength Percentile of Stock (relative to SPY)",
-            export=bool(export),
-        )
-        print_rich_table(
-            rsp_industry,
-            headers=list(rsp_industry.columns),
-            show_index=False,
-            title="Relative Strength Percentile of Industry the ticker is part of",
-            export=bool(export),
-        )
-        if tickers_show:
-            print_rich_table(
-                tickers,
-                headers=list(tickers.columns),
-                show_index=False,
-                title="Tickers in same industry as chosen stock",
-            )
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)).replace("common", "stocks"),
-            "rsp_stock",
-            df_stock_p,
-            sheet_name,
-        )
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)).replace("common", "stocks"),
-            "rsp_industry",
-            df_industries_p,
-            sheet_name,
-        )
+    recom = tradingview_model.get_tradingview_recommendation(
+        symbol, screener, exchange, interval
+    )
+
+    if (isinstance(recom, pd.DataFrame) and recom.empty) or (
+        not isinstance(recom, pd.DataFrame) and not recom
+    ):
+        console.print("[red]The API did not return any recommendations.[/red]\n")
+        return
+
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        "recom",
+        recom,
+        sheet_name,
+    )
+    print_rich_table(
+        recom,
+        headers=list(recom.columns),
+        title="Ticker Recommendation",
+        show_index=True,
+        export=bool(export),
+    )
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/technical_analysis/tradingview_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/technical_analysis/tradingview_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/bursa_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/bursa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/bursa_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/bursa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/tradinghours_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/tradinghours_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/stocks/tradinghours/tradinghours_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/stocks/tradinghours/tradinghours_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/terminal_controller.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/terminal_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from rich import panel
 
 import openbb_terminal.config_terminal as cfg
 from openbb_terminal.account.account_model import (
     get_login_called,
     set_login_called,
 )
-from openbb_terminal.common import feedparser_view, ultima_newsmonitor_view
+from openbb_terminal.common import feedparser_view
 from openbb_terminal.core.config.paths import (
     HOME_DIRECTORY,
     MISCELLANEOUS_DIRECTORY,
     REPOSITORY_DIRECTORY,
     SETTINGS_ENV_FILE,
 )
 from openbb_terminal.core.log.generation.custom_logger import log_terminal
@@ -240,34 +240,22 @@
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-t")
         news_parser = self.parse_known_args_and_warn(
             parse, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED, limit=5
         )
         if news_parser:
-            query = " ".join(news_parser.term).upper()
-            if query not in ultima_newsmonitor_view.supported_terms():
-                console.print(
-                    "[red]Ticker not supported by Ultima Insights News Monitor[/red]"
-                )
-                feedparser_view.display_news(
-                    term=query,
-                    sources=news_parser.sources,
-                    limit=news_parser.limit,
-                    export=news_parser.export,
-                    sheet_name=news_parser.sheet_name,
-                )
-            else:
-                ultima_newsmonitor_view.display_news(
-                    term=query,
-                    sources=news_parser.sources,
-                    limit=news_parser.limit,
-                    export=news_parser.export,
-                    sheet_name=news_parser.sheet_name,
-                )
+            query = " ".join(news_parser.term)
+            feedparser_view.display_news(
+                term=query,
+                sources=news_parser.sources,
+                limit=news_parser.limit,
+                export=news_parser.export,
+                sheet_name=news_parser.sheet_name,
+            )
 
     def call_guess(self, other_args: List[str]) -> None:
         """Process guess command."""
         import json
         import random
 
         current_user = get_current_user()
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/terminal_helper.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/terminal_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/openbb_terminal/thought_of_the_day.py` & `openbb_nightly-3.0.0rc1.dev20230409/openbb_terminal/thought_of_the_day.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/pyproject.toml` & `openbb_nightly-3.0.0rc1.dev20230409/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbb-nightly"
-version = "3.0.0rc1.dev20230408"
+version = "3.0.0rc1.dev20230409"
 description = "Investment Research for Everyone, Anywhere."
 license = "MIT"
 authors = ["Didier Rodrigues Lopes"]
 packages = [
     { include = "openbb_terminal" },
 ]
 include = ["terminal.py"]
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/terminal.py` & `openbb_nightly-3.0.0rc1.dev20230409/terminal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/website/pypi.md` & `openbb_nightly-3.0.0rc1.dev20230409/website/pypi.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 The command below provides access to the core functionalities behind the [OpenBB Terminal](https://openbb.co/products/terminal).
 
 ```python
 pip install openbb-nightly
 ```
 
-If you wish to utilize our **Portfolio Optimization** or **Machine Learning / Artificial Intelligence** toolkits, please see instructions [here](https://docs.openbb.co/sdk/quickstart/installation).
+If you wish to utilize our **Portfolio Optimization** or **Machine Learning / Artificial Intelligence** toolkits, please see instructions [here](https://docs.openbb.co/sdk/installation).
 
 ## Usage
 
 Access our fully fledged financial SDK with a single line of python code.
 
 ```python
 from openbb_terminal.sdk import openbb-nightly
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230408/PKG-INFO` & `openbb_nightly-3.0.0rc1.dev20230409/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 3.0.0rc1.dev20230408
+Version: 3.0.0rc1.dev20230409
 Summary: Investment Research for Everyone, Anywhere.
 Home-page: https://openbb.co
 License: MIT
 Author: Didier Rodrigues Lopes
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.11.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -140,15 +140,15 @@
 
 The command below provides access to the core functionalities behind the [OpenBB Terminal](https://openbb.co/products/terminal).
 
 ```python
 pip install openbb-nightly
 ```
 
-If you wish to utilize our **Portfolio Optimization** or **Machine Learning / Artificial Intelligence** toolkits, please see instructions [here](https://docs.openbb.co/sdk/quickstart/installation).
+If you wish to utilize our **Portfolio Optimization** or **Machine Learning / Artificial Intelligence** toolkits, please see instructions [here](https://docs.openbb.co/sdk/installation).
 
 ## Usage
 
 Access our fully fledged financial SDK with a single line of python code.
 
 ```python
 from openbb_terminal.sdk import openbb-nightly
```


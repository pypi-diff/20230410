# Comparing `tmp/autots-0.5.5.tar.gz` & `tmp/autots-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autots-0.5.5.tar", last modified: Mon Apr  3 03:05:58 2023, max compression
+gzip compressed data, was "autots-0.5.6.tar", last modified: Mon Apr 10 03:32:24 2023, max compression
```

## Comparing `autots-0.5.5.tar` & `autots-0.5.6.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.417259 autots-0.5.5/
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.225307 autots-0.5.5/AutoTS.egg-info/
--rw-rw-rw-   0        0        0     8893 2023-04-03 03:05:58.000000 autots-0.5.5/AutoTS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2148 2023-04-03 03:05:58.000000 autots-0.5.5/AutoTS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 03:05:58.000000 autots-0.5.5/AutoTS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-04-03 03:05:58.000000 autots-0.5.5/AutoTS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-04-03 03:05:58.000000 autots-0.5.5/AutoTS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2022-11-23 22:39:41.000000 autots-0.5.5/LICENSE
--rw-rw-rw-   0        0        0       97 2022-11-23 22:39:41.000000 autots-0.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     8893 2023-04-03 03:05:58.416247 autots-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     8248 2023-04-02 18:42:06.000000 autots-0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.227308 autots-0.5.5/autots/
--rw-rw-rw-   0        0        0     1384 2023-04-03 02:52:53.000000 autots-0.5.5/autots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.233336 autots-0.5.5/autots/datasets/
--rw-rw-rw-   0        0        0      535 2022-11-23 22:39:41.000000 autots-0.5.5/autots/datasets/__init__.py
--rw-rw-rw-   0        0        0    32839 2023-03-30 15:35:07.000000 autots-0.5.5/autots/datasets/_base.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.277769 autots-0.5.5/autots/datasets/data/
--rw-rw-rw-   0        0        0     4527 2022-11-23 22:39:41.000000 autots-0.5.5/autots/datasets/data/covid_daily.zip
--rw-rw-rw-   0        0        0    81380 2022-11-23 22:39:41.000000 autots-0.5.5/autots/datasets/data/eia_weekly.zip
--rw-rw-rw-   0        0        0    27440 2022-11-23 22:39:41.000000 autots-0.5.5/autots/datasets/data/fred_monthly.zip
--rw-rw-rw-   0        0        0     5553 2022-11-23 22:39:41.000000 autots-0.5.5/autots/datasets/data/fred_yearly.zip
--rw-rw-rw-   0        0        0   107751 2022-11-23 22:39:41.000000 autots-0.5.5/autots/datasets/data/holidays.zip
--rw-rw-rw-   0        0        0   158529 2022-11-23 22:39:41.000000 autots-0.5.5/autots/datasets/data/traffic_hourly.zip
--rw-rw-rw-   0        0        0     3376 2022-11-23 22:39:41.000000 autots-0.5.5/autots/datasets/fred.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.291172 autots-0.5.5/autots/evaluator/
--rw-rw-rw-   0        0        0       28 2022-11-23 22:39:41.000000 autots-0.5.5/autots/evaluator/__init__.py
--rw-rw-rw-   0        0        0    16440 2022-12-23 18:19:28.000000 autots-0.5.5/autots/evaluator/anomaly_detector.py
--rw-rw-rw-   0        0        0   108127 2023-04-03 02:46:28.000000 autots-0.5.5/autots/evaluator/auto_model.py
--rw-rw-rw-   0        0        0   135311 2023-04-03 02:46:29.000000 autots-0.5.5/autots/evaluator/auto_ts.py
--rw-rw-rw-   0        0        0    24446 2022-11-23 22:39:41.000000 autots-0.5.5/autots/evaluator/benchmark.py
--rw-rw-rw-   0        0        0    32646 2023-02-01 17:49:09.000000 autots-0.5.5/autots/evaluator/event_forecasting.py
--rw-rw-rw-   0        0        0    21929 2023-04-03 02:46:27.000000 autots-0.5.5/autots/evaluator/metrics.py
--rw-rw-rw-   0        0        0     6490 2023-02-01 17:49:09.000000 autots-0.5.5/autots/evaluator/validation.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.315989 autots-0.5.5/autots/models/
--rw-rw-rw-   0        0        0       24 2022-11-23 22:39:41.000000 autots-0.5.5/autots/models/__init__.py
--rw-rw-rw-   0        0        0    14112 2023-01-16 02:41:20.000000 autots-0.5.5/autots/models/arch.py
--rw-rw-rw-   0        0        0    23064 2023-04-03 02:46:27.000000 autots-0.5.5/autots/models/base.py
--rw-rw-rw-   0        0        0   112095 2023-04-03 02:46:29.000000 autots-0.5.5/autots/models/basics.py
--rw-rw-rw-   0        0        0   114816 2023-04-03 02:46:29.000000 autots-0.5.5/autots/models/cassandra.py
--rw-rw-rw-   0        0        0    16461 2022-11-23 22:39:41.000000 autots-0.5.5/autots/models/dnn.py
--rw-rw-rw-   0        0        0    61890 2023-04-03 02:46:28.000000 autots-0.5.5/autots/models/ensemble.py
--rw-rw-rw-   0        0        0    26048 2023-01-31 05:02:16.000000 autots-0.5.5/autots/models/gluonts.py
--rw-rw-rw-   0        0        0    10744 2022-11-23 22:39:41.000000 autots-0.5.5/autots/models/greykite.py
--rw-rw-rw-   0        0        0    33909 2022-11-23 22:39:41.000000 autots-0.5.5/autots/models/matrix_var.py
--rw-rw-rw-   0        0        0    18731 2023-04-03 02:46:27.000000 autots-0.5.5/autots/models/mlensemble.py
--rw-rw-rw-   0        0        0     8136 2023-03-31 21:04:36.000000 autots-0.5.5/autots/models/model_list.py
--rw-rw-rw-   0        0        0    33743 2022-11-23 22:39:41.000000 autots-0.5.5/autots/models/prophet.py
--rw-rw-rw-   0        0        0    19975 2022-11-23 22:39:41.000000 autots-0.5.5/autots/models/pytorch.py
--rw-rw-rw-   0        0        0   119209 2023-04-03 02:46:29.000000 autots-0.5.5/autots/models/sklearn.py
--rw-rw-rw-   0        0        0    93302 2023-02-01 17:49:10.000000 autots-0.5.5/autots/models/statsmodels.py
--rw-rw-rw-   0        0        0    21794 2022-11-23 22:39:41.000000 autots-0.5.5/autots/models/tfp.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.318014 autots-0.5.5/autots/templates/
--rw-rw-rw-   0        0        0       27 2022-11-23 22:39:41.000000 autots-0.5.5/autots/templates/__init__.py
--rw-rw-rw-   0        0        0    42365 2023-01-21 02:30:16.000000 autots-0.5.5/autots/templates/general.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.344580 autots-0.5.5/autots/tools/
--rw-rw-rw-   0        0        0       96 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/__init__.py
--rw-rw-rw-   0        0        0    42726 2022-12-23 01:25:04.000000 autots-0.5.5/autots/tools/anomaly_utils.py
--rw-rw-rw-   0        0        0     9328 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/calendar.py
--rw-rw-rw-   0        0        0     7163 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/cointegration.py
--rw-rw-rw-   0        0        0     1709 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/cpu_count.py
--rw-rw-rw-   0        0        0    40373 2023-03-11 22:20:32.000000 autots-0.5.5/autots/tools/fast_kalman.py
--rw-rw-rw-   0        0        0     5872 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/hierarchial.py
--rw-rw-rw-   0        0        0     4478 2022-12-13 20:06:14.000000 autots-0.5.5/autots/tools/holiday.py
--rw-rw-rw-   0        0        0     9153 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/impute.py
--rw-rw-rw-   0        0        0     5188 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/lunar.py
--rw-rw-rw-   0        0        0     4362 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/percentile.py
--rw-rw-rw-   0        0        0     7786 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/probabilistic.py
--rw-rw-rw-   0        0        0     1001 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/profile.py
--rw-rw-rw-   0        0        0    15116 2023-01-19 01:24:58.000000 autots-0.5.5/autots/tools/regressor.py
--rw-rw-rw-   0        0        0    16039 2023-03-15 15:21:07.000000 autots-0.5.5/autots/tools/seasonal.py
--rw-rw-rw-   0        0        0    18089 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/shaping.py
--rw-rw-rw-   0        0        0    19174 2022-11-23 22:39:41.000000 autots-0.5.5/autots/tools/thresholding.py
--rw-rw-rw-   0        0        0   149836 2023-04-03 02:46:30.000000 autots-0.5.5/autots/tools/transform.py
--rw-rw-rw-   0        0        0    18322 2023-04-03 02:46:27.000000 autots-0.5.5/autots/tools/window_functions.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.346171 autots-0.5.5/docs/
--rw-rw-rw-   0        0        0     2750 2023-04-03 02:52:50.000000 autots-0.5.5/docs/conf.py
--rw-rw-rw-   0        0        0     1176 2023-04-03 03:05:53.000000 autots-0.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-03 03:05:58.418262 autots-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1273 2023-04-03 02:53:53.000000 autots-0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:05:58.414994 autots-0.5.5/tests/
--rw-rw-rw-   0        0        0     4677 2022-11-23 22:39:41.000000 autots-0.5.5/tests/test_anomalies.py
--rw-rw-rw-   0        0        0    29300 2023-01-31 21:46:21.000000 autots-0.5.5/tests/test_autots.py
--rw-rw-rw-   0        0        0     4259 2022-11-23 22:39:41.000000 autots-0.5.5/tests/test_calendar_holiday.py
--rw-rw-rw-   0        0        0    10554 2023-04-02 03:12:25.000000 autots-0.5.5/tests/test_cassandra.py
--rw-rw-rw-   0        0        0     3654 2022-11-23 22:39:41.000000 autots-0.5.5/tests/test_event_forecasting.py
--rw-rw-rw-   0        0        0     1512 2022-11-23 22:39:41.000000 autots-0.5.5/tests/test_impute.py
--rw-rw-rw-   0        0        0     5112 2023-03-31 21:50:22.000000 autots-0.5.5/tests/test_metrics.py
--rw-rw-rw-   0        0        0     1514 2022-11-23 22:39:41.000000 autots-0.5.5/tests/test_percentile.py
--rw-rw-rw-   0        0        0     1836 2022-11-23 22:39:41.000000 autots-0.5.5/tests/test_regressor.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.619454 autots-0.5.6/
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.480050 autots-0.5.6/AutoTS.egg-info/
+-rw-rw-rw-   0        0        0     8893 2023-04-10 03:32:24.000000 autots-0.5.6/AutoTS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2148 2023-04-10 03:32:24.000000 autots-0.5.6/AutoTS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 03:32:24.000000 autots-0.5.6/AutoTS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      224 2023-04-10 03:32:24.000000 autots-0.5.6/AutoTS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-04-10 03:32:24.000000 autots-0.5.6/AutoTS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2022-11-23 22:39:41.000000 autots-0.5.6/LICENSE
+-rw-rw-rw-   0        0        0       61 2023-04-03 03:08:26.000000 autots-0.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     8893 2023-04-10 03:32:24.619454 autots-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8248 2023-04-02 18:42:06.000000 autots-0.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.480050 autots-0.5.6/autots/
+-rw-rw-rw-   0        0        0     1384 2023-04-03 14:59:13.000000 autots-0.5.6/autots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.480050 autots-0.5.6/autots/datasets/
+-rw-rw-rw-   0        0        0      535 2022-11-23 22:39:41.000000 autots-0.5.6/autots/datasets/__init__.py
+-rw-rw-rw-   0        0        0    32463 2023-04-08 14:56:53.000000 autots-0.5.6/autots/datasets/_base.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.521292 autots-0.5.6/autots/datasets/data/
+-rw-rw-rw-   0        0        0     4527 2022-11-23 22:39:41.000000 autots-0.5.6/autots/datasets/data/covid_daily.zip
+-rw-rw-rw-   0        0        0    81380 2022-11-23 22:39:41.000000 autots-0.5.6/autots/datasets/data/eia_weekly.zip
+-rw-rw-rw-   0        0        0    27440 2022-11-23 22:39:41.000000 autots-0.5.6/autots/datasets/data/fred_monthly.zip
+-rw-rw-rw-   0        0        0     5553 2022-11-23 22:39:41.000000 autots-0.5.6/autots/datasets/data/fred_yearly.zip
+-rw-rw-rw-   0        0        0   107751 2022-11-23 22:39:41.000000 autots-0.5.6/autots/datasets/data/holidays.zip
+-rw-rw-rw-   0        0        0   158529 2022-11-23 22:39:41.000000 autots-0.5.6/autots/datasets/data/traffic_hourly.zip
+-rw-rw-rw-   0        0        0     3377 2023-04-10 03:29:38.000000 autots-0.5.6/autots/datasets/fred.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.537294 autots-0.5.6/autots/evaluator/
+-rw-rw-rw-   0        0        0       28 2022-11-23 22:39:41.000000 autots-0.5.6/autots/evaluator/__init__.py
+-rw-rw-rw-   0        0        0    16533 2023-04-10 03:29:38.000000 autots-0.5.6/autots/evaluator/anomaly_detector.py
+-rw-rw-rw-   0        0        0   108611 2023-04-10 03:29:40.000000 autots-0.5.6/autots/evaluator/auto_model.py
+-rw-rw-rw-   0        0        0   139190 2023-04-10 03:29:40.000000 autots-0.5.6/autots/evaluator/auto_ts.py
+-rw-rw-rw-   0        0        0    24446 2022-11-23 22:39:41.000000 autots-0.5.6/autots/evaluator/benchmark.py
+-rw-rw-rw-   0        0        0    32646 2023-02-01 17:49:09.000000 autots-0.5.6/autots/evaluator/event_forecasting.py
+-rw-rw-rw-   0        0        0    21898 2023-04-10 03:29:38.000000 autots-0.5.6/autots/evaluator/metrics.py
+-rw-rw-rw-   0        0        0     6490 2023-02-01 17:49:09.000000 autots-0.5.6/autots/evaluator/validation.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.549472 autots-0.5.6/autots/models/
+-rw-rw-rw-   0        0        0       24 2022-11-23 22:39:41.000000 autots-0.5.6/autots/models/__init__.py
+-rw-rw-rw-   0        0        0    14112 2023-01-16 02:41:20.000000 autots-0.5.6/autots/models/arch.py
+-rw-rw-rw-   0        0        0    22960 2023-04-07 20:55:54.000000 autots-0.5.6/autots/models/base.py
+-rw-rw-rw-   0        0        0   112063 2023-04-10 03:29:40.000000 autots-0.5.6/autots/models/basics.py
+-rw-rw-rw-   0        0        0   114816 2023-04-03 02:46:29.000000 autots-0.5.6/autots/models/cassandra.py
+-rw-rw-rw-   0        0        0    16461 2022-11-23 22:39:41.000000 autots-0.5.6/autots/models/dnn.py
+-rw-rw-rw-   0        0        0    62892 2023-04-10 03:29:39.000000 autots-0.5.6/autots/models/ensemble.py
+-rw-rw-rw-   0        0        0    28446 2023-04-10 03:29:38.000000 autots-0.5.6/autots/models/gluonts.py
+-rw-rw-rw-   0        0        0    10745 2023-04-10 03:29:38.000000 autots-0.5.6/autots/models/greykite.py
+-rw-rw-rw-   0        0        0    33909 2022-11-23 22:39:41.000000 autots-0.5.6/autots/models/matrix_var.py
+-rw-rw-rw-   0        0        0    19900 2023-04-10 03:29:38.000000 autots-0.5.6/autots/models/mlensemble.py
+-rw-rw-rw-   0        0        0     8136 2023-03-31 21:04:36.000000 autots-0.5.6/autots/models/model_list.py
+-rw-rw-rw-   0        0        0    33743 2022-11-23 22:39:41.000000 autots-0.5.6/autots/models/prophet.py
+-rw-rw-rw-   0        0        0    19975 2022-11-23 22:39:41.000000 autots-0.5.6/autots/models/pytorch.py
+-rw-rw-rw-   0        0        0   119304 2023-04-09 12:36:00.000000 autots-0.5.6/autots/models/sklearn.py
+-rw-rw-rw-   0        0        0    93302 2023-02-01 17:49:10.000000 autots-0.5.6/autots/models/statsmodels.py
+-rw-rw-rw-   0        0        0    21794 2022-11-23 22:39:41.000000 autots-0.5.6/autots/models/tfp.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.551032 autots-0.5.6/autots/templates/
+-rw-rw-rw-   0        0        0       27 2022-11-23 22:39:41.000000 autots-0.5.6/autots/templates/__init__.py
+-rw-rw-rw-   0        0        0    42365 2023-01-21 02:30:16.000000 autots-0.5.6/autots/templates/general.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.563306 autots-0.5.6/autots/tools/
+-rw-rw-rw-   0        0        0       96 2022-11-23 22:39:41.000000 autots-0.5.6/autots/tools/__init__.py
+-rw-rw-rw-   0        0        0    42765 2023-04-10 03:29:39.000000 autots-0.5.6/autots/tools/anomaly_utils.py
+-rw-rw-rw-   0        0        0     9168 2023-04-08 14:59:14.000000 autots-0.5.6/autots/tools/calendar.py
+-rw-rw-rw-   0        0        0     7163 2022-11-23 22:39:41.000000 autots-0.5.6/autots/tools/cointegration.py
+-rw-rw-rw-   0        0        0     1709 2022-11-23 22:39:41.000000 autots-0.5.6/autots/tools/cpu_count.py
+-rw-rw-rw-   0        0        0    40373 2023-03-11 22:20:32.000000 autots-0.5.6/autots/tools/fast_kalman.py
+-rw-rw-rw-   0        0        0     5872 2022-11-23 22:39:41.000000 autots-0.5.6/autots/tools/hierarchial.py
+-rw-rw-rw-   0        0        0     4491 2023-04-08 15:58:34.000000 autots-0.5.6/autots/tools/holiday.py
+-rw-rw-rw-   0        0        0     9153 2022-11-23 22:39:41.000000 autots-0.5.6/autots/tools/impute.py
+-rw-rw-rw-   0        0        0     5188 2022-11-23 22:39:41.000000 autots-0.5.6/autots/tools/lunar.py
+-rw-rw-rw-   0        0        0     4362 2022-11-23 22:39:41.000000 autots-0.5.6/autots/tools/percentile.py
+-rw-rw-rw-   0        0        0     7786 2022-11-23 22:39:41.000000 autots-0.5.6/autots/tools/probabilistic.py
+-rw-rw-rw-   0        0        0     1001 2022-11-23 22:39:41.000000 autots-0.5.6/autots/tools/profile.py
+-rw-rw-rw-   0        0        0    15361 2023-04-09 14:46:49.000000 autots-0.5.6/autots/tools/regressor.py
+-rw-rw-rw-   0        0        0    16300 2023-04-10 03:29:39.000000 autots-0.5.6/autots/tools/seasonal.py
+-rw-rw-rw-   0        0        0    18046 2023-04-08 14:58:25.000000 autots-0.5.6/autots/tools/shaping.py
+-rw-rw-rw-   0        0        0    19147 2023-04-08 14:59:28.000000 autots-0.5.6/autots/tools/thresholding.py
+-rw-rw-rw-   0        0        0   149956 2023-04-10 03:29:41.000000 autots-0.5.6/autots/tools/transform.py
+-rw-rw-rw-   0        0        0    18154 2023-04-10 03:29:39.000000 autots-0.5.6/autots/tools/window_functions.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.564208 autots-0.5.6/docs/
+-rw-rw-rw-   0        0        0     2750 2023-04-08 14:52:49.000000 autots-0.5.6/docs/conf.py
+-rw-rw-rw-   0        0        0     1176 2023-04-08 14:52:59.000000 autots-0.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 03:32:24.619454 autots-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1273 2023-04-08 14:52:53.000000 autots-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:32:24.619454 autots-0.5.6/tests/
+-rw-rw-rw-   0        0        0     4677 2022-11-23 22:39:41.000000 autots-0.5.6/tests/test_anomalies.py
+-rw-rw-rw-   0        0        0    29300 2023-04-03 04:16:21.000000 autots-0.5.6/tests/test_autots.py
+-rw-rw-rw-   0        0        0     4259 2022-11-23 22:39:41.000000 autots-0.5.6/tests/test_calendar_holiday.py
+-rw-rw-rw-   0        0        0    10554 2023-04-02 03:12:25.000000 autots-0.5.6/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     3654 2022-11-23 22:39:41.000000 autots-0.5.6/tests/test_event_forecasting.py
+-rw-rw-rw-   0        0        0     1512 2022-11-23 22:39:41.000000 autots-0.5.6/tests/test_impute.py
+-rw-rw-rw-   0        0        0     5112 2023-03-31 21:50:22.000000 autots-0.5.6/tests/test_metrics.py
+-rw-rw-rw-   0        0        0     1514 2022-11-23 22:39:41.000000 autots-0.5.6/tests/test_percentile.py
+-rw-rw-rw-   0        0        0     1836 2022-11-23 22:39:41.000000 autots-0.5.6/tests/test_regressor.py
```

### Comparing `autots-0.5.5/AutoTS.egg-info/PKG-INFO` & `autots-0.5.6/AutoTS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autots
-Version: 0.5.5
+Version: 0.5.6
 Summary: Automated Time Series Forecasting
 Home-page: https://github.com/winedarksea/AutoTS
 Author: Colin Catlin
 Author-email: Colin Catlin <colin.catlin@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/winedarksea/AutoTS
 Project-URL: Bug Tracker, https://github.com/winedarksea/AutoTS/issues
```

### Comparing `autots-0.5.5/AutoTS.egg-info/SOURCES.txt` & `autots-0.5.6/AutoTS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/LICENSE` & `autots-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/PKG-INFO` & `autots-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autots
-Version: 0.5.5
+Version: 0.5.6
 Summary: Automated Time Series Forecasting
 Home-page: https://github.com/winedarksea/AutoTS
 Author: Colin Catlin
 Author-email: Colin Catlin <colin.catlin@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/winedarksea/AutoTS
 Project-URL: Bug Tracker, https://github.com/winedarksea/AutoTS/issues
```

### Comparing `autots-0.5.5/README.md` & `autots-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/__init__.py` & `autots-0.5.6/autots/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from autots.tools.shaping import long_to_wide
 from autots.tools.regressor import create_lagged_regressor, create_regressor
 from autots.evaluator.auto_model import model_forecast
 from autots.evaluator.anomaly_detector import AnomalyDetector, HolidayDetector
 from autots.models.cassandra import Cassandra
 
 
-__version__ = '0.5.5'
+__version__ = '0.5.6'
 
 TransformTS = GeneralTransformer
 
 __all__ = [
     'load_daily',
     'load_monthly',
     'load_yearly',
```

### Comparing `autots-0.5.5/autots/datasets/__init__.py` & `autots-0.5.6/autots/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/datasets/_base.py` & `autots-0.5.6/autots/datasets/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,17 +55,15 @@
                               }
     monthly_data = get_fred_data(fredkey = 'XXXXXXXXX', SeriesNameDict = SeriesNameDict)
     """
     module_path = dirname(__file__)
     data_file_name = join(module_path, 'data', 'fred_monthly.zip')
 
     df_long = pd.read_csv(data_file_name, compression='zip')
-    df_long['datetime'] = pd.to_datetime(
-        df_long['datetime'], infer_datetime_format=True
-    )
+    df_long['datetime'] = pd.to_datetime(df_long['datetime'])
 
     return df_long
 
 
 def load_monthly(long: bool = True):
     """Federal Reserve of St. Louis monthly economic indicators."""
     if long:
@@ -103,17 +101,15 @@
                   }
     monthly_data = get_fred_data(fredkey = 'XXXXXXXXX', SeriesNameDict = SeriesNameDict)
     """
     module_path = dirname(__file__)
     data_file_name = join(module_path, 'data', 'fred_yearly.zip')
 
     df_long = pd.read_csv(data_file_name)
-    df_long['datetime'] = pd.to_datetime(
-        df_long['datetime'], infer_datetime_format=True
-    )
+    df_long['datetime'] = pd.to_datetime(df_long['datetime'])
 
     return df_long
 
 
 def load_yearly(long: bool = True):
     """Federal Reserve of St. Louis annual economic indicators."""
     if long:
@@ -159,17 +155,15 @@
 
 def load_eia_weekly():
     """Weekly petroleum industry data from the EIA."""
     module_path = dirname(__file__)
     data_file_name = join(module_path, 'data', 'eia_weekly.zip')
 
     df_long = pd.read_csv(data_file_name, compression='zip')
-    df_long['datetime'] = pd.to_datetime(
-        df_long['datetime'], infer_datetime_format=True
-    )
+    df_long['datetime'] = pd.to_datetime(df_long['datetime'])
     return df_long
 
 
 def load_weekly(long: bool = True):
     """Weekly petroleum industry data from the EIA."""
     if long:
         return load_eia_weekly()
@@ -347,15 +341,15 @@
                 wargs = (
                     wargs
                     + f"&startDate={start_date}&endDate={str_end_time}&boundingBox=90,-180,-90,180&units=standard&format=csv"
                 )
                 wdf = pd.read_csv(
                     io.StringIO(s.get(wbase + wargs, timeout=timeout).text)
                 )
-                wdf['DATE'] = pd.to_datetime(wdf['DATE'], infer_datetime_format=True)
+                wdf['DATE'] = pd.to_datetime(wdf['DATE'])
                 wdf = wdf.set_index('DATE').drop(columns=['STATION'])
                 wdf.rename(columns=lambda x: wstation + "_" + x, inplace=True)
                 dataset_lists.append(wdf)
                 time.sleep(sleep_seconds)
             except Exception as e:
                 print(f"weather data failed: {repr(e)}")
 
@@ -387,15 +381,15 @@
             start_date = (
                 current_date - datetime.timedelta(days=earthquake_days)
             ).strftime("%Y-%m-%d")
             # is limited to ~1000 rows of data, ie individual earthquakes
             ebase = "https://earthquake.usgs.gov/fdsnws/event/1/query?"
             eargs = f"format=csv&starttime={start_date}&endtime={str_end_time}&minmagnitude={earthquake_min_magnitude}"
             eq = pd.read_csv(ebase + eargs)
-            eq["time"] = pd.to_datetime(eq["time"], infer_datetime_format=True)
+            eq["time"] = pd.to_datetime(eq["time"])
             eq["time"] = eq["time"].dt.tz_localize(None)
             eq.set_index("time", inplace=True)
             global_earthquakes = eq.resample("1D").agg(
                 {"mag": "mean", "depth": "count"}
             )
             global_earthquakes["mag"] = global_earthquakes["mag"].fillna(
                 earthquake_min_magnitude
@@ -429,17 +423,15 @@
                 gresult.name = domain
                 dataset_lists.append(gresult.to_frame())
                 time.sleep(sleep_seconds)
         except Exception as e:
             print(f"analytics.gov data failed with {repr(e)}")
 
     if wikipedia_pages is not None:
-        str_start = pd.to_datetime(
-            observation_start, infer_datetime_format=True
-        ).strftime("%Y%m%d00")
+        str_start = pd.to_datetime(observation_start).strftime("%Y%m%d00")
         str_end = current_date.strftime("%Y%m%d00")
         headers = {
             'User-Agent': 'AutoTS load_live_daily',
         }
         for page in wikipedia_pages:
             try:
                 if page == "all":
@@ -467,20 +459,16 @@
                 url = f"https://www.ncdc.noaa.gov/stormevents/csv?eventType={event_type}&beginDate_mm=01&beginDate_dd=01&beginDate_yyyy=2000&endDate_mm=09&endDate_dd=30&endDate_yyyy=9999&hailfilter=0.00&tornfilter=2&windfilter=000&sort=DN&statefips=-999%2CALL"
                 csv_in = io.StringIO(s.get(url, timeout=timeout).text)
                 try:
                     # new in 1.3.0 of pandas
                     df = pd.read_csv(csv_in, low_memory=False, on_bad_lines='skip')
                 except Exception:
                     df = pd.read_csv(csv_in, low_memory=False, error_bad_lines=False)
-                df['BEGIN_DATE'] = pd.to_datetime(
-                    df['BEGIN_DATE'], infer_datetime_format=True
-                )
-                df['END_DATE'] = pd.to_datetime(
-                    df['END_DATE'], infer_datetime_format=True
-                )
+                df['BEGIN_DATE'] = pd.to_datetime(df['BEGIN_DATE'])
+                df['END_DATE'] = pd.to_datetime(df['END_DATE'])
                 df['day'] = df.apply(
                     lambda row: pd.date_range(
                         row["BEGIN_DATE"], row['END_DATE'], freq='D'
                     ),
                     axis=1,
                 )
                 df = df.explode('day')
```

### Comparing `autots-0.5.5/autots/datasets/data/covid_daily.zip` & `autots-0.5.6/autots/datasets/data/covid_daily.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/datasets/data/eia_weekly.zip` & `autots-0.5.6/autots/datasets/data/eia_weekly.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/datasets/data/fred_monthly.zip` & `autots-0.5.6/autots/datasets/data/fred_monthly.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/datasets/data/fred_yearly.zip` & `autots-0.5.6/autots/datasets/data/fred_yearly.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/datasets/data/holidays.zip` & `autots-0.5.6/autots/datasets/data/holidays.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/datasets/data/traffic_hourly.zip` & `autots-0.5.6/autots/datasets/data/traffic_hourly.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/datasets/fred.py` & `autots-0.5.6/autots/datasets/fred.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 def get_fred_data(
     fredkey: str,
     SeriesNameDict: dict = None,
     long=True,
     observation_start=None,
     sleep_seconds: int = 1,
-    **kwargs
+    **kwargs,
 ):
     """Imports Data from Federal Reserve.
     For simplest results, make sure requested series are all of the same frequency.
 
     args:
         fredkey (str): an API key from FRED
         SeriesNameDict (dict): pairs of FRED Series IDs and Series Names like: {'SeriesID': 'SeriesName'} or a list of FRED IDs.
```

### Comparing `autots-0.5.5/autots/evaluator/anomaly_detector.py` & `autots-0.5.6/autots/evaluator/anomaly_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,19 @@
             id_vars="date", var_name='series', value_name="value"
         )
         scores_flat['series'] = pd.Categorical(
             scores_flat['series'], categories=self.score_categories
         )
         res = self.anomaly_classifier.predict(
             pd.concat(
-                [pd.get_dummies(scores_flat['series']), scores_flat['value']], axis=1
+                [
+                    pd.get_dummies(scores_flat['series'], dtype=float),
+                    scores_flat['value'],
+                ],
+                axis=1,
             )
         )
         res = pd.concat(
             [scores_flat[['date', "series"]], pd.Series(res, name='value')], axis=1
         ).pivot_table(index='date', columns='series', values="value")
         return res[scores.columns]
```

### Comparing `autots-0.5.5/autots/evaluator/auto_model.py` & `autots-0.5.6/autots/evaluator/auto_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,14 +611,24 @@
             forecast_length=forecast_length,
             prediction_interval=prediction_interval,
             random_seed=random_seed,
             verbose=verbose,
             n_jobs=n_jobs,
             **parameters,
         )
+    elif model == "Motif":
+        return Motif(
+            frequency=frequency,
+            prediction_interval=prediction_interval,
+            random_seed=random_seed,
+            verbose=verbose,
+            n_jobs=n_jobs,
+            multivariate=parameters.get("multivariate", False),
+            **parameters,
+        )
     else:
         raise AttributeError(
             ("Model String '{}' not a recognized model type").format(model)
         )
 
 
 def ModelPrediction(
@@ -1266,14 +1276,21 @@
         'Model',
         'ModelParameters',
         'TransformationParameters',
         'Ensemble',
     ],
     traceback: bool = False,
     current_model_file: str = None,
+    mosaic_list=[
+        'mosaic-window',
+        'mosaic',
+        'mosaic_crosshair',
+        "mosaic_window",
+        "mosaic-crosshair",
+    ],
 ):
     """
     Take Template, returns Results.
 
     There are some who call me... Tim. - Python
 
     Args:
@@ -1520,15 +1537,15 @@
             if 'distance' in ensemble:
                 cur_smape = model_error.per_timestamp.loc['weighted_smape']
                 cur_smape = pd.DataFrame(cur_smape).transpose()
                 cur_smape.index = [model_id]
                 template_result.per_timestamp_smape = pd.concat(
                     [template_result.per_timestamp_smape, cur_smape], axis=0
                 )
-            if 'mosaic' in ensemble or 'mosaic-window' in ensemble:
+            if any([x in mosaic_list for x in ensemble]):
                 template_result.full_mae_errors.extend([model_error.full_mae_errors])
                 template_result.squared_errors.extend([model_error.squared_errors])
                 template_result.full_pl_errors.extend(
                     [model_error.upper_pl + model_error.lower_pl]
                 )
                 template_result.full_mae_ids.extend([model_id])
```

### Comparing `autots-0.5.5/autots/evaluator/auto_ts.py` & `autots-0.5.6/autots/evaluator/auto_ts.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     remove_leading_zeros,
     horizontal_template_to_model_list,
 )
 from autots.models.ensemble import (
     EnsembleTemplateGenerator,
     HorizontalTemplateGenerator,
     generate_mosaic_template,
+    generate_crosshair_score,
 )
 from autots.models.model_list import model_lists, no_shared
 from autots.tools import cpu_count
 from autots.evaluator.validation import (
     validate_num_validations,
     generate_validation_indices,
 )
@@ -239,17 +240,27 @@
         # just a list of horizontal types in general
         self.h_ens_list = [
             'horizontal',
             'probabilistic',
             'hdist',
             "mosaic",
             'mosaic-window',
+            'mosaic_window',
+            'mosaic_crosshair',
+            'mosaic-crosshair',
             'horizontal-max',
             'horizontal-min',
         ]
+        self.mosaic_list = [
+            'mosaic',
+            'mosaic-window',
+            "mosaic_window",
+            'mosaic_crosshair',
+            "mosaic-crosshair",
+        ]
         if isinstance(ensemble, str):
             ensemble = str(ensemble).lower()
         if ensemble == 'all':
             ensemble = [
                 'simple',
                 "distance",
                 "horizontal",
@@ -447,15 +458,15 @@
                 print("\N{dagger} " + msg)
             except Exception:
                 print(msg)
 
     @staticmethod
     def get_new_params(method='random'):
         """Randomly generate new parameters for the class."""
-        if method == 'full':
+        if method != 'full':
             ensemble_choice = random.choices(
                 [
                     None,
                     ['simple'],
                     ['simple', 'horizontal-max'],
                     [
                         'simple',
@@ -475,14 +486,15 @@
                     [
                         'simple',
                         "distance",
                         "horizontal",
                         "horizontal-max",
                         "mosaic",
                         'mosaic-window',
+                        'mosaic-crosshair',
                         "subsample",
                         "mlensemble",
                     ],
                 ],
                 [0.3, 0.1, 0.2, 0.2],
             )[0]
         if method == "full":
@@ -1307,24 +1319,84 @@
                 models_to_use = horizontal_template_to_model_list(ens_templates)
             except Exception as e:
                 if self.verbose >= 0:
                     print(f"Horizontal Ensemble Generation Error: {repr(e)}")
                     time.sleep(5)
             try:
                 # eventually plan to allow window size to be controlled by params
-                if 'mosaic-window' in ensemble or 'mosaic' in ensemble:
+                if any([x in self.mosaic_list for x in ensemble]):
                     weight_per_value = (
                         self.initial_results.full_mae_errors
                         * metric_weighting.get('mae_weighting', 0)
                         + self.initial_results.full_pl_errors
                         * metric_weighting.get('spl_weighting', 0)
                         + self.initial_results.squared_errors
                         * metric_weighting.get('rmse_weighting', 0)
                     )
-                if 'mosaic-window' in ensemble:
+                if "mosaic_crosshair" in ensemble or "mosaic-crosshair" in ensemble:
+                    ens_templates = generate_mosaic_template(
+                        initial_results=self.initial_results.model_results,
+                        full_mae_ids=self.initial_results.full_mae_ids,
+                        num_validations=self.num_validations,
+                        col_names=df_subset.columns,
+                        full_mae_errors=[
+                            generate_crosshair_score(x)
+                            for x in self.initial_results.full_mae_errors
+                        ],
+                        smoothing_window=None,
+                        metric_name="mae-crosshair",
+                    )
+                    ensemble_templates = pd.concat(
+                        [ensemble_templates, ens_templates], axis=0
+                    )
+                    ens_templates = generate_mosaic_template(
+                        initial_results=self.initial_results.model_results,
+                        full_mae_ids=self.initial_results.full_mae_ids,
+                        num_validations=self.num_validations,
+                        col_names=df_subset.columns,
+                        full_mae_errors=[
+                            generate_crosshair_score(x)
+                            for x in self.initial_results.squared_errors
+                        ],
+                        smoothing_window=None,
+                        metric_name="se-crosshair",
+                    )
+                    ensemble_templates = pd.concat(
+                        [ensemble_templates, ens_templates], axis=0
+                    )
+                    ens_templates = generate_mosaic_template(
+                        initial_results=self.initial_results.model_results,
+                        full_mae_ids=self.initial_results.full_mae_ids,
+                        num_validations=self.num_validations,
+                        col_names=df_subset.columns,
+                        full_mae_errors=[
+                            generate_crosshair_score(x)
+                            for x in self.initial_results.full_pl_errors
+                        ],
+                        smoothing_window=3,
+                        metric_name="spl-crosshair",
+                    )
+                    ensemble_templates = pd.concat(
+                        [ensemble_templates, ens_templates], axis=0
+                    )
+                    ens_templates = generate_mosaic_template(
+                        initial_results=self.initial_results.model_results,
+                        full_mae_ids=self.initial_results.full_mae_ids,
+                        num_validations=self.num_validations,
+                        col_names=df_subset.columns,
+                        full_mae_errors=[
+                            generate_crosshair_score(x) for x in weight_per_value
+                        ],
+                        smoothing_window=None,
+                        metric_name="weighted-crosshair",
+                    )
+                    ensemble_templates = pd.concat(
+                        [ensemble_templates, ens_templates], axis=0
+                    )
+                if "mosaic_window" in ensemble or "mosaic-window" in ensemble:
                     ens_templates = generate_mosaic_template(
                         initial_results=self.initial_results.model_results,
                         full_mae_ids=self.initial_results.full_mae_ids,
                         num_validations=self.num_validations,
                         col_names=df_subset.columns,
                         full_mae_errors=self.initial_results.full_mae_errors,
                         smoothing_window=14,
@@ -1405,27 +1477,27 @@
                         full_mae_errors=weight_per_value,
                         smoothing_window=10,
                         metric_name="Weighted",
                     )
                     ensemble_templates = pd.concat(
                         [ensemble_templates, ens_templates], axis=0
                     )
+                if 'mosaic' in ensemble:
                     ens_templates = generate_mosaic_template(
                         initial_results=self.initial_results.model_results,
                         full_mae_ids=self.initial_results.full_mae_ids,
                         num_validations=self.num_validations,
                         col_names=df_subset.columns,
                         full_mae_errors=self.initial_results.squared_errors,
                         smoothing_window=None,
                         metric_name="SE",
                     )
                     ensemble_templates = pd.concat(
                         [ensemble_templates, ens_templates], axis=0
                     )
-                if 'mosaic' in ensemble:
                     ens_templates = generate_mosaic_template(
                         initial_results=self.initial_results.model_results,
                         full_mae_ids=self.initial_results.full_mae_ids,
                         num_validations=self.num_validations,
                         col_names=df_subset.columns,
                         full_mae_errors=self.initial_results.full_mae_errors,
                         smoothing_window=None,
@@ -1659,15 +1731,15 @@
                 print("Validation Round: {}".format(str(y + 1)))
             # slice the validation data into current validation slice
             current_slice = df_wide_numeric.reindex(self.validation_indexes[(y + 1)])
 
             # subset series (if used) and take a new train/test split
             if self.subset_flag:
                 # mosaic can't handle different cols in each validation
-                if "mosaic" in self.ensemble or "mosaic-window" in self.ensemble:
+                if any([x in self.mosaic_list for x in self.ensemble]):
                     rand_st = self.random_seed
                 else:
                     rand_st = self.random_seed + y + 1
                 df_subset = subset_series(
                     current_slice,
                     list((self.weights.get(i)) for i in current_slice.columns),
                     n=self.subset,
@@ -2212,17 +2284,24 @@
 
     def plot_horizontal_per_generation(
         self,
         title="Horizontal Ensemble Accuracy Gain (first eval sample only)",
         **kwargs,
     ):
         """Plot how well the horizontal ensembles would do after each new generation. Slow."""
-        self.horizontal_per_generation().model_results['Score'].plot(
-            ylabel="Lowest Score", xlabel="Generation", title=title, **kwargs
-        )
+        if (
+            self.best_model_ensemble == 2
+            and str(self.best_model_params.get('model_name', "Mosaic")).lower()
+            != "mosaic"
+        ):
+            self.horizontal_per_generation().model_results['Score'].plot(
+                ylabel="Lowest Score", xlabel="Generation", title=title, **kwargs
+            )
+        else:
+            print("not a valid horizontal model")
 
     def back_forecast(
         self, series=None, n_splits: int = "auto", tail: int = "auto", verbose: int = 0
     ):
         """Create forecasts for the historical training data, ie. backcast or back forecast. OUT OF SAMPLE
 
         This actually forecasts on historical data, these are not fit model values as are often returned by other packages.
```

### Comparing `autots-0.5.5/autots/evaluator/benchmark.py` & `autots-0.5.6/autots/evaluator/benchmark.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/evaluator/event_forecasting.py` & `autots-0.5.6/autots/evaluator/event_forecasting.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/evaluator/metrics.py` & `autots-0.5.6/autots/evaluator/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,15 @@
             Without, it is an "unanchored" shape fitting metric.
             This will also allow this to work on forecast_length = 1 forecasts
         scaler (np.array): if provided, metrics are scaled by this. 1d array of shape (num_series,)
     """
     # scaler = np.mean(A, axis=0)  # debate over whether to make this scaled
     if df_train is not None:
         last_of_array = np.nan_to_num(
-            df_train[
-                df_train.shape[0] - 1 : df_train.shape[0],
-            ]
+            df_train[df_train.shape[0] - 1 : df_train.shape[0],]
         )
         # last_of_array = df_train.tail(1).fillna(0).to_numpy()
         # assigning to new because I'm paranoid about overwrite existing objects
         lA = np.concatenate([last_of_array, A])
         lF = np.concatenate([last_of_array, F])
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=RuntimeWarning)
@@ -425,15 +423,15 @@
     upper_forecast,
     lower_forecast,
     df_train,
     prediction_interval,
     columns=None,
     scaler=None,
     return_components=False,
-    **kwargs
+    **kwargs,
 ):
     """Create a pd.DataFrame of metrics per series given actuals, forecast, and precalculated errors.
 
     Args:
         A (np.array): array or df of actuals
         F (np.array): array or df of forecasts
         return_components (bool): if True, return tuple of detailed errors
```

### Comparing `autots-0.5.5/autots/evaluator/validation.py` & `autots-0.5.6/autots/evaluator/validation.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/models/arch.py` & `autots-0.5.6/autots/models/arch.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/models/base.py` & `autots-0.5.6/autots/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,18 +393,16 @@
                 method=interpolate, limit_direction="backward"
             )
             plot_df["forecast"] = plot_df["forecast"].interpolate(
                 method=interpolate, limit_direction="backward", limit=5
             )
 
         if start_date is not None:
-            start_date = pd.to_datetime(start_date, infer_datetime_format=True)
-            if plot_df.index.max() < pd.to_datetime(
-                start_date, infer_datetime_format=True
-            ):
+            start_date = pd.to_datetime(start_date)
+            if plot_df.index.max() < start_date:
                 raise ValueError("start_date is more recent than all data provided")
             plot_df = plot_df[plot_df.index >= start_date]
         return plot_df
 
     def plot(
         self,
         df_wide=None,
```

### Comparing `autots-0.5.5/autots/models/basics.py` & `autots-0.5.6/autots/models/basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -687,17 +687,15 @@
             replace=False,
         )
 
         # make this faster
         motif_vecs_list = []
         # takes random slices of the time series and rearranges as phrase_n length vectors
         for z in numbers:
-            rand_slice = df.iloc[
-                z : (z + phrase_n),
-            ]
+            rand_slice = df.iloc[z : (z + phrase_n),]
             rand_slice = (
                 rand_slice.reset_index(drop=True)
                 .transpose()
                 .set_index(np.repeat(z, (df.shape[1],)), append=True)
             )
             # motif_vecs = pd.concat([motif_vecs, rand_slice], axis=0)
             motif_vecs_list.append(rand_slice)
```

### Comparing `autots-0.5.5/autots/models/cassandra.py` & `autots-0.5.6/autots/models/cassandra.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/models/dnn.py` & `autots-0.5.6/autots/models/dnn.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/models/ensemble.py` & `autots-0.5.6/autots/models/ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,14 +448,15 @@
         full_models = available_models  # hope it doesn't need to fill
     # print(f"FULLMODEL {len(full_models)}: {full_models}")
     if prematched_series is None:
         prematched_series = ensemble_params['series']
     all_series = generalize_horizontal(
         df_train, prematched_series, available_models, full_models
     )
+    ensemble_params['series'] = all_series
     # print(f"ALLSERIES {len(all_series.keys())}: {all_series}")
 
     org_idx = df_train.columns
 
     forelist, forelist_l, forelist_u = [], [], []
     """
     # forelist = [forecasts.get(mod_id)[series] for series, mod_id in all_series.items()]
@@ -1300,14 +1301,45 @@
         best5_params = pd.DataFrame(best5_params, index=[0])
         ensemble_templates = pd.concat(
             [ensemble_templates, best5_params], axis=0, ignore_index=True
         )
     return ensemble_templates
 
 
+def generate_crosshair_score(error_matrix):
+    arr_size = error_matrix.size
+    base_weight = 0.001 / arr_size
+    sum_error = np.sum(error_matrix) * base_weight
+
+    cross_base = error_matrix * (base_weight * 50)
+    row_sums = cross_base.sum(axis=1)
+    col_sums = cross_base.sum(axis=0)
+    outer_sum = np.add.outer(row_sums, col_sums)
+
+    return error_matrix + sum_error + outer_sum
+
+
+def generate_crosshair_score_list(error_list):
+    # unfinished 3d version
+    arr_size = error_list[-1].size
+    base_weight = 0.001 / arr_size
+
+    full_arr = np.array(error_list)
+
+    sum_error = np.sum(full_arr, axis=(-1, 1))
+
+    cross_base = full_arr * (base_weight * 50)
+    row_sums = cross_base.sum(axis=2)
+    col_sums = cross_base.sum(axis=1)
+    # stops working here
+    outer_sum = np.add.outer(row_sums, col_sums)  # noqa
+
+    return list(full_arr + sum_error)  # + outer_sum
+
+
 def generate_mosaic_template(
     initial_results,
     full_mae_ids,
     num_validations,
     col_names,
     full_mae_errors,
     smoothing_window=None,
@@ -1519,14 +1551,15 @@
     l_forecast_df = l_forecast_df.reindex(columns=org_idx)
     # combine runtimes
     try:
         ens_runtime = sum(list(forecasts_runtime.values()), datetime.timedelta())
     except Exception:
         ens_runtime = datetime.timedelta(0)
 
+    ensemble_params['series'] = all_series
     ens_result = PredictionObject(
         model_name="Ensemble",
         forecast_length=len(sample_idx),
         forecast_index=sample_idx,
         forecast_columns=org_idx,
         lower_forecast=l_forecast_df,
         forecast=forecast_df,
```

### Comparing `autots-0.5.5/autots/models/gluonts.py` & `autots-0.5.6/autots/models/gluonts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 GluonTS
 
 Best neuralnet models currently available, released by Amazon, scale well.
 Except it is really the only thing I use that runs mxnet, and it takes a while to train these guys...
 
-Note that there are routinely package version issues with this and its dependencies
+Note that there are routinely package version issues with this and its dependencies. Stability is not the strong suit of GluonTS.
 """
 import logging
 import random
 import datetime
 import numpy as np
 import pandas as pd
 from autots.models.base import ModelObject, PredictionObject
 
 try:
     from gluonts.dataset.common import ListDataset
 
     # GluonTS looooves to move import locations...
     try:
-        from gluonts.transform import FieldName  # old way (0.3.3 and older)
-    except Exception:
         from gluonts.dataset.field_names import FieldName  # new way
+    except Exception:
+        from gluonts.transform import FieldName  # old way (0.3.3 and older)
     try:  # new way
         from gluonts.mx.trainer import Trainer
     except Exception:  # old way < 0.5.x
         from gluonts.trainer import Trainer
 except Exception:  # except ImportError
     _has_gluonts = False
 else:
@@ -89,15 +89,15 @@
         """Train algorithm given data supplied.
 
         Args:
             df (pandas.DataFrame): Datetime Indexed
         """
         if not _has_gluonts:
             raise ImportError(
-                "GluonTS installation not found or installed version is incompatible with AutoTS."
+                "GluonTS installation is incompatible with AutoTS. The numpy version is sometimes the issue."
             )
 
         df = self.basic_profile(df)
 
         try:
             from mxnet.random import seed as mxnet_seed
 
@@ -141,14 +141,15 @@
             'start_ts': df.index[0],
             'gluon_start': [
                 self.train_columns[0] for _ in range(len(self.train_index))
             ],
             'context_length': self.gluon_context_length,
             'forecast_length': self.forecast_length,
         }
+        npts_flag = False
         if self.gluon_model in self.multivariate_mods:
             if self.regression_type == "User":
                 regr = future_regressor.to_numpy().T
                 self.regr_train = regr
                 self.test_ds = ListDataset(
                     [
                         {
@@ -191,185 +192,242 @@
                         for (target, start) in zip(
                             gluon_train, ts_metadata['gluon_start']
                         )
                     ],
                     freq=ts_metadata['freq'],
                 )
         if self.gluon_model == 'DeepAR':
-            from gluonts.model.deepar import DeepAREstimator
+            try:
+                from gluonts.mx import DeepAREstimator
+            except Exception:
+                from gluonts.model.deepar import DeepAREstimator
 
             estimator = DeepAREstimator(
                 freq=ts_metadata['freq'],
                 context_length=ts_metadata['context_length'],
                 prediction_length=ts_metadata['forecast_length'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'NPTS':
-            from gluonts.model.npts import NPTSEstimator
+            try:
+                from gluonts.model.npts import NPTSPredictor
 
-            estimator = NPTSEstimator(
-                freq=ts_metadata['freq'],
-                context_length=ts_metadata['context_length'],
-                prediction_length=ts_metadata['forecast_length'],
-            )
+                estimator = NPTSPredictor(
+                    freq=ts_metadata['freq'],
+                    context_length=ts_metadata['context_length'],
+                    prediction_length=ts_metadata['forecast_length'],
+                )
+                npts_flag = True
+            except Exception:
+                from gluonts.model.npts import NPTSEstimator
+
+                estimator = NPTSEstimator(
+                    freq=ts_metadata['freq'],
+                    context_length=ts_metadata['context_length'],
+                    prediction_length=ts_metadata['forecast_length'],
+                )
 
         elif self.gluon_model == 'MQCNN':
-            from gluonts.model.seq2seq import MQCNNEstimator
+            try:
+                from gluonts.mx import MQCNNEstimator
+            except Exception:
+                from gluonts.model.seq2seq import MQCNNEstimator
 
             estimator = MQCNNEstimator(
                 freq=ts_metadata['freq'],
                 context_length=ts_metadata['context_length'],
                 prediction_length=ts_metadata['forecast_length'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
 
         elif self.gluon_model == 'SFF':
-            from gluonts.model.simple_feedforward import SimpleFeedForwardEstimator
+            try:
+                from gluonts.mx import SimpleFeedForwardEstimator
+            except Exception:
+                from gluonts.model.simple_feedforward import SimpleFeedForwardEstimator
 
             estimator = SimpleFeedForwardEstimator(
                 prediction_length=ts_metadata['forecast_length'],
                 context_length=ts_metadata['context_length'],
-                freq=ts_metadata['freq'],
+                # freq=ts_metadata['freq'],
                 trainer=Trainer(
                     epochs=self.epochs,
                     learning_rate=self.learning_rate,
                     hybridize=False,
                     num_batches_per_epoch=100,
                 ),
             )
 
         elif self.gluon_model == 'Transformer':
-            from gluonts.model.transformer import TransformerEstimator
+            try:
+                from gluonts.mx import TransformerEstimator
+            except Exception:
+                from gluonts.model.transformer import TransformerEstimator
 
             estimator = TransformerEstimator(
                 prediction_length=ts_metadata['forecast_length'],
                 context_length=ts_metadata['context_length'],
                 freq=ts_metadata['freq'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
 
         elif self.gluon_model == 'DeepState':
-            from gluonts.model.deepstate import DeepStateEstimator
+            try:
+                from gluonts.mx import DeepStateEstimator
+            except Exception:
+                from gluonts.model.deepstate import DeepStateEstimator
 
             estimator = DeepStateEstimator(
                 prediction_length=ts_metadata['forecast_length'],
                 past_length=ts_metadata['context_length'],
                 freq=ts_metadata['freq'],
                 use_feat_static_cat=False,
                 cardinality=[1],
                 trainer=Trainer(
                     ctx='cpu', epochs=self.epochs, learning_rate=self.learning_rate
                 ),
             )
 
         elif self.gluon_model == 'DeepFactor':
-            from gluonts.model.deep_factor import DeepFactorEstimator
+            try:
+                from gluonts.mx import DeepFactorEstimator
+            except Exception:
+                from gluonts.model.deep_factor import DeepFactorEstimator
 
             estimator = DeepFactorEstimator(
                 freq=ts_metadata['freq'],
                 context_length=ts_metadata['context_length'],
                 prediction_length=ts_metadata['forecast_length'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
 
         elif self.gluon_model == 'WaveNet':
             # Usually needs more epochs/training iterations than other models do
-            from gluonts.model.wavenet import WaveNetEstimator
+            try:
+                from gluonts.mx import WaveNetEstimator
+            except Exception:
+                from gluonts.model.wavenet import WaveNetEstimator
 
             estimator = WaveNetEstimator(
                 freq=ts_metadata['freq'],
                 prediction_length=ts_metadata['forecast_length'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'DeepVAR':
-            from gluonts.model.deepvar import DeepVAREstimator
+            try:
+                from gluonts.mx import DeepVAREstimator
+            except Exception:
+                from gluonts.model.deepvar import DeepVAREstimator
 
             estimator = DeepVAREstimator(
                 target_dim=gluon_train.shape[0],
                 freq=ts_metadata['freq'],
                 context_length=ts_metadata['context_length'],
                 prediction_length=ts_metadata['forecast_length'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'GPVAR':
-            from gluonts.model.gpvar import GPVAREstimator
+            try:
+                from gluonts.mx import GPVAREstimator
+            except Exception:
+                from gluonts.model.gpvar import GPVAREstimator
 
             estimator = GPVAREstimator(
                 target_dim=gluon_train.shape[0],
                 freq=ts_metadata['freq'],
                 context_length=ts_metadata['context_length'],
                 prediction_length=ts_metadata['forecast_length'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'LSTNet':
-            from gluonts.model.lstnet import LSTNetEstimator
+            try:
+                from gluonts.mx import LSTNetEstimator
+            except Exception:
+                from gluonts.model.lstnet import LSTNetEstimator
 
             estimator = LSTNetEstimator(
-                freq=ts_metadata['freq'],
+                # freq=ts_metadata['freq'],
                 num_series=len(self.train_index),
-                skip_size=0,
+                skip_size=1,
                 ar_window=1,
                 channels=2,
                 context_length=ts_metadata['context_length'],
                 prediction_length=ts_metadata['forecast_length'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'NBEATS':
-            from gluonts.model.n_beats import NBEATSEstimator
+            try:
+                from gluonts.mx import NBEATSEstimator
+            except Exception:
+                from gluonts.model.n_beats import NBEATSEstimator
 
             estimator = NBEATSEstimator(
                 freq=ts_metadata['freq'],
                 context_length=ts_metadata['context_length'],
                 prediction_length=ts_metadata['forecast_length'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'Rotbaum':
-            from gluonts.model.rotbaum import TreeEstimator
+            try:
+                from gluonts.ext.rotbaum import TreeEstimator
+            except Exception:
+                from gluonts.model.rotbaum import TreeEstimator
 
             estimator = TreeEstimator(
                 freq=ts_metadata['freq'],
                 context_length=ts_metadata['context_length'],
                 prediction_length=ts_metadata['forecast_length'],
                 # trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'DeepRenewalProcess':
-            from gluonts.model.renewal import DeepRenewalProcessEstimator
+            try:
+                from gluonts.mx import DeepRenewalProcessEstimator
+            except Exception:
+                from gluonts.model.renewal import DeepRenewalProcessEstimator
 
             estimator = DeepRenewalProcessEstimator(
                 prediction_length=ts_metadata['forecast_length'],
                 context_length=ts_metadata['context_length'],
                 num_layers=1,  # original paper used 1 layer, 10 cells
                 num_cells=10,
-                freq=ts_metadata['freq'],
+                # freq=ts_metadata['freq'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'SelfAttention':
-            from gluonts.model.san import SelfAttentionEstimator
+            try:
+                from gluonts.nursery.san import SelfAttentionEstimator
+            except Exception:
+                from gluonts.model.san import SelfAttentionEstimator
 
             estimator = SelfAttentionEstimator(
                 prediction_length=ts_metadata['forecast_length'],
                 context_length=ts_metadata['context_length'],
                 freq=ts_metadata['freq'],
                 trainer=Trainer(
                     epochs=self.epochs,
                     learning_rate=self.learning_rate,
-                    use_feature_dynamic_real=False,
                 ),
             )
         elif self.gluon_model == 'TemporalFusionTransformer':
-            from gluonts.model.tft import TemporalFusionTransformerEstimator
+            try:
+                from gluonts.mx import TemporalFusionTransformerEstimator
+            except Exception:
+                from gluonts.model.tft import TemporalFusionTransformerEstimator
 
             estimator = TemporalFusionTransformerEstimator(
                 prediction_length=ts_metadata['forecast_length'],
                 context_length=ts_metadata['context_length'],
                 freq=ts_metadata['freq'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'DeepTPP':
-            from gluonts.model.tpp.deeptpp import DeepTPPEstimator
+            try:
+                from gluonts.mx import DeepTPPEstimator
+            except Exception:
+                from gluonts.model.tpp.deeptpp import DeepTPPEstimator
 
             estimator = DeepTPPEstimator(
                 prediction_interval_length=ts_metadata['forecast_length'],
                 context_interval_length=ts_metadata['context_length'],
                 num_marks=1,  # cardinality
                 freq=ts_metadata['freq'],
                 trainer=Trainer(
@@ -377,15 +435,18 @@
                     learning_rate=self.learning_rate,
                     hybridize=False,
                 ),
             )
         else:
             raise ValueError("'gluon_model' not recognized.")
 
-        self.GluonPredictor = estimator.train(self.test_ds)
+        if self.gluon_model == 'NPTS' and npts_flag:
+            self.GluonPredictor = estimator
+        else:
+            self.GluonPredictor = estimator.train(self.test_ds)
         self.ts_metadata = ts_metadata
         self.fit_runtime = datetime.datetime.now() - self.startTime
         return self
 
     def predict(
         self, forecast_length: int, future_regressor=[], just_point_forecast=False
     ):
@@ -543,17 +604,17 @@
                     0.1,
                     0.1,
                     0.1,
                     0.05,
                     0.1,
                     0.1,
                     0.1,
+                    0.01,
                     0.1,
-                    0.1,
-                    0.1,
+                    0.01,
                 ],
                 k=1,
             )[0]
             epochs_choice = random.choices(
                 [20, 40, 80, 150, 300, 500], [0.58, 0.35, 0.05, 0.05, 0.05, 0.02]
             )[0]
         else:
```

### Comparing `autots-0.5.5/autots/models/greykite.py` & `autots-0.5.6/autots/models/greykite.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     model_template='silverkite',
     growth=None,
     holiday=True,
     holiday_country="UnitedStates",
     regressors=None,
     verbose=0,
     inner_n_jobs=1,
-    **kwargs
+    **kwargs,
 ):
     """Internal. For loop or parallel version of Greykite."""
     inner_df = pd.DataFrame(
         {
             'ts': df_index,
             'y': series,
         }
```

### Comparing `autots-0.5.5/autots/models/matrix_var.py` & `autots-0.5.6/autots/models/matrix_var.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/models/mlensemble.py` & `autots-0.5.6/autots/models/mlensemble.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,31 +19,31 @@
     validate_num_validations,
     generate_validation_indices,
 )
 from autots.models.sklearn import (
     retrieve_regressor,
 )  # generate_regressor_params, datepart_model_dict
 from autots.tools.shaping import simple_train_test_split
+from autots.tools.seasonal import date_part
 
 
 def create_feature(
     df_train,
     models,
     forecast_length,
     future_regressor_train=None,
     future_regressor_forecast=None,
+    datepart_method=None,
 ):
     result_windows = None
     res = []
     # add last value as a feature
     res.append(
         np.repeat(
-            df_train.iloc[
-                -1:,
-            ].to_numpy(),
+            df_train.iloc[-1:,].to_numpy(),
             forecast_length,
             axis=0,
         )
     )
     # add averages
     res.append(
         np.repeat(df_train.mean().to_numpy()[np.newaxis, :], forecast_length, axis=0)
@@ -123,14 +123,23 @@
                 [0] * forecast_length,
                 [res.shape[2] - 1] * forecast_length,
                 res.shape[2],
             ).T[np.newaxis, :, :],
         ),
         axis=0,
     )
+    if datepart_method not in [None, "None", "none"]:
+        date_part_df = date_part(forecasts.forecast.index, method=datepart_method)
+        res = np.concatenate(
+            (
+                res,
+                np.repeat(date_part_df.to_numpy()[np.newaxis, :, :], 21, axis=0).T,
+            ),
+            axis=0,
+        )
 
     sys.stdout.flush()
     return res
 
 
 """
 X = []
@@ -231,14 +240,15 @@
                 'ModelParameters': {},
                 "TransformationParameters": {},
             },
         ],
         num_validations=2,
         validation_method="backwards",
         min_allowed_train_percent=0.5,
+        datepart_method="expanded_binarized",
         models_source: str = 'random',
         **kwargs,
     ):
         ModelObject.__init__(
             self,
             name,
             frequency,
@@ -249,14 +259,15 @@
             regression_type=regression_type,
         )
         self.forecast_length = forecast_length
         assert num_validations >= 0, f"window {num_validations} must be >= 0"
         self.num_validations = int(num_validations)
         self.validation_method = validation_method
         self.min_allowed_train_percent = min_allowed_train_percent
+        self.datepart_method = datepart_method
         if regression_model is None:
             try:
                 import xgboost  # noqa
 
                 regression_model = {
                     "model": 'XGBRegressor',
                     "model_params": {
@@ -361,41 +372,42 @@
             if future_regressor is not None:
                 regr_subset_t = future_regressor.reindex(index=df_train.index)
                 regr_subset_f = future_regressor.reindex(index=df_test.index)
             else:
                 regr_subset_t = None
                 regr_subset_f = None
             try:
-                res = create_feature(
+                self.res = create_feature(
                     df_train,
                     self.models,
                     self.forecast_length,
                     future_regressor_train=regr_subset_t,
                     future_regressor_forecast=regr_subset_f,
+                    datepart_method=self.datepart_method,
                 )
-                X.append(res.reshape(res.shape[0], -1))
+                X.append(self.res.reshape(self.res.shape[0], -1))
                 y.append(df_test.to_numpy().reshape(-1))
             except Exception as e:
                 if val < 1:
                     raise e
                 else:
                     print(f"validation round {y} failed with {repr(e)}")
 
-        X = np.concatenate(X, axis=1).T
-        y = np.concatenate(y, axis=0)
+        self.X = np.concatenate(X, axis=1).T
+        self.y = np.concatenate(y, axis=0)
 
         self.regr = retrieve_regressor(
             regression_model=self.regression_model,
             verbose=self.verbose,
             verbose_bool=False,
             random_seed=self.random_seed,
             n_jobs=self.n_jobs,
             multioutput=False,
         )
-        self.regr.fit(X, y)
+        self.regr.fit(self.X, self.y)
         self.fit_runtime = datetime.datetime.now() - self.startTime
         return self
 
     def predict(
         self,
         forecast_length: int = None,
         future_regressor=None,
@@ -420,14 +432,15 @@
         X = []
         res = create_feature(
             self.df,
             self.models,
             self.forecast_length,
             future_regressor_train=self.regressor_train,
             future_regressor_forecast=future_regressor,
+            datepart_method=self.datepart_method,
         )
         X.append(res.reshape(res.shape[0], -1))
         X = np.concatenate(X, axis=1).T
         forecast = pd.DataFrame(
             self.regr.predict(X).reshape(self.forecast_length, self.df.shape[1]),
             index=test_index,
             columns=self.df.columns,
@@ -461,44 +474,59 @@
     def get_new_params(self, method: str = 'random'):
         """Returns dict of new parameters for parameter tuning"""
         if "regressor" in method:
             regression_type_choice = "User"
         else:
             regression_type_choice = None
         # regr_params = generate_regressor_params(model_dict=datepart_model_dict)
-        model3 = random.choice(['FBProphet', "SeasonalityMotif", "DatepartRegression"])
+        # model3 = random.choice(['Cassandra', 'MetricMotif', 'FBProphet', "SeasonalityMotif", "DatepartRegression"])
         models = RandomTemplate(
             n=3,
-            model_list=['Cassandra', 'MetricMotif', model3],
+            model_list='fast',
             transformer_max_depth=4,
             transformer_list='fast',
         )
         models = models[
             ['Model', 'ModelParameters', 'TransformationParameters']
         ].to_dict(orient='records')
 
         return {
             "num_validations": random.choices([0, 1, 2], [0.5, 0.3, 0.2])[0],
             "validation_method": random.choices(
                 ["backwards", "similarity", "seasonal"], [0.5, 0.3, 0.2]
             )[0],
             "regression_model": None,
             "models": models,
+            "datepart_method": random.choices(
+                [
+                    None,
+                    "recurring",
+                    "simple",
+                    "expanded",
+                    "simple_2",
+                    "simple_binarized",
+                    "expanded_binarized",
+                    'common_fourier',
+                    'common_fourier_rw',
+                ],
+                [0.2, 0.2, 0.1, 0.3, 0.3, 0.4, 0.35, 0.45, 0.2],
+            )[0],
             "regression_type": regression_type_choice,
             "models_source": 'random',
         }
 
     def get_params(self):
         """Return dict of current parameters"""
         return {
             "num_validations": self.num_validations,
             "validation_method": self.validation_method,
             "regression_type": self.regression_type,
             "models_source": self.models_source,
             "models": self.models,
+            "datepart_method": self.datepart_method,
             "regression_model": self.regression_model,
         }
 
 
 """
 from flaml import AutoML
```

### Comparing `autots-0.5.5/autots/models/model_list.py` & `autots-0.5.6/autots/models/model_list.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/models/prophet.py` & `autots-0.5.6/autots/models/prophet.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/models/pytorch.py` & `autots-0.5.6/autots/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/models/sklearn.py` & `autots-0.5.6/autots/models/sklearn.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
         )
     else:
         regression_model['model'] = 'RandomForest'
         from sklearn.ensemble import RandomForestRegressor
 
         regr = RandomForestRegressor(
             random_state=random_seed,
-            verbose=verbose,
+            verbose=verbose_bool,
             n_jobs=n_jobs,
             **model_param_dict,
         )
         return regr
 
 
 # models that can more quickly handle many X/Y obs, with modest number of features
@@ -2908,16 +2908,18 @@
                 'simple',
                 'expanded',
                 'recurring',
                 "simple_2",
                 "simple_2_poly",
                 "simple_binarized",
                 "common_fourier",
+                "expanded_binarized",
+                "common_fourier_rw",
             ],
-            [0.5, 0.05, 0.1, 0.1, 0.05, 0.1, 0.05, 0.05],
+            [0.2, 0.05, 0.1, 0.1, 0.05, 0.1, 0.05, 0.05, 0.05, 0.025],
         )[0]
         holiday_choice = random.choices([True, False], [0.1, 0.9])[0]
         polynomial_degree_choice = random.choices([None, 2], [0.995, 0.005])[0]
         if "regressor" in method:
             regression_choice = "User"
         else:
             regression_choice = random.choices([None, 'User'], [0.7, 0.3])[0]
```

### Comparing `autots-0.5.5/autots/models/statsmodels.py` & `autots-0.5.6/autots/models/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/models/tfp.py` & `autots-0.5.6/autots/models/tfp.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/templates/general.py` & `autots-0.5.6/autots/templates/general.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/tools/anomaly_utils.py` & `autots-0.5.6/autots/tools/anomaly_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -993,15 +993,16 @@
                 if style == "flag":
                     populated_holidays['holiday_name'] = pd.Categorical(
                         populated_holidays['holiday_name'],
                         categories=holiday_df['holiday_name'].unique(),
                         ordered=True,
                     )
                     result_per_holiday = pd.get_dummies(
-                        populated_holidays['holiday_name']
+                        populated_holidays['holiday_name'],
+                        dtype=float,
                     )
                     result_per_holiday.index = populated_holidays['date']
                     result.append(result_per_holiday.groupby(level=0).sum())
                 elif style in ["impact", 'series_flag']:
                     temp = populated_holidays.pivot(
                         index='date', columns='series', values='holiday_name'
                     ).reindex(columns=df_cols)
```

### Comparing `autots-0.5.5/autots/tools/calendar.py` & `autots-0.5.6/autots/tools/calendar.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,15 @@
     new_years['lunar_month'] = new_years.groupby('syear').cumcount() + 1
     return new_years
 
 
 def gregorian_to_christian_lunar(datetime_index):
     """Convert a pandas DatetimeIndex to Christian Lunar calendar. Aspiration it doesn't work exactly."""
     if isinstance(datetime_index, (str, list)):
-        datetime_input = pd.to_datetime(
-            datetime_index, infer_datetime_format=True
-        ).sort_values()
+        datetime_input = pd.to_datetime(datetime_index).sort_values()
     else:
         datetime_input = datetime_index.sort_values()
     expanded_dates = pd.date_range(
         datetime_input[0] - pd.Timedelta(days=365), datetime_input[-1], freq='D'
     )
     min_year = np.min(expanded_dates.year)
     moon_df = moon_phase_df(expanded_dates, epoch=2444238.5)
@@ -74,17 +72,15 @@
         ['lunar_year', 'lunar_month', 'lunar_day', 'weekofmonth', 'dayofweek'],
     ].astype(int)
 
 
 def gregorian_to_chinese(datetime_index):
     """Convert a pandas DatetimeIndex to Chinese Lunar calendar. Potentially has errors."""
     if isinstance(datetime_index, (str, list)):
-        datetime_input = pd.to_datetime(
-            datetime_index, infer_datetime_format=True
-        ).sort_values()
+        datetime_input = pd.to_datetime(datetime_index).sort_values()
     else:
         datetime_input = datetime_index.sort_values()
     expanded_dates = pd.date_range(
         datetime_input[0] - pd.Timedelta(days=365), datetime_input[-1], freq='D'
     )
     min_year = np.min(expanded_dates.year)
     moon_df = moon_phase_df(expanded_dates, epoch=2444238.5)
@@ -119,15 +115,15 @@
 def gregorian_to_islamic(date, epoch_adjustment=1.5):
     """Calculate Islamic dates for pandas DatetimeIndex. Approximately. From convertdate by fitnr.
 
     Args:
         epoch_adjustment (float): 1.0 and that needs to be adjusted by about +/- 0.5 to account for timezone
     """
     if isinstance(date, (str, list)):
-        date = pd.to_datetime(date, infer_datetime_format=True)
+        date = pd.to_datetime(date)
     jd = date.to_julian_date()
     jd = np.floor(jd) + epoch_adjustment
     year = np.floor(((30 * (jd - 1948439.5)) + 10646) / 10631)
     month = np.minimum(12, np.ceil((jd - (29 + to_jd(year, 1, 1))) / 29.5) + 1)
     day = (jd - to_jd(year, month, 1)).astype(int) + 1
     return (
         pd.DataFrame({'year': year, 'month': month, 'day': day}, index=date)
@@ -214,15 +210,15 @@
 
 def gregorian_to_hebrew(dates):
     """Convert pd.Datetimes to a Hebrew date. From pyluach by simlist.
 
     This is the slowest of the lot and needs to be improved.
     """
     if isinstance(dates, (str, list)):
-        day = pd.to_datetime(dates, infer_datetime_format=True).to_julian_date()
+        day = pd.to_datetime(dates).to_julian_date()
     else:
         day = dates.to_julian_date()
     if (day <= 347997).any():
         raise ValueError("According to this calendar, this time doesn't exist")
 
     jd = (day + 0.5).astype(int)  # Try to account for half day
     jd -= 347997
```

### Comparing `autots-0.5.5/autots/tools/cointegration.py` & `autots-0.5.6/autots/tools/cointegration.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/tools/cpu_count.py` & `autots-0.5.6/autots/tools/cpu_count.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/tools/fast_kalman.py` & `autots-0.5.6/autots/tools/fast_kalman.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/tools/hierarchial.py` & `autots-0.5.6/autots/tools/hierarchial.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/tools/holiday.py` & `autots-0.5.6/autots/tools/holiday.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             encoder.fit_transform(country_holidays.to_numpy().reshape(-1, 1)).flatten(),
             name="HolidayFlag",
         )
         # since zeroes are reserved for non-holidays
         holi_days = holi_days + 1
         holi_days.index = country_holidays.index
         """
-        holi_days = pd.get_dummies(country_holidays)
+        holi_days = pd.get_dummies(country_holidays, dtype=float)
     else:
         country_holidays = country_holidays_base.keys()
         if not country_holidays:
             holi_days = pd.Series(0, name='HolidayFlag', dtype=int)
         else:
             holi_days = pd.Series(
                 np.repeat(1, len(country_holidays)),
```

### Comparing `autots-0.5.5/autots/tools/impute.py` & `autots-0.5.6/autots/tools/impute.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/tools/lunar.py` & `autots-0.5.6/autots/tools/lunar.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/tools/percentile.py` & `autots-0.5.6/autots/tools/percentile.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/tools/probabilistic.py` & `autots-0.5.6/autots/tools/probabilistic.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/tools/profile.py` & `autots-0.5.6/autots/tools/profile.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/autots/tools/regressor.py` & `autots-0.5.6/autots/tools/regressor.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         },
     },
     holiday_regr_style="flag",
 ):
     """Create a regressor from information available in the existing dataset.
     Components: are lagged data, datepart information, and holiday.
 
-    All of this info and more is already created by the ~Regression models, but this may help some other models (GLM, WindowRegression)
+    This function has been confusing people. This is NOT necessary for machine learning models, in AutoTS they internally create more elaborate feature sets separately.
+    This instead may help some other models (GLM, ARIMA) which accept regressors but won't build a regressor feature set internally.
+    And this allows post-hoc customization as needed before input to AutoTS.
 
     It is recommended that the .head(forecast_length) of both regressor_train and the df for training are dropped.
     `df = df.iloc[forecast_length:]`
     If you don't want the lagged features, set summarize="median" which will only give one column of such, which can then be easily dropped
 
     Args:
         df (pd.DataFrame): WIDE style dataframe (use long_to_wide if the data isn't already)
```

### Comparing `autots-0.5.5/autots/tools/seasonal.py` & `autots-0.5.6/autots/tools/seasonal.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,17 @@
                 ),
                 'weekend': (DTindex.weekday > 4).astype(int),
                 'quarter': DTindex.quarter,
                 'epoch': DTindex.to_julian_date(),
             }
         )
         # date_part_df['weekday'] = date_part_df['month'].astype(pd.CategoricalDtype(categories=list(range(6))))
-        date_part_df = pd.get_dummies(date_part_df, columns=['month', 'weekday'])
+        date_part_df = pd.get_dummies(
+            date_part_df, columns=['month', 'weekday'], dtype=float
+        )
         if method == "lunar_phase":
             date_part_df['phase'] = moon_phase(DTindex)
     elif "simple_binarized" in method:
         date_part_df = pd.DataFrame(
             {
                 'month': pd.Categorical(
                     DTindex.month, categories=list(range(1, 13)), ordered=True
@@ -156,15 +158,17 @@
                     DTindex.weekday, categories=list(range(7)), ordered=True
                 ),
                 'day': DTindex.day,
                 'weekend': (DTindex.weekday > 4).astype(int),
                 'epoch': DTindex.to_julian_date(),
             }
         )
-        date_part_df = pd.get_dummies(date_part_df, columns=['month', 'weekday'])
+        date_part_df = pd.get_dummies(
+            date_part_df, columns=['month', 'weekday'], dtype=float
+        )
     elif method in "expanded_binarized":
         date_part_df = pd.DataFrame(
             {
                 'month': pd.Categorical(
                     DTindex.month, categories=list(range(1, 13)), ordered=True
                 ),
                 'weekday': pd.Categorical(
@@ -180,15 +184,17 @@
                 ),
                 'weekend': (DTindex.weekday > 4).astype(int),
                 'quarter': DTindex.quarter,
                 'epoch': DTindex.to_julian_date(),
             }
         )
         date_part_df = pd.get_dummies(
-            date_part_df, columns=['month', 'weekday', 'day', 'weekdayofmonth']
+            date_part_df,
+            columns=['month', 'weekday', 'day', 'weekdayofmonth'],
+            dtype=float,
         )
     elif method in ["common_fourier", "common_fourier_rw"]:
         seasonal_list = []
         DTmin = DTindex.min()
         DTmax = DTindex.max()
         # 1 time step will always not work with this
         # for new seasonal_ratio, worse case scenario is 2 steps ahead so one season / 2
@@ -320,39 +326,44 @@
             history_days = (DTindex.max() - DTindex.min()).days
         return pd.DataFrame(
             fourier_series(np.asarray(t), seasonality / history_days, n=10)
         ).rename(columns=lambda x: f"seasonality{seasonality}_" + str(x))
     # dateparts
     elif seasonality == "dayofweek":
         return pd.get_dummies(
-            pd.Categorical(DTindex.weekday, categories=list(range(7)), ordered=True)
+            pd.Categorical(DTindex.weekday, categories=list(range(7)), ordered=True),
+            dtype=np.uint8,
         ).rename(columns=lambda x: f"{seasonality}_" + str(x))
     elif seasonality == "month":
         return pd.get_dummies(
-            pd.Categorical(DTindex.month, categories=list(range(1, 13)), ordered=True)
+            pd.Categorical(DTindex.month, categories=list(range(1, 13)), ordered=True),
+            dtype=np.uint8,
         ).rename(columns=lambda x: f"{seasonality}_" + str(x))
     elif seasonality == "weekend":
         return pd.DataFrame((DTindex.weekday > 4).astype(int), columns=["weekend"])
     elif seasonality == "weekdayofmonth":
         return pd.get_dummies(
             pd.Categorical(
                 (DTindex.day - 1) // 7 + 1,
                 categories=list(range(1, 6)),
                 ordered=True,
-            )
+            ),
+            dtype=float,
         ).rename(columns=lambda x: f"{seasonality}_" + str(x))
     elif seasonality == "hour":
         return pd.get_dummies(
-            pd.Categorical(DTindex.hour, categories=list(range(1, 25)), ordered=True)
+            pd.Categorical(DTindex.hour, categories=list(range(1, 25)), ordered=True),
+            dtype=np.uint8,
         ).rename(columns=lambda x: f"{seasonality}_" + str(x))
     elif seasonality == "daysinmonth":
         return pd.DataFrame({'daysinmonth': DTindex.daysinmonth})
     elif seasonality == "quarter":
         return pd.get_dummies(
-            pd.Categorical(DTindex.quarter, categories=list(range(1, 5)), ordered=True)
+            pd.Categorical(DTindex.quarter, categories=list(range(1, 5)), ordered=True),
+            dtype=np.uint8,
         ).rename(columns=lambda x: f"{seasonality}_" + str(x))
     elif seasonality in date_part_methods:
         return date_part(DTindex, method=seasonality, set_index=False)
     else:
         return ValueError(
             f"Seasonality `{seasonality}` not recognized. Must be int, float, or a select type string such as 'dayofweek'"
         )
```

### Comparing `autots-0.5.5/autots/tools/shaping.py` & `autots-0.5.6/autots/tools/shaping.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,22 @@
         DTindex = df_wide.index
     elif isinstance(df_wide, pd.DatetimeIndex):
         DTindex = df_wide
     else:
         raise ValueError(
             "infer_frequency failed due to input not being pandas DF or DT index"
         )
-    frequency = pd.infer_freq(DTindex, warn=True)
+    # 'warn' arg removed in pandas 2.0.0
+    frequency = pd.infer_freq(DTindex)
     if frequency is None:
         # hack to get around data which has a few oddities
-        frequency = pd.infer_freq(DTindex[-10:], warn=True)
+        frequency = pd.infer_freq(DTindex[-10:])
     if frequency is None:
         # hack to get around data which has a few oddities
-        frequency = pd.infer_freq(DTindex[:10], warn=True)
+        frequency = pd.infer_freq(DTindex[:10])
     return frequency
 
 
 def df_cleanup(
     df_wide,
     frequency: str = "infer",
     prefill_na: str = None,
@@ -131,17 +132,15 @@
             other options include "mean" and other numpy functions, beware data *must* already be input as numeric type for these to work.
             if categorical data is provided, `aggfunc='first'` is recommended
     """
     df_long = df.copy()
 
     # Attempt to convert to datetime format if not already
     try:
-        df_long[date_col] = pd.to_datetime(
-            df_long[date_col], infer_datetime_format=True
-        )
+        df_long[date_col] = pd.to_datetime(df_long[date_col])
     except Exception:
         raise ValueError(
             "Could not convert date to datetime format. Incorrect column name or preformat with pandas to_datetime"
         )
 
     # handle no id_col for if only one time series
     if id_col in [None, 'None']:
```

### Comparing `autots-0.5.5/autots/tools/thresholding.py` & `autots-0.5.6/autots/tools/thresholding.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,15 +380,15 @@
         columns=["anomaly"],
     )
     return res, scores
 
 
 """
 df = pd.read_csv(
-    "holidays.csv", index_col=0, parse_dates=[0], infer_datetime_format=True
+    "holidays.csv", index_col=0, parse_dates=[0],
 )
 
 from autots.evaluator.auto_model import back_forecast
 
 backcast = back_forecast(
     df,
     model_name="LastValueNaive",
```

### Comparing `autots-0.5.5/autots/tools/transform.py` & `autots-0.5.6/autots/tools/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -2662,15 +2662,16 @@
         from sklearn.tree import DecisionTreeClassifier
 
         scores_flat = self.scores.melt(var_name='series', value_name="value")
         categor = pd.Categorical(scores_flat['series'])
         self.score_categories = categor.categories
         scores_flat['series'] = categor
         scores_flat = pd.concat(
-            [pd.get_dummies(scores_flat['series']), scores_flat['value']], axis=1
+            [pd.get_dummies(scores_flat['series'], dtype=float), scores_flat['value']],
+            axis=1,
         )
         anomalies_flat = self.anomalies.melt(var_name='series', value_name="value")
         self.anomaly_classifier = DecisionTreeClassifier(max_depth=None).fit(
             scores_flat, anomalies_flat['value']
         )
         # anomaly_classifier.score(scores_flat, anomalies_flat['value'])
 
@@ -2683,15 +2684,19 @@
             id_vars="date", var_name='series', value_name="value"
         )
         scores_flat['series'] = pd.Categorical(
             scores_flat['series'], categories=self.score_categories
         )
         res = self.anomaly_classifier.predict(
             pd.concat(
-                [pd.get_dummies(scores_flat['series']), scores_flat['value']], axis=1
+                [
+                    pd.get_dummies(scores_flat['series'], dtype=float),
+                    scores_flat['value'],
+                ],
+                axis=1,
             )
         )
         res = pd.concat(
             [scores_flat[['date', "series"]], pd.Series(res, name='value')], axis=1
         ).pivot_table(index='date', columns='series', values="value")
         return res[scores.columns]
```

### Comparing `autots-0.5.5/autots/tools/window_functions.py` & `autots-0.5.6/autots/tools/window_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,32 +93,26 @@
             if shuffle:
                 np.random.shuffle(numbers)
 
         X = pd.DataFrame()
         Y = pd.DataFrame()
         for z in numbers:
             if input_dim == 'univariate':
-                rand_slice = df.iloc[
-                    z : (z + phrase_n),
-                ]
+                rand_slice = df.iloc[z : (z + phrase_n),]
                 rand_slice = (
                     rand_slice.reset_index(drop=True)
                     .transpose()
                     .set_index(np.repeat(z, (df.shape[1],)), append=True)
                 )
                 cX = rand_slice.iloc[:, 0:(window_size)]
                 cY = rand_slice.iloc[:, window_size:]
             else:
-                cX = df.iloc[
-                    z : (z + window_size),
-                ]
+                cX = df.iloc[z : (z + window_size),]
                 cX = pd.DataFrame(cX.stack().reset_index(drop=True)).transpose()
-                cY = df.iloc[
-                    (z + window_size) : (z + phrase_n),
-                ]
+                cY = df.iloc[(z + window_size) : (z + phrase_n),]
                 cY = pd.DataFrame(cY.stack().reset_index(drop=True)).transpose()
             X = pd.concat([X, cX], axis=0)
             Y = pd.concat([Y, cY], axis=0)
         if normalize_window:
             X = X.div(X.sum(axis=1), axis=0)
         X.columns = [str(x) for x in range(len(X.columns))]
 
@@ -131,26 +125,22 @@
     input_dim: str = 'univariate',
     normalize_window: bool = False,
 ):
     """Pandas based function to provide the last window of window_maker."""
     z = df.shape[0] - window_size
     shape_1 = df.shape[1] if df.ndim > 1 else 1
     if input_dim == 'univariate':
-        cX = df.iloc[
-            z : (z + window_size),
-        ]
+        cX = df.iloc[z : (z + window_size),]
         cX = (
             cX.reset_index(drop=True)
             .transpose()
             .set_index(np.repeat(z, (shape_1,)), append=True)
         )
     else:
-        cX = df.iloc[
-            z : (z + window_size),
-        ]
+        cX = df.iloc[z : (z + window_size),]
         cX = pd.DataFrame(cX.stack().reset_index(drop=True)).transpose()
     if normalize_window:
         cX = cX.div(cX.sum(axis=1), axis=0)
 
     return cX
```

### Comparing `autots-0.5.5/docs/conf.py` & `autots-0.5.6/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 copyright = u'%s, Colin Catlin' % date.today().year
 author = 'Colin Catlin'
 
 # The full version, including alpha/beta/rc tags
 # import AutoTS
 # from  AutoTS import __version__
 # release = __version__
-release = "0.5.5"
+release = "0.5.6"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 # Add napoleon to the extensions list
```

### Comparing `autots-0.5.5/pyproject.toml` & `autots-0.5.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autots"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
   { name="Colin Catlin", email="colin.catlin@gmail.com" },
 ]
 description = "Automated Time Series Forecasting"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {text = "MIT License"}
```

### Comparing `autots-0.5.5/setup.py` & `autots-0.5.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 }
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AutoTS",
-    version="0.5.5",
+    version="0.5.6",
     author="Colin Catlin",
     author_email="colin.catlin@syllepsis.live",
     description="Automated Time Series Forecasting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/winedarksea/AutoTS",
     packages=setuptools.find_packages(),
```

### Comparing `autots-0.5.5/tests/test_anomalies.py` & `autots-0.5.6/tests/test_anomalies.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/tests/test_autots.py` & `autots-0.5.6/tests/test_autots.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/tests/test_calendar_holiday.py` & `autots-0.5.6/tests/test_calendar_holiday.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/tests/test_cassandra.py` & `autots-0.5.6/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/tests/test_event_forecasting.py` & `autots-0.5.6/tests/test_event_forecasting.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/tests/test_impute.py` & `autots-0.5.6/tests/test_impute.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/tests/test_metrics.py` & `autots-0.5.6/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/tests/test_percentile.py` & `autots-0.5.6/tests/test_percentile.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.5/tests/test_regressor.py` & `autots-0.5.6/tests/test_regressor.py`

 * *Files identical despite different names*


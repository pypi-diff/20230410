# Comparing `tmp/ht_pricing_module-0.1.34.tar.gz` & `tmp/ht_pricing_module-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht_pricing_module-0.1.34.tar", last modified: Thu Apr  6 07:37:07 2023, max compression
+gzip compressed data, was "ht_pricing_module-0.1.35.tar", last modified: Mon Apr 10 00:35:43 2023, max compression
```

## Comparing `ht_pricing_module-0.1.34.tar` & `ht_pricing_module-0.1.35.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.636507 ht_pricing_module-0.1.34/
--rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.1.34/MANIFEST.in
--rw-rw-rw-   0        0        0      264 2023-04-06 07:37:07.635510 ht_pricing_module-0.1.34/PKG-INFO
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.248463 ht_pricing_module-0.1.34/ht_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.1.34/ht_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.279381 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/
--rw-rw-rw-   0        0        0      216 2023-02-17 00:36:34.000000 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/__init__.py
--rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/api.py
--rw-rw-rw-   0        0        0      393 2023-03-23 06:42:27.000000 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/packages.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.287359 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/
--rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.232509 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.319278 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/api/
--rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
--rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/api/http.proto
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.335261 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/protobuf/
--rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
--rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
--rw-rw-rw-   0        0        0    45777 2023-04-03 01:09:32.000000 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/pricer.proto
--rw-rw-rw-   0        0        0     3252 2023-03-20 08:23:43.000000 ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.349224 ht_pricing_module-0.1.34/ht_pricing_module/finite_difference_engine/
--rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/finite_difference_engine/__init__.py
--rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.1.34/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.359224 ht_pricing_module-0.1.34/ht_pricing_module/monte_carlo_engine/
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/monte_carlo_engine/__init__.py
--rw-rw-rw-   0        0        0     3127 2023-03-20 08:34:06.000000 ht_pricing_module-0.1.34/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.373187 ht_pricing_module-0.1.34/ht_pricing_module/multi_asset_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.1.34/ht_pricing_module/multi_asset_pricing_module/__init__.py
--rw-rw-rw-   0        0        0     4419 2023-03-23 01:53:37.000000 ht_pricing_module-0.1.34/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.387149 ht_pricing_module-0.1.34/ht_pricing_module/multi_asset_pricing_module/quotient/
--rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.1.34/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.1.34/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.399118 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/
--rw-rw-rw-   0        0        0      365 2023-03-22 13:14:15.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.477907 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/
--rw-rw-rw-   0        0        0      506 2023-03-22 14:42:29.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
--rw-rw-rw-   0        0        0     4297 2023-03-20 08:02:19.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
--rw-rw-rw-   0        0        0     3465 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
--rw-rw-rw-   0        0        0     4274 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
--rw-rw-rw-   0        0        0     5175 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
--rw-rw-rw-   0        0        0     4452 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4257 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
--rw-rw-rw-   0        0        0     3519 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
--rw-rw-rw-   0        0        0     4506 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4583 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
--rw-rw-rw-   0        0        0     5223 2023-04-03 01:46:37.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.479901 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/airbag/
--rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
--rw-rw-rw-   0        0        0     4012 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.501868 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/asian/
--rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
--rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
--rw-rw-rw-   0        0        0     2354 2023-03-24 08:39:50.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.534779 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/
--rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
--rw-rw-rw-   0        0        0     6176 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
--rw-rw-rw-   0        0        0     5340 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
--rw-rw-rw-   0        0        0     1876 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
--rw-rw-rw-   0        0        0     1797 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
--rw-rw-rw-   0        0        0     4573 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.537771 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/basket/
--rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
--rw-rw-rw-   0        0        0     1131 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
--rw-rw-rw-   0        0        0     2298 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.562704 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/binary/
--rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
--rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
--rw-rw-rw-   0        0        0     2302 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
--rw-rw-rw-   0        0        0     2343 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
--rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.583648 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/forward/
--rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
--rw-rw-rw-   0        0        0      198 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
--rw-rw-rw-   0        0        0     3634 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.595616 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/sharkfin/
--rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
--rw-rw-rw-   0        0        0     2555 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
--rw-rw-rw-   0        0        0     2330 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.603595 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/snowball/
--rw-rw-rw-   0        0        0       37 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
--rw-rw-rw-   0        0        0     7325 2023-02-23 05:31:40.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.614566 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/spread/
--rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
--rw-rw-rw-   0        0        0     2396 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.630523 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/touch/
--rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
--rw-rw-rw-   0        0        0     1656 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
--rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
--rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.633515 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/vanilla/
--rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
--rw-rw-rw-   0        0        0     2260 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
--rw-rw-rw-   0        0        0    43817 2023-04-03 01:07:06.000000 ht_pricing_module-0.1.34/ht_pricing_module/simple_pricer_engine.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:37:07.266414 ht_pricing_module-0.1.34/ht_pricing_module.egg-info/
--rw-rw-rw-   0        0        0      264 2023-04-06 07:37:07.000000 ht_pricing_module-0.1.34/ht_pricing_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4791 2023-04-06 07:37:07.000000 ht_pricing_module-0.1.34/ht_pricing_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 07:37:07.000000 ht_pricing_module-0.1.34/ht_pricing_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-04-06 07:37:07.000000 ht_pricing_module-0.1.34/ht_pricing_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-06 07:37:07.000000 ht_pricing_module-0.1.34/ht_pricing_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 07:37:07.636507 ht_pricing_module-0.1.34/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-04-06 07:36:57.000000 ht_pricing_module-0.1.34/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.864309 ht_pricing_module-0.1.35/
+-rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.1.35/MANIFEST.in
+-rw-rw-rw-   0        0        0      264 2023-04-10 00:35:43.863311 ht_pricing_module-0.1.35/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.503477 ht_pricing_module-0.1.35/ht_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.1.35/ht_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.532510 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/
+-rw-rw-rw-   0        0        0      216 2023-02-17 00:36:34.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/api.py
+-rw-rw-rw-   0        0        0      393 2023-03-23 06:42:27.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/packages.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.542227 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/
+-rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.492476 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.562384 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/api/
+-rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
+-rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/api/http.proto
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.581201 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/protobuf/
+-rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
+-rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
+-rw-rw-rw-   0        0        0    45777 2023-04-03 01:09:32.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/pricer.proto
+-rw-rw-rw-   0        0        0     3252 2023-03-20 08:23:43.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.595197 ht_pricing_module-0.1.35/ht_pricing_module/finite_difference_engine/
+-rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/finite_difference_engine/__init__.py
+-rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.1.35/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.604439 ht_pricing_module-0.1.35/ht_pricing_module/monte_carlo_engine/
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/monte_carlo_engine/__init__.py
+-rw-rw-rw-   0        0        0     3138 2023-04-10 00:30:32.000000 ht_pricing_module-0.1.35/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.606385 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/__init__.py
+-rw-rw-rw-   0        0        0     4419 2023-03-23 01:53:37.000000 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.616492 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/quotient/
+-rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.629662 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/
+-rw-rw-rw-   0        0        0      365 2023-03-22 13:14:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.707738 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/
+-rw-rw-rw-   0        0        0      506 2023-03-22 14:42:29.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     4297 2023-03-20 08:02:19.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3465 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
+-rw-rw-rw-   0        0        0     4274 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
+-rw-rw-rw-   0        0        0     5175 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
+-rw-rw-rw-   0        0        0     4452 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4257 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3519 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
+-rw-rw-rw-   0        0        0     4506 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4583 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
+-rw-rw-rw-   0        0        0     5223 2023-04-03 01:46:37.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.709733 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/airbag/
+-rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
+-rw-rw-rw-   0        0        0     4012 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.731864 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/
+-rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
+-rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
+-rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
+-rw-rw-rw-   0        0        0     2354 2023-03-24 08:39:50.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.772114 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/
+-rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
+-rw-rw-rw-   0        0        0     6176 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
+-rw-rw-rw-   0        0        0     5340 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
+-rw-rw-rw-   0        0        0     1876 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
+-rw-rw-rw-   0        0        0     1797 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     4573 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.775107 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/
+-rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
+-rw-rw-rw-   0        0        0     1131 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
+-rw-rw-rw-   0        0        0     2298 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.800351 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/
+-rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
+-rw-rw-rw-   0        0        0     2302 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
+-rw-rw-rw-   0        0        0     2343 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
+-rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.809358 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/forward/
+-rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
+-rw-rw-rw-   0        0        0     3634 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.812349 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/
+-rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
+-rw-rw-rw-   0        0        0     2555 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
+-rw-rw-rw-   0        0        0     2330 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.824317 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/snowball/
+-rw-rw-rw-   0        0        0       37 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+-rw-rw-rw-   0        0        0     7325 2023-02-23 05:31:40.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.835317 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/
+-rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
+-rw-rw-rw-   0        0        0     2396 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.851344 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/
+-rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
+-rw-rw-rw-   0        0        0     1656 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
+-rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
+-rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.855333 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/
+-rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
+-rw-rw-rw-   0        0        0     2260 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
+-rw-rw-rw-   0        0        0    43817 2023-04-03 01:07:06.000000 ht_pricing_module-0.1.35/ht_pricing_module/simple_pricer_engine.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.520406 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-04-10 00:35:43.000000 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4791 2023-04-10 00:35:43.000000 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 00:35:43.000000 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-04-10 00:35:43.000000 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-10 00:35:43.000000 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 00:35:43.864309 ht_pricing_module-0.1.35/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-04-10 00:18:37.000000 ht_pricing_module-0.1.35/setup.py
```

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/api.py` & `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/api.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto` & `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/api/http.proto` & `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto` & `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto` & `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/protos/pricer.proto` & `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/pricer.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/api_and_utils/utils.py` & `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/utils.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/finite_difference_engine/fd_grid_generator.py` & `ht_pricing_module-0.1.35/ht_pricing_module/finite_difference_engine/fd_grid_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/monte_carlo_engine/mc_path_generator.py` & `ht_pricing_module-0.1.35/ht_pricing_module/monte_carlo_engine/mc_path_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..api_and_utils import np, qmc, warnings, lru_cache, wraps
 
 warnings.filterwarnings('ignore')
 
 
 def mc_np_cache(function):
-    @lru_cache
+    @lru_cache(maxsize=2)
     def cached_wrapper(qmc_flag, antithetic_flag, random_seed, M, drift, volatility, hashable_array):
         return function(qmc_flag, antithetic_flag, random_seed, M, drift, volatility,  np.array(hashable_array))
 
     @wraps(function)
     def wrapper(qmc_flag, antithetic_flag, random_seed, M, drift, volatility, array):
         return cached_wrapper(qmc_flag, antithetic_flag, random_seed, M, drift, volatility, tuple(array))
```

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py` & `ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py` & `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module/simple_pricer_engine.py` & `ht_pricing_module-0.1.35/ht_pricing_module/simple_pricer_engine.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/ht_pricing_module.egg-info/SOURCES.txt` & `ht_pricing_module-0.1.35/ht_pricing_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.34/setup.py` & `ht_pricing_module-0.1.35/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.1.34"
+VERSION = "0.1.35"
 
 
 def filter_package():
     packages = []
     packages_all = find_packages()
     for i in packages_all:
         if i.split(".")[0] == 'ht_pricing_module':
```


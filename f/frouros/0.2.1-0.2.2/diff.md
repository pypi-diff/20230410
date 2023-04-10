# Comparing `tmp/frouros-0.2.1.tar.gz` & `tmp/frouros-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.2.1.tar", last modified: Fri Mar 17 19:11:07 2023, max compression
+gzip compressed data, was "frouros-0.2.2.tar", last modified: Mon Apr 10 10:18:37 2023, max compression
```

## Comparing `frouros-0.2.1.tar` & `frouros-0.2.2.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.400397 frouros-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-03-17 19:10:52.000000 frouros-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-17 19:10:52.000000 frouros-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-03-17 19:11:07.400397 frouros-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-03-17 19:10:52.000000 frouros-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.388396 frouros-0.2.1/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.388396 frouros-0.2.1/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.392396 frouros-0.2.1/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/callbacks/batch/reset_drift.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.392396 frouros-0.2.1/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.392396 frouros-0.2.1/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.392396 frouros-0.2.1/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.392396 frouros-0.2.1/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.392396 frouros-0.2.1/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.392396 frouros-0.2.1/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.392396 frouros-0.2.1/frouros/detectors/concept_drift/streaming/cusum_based/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/cusum_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.396396 frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10776 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4794 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12400 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23064 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.396396 frouros-0.2.1/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/concept_drift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.396396 frouros-0.2.1/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.396396 frouros-0.2.1/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.396396 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8677 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/histogram_intersection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     3468 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.400397 frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.400397 frouros-0.2.1/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.400397 frouros-0.2.1/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7249 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.400397 frouros-0.2.1/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.400397 frouros-0.2.1/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.400397 frouros-0.2.1/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6497 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    10766 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.400397 frouros-0.2.1/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.400397 frouros-0.2.1/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.400397 frouros-0.2.1/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21066 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     6157 2023-03-17 19:10:52.000000 frouros-0.2.1/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 19:11:07.388396 frouros-0.2.1/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-03-17 19:11:06.000000 frouros-0.2.1/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4397 2023-03-17 19:11:07.000000 frouros-0.2.1/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 19:11:06.000000 frouros-0.2.1/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 19:11:06.000000 frouros-0.2.1/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-03-17 19:11:07.000000 frouros-0.2.1/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-03-17 19:11:07.000000 frouros-0.2.1/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-03-17 19:10:52.000000 frouros-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-17 19:11:07.404397 frouros-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-03-17 19:10:52.000000 frouros-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.900965 frouros-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-04-10 10:18:18.000000 frouros-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-10 10:18:18.000000 frouros-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-10 10:18:37.900965 frouros-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-04-10 10:18:18.000000 frouros-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.884965 frouros-0.2.2/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/batch/reset_drift.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10776 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4794 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12400 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23064 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6426 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8762 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8221 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7249 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.900965 frouros-0.2.2/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6499 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12399 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.900965 frouros-0.2.2/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.900965 frouros-0.2.2/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.900965 frouros-0.2.2/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21066 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6157 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.884965 frouros-0.2.2/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4399 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-04-10 10:18:18.000000 frouros-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 10:18:37.900965 frouros-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-04-10 10:18:18.000000 frouros-0.2.2/setup.py
```

### Comparing `frouros-0.2.1/LICENSE` & `frouros-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/PKG-INFO` & `frouros-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python library for drift detection in Machine Learning problems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.2.1 Summary: A Python library
+Metadata-Version: 2.1 Name: frouros Version: 0.2.2 Summary: A Python library
 for drift detection in Machine Learning problems Home-page: https://github.com/
 IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
```

### Comparing `frouros-0.2.1/README.md` & `frouros-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/callbacks/base.py` & `frouros-0.2.2/frouros/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/callbacks/batch/base.py` & `frouros-0.2.2/frouros/callbacks/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/callbacks/batch/permutation_test.py` & `frouros-0.2.2/frouros/callbacks/batch/permutation_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/callbacks/batch/reset_drift.py` & `frouros-0.2.2/frouros/callbacks/batch/reset_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/callbacks/streaming/base.py` & `frouros-0.2.2/frouros/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/callbacks/streaming/history.py` & `frouros-0.2.2/frouros/callbacks/streaming/history.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.2.2/frouros/callbacks/streaming/warning_samples.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/datasets/base.py` & `frouros-0.2.2/frouros/datasets/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/datasets/real.py` & `frouros-0.2.2/frouros/datasets/real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/datasets/synthetic.py` & `frouros-0.2.2/frouros/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/base.py` & `frouros-0.2.2/frouros/detectors/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/__init__.py` & `frouros-0.2.2/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/base.py` & `frouros-0.2.2/frouros/detectors/concept_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/cusum_based/base.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/base.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/base.py` & `frouros-0.2.2/frouros/detectors/data_drift/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,26 +171,26 @@
         :param value: value to be set
         :type value: Optional[numpy.ndarray]
         """
         if value is not None:
             self._check_array(X=value)
         self._X_ref = value
 
-    def fit(self, X: np.ndarray) -> Dict[str, Any]:  # noqa: N803
+    def fit(self, X: np.ndarray, **kwargs) -> Dict[str, Any]:  # noqa: N803
         """Fit detector.
 
         :param X: feature data
         :type X: numpy.ndarray
         :return: callbacks logs
         :rtype: Dict[str, Any]
         """
         self._check_fit_dimensions(X=X)
         for callback in self.callbacks:  # type: ignore
             callback.on_fit_start()
-        self._fit(X=X)
+        self._fit(X=X, **kwargs)
         for callback in self.callbacks:  # type: ignore
             callback.on_fit_end()
 
         logs = self._get_callbacks_logs()
         return logs
 
     def reset(self) -> None:
```

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Data drift batch detection methods init."""
 
 from .distance_based import (
     BhattacharyyaDistance,
     EMD,
     HellingerDistance,
-    HistogramIntersection,
+    HINormalizedComplement,
     JS,
     KL,
     PSI,
     MMD,
 )
 from .statistical_test import (
     ChiSquareTest,
@@ -19,15 +19,15 @@
 
 __all__ = [
     "BhattacharyyaDistance",
     "ChiSquareTest",
     "CVMTest",
     "EMD",
     "HellingerDistance",
-    "HistogramIntersection",
+    "HINormalizedComplement",
     "JS",
     "KL",
     "KSTest",
     "PSI",
     "MMD",
     "WelchTTest",
 ]
```

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/base.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,14 +104,15 @@
         return distance  # type: ignore
 
     @abc.abstractmethod
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
+        **kwargs,
     ) -> DistanceResult:
         pass
 
 
 class DistanceBinsBasedBase(DistanceBasedBase):
     """Abstract class representing a distance bins based detector."""
 
@@ -162,14 +163,15 @@
             raise ValueError("value must be greater than 0.")
         self._num_bins = value
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
+        **kwargs,
     ) -> DistanceResult:
         distance_bins = self._distance_measure_bins(X_ref=X_ref, X=X)
         distance = DistanceResult(distance=distance_bins)
         return distance
 
     @staticmethod
     def _calculate_bins_values(
@@ -182,15 +184,17 @@
             np.histogram(a=X_ref, bins=bins)[0] / X_ref.shape[0]
         )  # noqa: N806
         X_percents = np.histogram(a=X, bins=bins)[0] / X.shape[0]  # noqa: N806
         return X_ref_percents, X_percents
 
     @abc.abstractmethod
     def _distance_measure_bins(
-        self, X_ref: np.ndarray, X: np.ndarray  # noqa: N803
+        self,
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,  # noqa: N803
     ) -> float:
         pass
 
 
 class DistanceProbabilityBasedBase(DistanceBasedBase):
     """Abstract class representing a distance probability based detector."""
 
@@ -242,14 +246,15 @@
         self._num_bins = value
 
     @abc.abstractmethod
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
+        **kwargs,
     ) -> DistanceResult:
         pass
 
     @staticmethod
     def _calculate_probabilities(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
```

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         )
         self.kwargs = kwargs
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
+        **kwargs,
     ) -> DistanceResult:
         emd = self._emd(X=X_ref, Y=X, **self.kwargs)
         distance = DistanceResult(distance=emd)
         return distance
 
     @staticmethod
     def _emd(X: np.ndarray, Y: np.ndarray, **kwargs) -> float:  # noqa: N803
```

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/histogram_intersection.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Histogram intersection module."""
+"""HI (Histogram intersection) normalized complement module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
 from frouros.callbacks import Callback
 from frouros.detectors.data_drift.batch.distance_based.base import (
     DistanceBinsBasedBase,
 )
 
 
-class HistogramIntersection(DistanceBinsBasedBase):
-    """Histogram intersection [swain1991color]_ detector.
+class HINormalizedComplement(DistanceBinsBasedBase):
+    """HI (Histogram intersection) normalized complement [swain1991color]_ detector.
 
     :References:
 
     .. [swain1991color] Swain, M. J., and D. H. Ballard.
         "Color Indexing International Journal of Computer
         Vision 7." (1991): 11-32.
     """
@@ -29,34 +29,34 @@
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
         :type callbacks: Optional[Union[Callback, List[Callback]]]
         """
         super().__init__(
-            statistical_method=self._histogram_intersection,
+            statistical_method=self._hi_normalized_complement,
             statistical_kwargs={
                 "num_bins": num_bins,
             },
             callbacks=callbacks,
         )
         self.num_bins = num_bins
 
     def _distance_measure_bins(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
     ) -> float:
-        no_intersection = self._histogram_intersection(
+        intersection_normalized_complement = self._hi_normalized_complement(
             X=X_ref, Y=X, num_bins=self.num_bins
         )
-        return no_intersection
+        return intersection_normalized_complement
 
     @staticmethod
-    def _histogram_intersection(
+    def _hi_normalized_complement(
         X: np.ndarray,  # noqa: N803
         Y: np.ndarray,
         *,
         num_bins: int,
     ) -> float:
         hist_range = (
             np.min([np.min(X), np.min(Y)]),
@@ -64,10 +64,10 @@
         )
         X_hist, _ = np.histogram(  # noqa: N806
             X, bins=num_bins, range=hist_range  # noqa: N806
         )
         X_hist = X_hist / X.shape[0]  # noqa: N806
         Y_hist, _ = np.histogram(Y, bins=num_bins, range=hist_range)  # noqa: N806
         Y_hist = Y_hist / Y.shape[0]  # noqa: N806
-        no_intersection = 1 - np.sum(np.minimum(X_hist, Y_hist))
+        intersection_normalized_complement = 1 - np.sum(np.minimum(X_hist, Y_hist))
 
-        return no_intersection
+        return intersection_normalized_complement
```

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         IEEE Transactions on Information theory 37.1 (1991): 145-151.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
         callbacks: Optional[Union[Callback, List[Callback]]] = None,
-        **kwargs
+        **kwargs,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
         :type callbacks: Optional[Union[Callback, List[Callback]]]
@@ -46,26 +46,27 @@
         self.num_bins = num_bins
         self.kwargs = kwargs
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
+        **kwargs,
     ) -> DistanceResult:
         js = self._js(X=X_ref, Y=X, num_bins=self.num_bins, **self.kwargs)
         distance = DistanceResult(distance=js)
         return distance
 
     @staticmethod
     def _js(
         X: np.ndarray,  # noqa: N803
         Y: np.ndarray,
         *,
         num_bins: int,
-        **kwargs: Dict[str, Any]
+        **kwargs: Dict[str, Any],
     ) -> float:
         (  # noqa: N806
             X_ref_rvs,
             X_rvs,
         ) = DistanceProbabilityBasedBase._calculate_probabilities(
             X_ref=X,
             X=Y,
```

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         self.num_bins = num_bins
         self.kwargs = kwargs
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
+        **kwargs,
     ) -> DistanceResult:
         kl = self._kl(X=X_ref, Y=X, num_bins=self.num_bins, **self.kwargs)
         distance = DistanceResult(distance=kl)
         return distance
 
     @staticmethod
     def _kl(
```

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.2.2/frouros/detectors/data_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/metrics/base.py` & `frouros-0.2.2/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/metrics/prequential_error.py` & `frouros-0.2.2/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/tests/conftest.py` & `frouros-0.2.2/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/tests/integration/test_callback.py` & `frouros-0.2.2/frouros/tests/integration/test_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from frouros.detectors.concept_drift.base import ConceptDriftBase
 from frouros.detectors.concept_drift.streaming.ddm_based.base import DDMBased
 from frouros.detectors.data_drift.batch import (
     BhattacharyyaDistance,
     CVMTest,
     EMD,
     HellingerDistance,
-    HistogramIntersection,
+    HINormalizedComplement,
     JS,
     KL,
     KSTest,
     MMD,
     PSI,
     WelchTTest,
 )
@@ -48,15 +48,15 @@
 
 @pytest.mark.parametrize(
     "detector, expected_distance, expected_p_value",
     [
         (BhattacharyyaDistance, 0.55516059, 0.0),
         (EMD, 3.85346006, 0.0),
         (HellingerDistance, 0.74509099, 0.0),
-        (HistogramIntersection, 0.78, 0.0),
+        (HINormalizedComplement, 0.78, 0.0),
         (JS, 0.67010107, 0.0),
         (KL, np.inf, 0.0),
         (MMD, 0.71529206, 0.0),
         (PSI, 461.20379435, 0.0),
     ],
 )
 def test_batch_permutation_test_data_univariate_different_distribution(
```

### Comparing `frouros-0.2.1/frouros/tests/integration/test_concept_drift.py` & `frouros-0.2.2/frouros/tests/integration/test_concept_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/tests/integration/test_data_drift.py` & `frouros-0.2.2/frouros/tests/integration/test_data_drift.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Test data drift detectors."""
 
-from typing import Tuple
+from typing import Tuple, Union
 
 import pytest  # type: ignore
 import numpy as np  # type: ignore
 
 from frouros.detectors.data_drift.batch.base import DataDriftBatchBase
 from frouros.detectors.data_drift.batch import (
     BhattacharyyaDistance,
     EMD,
     HellingerDistance,
-    HistogramIntersection,
+    HINormalizedComplement,
     PSI,
     JS,
     KL,
     MMD,
 )
 from frouros.detectors.data_drift.batch import (
     ChiSquareTest,
@@ -57,15 +57,15 @@
 
 @pytest.mark.parametrize(
     "detector, expected_distance",
     [
         (EMD(), 3.85346006),
         (JS(), 0.67010107),
         (KL(), np.inf),
-        (HistogramIntersection(), 0.78),
+        (HINormalizedComplement(), 0.78),
     ],
 )
 def test_batch_distance_based_univariate(
     X_ref_univariate: np.ndarray,  # noqa: N803
     X_test_univariate: np.ndarray,  # noqa: N803
     detector: DataDriftBatchBase,
     expected_distance: float,
@@ -240,14 +240,64 @@
     _ = detector.fit(X=X_ref)
     statistic, _ = detector.compare(X=X_test)
 
     assert np.isclose(statistic, expected_distance)
 
 
 @pytest.mark.parametrize(
+    "detector, expected_distance",
+    [(MMD(chunk_size=10), 0.12183835), (MMD(chunk_size=None), 0.12183835)],
+)
+def test_batch_distance_based_chunk_size_valid(
+    X_ref_multivariate: np.ndarray,  # noqa: N803
+    X_test_multivariate: np.ndarray,  # noqa: N803
+    detector: DataDriftBatchBase,
+    expected_distance: float,
+) -> None:
+    """Test batch distance based chunk size valid method.
+
+    :param X_ref_multivariate: reference multivariate data
+    :type X_ref_multivariate: numpy.ndarray
+    :param X_test_multivariate: test multivariate data
+    :type X_test_multivariate: numpy.ndarray
+    :param detector: detector test
+    :type detector: DataDriftBatchBase
+    :param expected_distance: expected distance value
+    :type expected_distance: float
+    """
+    _ = detector.fit(X=X_ref_multivariate)
+    statistic, _ = detector.compare(X=X_test_multivariate)
+
+    assert np.isclose(statistic, expected_distance)
+
+
+@pytest.mark.parametrize(
+    "chunk_size, expected_exception",
+    [
+        (1.5, TypeError),
+        ("10", TypeError),
+        (-1, ValueError),
+    ],
+)
+def test_batch_distance_based_chunk_size_invalid(
+    chunk_size: Union[int, float, str],
+    expected_exception: Union[TypeError, ValueError],
+) -> None:
+    """Test batch distance based chunk size invalid method.
+
+    :param chunk_size: chunk size
+    :type chunk_size: Union[int, float, str]
+    :param expected_exception: expected exception
+    :type expected_exception: Union[TypeError, ValueError]
+    """
+    with pytest.raises(expected_exception):
+        _ = MMD(chunk_size=chunk_size)  # type: ignore
+
+
+@pytest.mark.parametrize(
     "detector, expected_statistic, expected_p_value",
     [
         (IncrementalKSTest(), 0.27, 0.46046910),
     ],
 )
 def test_streaming_statistical_univariate_same_distribution(
     univariate_distribution_p: Tuple[float, float],
```

### Comparing `frouros-0.2.1/frouros/tests/integration/test_real.py` & `frouros-0.2.2/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/tests/integration/test_synthetic.py` & `frouros-0.2.2/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.2.2/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/utils/data_structures.py` & `frouros-0.2.2/frouros/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/utils/decorators.py` & `frouros-0.2.2/frouros/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros/utils/stats.py` & `frouros-0.2.2/frouros/utils/stats.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.1/frouros.egg-info/PKG-INFO` & `frouros-0.2.2/frouros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python library for drift detection in Machine Learning problems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.2.1 Summary: A Python library
+Metadata-Version: 2.1 Name: frouros Version: 0.2.2 Summary: A Python library
 for drift detection in Machine Learning problems Home-page: https://github.com/
 IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
```

### Comparing `frouros-0.2.1/frouros.egg-info/SOURCES.txt` & `frouros-0.2.2/frouros.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 frouros/detectors/data_drift/batch/__init__.py
 frouros/detectors/data_drift/batch/base.py
 frouros/detectors/data_drift/batch/distance_based/__init__.py
 frouros/detectors/data_drift/batch/distance_based/base.py
 frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
 frouros/detectors/data_drift/batch/distance_based/emd.py
 frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
-frouros/detectors/data_drift/batch/distance_based/histogram_intersection.py
+frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
 frouros/detectors/data_drift/batch/distance_based/js.py
 frouros/detectors/data_drift/batch/distance_based/kl.py
 frouros/detectors/data_drift/batch/distance_based/mmd.py
 frouros/detectors/data_drift/batch/distance_based/psi.py
 frouros/detectors/data_drift/batch/statistical_test/__init__.py
 frouros/detectors/data_drift/batch/statistical_test/base.py
 frouros/detectors/data_drift/batch/statistical_test/chisquare.py
```

### Comparing `frouros-0.2.1/pyproject.toml` & `frouros-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frouros"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Python library for drift detection in Machine Learning problems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
```

### Comparing `frouros-0.2.1/setup.py` & `frouros-0.2.2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/AttentionMOI-0.0.2.tar.gz` & `tmp/AttentionMOI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AttentionMOI-0.0.2.tar", last modified: Fri Mar 24 10:46:43 2023, max compression
+gzip compressed data, was "AttentionMOI-0.0.3.tar", last modified: Mon Apr 10 09:12:41 2023, max compression
```

## Comparing `AttentionMOI-0.0.2.tar` & `AttentionMOI-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 10:46:43.138004 AttentionMOI-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-03-24 10:46:42.937583 AttentionMOI-0.0.2/AttentionMOI/
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/__init__.py
--rw-rw-rw-   0        0        0     2673 2023-03-24 10:35:08.000000 AttentionMOI-0.0.2/AttentionMOI/deepmoi.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:46:42.990090 AttentionMOI-0.0.2/AttentionMOI/example/
--rw-rw-rw-   0        0        0     7419 2022-08-26 01:04:12.000000 AttentionMOI-0.0.2/AttentionMOI/example/cnv.csv.gz
--rw-rw-rw-   0        0        0    13651 2022-08-26 01:04:12.000000 AttentionMOI-0.0.2/AttentionMOI/example/label.csv
--rw-rw-rw-   0        0        0    77257 2022-08-26 01:04:12.000000 AttentionMOI-0.0.2/AttentionMOI/example/met.csv.gz
--rw-rw-rw-   0        0        0   118903 2022-08-26 01:04:12.000000 AttentionMOI-0.0.2/AttentionMOI/example/rna.csv.gz
-drwxrwxrwx   0        0        0        0 2023-03-24 10:46:43.035077 AttentionMOI-0.0.2/AttentionMOI/src/
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/src/__init__.py
--rw-rw-rw-   0        0        0      488 2022-11-07 18:45:20.000000 AttentionMOI-0.0.2/AttentionMOI/src/explain.py
--rw-rw-rw-   0        0        0     2944 2022-11-07 18:45:20.000000 AttentionMOI-0.0.2/AttentionMOI/src/feature_selection.py
--rw-rw-rw-   0        0        0     7108 2022-11-24 00:13:04.000000 AttentionMOI-0.0.2/AttentionMOI/src/fsd.py
--rw-rw-rw-   0        0        0     1962 2023-03-24 06:27:29.000000 AttentionMOI-0.0.2/AttentionMOI/src/main.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:46:43.052064 AttentionMOI-0.0.2/AttentionMOI/src/moanna/
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/__init__.py
--rw-rw-rw-   0        0        0       22 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/__meta__.py
--rw-rw-rw-   0        0        0     2734 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:46:43.076111 AttentionMOI-0.0.2/AttentionMOI/src/moanna/helper/
--rw-rw-rw-   0        0        0     3501 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/helper/ClusteringMetricsHelper.py
--rw-rw-rw-   0        0        0    21017 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/helper/DataCleanUpFunctions.py
--rw-rw-rw-   0        0        0     2994 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/helper/SurvivalHelperFunctions.py
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/helper/__init__.py
--rw-rw-rw-   0        0        0     7542 2023-03-23 07:59:37.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/main.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:46:43.096731 AttentionMOI-0.0.2/AttentionMOI/src/moanna/model/
--rw-rw-rw-   0        0        0     6780 2023-03-24 08:37:52.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/model/Autoencoder.py
--rw-rw-rw-   0        0        0     5066 2023-03-23 06:48:20.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/model/ClassificationModel.py
--rw-rw-rw-   0        0        0     1458 2023-03-23 09:16:06.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/model/Moanna.py
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/src/moanna/model/__init__.py
--rw-rw-rw-   0        0        0     3439 2022-11-07 18:45:20.000000 AttentionMOI-0.0.2/AttentionMOI/src/module.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:46:43.130025 AttentionMOI-0.0.2/AttentionMOI/src/mogonet/
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.2/AttentionMOI/src/mogonet/__init__.py
--rw-rw-rw-   0        0        0     3753 2021-03-31 20:51:34.000000 AttentionMOI-0.0.2/AttentionMOI/src/mogonet/feat_importance.py
--rw-rw-rw-   0        0        0      675 2021-03-31 20:51:34.000000 AttentionMOI-0.0.2/AttentionMOI/src/mogonet/main_biomarker.py
--rw-rw-rw-   0        0        0     1150 2023-03-24 07:18:32.000000 AttentionMOI-0.0.2/AttentionMOI/src/mogonet/main_mogonet.py
--rw-rw-rw-   0        0        0     3711 2021-03-31 20:51:34.000000 AttentionMOI-0.0.2/AttentionMOI/src/mogonet/models.py
--rw-rw-rw-   0        0        0     9308 2023-03-24 10:46:36.000000 AttentionMOI-0.0.2/AttentionMOI/src/mogonet/train_test.py
--rw-rw-rw-   0        0        0     4594 2023-03-24 05:54:54.000000 AttentionMOI-0.0.2/AttentionMOI/src/mogonet/utils.py
--rw-rw-rw-   0        0        0     7379 2022-11-23 23:48:44.000000 AttentionMOI-0.0.2/AttentionMOI/src/prediction.py
--rw-rw-rw-   0        0        0     2164 2022-11-07 18:45:20.000000 AttentionMOI-0.0.2/AttentionMOI/src/preprocess.py
--rw-rw-rw-   0        0        0    23921 2023-03-24 10:44:22.000000 AttentionMOI-0.0.2/AttentionMOI/src/train.py
--rw-rw-rw-   0        0        0     9205 2022-11-07 18:45:20.000000 AttentionMOI-0.0.2/AttentionMOI/src/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:46:42.970525 AttentionMOI-0.0.2/AttentionMOI.egg-info/
--rw-rw-rw-   0        0        0      391 2023-03-24 10:46:41.000000 AttentionMOI-0.0.2/AttentionMOI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1507 2023-03-24 10:46:42.000000 AttentionMOI-0.0.2/AttentionMOI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 10:46:41.000000 AttentionMOI-0.0.2/AttentionMOI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-03-24 10:46:42.000000 AttentionMOI-0.0.2/AttentionMOI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      203 2023-03-24 10:46:42.000000 AttentionMOI-0.0.2/AttentionMOI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-24 10:46:42.000000 AttentionMOI-0.0.2/AttentionMOI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2023-03-16 08:33:55.000000 AttentionMOI-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      391 2023-03-24 10:46:43.136560 AttentionMOI-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2216 2023-03-24 09:41:22.000000 AttentionMOI-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-24 10:46:43.138004 AttentionMOI-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1363 2023-03-24 10:36:09.000000 AttentionMOI-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:12:41.255468 AttentionMOI-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-04-10 09:12:41.036476 AttentionMOI-0.0.3/AttentionMOI/
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/__init__.py
+-rw-rw-rw-   0        0        0     2673 2023-03-24 10:35:08.000000 AttentionMOI-0.0.3/AttentionMOI/deepmoi.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:12:41.088444 AttentionMOI-0.0.3/AttentionMOI/example/
+-rw-rw-rw-   0        0        0     7419 2022-08-26 01:04:12.000000 AttentionMOI-0.0.3/AttentionMOI/example/cnv.csv.gz
+-rw-rw-rw-   0        0        0    13651 2022-08-26 01:04:12.000000 AttentionMOI-0.0.3/AttentionMOI/example/label.csv
+-rw-rw-rw-   0        0        0    77257 2022-08-26 01:04:12.000000 AttentionMOI-0.0.3/AttentionMOI/example/met.csv.gz
+-rw-rw-rw-   0        0        0   118903 2022-08-26 01:04:12.000000 AttentionMOI-0.0.3/AttentionMOI/example/rna.csv.gz
+drwxrwxrwx   0        0        0        0 2023-04-10 09:12:41.139605 AttentionMOI-0.0.3/AttentionMOI/src/
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/src/__init__.py
+-rw-rw-rw-   0        0        0      488 2022-11-07 18:45:20.000000 AttentionMOI-0.0.3/AttentionMOI/src/explain.py
+-rw-rw-rw-   0        0        0     2944 2022-11-07 18:45:20.000000 AttentionMOI-0.0.3/AttentionMOI/src/feature_selection.py
+-rw-rw-rw-   0        0        0     7085 2023-03-24 10:49:51.000000 AttentionMOI-0.0.3/AttentionMOI/src/fsd.py
+-rw-rw-rw-   0        0        0     1962 2023-03-24 06:27:29.000000 AttentionMOI-0.0.3/AttentionMOI/src/main.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:12:41.161484 AttentionMOI-0.0.3/AttentionMOI/src/moanna/
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/__init__.py
+-rw-rw-rw-   0        0        0       22 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/__meta__.py
+-rw-rw-rw-   0        0        0     2734 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:12:41.183494 AttentionMOI-0.0.3/AttentionMOI/src/moanna/helper/
+-rw-rw-rw-   0        0        0     3501 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/helper/ClusteringMetricsHelper.py
+-rw-rw-rw-   0        0        0    21017 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/helper/DataCleanUpFunctions.py
+-rw-rw-rw-   0        0        0     2994 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/helper/SurvivalHelperFunctions.py
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/helper/__init__.py
+-rw-rw-rw-   0        0        0     7542 2023-03-23 07:59:37.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/main.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:12:41.211737 AttentionMOI-0.0.3/AttentionMOI/src/moanna/model/
+-rw-rw-rw-   0        0        0     6780 2023-03-24 08:37:52.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/model/Autoencoder.py
+-rw-rw-rw-   0        0        0     5066 2023-03-23 06:48:20.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/model/ClassificationModel.py
+-rw-rw-rw-   0        0        0     1458 2023-03-23 09:16:06.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/model/Moanna.py
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/src/moanna/model/__init__.py
+-rw-rw-rw-   0        0        0     3439 2022-11-07 18:45:20.000000 AttentionMOI-0.0.3/AttentionMOI/src/module.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:12:41.251361 AttentionMOI-0.0.3/AttentionMOI/src/mogonet/
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.3/AttentionMOI/src/mogonet/__init__.py
+-rw-rw-rw-   0        0        0     3753 2021-03-31 20:51:34.000000 AttentionMOI-0.0.3/AttentionMOI/src/mogonet/feat_importance.py
+-rw-rw-rw-   0        0        0      675 2021-03-31 20:51:34.000000 AttentionMOI-0.0.3/AttentionMOI/src/mogonet/main_biomarker.py
+-rw-rw-rw-   0        0        0     1150 2023-03-24 07:18:32.000000 AttentionMOI-0.0.3/AttentionMOI/src/mogonet/main_mogonet.py
+-rw-rw-rw-   0        0        0     3711 2021-03-31 20:51:34.000000 AttentionMOI-0.0.3/AttentionMOI/src/mogonet/models.py
+-rw-rw-rw-   0        0        0     9308 2023-03-24 10:46:36.000000 AttentionMOI-0.0.3/AttentionMOI/src/mogonet/train_test.py
+-rw-rw-rw-   0        0        0     4594 2023-03-24 05:54:54.000000 AttentionMOI-0.0.3/AttentionMOI/src/mogonet/utils.py
+-rw-rw-rw-   0        0        0     7379 2022-11-23 23:48:44.000000 AttentionMOI-0.0.3/AttentionMOI/src/prediction.py
+-rw-rw-rw-   0        0        0     2164 2022-11-07 18:45:20.000000 AttentionMOI-0.0.3/AttentionMOI/src/preprocess.py
+-rw-rw-rw-   0        0        0    23921 2023-03-24 10:44:22.000000 AttentionMOI-0.0.3/AttentionMOI/src/train.py
+-rw-rw-rw-   0        0        0     9205 2022-11-07 18:45:20.000000 AttentionMOI-0.0.3/AttentionMOI/src/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:12:41.068500 AttentionMOI-0.0.3/AttentionMOI.egg-info/
+-rw-rw-rw-   0        0        0      391 2023-04-10 09:12:40.000000 AttentionMOI-0.0.3/AttentionMOI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1507 2023-04-10 09:12:40.000000 AttentionMOI-0.0.3/AttentionMOI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       62 2023-04-10 09:12:40.000000 AttentionMOI-0.0.3/AttentionMOI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-10 09:12:40.000000 AttentionMOI-0.0.3/AttentionMOI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      227 2023-04-10 09:12:40.000000 AttentionMOI-0.0.3/AttentionMOI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 09:12:40.000000 AttentionMOI-0.0.3/AttentionMOI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2023-03-16 08:33:55.000000 AttentionMOI-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      391 2023-04-10 09:12:41.254364 AttentionMOI-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2216 2023-03-24 09:41:22.000000 AttentionMOI-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 09:12:41.256435 AttentionMOI-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1526 2023-04-10 09:12:32.000000 AttentionMOI-0.0.3/setup.py
```

### Comparing `AttentionMOI-0.0.2/AttentionMOI/deepmoi.py` & `AttentionMOI-0.0.3/AttentionMOI/deepmoi.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/example/cnv.csv.gz` & `AttentionMOI-0.0.3/AttentionMOI/example/cnv.csv.gz`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/example/label.csv` & `AttentionMOI-0.0.3/AttentionMOI/example/label.csv`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/example/met.csv.gz` & `AttentionMOI-0.0.3/AttentionMOI/example/met.csv.gz`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/example/rna.csv.gz` & `AttentionMOI-0.0.3/AttentionMOI/example/rna.csv.gz`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/feature_selection.py` & `AttentionMOI-0.0.3/AttentionMOI/src/feature_selection.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/fsd.py` & `AttentionMOI-0.0.3/AttentionMOI/src/fsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,16 +132,14 @@
     data = np.nan_to_num(data)
     data = data.astype('float32')
     if data.shape[1] == 0:
         print(
             'Program terminated! The reason is that no features passed the feature filter. Please check the data or adjust the feature selection parameters.')
         sys.exit(1)
 
-    print(data.shape)
-
     # 6. return dataset
     return data, chosen_feat_name, chosen_omic_group, labels
 
 
 def feature_selection(args, df_omic, label):
     """
     select feature according to specific method -- (ANOVA, RFE, LASSO, PCA)
```

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/main.py` & `AttentionMOI-0.0.3/AttentionMOI/src/main.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/moanna/cli.py` & `AttentionMOI-0.0.3/AttentionMOI/src/moanna/cli.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/moanna/helper/ClusteringMetricsHelper.py` & `AttentionMOI-0.0.3/AttentionMOI/src/moanna/helper/ClusteringMetricsHelper.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/moanna/helper/DataCleanUpFunctions.py` & `AttentionMOI-0.0.3/AttentionMOI/src/moanna/helper/DataCleanUpFunctions.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/moanna/helper/SurvivalHelperFunctions.py` & `AttentionMOI-0.0.3/AttentionMOI/src/moanna/helper/SurvivalHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/moanna/main.py` & `AttentionMOI-0.0.3/AttentionMOI/src/moanna/main.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/moanna/model/Autoencoder.py` & `AttentionMOI-0.0.3/AttentionMOI/src/moanna/model/Autoencoder.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/moanna/model/ClassificationModel.py` & `AttentionMOI-0.0.3/AttentionMOI/src/moanna/model/ClassificationModel.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/moanna/model/Moanna.py` & `AttentionMOI-0.0.3/AttentionMOI/src/moanna/model/Moanna.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/module.py` & `AttentionMOI-0.0.3/AttentionMOI/src/module.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/mogonet/feat_importance.py` & `AttentionMOI-0.0.3/AttentionMOI/src/mogonet/feat_importance.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/mogonet/main_biomarker.py` & `AttentionMOI-0.0.3/AttentionMOI/src/mogonet/main_biomarker.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/mogonet/main_mogonet.py` & `AttentionMOI-0.0.3/AttentionMOI/src/mogonet/main_mogonet.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/mogonet/models.py` & `AttentionMOI-0.0.3/AttentionMOI/src/mogonet/models.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/mogonet/train_test.py` & `AttentionMOI-0.0.3/AttentionMOI/src/mogonet/train_test.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/mogonet/utils.py` & `AttentionMOI-0.0.3/AttentionMOI/src/mogonet/utils.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/prediction.py` & `AttentionMOI-0.0.3/AttentionMOI/src/prediction.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/preprocess.py` & `AttentionMOI-0.0.3/AttentionMOI/src/preprocess.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/train.py` & `AttentionMOI-0.0.3/AttentionMOI/src/train.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI/src/utils.py` & `AttentionMOI-0.0.3/AttentionMOI/src/utils.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/AttentionMOI.egg-info/SOURCES.txt` & `AttentionMOI-0.0.3/AttentionMOI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/LICENSE` & `AttentionMOI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/README.md` & `AttentionMOI-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.2/setup.py` & `AttentionMOI-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,46 +5,52 @@
     'captum==0.4.1',
     'mygene==3.2.2',
     'openpyxl==3.0.9',
     'packaging==21.3',
     'pandas==1.2.5',
     'pandocfilters==1.5.0',
     'seaborn==0.11.2',
-    'torch==1.13.1',
+    'torch==1.13.1+cpu',
     'scikit-learn==1.2.2',
     'numpy==1.23.5',
     'matplotlib==3.6.2',
+    'xgboost==1.7.4',
     'livelossplot', 
     'tensorboardX',
+    'tqdm'
 ]
 
 setup(
     # 应用名
     name='AttentionMOI',
     # 作者名
     author='Billy',
     # 作者邮箱
     author_email='liangbilin0324@163.com',
     # 版本号
-    version='0.0.2',
+    version='0.0.3',
     # 要求python版本
     python_requires=">=3.9.*",
     # 找到本目录下的所有python包
     packages=find_packages(),
     # 自动安装依赖
     install_requires=install_packages,
+    dependency_links=[
+        "https://pypi.org/simple/",
+        "https://download.pytorch.org/whl/cpu",
+        ],
     # 程序网站
     url='https://github.com/BioAI-kits/AttentionMOI',
     # 程序简单描述
     description="A Denoised Multi-omics Integration Framework for Cancer Subtype Classification and Survival Prediction.",
     # 开源许可
     license='Apache License 2.0',
     # 包含的数据
     data_files=['AttentionMOI/example/cnv.csv.gz', 'AttentionMOI/example/met.csv.gz', 'AttentionMOI/example/rna.csv.gz', 'AttentionMOI/example/label.csv'],
     # 命令行
     entry_points={
         'console_scripts': ['moi = moi:moi',
-                            ]
-    }
+                            ],
+    },
 )
```


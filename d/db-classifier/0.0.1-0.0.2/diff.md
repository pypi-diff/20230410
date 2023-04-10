# Comparing `tmp/db-classifier-0.0.1.tar.gz` & `tmp/db-classifier-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db-classifier-0.0.1.tar", last modified: Mon Apr 10 00:25:26 2023, max compression
+gzip compressed data, was "db-classifier-0.0.2.tar", last modified: Mon Apr 10 00:57:18 2023, max compression
```

## Comparing `db-classifier-0.0.1.tar` & `db-classifier-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 00:25:26.424942 db-classifier-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-04-07 15:28:56.000000 db-classifier-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      854 2023-04-10 00:25:26.424942 db-classifier-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-09 19:19:34.000000 db-classifier-0.0.1/README.md
--rw-rw-rw-   0        0        0      657 2023-04-10 00:24:26.000000 db-classifier-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 00:25:26.424942 db-classifier-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 00:25:26.403943 db-classifier-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-03-01 01:00:33.000000 db-classifier-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:25:26.405942 db-classifier-0.0.1/src/dataset/
--rw-rw-rw-   0        0        0        0 2019-05-31 02:14:42.000000 db-classifier-0.0.1/src/dataset/__init__.py
--rw-rw-rw-   0        0        0     6550 2023-04-09 17:14:03.000000 db-classifier-0.0.1/src/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:25:26.411941 db-classifier-0.0.1/src/db_classifier.egg-info/
--rw-rw-rw-   0        0        0      854 2023-04-10 00:25:26.000000 db-classifier-0.0.1/src/db_classifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2023-04-10 00:25:26.000000 db-classifier-0.0.1/src/db_classifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 00:25:26.000000 db-classifier-0.0.1/src/db_classifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-10 00:25:26.000000 db-classifier-0.0.1/src/db_classifier.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 00:25:26.414940 db-classifier-0.0.1/src/dbclass/
--rw-rw-rw-   0        0        0        0 2019-05-31 02:14:42.000000 db-classifier-0.0.1/src/dbclass/__init__.py
--rw-rw-rw-   0        0        0     4042 2023-04-09 18:27:28.000000 db-classifier-0.0.1/src/dbclass/dbclass.py
--rw-rw-rw-   0        0        0     9105 2023-04-09 18:33:35.000000 db-classifier-0.0.1/src/dbclass/dbclass_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:25:26.422946 db-classifier-0.0.1/src/reports/
--rw-rw-rw-   0        0        0     2923 2019-06-23 19:05:08.000000 db-classifier-0.0.1/src/reports/IMG_001_probability_score.py
--rw-rw-rw-   0        0        0     3304 2019-06-23 18:02:55.000000 db-classifier-0.0.1/src/reports/IMG_001_probability_score_multifeatures.py
--rw-rw-rw-   0        0        0     4873 2019-06-13 23:31:16.000000 db-classifier-0.0.1/src/reports/plot_classifier_comparison.py
--rw-rw-rw-   0        0        0     4729 2023-04-07 17:04:23.000000 db-classifier-0.0.1/src/reports/plot_classifier_comparison_dbclass.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.125073 db-classifier-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-04-07 15:28:56.000000 db-classifier-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2190 2023-04-10 00:57:18.123370 db-classifier-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-09 19:19:34.000000 db-classifier-0.0.2/README.md
+-rw-rw-rw-   0        0        0      887 2023-04-10 00:50:04.000000 db-classifier-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     2886 2023-04-10 00:57:00.000000 db-classifier-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 00:57:18.125073 db-classifier-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.099372 db-classifier-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-03-01 01:00:33.000000 db-classifier-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.101373 db-classifier-0.0.2/src/dataset/
+-rw-rw-rw-   0        0        0        0 2019-05-31 02:14:42.000000 db-classifier-0.0.2/src/dataset/__init__.py
+-rw-rw-rw-   0        0        0     6550 2023-04-09 17:14:03.000000 db-classifier-0.0.2/src/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.109375 db-classifier-0.0.2/src/db_classifier.egg-info/
+-rw-rw-rw-   0        0        0     2190 2023-04-10 00:57:18.000000 db-classifier-0.0.2/src/db_classifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-04-10 00:57:18.000000 db-classifier-0.0.2/src/db_classifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 00:57:18.000000 db-classifier-0.0.2/src/db_classifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2734 2023-04-10 00:57:18.000000 db-classifier-0.0.2/src/db_classifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-04-10 00:57:18.000000 db-classifier-0.0.2/src/db_classifier.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.113385 db-classifier-0.0.2/src/dbclass/
+-rw-rw-rw-   0        0        0        0 2019-05-31 02:14:42.000000 db-classifier-0.0.2/src/dbclass/__init__.py
+-rw-rw-rw-   0        0        0     4042 2023-04-09 18:27:28.000000 db-classifier-0.0.2/src/dbclass/dbclass.py
+-rw-rw-rw-   0        0        0     9105 2023-04-09 18:33:35.000000 db-classifier-0.0.2/src/dbclass/dbclass_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.121371 db-classifier-0.0.2/src/reports/
+-rw-rw-rw-   0        0        0     2923 2019-06-23 19:05:08.000000 db-classifier-0.0.2/src/reports/IMG_001_probability_score.py
+-rw-rw-rw-   0        0        0     3304 2019-06-23 18:02:55.000000 db-classifier-0.0.2/src/reports/IMG_001_probability_score_multifeatures.py
+-rw-rw-rw-   0        0        0     4873 2019-06-13 23:31:16.000000 db-classifier-0.0.2/src/reports/plot_classifier_comparison.py
+-rw-rw-rw-   0        0        0     4729 2023-04-07 17:04:23.000000 db-classifier-0.0.2/src/reports/plot_classifier_comparison_dbclass.py
```

### Comparing `db-classifier-0.0.1/LICENSE` & `db-classifier-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.1/src/dataset/dataset.py` & `db-classifier-0.0.2/src/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.1/src/db_classifier.egg-info/SOURCES.txt` & `db-classifier-0.0.2/src/db_classifier.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
 src/__init__.py
 src/dataset/__init__.py
 src/dataset/dataset.py
 src/db_classifier.egg-info/PKG-INFO
 src/db_classifier.egg-info/SOURCES.txt
 src/db_classifier.egg-info/dependency_links.txt
+src/db_classifier.egg-info/requires.txt
 src/db_classifier.egg-info/top_level.txt
 src/dbclass/__init__.py
 src/dbclass/dbclass.py
 src/dbclass/dbclass_utils.py
 src/reports/IMG_001_probability_score.py
 src/reports/IMG_001_probability_score_multifeatures.py
 src/reports/plot_classifier_comparison.py
```

### Comparing `db-classifier-0.0.1/src/dbclass/dbclass.py` & `db-classifier-0.0.2/src/dbclass/dbclass.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.1/src/dbclass/dbclass_utils.py` & `db-classifier-0.0.2/src/dbclass/dbclass_utils.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.1/src/reports/IMG_001_probability_score.py` & `db-classifier-0.0.2/src/reports/IMG_001_probability_score.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.1/src/reports/IMG_001_probability_score_multifeatures.py` & `db-classifier-0.0.2/src/reports/IMG_001_probability_score_multifeatures.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.1/src/reports/plot_classifier_comparison.py` & `db-classifier-0.0.2/src/reports/plot_classifier_comparison.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.1/src/reports/plot_classifier_comparison_dbclass.py` & `db-classifier-0.0.2/src/reports/plot_classifier_comparison_dbclass.py`

 * *Files identical despite different names*


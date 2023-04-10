# Comparing `tmp/db-classifier-0.0.2.tar.gz` & `tmp/db-classifier-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db-classifier-0.0.2.tar", last modified: Mon Apr 10 00:57:18 2023, max compression
+gzip compressed data, was "db-classifier-0.0.3.tar", last modified: Mon Apr 10 01:09:04 2023, max compression
```

## Comparing `db-classifier-0.0.2.tar` & `db-classifier-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.125073 db-classifier-0.0.2/
--rw-rw-rw-   0        0        0     1094 2023-04-07 15:28:56.000000 db-classifier-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2190 2023-04-10 00:57:18.123370 db-classifier-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-09 19:19:34.000000 db-classifier-0.0.2/README.md
--rw-rw-rw-   0        0        0      887 2023-04-10 00:50:04.000000 db-classifier-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     2886 2023-04-10 00:57:00.000000 db-classifier-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 00:57:18.125073 db-classifier-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.099372 db-classifier-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-03-01 01:00:33.000000 db-classifier-0.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.101373 db-classifier-0.0.2/src/dataset/
--rw-rw-rw-   0        0        0        0 2019-05-31 02:14:42.000000 db-classifier-0.0.2/src/dataset/__init__.py
--rw-rw-rw-   0        0        0     6550 2023-04-09 17:14:03.000000 db-classifier-0.0.2/src/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.109375 db-classifier-0.0.2/src/db_classifier.egg-info/
--rw-rw-rw-   0        0        0     2190 2023-04-10 00:57:18.000000 db-classifier-0.0.2/src/db_classifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-04-10 00:57:18.000000 db-classifier-0.0.2/src/db_classifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 00:57:18.000000 db-classifier-0.0.2/src/db_classifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2734 2023-04-10 00:57:18.000000 db-classifier-0.0.2/src/db_classifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-04-10 00:57:18.000000 db-classifier-0.0.2/src/db_classifier.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.113385 db-classifier-0.0.2/src/dbclass/
--rw-rw-rw-   0        0        0        0 2019-05-31 02:14:42.000000 db-classifier-0.0.2/src/dbclass/__init__.py
--rw-rw-rw-   0        0        0     4042 2023-04-09 18:27:28.000000 db-classifier-0.0.2/src/dbclass/dbclass.py
--rw-rw-rw-   0        0        0     9105 2023-04-09 18:33:35.000000 db-classifier-0.0.2/src/dbclass/dbclass_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:57:18.121371 db-classifier-0.0.2/src/reports/
--rw-rw-rw-   0        0        0     2923 2019-06-23 19:05:08.000000 db-classifier-0.0.2/src/reports/IMG_001_probability_score.py
--rw-rw-rw-   0        0        0     3304 2019-06-23 18:02:55.000000 db-classifier-0.0.2/src/reports/IMG_001_probability_score_multifeatures.py
--rw-rw-rw-   0        0        0     4873 2019-06-13 23:31:16.000000 db-classifier-0.0.2/src/reports/plot_classifier_comparison.py
--rw-rw-rw-   0        0        0     4729 2023-04-07 17:04:23.000000 db-classifier-0.0.2/src/reports/plot_classifier_comparison_dbclass.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:09:04.866151 db-classifier-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-04-07 15:28:56.000000 db-classifier-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2190 2023-04-10 01:09:04.865152 db-classifier-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-09 19:19:34.000000 db-classifier-0.0.3/README.md
+-rw-rw-rw-   0        0        0      887 2023-04-10 01:08:35.000000 db-classifier-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      126 2023-04-10 01:08:04.000000 db-classifier-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 01:09:04.866151 db-classifier-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 01:09:04.847154 db-classifier-0.0.3/src/
+-rw-rw-rw-   0        0        0        0 2023-03-01 01:00:33.000000 db-classifier-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:09:04.849154 db-classifier-0.0.3/src/dataset/
+-rw-rw-rw-   0        0        0        0 2019-05-31 02:14:42.000000 db-classifier-0.0.3/src/dataset/__init__.py
+-rw-rw-rw-   0        0        0     6550 2023-04-09 17:14:03.000000 db-classifier-0.0.3/src/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:09:04.856152 db-classifier-0.0.3/src/db_classifier.egg-info/
+-rw-rw-rw-   0        0        0     2190 2023-04-10 01:09:04.000000 db-classifier-0.0.3/src/db_classifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-04-10 01:09:04.000000 db-classifier-0.0.3/src/db_classifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 01:09:04.000000 db-classifier-0.0.3/src/db_classifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-04-10 01:09:04.000000 db-classifier-0.0.3/src/db_classifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-04-10 01:09:04.000000 db-classifier-0.0.3/src/db_classifier.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 01:09:04.859151 db-classifier-0.0.3/src/dbclass/
+-rw-rw-rw-   0        0        0        0 2019-05-31 02:14:42.000000 db-classifier-0.0.3/src/dbclass/__init__.py
+-rw-rw-rw-   0        0        0     4042 2023-04-09 18:27:28.000000 db-classifier-0.0.3/src/dbclass/dbclass.py
+-rw-rw-rw-   0        0        0     9105 2023-04-09 18:33:35.000000 db-classifier-0.0.3/src/dbclass/dbclass_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:09:04.864152 db-classifier-0.0.3/src/reports/
+-rw-rw-rw-   0        0        0     2923 2019-06-23 19:05:08.000000 db-classifier-0.0.3/src/reports/IMG_001_probability_score.py
+-rw-rw-rw-   0        0        0     3304 2019-06-23 18:02:55.000000 db-classifier-0.0.3/src/reports/IMG_001_probability_score_multifeatures.py
+-rw-rw-rw-   0        0        0     4873 2019-06-13 23:31:16.000000 db-classifier-0.0.3/src/reports/plot_classifier_comparison.py
+-rw-rw-rw-   0        0        0     4729 2023-04-07 17:04:23.000000 db-classifier-0.0.3/src/reports/plot_classifier_comparison_dbclass.py
```

### Comparing `db-classifier-0.0.2/LICENSE` & `db-classifier-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.2/PKG-INFO` & `db-classifier-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-classifier
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Probabilistic Approach to Multiclass Classification with Unknown Instances
 Author-email: Weld Lucas Cunha <cunha.lucas012@gmail.com>
 Maintainer-email: Weld Lucas Cunha <cunha.lucas012@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Weld Lucas Cunha
```

### Comparing `db-classifier-0.0.2/pyproject.toml` & `db-classifier-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "db-classifier"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Probabilistic Approach to Multiclass Classification with Unknown Instances"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   { name="Weld Lucas Cunha", email="cunha.lucas012@gmail.com" },
 ]
```

### Comparing `db-classifier-0.0.2/src/dataset/dataset.py` & `db-classifier-0.0.3/src/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.2/src/db_classifier.egg-info/PKG-INFO` & `db-classifier-0.0.3/src/db_classifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-classifier
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Probabilistic Approach to Multiclass Classification with Unknown Instances
 Author-email: Weld Lucas Cunha <cunha.lucas012@gmail.com>
 Maintainer-email: Weld Lucas Cunha <cunha.lucas012@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Weld Lucas Cunha
```

### Comparing `db-classifier-0.0.2/src/db_classifier.egg-info/SOURCES.txt` & `db-classifier-0.0.3/src/db_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.2/src/dbclass/dbclass.py` & `db-classifier-0.0.3/src/dbclass/dbclass.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.2/src/dbclass/dbclass_utils.py` & `db-classifier-0.0.3/src/dbclass/dbclass_utils.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.2/src/reports/IMG_001_probability_score.py` & `db-classifier-0.0.3/src/reports/IMG_001_probability_score.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.2/src/reports/IMG_001_probability_score_multifeatures.py` & `db-classifier-0.0.3/src/reports/IMG_001_probability_score_multifeatures.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.2/src/reports/plot_classifier_comparison.py` & `db-classifier-0.0.3/src/reports/plot_classifier_comparison.py`

 * *Files identical despite different names*

### Comparing `db-classifier-0.0.2/src/reports/plot_classifier_comparison_dbclass.py` & `db-classifier-0.0.3/src/reports/plot_classifier_comparison_dbclass.py`

 * *Files identical despite different names*


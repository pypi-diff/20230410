# Comparing `tmp/frequency_analysis-0.1.4.3.tar.gz` & `tmp/frequency_analysis-0.1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequency_analysis-0.1.4.3.tar", last modified: Sat Jan  7 11:48:36 2023, max compression
+gzip compressed data, was "frequency_analysis-0.1.4.4.tar", last modified: Mon Apr 10 07:35:15 2023, max compression
```

## Comparing `frequency_analysis-0.1.4.3.tar` & `frequency_analysis-0.1.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-07 11:48:36.902429 frequency_analysis-0.1.4.3/
--rw-rw-rw-   0        0        0     9772 2023-01-07 11:48:36.902429 frequency_analysis-0.1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     9345 2023-01-07 11:46:18.000000 frequency_analysis-0.1.4.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-07 11:48:36.883894 frequency_analysis-0.1.4.3/frequency_analysis/
--rw-rw-rw-   0        0        0      211 2023-01-07 11:47:07.000000 frequency_analysis-0.1.4.3/frequency_analysis/__init__.py
--rw-rw-rw-   0        0        0     5047 2022-04-24 10:46:42.000000 frequency_analysis-0.1.4.3/frequency_analysis/db_create.py
--rw-rw-rw-   0        0        0    13979 2022-04-24 10:46:42.000000 frequency_analysis-0.1.4.3/frequency_analysis/frequency.py
--rw-rw-rw-   0        0        0    28639 2022-04-24 10:46:42.000000 frequency_analysis-0.1.4.3/frequency_analysis/results.py
-drwxrwxrwx   0        0        0        0 2023-01-07 11:48:36.899526 frequency_analysis-0.1.4.3/frequency_analysis.egg-info/
--rw-rw-rw-   0        0        0     9772 2023-01-07 11:48:36.000000 frequency_analysis-0.1.4.3/frequency_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-01-07 11:48:36.000000 frequency_analysis-0.1.4.3/frequency_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-07 11:48:36.000000 frequency_analysis-0.1.4.3/frequency_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-01-07 11:48:36.000000 frequency_analysis-0.1.4.3/frequency_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-01-07 11:48:36.000000 frequency_analysis-0.1.4.3/frequency_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-07 11:48:36.902429 frequency_analysis-0.1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-01-07 11:46:50.000000 frequency_analysis-0.1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:35:15.458979 frequency_analysis-0.1.4.4/
+-rw-rw-rw-   0        0        0     9772 2023-04-10 07:35:15.456326 frequency_analysis-0.1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9345 2023-01-07 11:46:18.000000 frequency_analysis-0.1.4.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 07:35:15.441336 frequency_analysis-0.1.4.4/frequency_analysis/
+-rw-rw-rw-   0        0        0      211 2023-01-07 11:47:07.000000 frequency_analysis-0.1.4.4/frequency_analysis/__init__.py
+-rw-rw-rw-   0        0        0     5047 2022-04-24 10:46:42.000000 frequency_analysis-0.1.4.4/frequency_analysis/db_create.py
+-rw-rw-rw-   0        0        0    13979 2022-04-24 10:46:42.000000 frequency_analysis-0.1.4.4/frequency_analysis/frequency.py
+-rw-rw-rw-   0        0        0    28639 2022-04-24 10:46:42.000000 frequency_analysis-0.1.4.4/frequency_analysis/results.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:35:15.456326 frequency_analysis-0.1.4.4/frequency_analysis.egg-info/
+-rw-rw-rw-   0        0        0     9772 2023-04-10 07:35:15.000000 frequency_analysis-0.1.4.4/frequency_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-04-10 07:35:15.000000 frequency_analysis-0.1.4.4/frequency_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 07:35:15.000000 frequency_analysis-0.1.4.4/frequency_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-10 07:35:15.000000 frequency_analysis-0.1.4.4/frequency_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-10 07:35:15.000000 frequency_analysis-0.1.4.4/frequency_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 07:35:15.458979 frequency_analysis-0.1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      773 2023-04-10 07:34:03.000000 frequency_analysis-0.1.4.4/setup.py
```

### Comparing `frequency_analysis-0.1.4.3/PKG-INFO` & `frequency_analysis-0.1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequency_analysis
-Version: 0.1.4.3
+Version: 0.1.4.4
 Summary: Symbol/symbol bigram/word/word bigram frequency analyzer with excel output.
 Home-page: https://github.com/uqqu/frequency_analysis
 Author: uqqu
 Keywords: frequency analysis bigram linguistic cryptanalysis
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Text Processing :: Linguistic
 Description-Content-Type: text/x-rst
```

### Comparing `frequency_analysis-0.1.4.3/README.rst` & `frequency_analysis-0.1.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `frequency_analysis-0.1.4.3/frequency_analysis/db_create.py` & `frequency_analysis-0.1.4.4/frequency_analysis/db_create.py`

 * *Files identical despite different names*

### Comparing `frequency_analysis-0.1.4.3/frequency_analysis/frequency.py` & `frequency_analysis-0.1.4.4/frequency_analysis/frequency.py`

 * *Files identical despite different names*

### Comparing `frequency_analysis-0.1.4.3/frequency_analysis/results.py` & `frequency_analysis-0.1.4.4/frequency_analysis/results.py`

 * *Files identical despite different names*

### Comparing `frequency_analysis-0.1.4.3/frequency_analysis.egg-info/PKG-INFO` & `frequency_analysis-0.1.4.4/frequency_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequency-analysis
-Version: 0.1.4.3
+Version: 0.1.4.4
 Summary: Symbol/symbol bigram/word/word bigram frequency analyzer with excel output.
 Home-page: https://github.com/uqqu/frequency_analysis
 Author: uqqu
 Keywords: frequency analysis bigram linguistic cryptanalysis
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Text Processing :: Linguistic
 Description-Content-Type: text/x-rst
```

### Comparing `frequency_analysis-0.1.4.3/setup.py` & `frequency_analysis-0.1.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ﻿from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.rst").read_text()
+long_description = (this_directory / "README.rst").read_text('utf-8')
 
 setup(
     name='frequency_analysis',
-    version='0.1.4.3',
+    version='0.1.4.4',
     description='Symbol/symbol bigram/word/word bigram frequency analyzer with excel output.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='uqqu',
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'Topic :: Text Processing :: Linguistic',
```


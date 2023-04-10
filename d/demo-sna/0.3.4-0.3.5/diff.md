# Comparing `tmp/demo_sna-0.3.4.tar.gz` & `tmp/demo_sna-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demo_sna-0.3.4.tar", last modified: Mon Apr 10 20:56:45 2023, max compression
+gzip compressed data, was "demo_sna-0.3.5.tar", last modified: Mon Apr 10 21:51:16 2023, max compression
```

## Comparing `demo_sna-0.3.4.tar` & `demo_sna-0.3.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.381035 demo_sna-0.3.4/
--rw-rw-rw-   0        0        0      172 2023-03-28 19:17:05.000000 demo_sna-0.3.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     3619 2023-03-28 19:17:05.000000 demo_sna-0.3.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-03-28 19:17:05.000000 demo_sna-0.3.4/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-03-28 19:17:05.000000 demo_sna-0.3.4/LICENSE
--rw-rw-rw-   0        0        0      273 2023-03-28 19:17:05.000000 demo_sna-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1121 2023-04-10 20:56:45.381035 demo_sna-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-03-29 10:28:31.000000 demo_sna-0.3.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.315805 demo_sna-0.3.4/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 demo_sna-0.3.4/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.323898 demo_sna-0.3.4/demo_sna/
--rw-rw-rw-   0        0        0      130 2023-03-28 19:17:05.000000 demo_sna-0.3.4/demo_sna/__init__.py
--rw-rw-rw-   0        0        0     1671 2023-03-28 11:35:04.000000 demo_sna-0.3.4/demo_sna/aned.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.336898 demo_sna-0.3.4/demo_sna/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.4/demo_sna/arabiner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.338897 demo_sna-0.3.4/demo_sna/arabiner/bin/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.4/demo_sna/arabiner/bin/__init__.py
--rw-rw-rw-   0        0        0     1211 2023-04-01 08:52:56.000000 demo_sna-0.3.4/demo_sna/arabiner/bin/infer.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.341897 demo_sna-0.3.4/demo_sna/arabiner/utils/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.4/demo_sna/arabiner/utils/__init__.py
--rw-rw-rw-   0        0        0     4220 2023-03-29 20:22:54.000000 demo_sna-0.3.4/demo_sna/arabiner/utils/data.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 demo_sna-0.3.4/demo_sna/arabiner/utils/helpers.py
--rw-rw-rw-   0        0        0      446 2023-03-28 19:17:05.000000 demo_sna-0.3.4/demo_sna/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.344903 demo_sna-0.3.4/demo_sna/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 demo_sna-0.3.4/demo_sna/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7430 2023-04-08 19:52:51.000000 demo_sna-0.3.4/demo_sna/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.356279 demo_sna-0.3.4/demo_sna/morph/
--rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 demo_sna-0.3.4/demo_sna/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 demo_sna-0.3.4/demo_sna/morph/charsets.py
--rw-rw-rw-   0        0        0     2803 2023-04-08 19:53:06.000000 demo_sna-0.3.4/demo_sna/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     8267 2023-04-10 20:56:28.000000 demo_sna-0.3.4/demo_sna/morph/morph_tagger.py
--rw-rw-rw-   0        0        0      197 2023-04-01 20:15:05.000000 demo_sna-0.3.4/demo_sna/morph/serializers.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 demo_sna-0.3.4/demo_sna/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-08 19:53:07.000000 demo_sna-0.3.4/demo_sna/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0     6053 2023-04-05 20:55:34.000000 demo_sna-0.3.4/demo_sna/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.363281 demo_sna-0.3.4/demo_sna/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 demo_sna-0.3.4/demo_sna/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 demo_sna-0.3.4/demo_sna/salma/implication.py
--rw-rw-rw-   0        0        0      513 2023-04-08 09:06:50.000000 demo_sna-0.3.4/demo_sna/salma/tokenizers_words.py
--rw-rw-rw-   0        0        0    17930 2023-02-26 06:10:53.000000 demo_sna-0.3.4/demo_sna/salma/views.py
--rw-rw-rw-   0        0        0     7710 2023-04-06 11:49:15.000000 demo_sna-0.3.4/demo_sna/salma/wsd.py
--rw-rw-rw-   0        0        0     1089 2023-04-01 19:55:10.000000 demo_sna-0.3.4/demo_sna/wsd.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.334903 demo_sna-0.3.4/demo_sna.egg-info/
--rw-rw-rw-   0        0        0     1121 2023-04-10 20:56:45.000000 demo_sna-0.3.4/demo_sna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1240 2023-04-10 20:56:45.000000 demo_sna-0.3.4/demo_sna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 20:56:45.000000 demo_sna-0.3.4/demo_sna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-10 20:56:45.000000 demo_sna-0.3.4/demo_sna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-08 20:11:58.000000 demo_sna-0.3.4/demo_sna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      204 2023-04-10 20:56:45.000000 demo_sna-0.3.4/demo_sna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 20:56:45.000000 demo_sna-0.3.4/demo_sna.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.377035 demo_sna-0.3.4/docs/
--rw-rw-rw-   0        0        0      625 2023-03-28 19:17:05.000000 demo_sna-0.3.4/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-03-28 19:17:05.000000 demo_sna-0.3.4/docs/authors.rst
--rw-rw-rw-   0        0        0     4907 2023-04-08 19:52:39.000000 demo_sna-0.3.4/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-03-28 19:17:05.000000 demo_sna-0.3.4/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-03-28 19:17:05.000000 demo_sna-0.3.4/docs/history.rst
--rw-rw-rw-   0        0        0      321 2023-03-28 19:17:05.000000 demo_sna-0.3.4/docs/index.rst
--rw-rw-rw-   0        0        0     1145 2023-03-28 19:17:05.000000 demo_sna-0.3.4/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-03-28 19:17:05.000000 demo_sna-0.3.4/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-03-28 19:17:05.000000 demo_sna-0.3.4/docs/readme.rst
--rw-rw-rw-   0        0        0       70 2023-03-28 19:17:05.000000 demo_sna-0.3.4/docs/usage.rst
--rw-rw-rw-   0        0        0      399 2023-04-10 20:56:45.383038 demo_sna-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     2845 2023-04-10 20:44:59.000000 demo_sna-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:56:45.380035 demo_sna-0.3.4/tests/
--rw-rw-rw-   0        0        0       35 2023-03-28 19:17:05.000000 demo_sna-0.3.4/tests/__init__.py
--rw-rw-rw-   0        0        0      397 2023-04-08 19:53:09.000000 demo_sna-0.3.4/tests/test_demo.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.570074 demo_sna-0.3.5/
+-rw-rw-rw-   0        0        0      172 2023-03-28 19:17:05.000000 demo_sna-0.3.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3619 2023-03-28 19:17:05.000000 demo_sna-0.3.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-03-28 19:17:05.000000 demo_sna-0.3.5/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-03-28 19:17:05.000000 demo_sna-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-03-28 19:17:05.000000 demo_sna-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1121 2023-04-10 21:51:16.570074 demo_sna-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-03-29 10:28:31.000000 demo_sna-0.3.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.410981 demo_sna-0.3.5/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 demo_sna-0.3.5/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.433262 demo_sna-0.3.5/demo_sna/
+-rw-rw-rw-   0        0        0      130 2023-03-28 19:17:05.000000 demo_sna-0.3.5/demo_sna/__init__.py
+-rw-rw-rw-   0        0        0     1671 2023-03-28 11:35:04.000000 demo_sna-0.3.5/demo_sna/aned.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.455018 demo_sna-0.3.5/demo_sna/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.5/demo_sna/arabiner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.462750 demo_sna-0.3.5/demo_sna/arabiner/bin/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.5/demo_sna/arabiner/bin/__init__.py
+-rw-rw-rw-   0        0        0     1211 2023-04-01 08:52:56.000000 demo_sna-0.3.5/demo_sna/arabiner/bin/infer.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.477336 demo_sna-0.3.5/demo_sna/arabiner/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.5/demo_sna/arabiner/utils/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-03-29 20:22:54.000000 demo_sna-0.3.5/demo_sna/arabiner/utils/data.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 demo_sna-0.3.5/demo_sna/arabiner/utils/helpers.py
+-rw-rw-rw-   0        0        0      446 2023-03-28 19:17:05.000000 demo_sna-0.3.5/demo_sna/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.485357 demo_sna-0.3.5/demo_sna/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 demo_sna-0.3.5/demo_sna/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7430 2023-04-08 19:52:51.000000 demo_sna-0.3.5/demo_sna/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.508719 demo_sna-0.3.5/demo_sna/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 demo_sna-0.3.5/demo_sna/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 demo_sna-0.3.5/demo_sna/morph/charsets.py
+-rw-rw-rw-   0        0        0     2803 2023-04-08 19:53:06.000000 demo_sna-0.3.5/demo_sna/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     8295 2023-04-10 21:50:47.000000 demo_sna-0.3.5/demo_sna/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0      197 2023-04-01 20:15:05.000000 demo_sna-0.3.5/demo_sna/morph/serializers.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 demo_sna-0.3.5/demo_sna/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-08 19:53:07.000000 demo_sna-0.3.5/demo_sna/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0     6053 2023-04-05 20:55:34.000000 demo_sna-0.3.5/demo_sna/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.526457 demo_sna-0.3.5/demo_sna/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 demo_sna-0.3.5/demo_sna/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 demo_sna-0.3.5/demo_sna/salma/implication.py
+-rw-rw-rw-   0        0        0      513 2023-04-08 09:06:50.000000 demo_sna-0.3.5/demo_sna/salma/tokenizers_words.py
+-rw-rw-rw-   0        0        0    17930 2023-02-26 06:10:53.000000 demo_sna-0.3.5/demo_sna/salma/views.py
+-rw-rw-rw-   0        0        0     7710 2023-04-06 11:49:15.000000 demo_sna-0.3.5/demo_sna/salma/wsd.py
+-rw-rw-rw-   0        0        0     1089 2023-04-01 19:55:10.000000 demo_sna-0.3.5/demo_sna/wsd.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.453019 demo_sna-0.3.5/demo_sna.egg-info/
+-rw-rw-rw-   0        0        0     1121 2023-04-10 21:51:16.000000 demo_sna-0.3.5/demo_sna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1240 2023-04-10 21:51:16.000000 demo_sna-0.3.5/demo_sna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 21:51:16.000000 demo_sna-0.3.5/demo_sna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-10 21:51:16.000000 demo_sna-0.3.5/demo_sna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-08 20:11:58.000000 demo_sna-0.3.5/demo_sna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      204 2023-04-10 21:51:16.000000 demo_sna-0.3.5/demo_sna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-10 21:51:16.000000 demo_sna-0.3.5/demo_sna.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.561622 demo_sna-0.3.5/docs/
+-rw-rw-rw-   0        0        0      625 2023-03-28 19:17:05.000000 demo_sna-0.3.5/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-03-28 19:17:05.000000 demo_sna-0.3.5/docs/authors.rst
+-rw-rw-rw-   0        0        0     4907 2023-04-08 19:52:39.000000 demo_sna-0.3.5/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-03-28 19:17:05.000000 demo_sna-0.3.5/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-03-28 19:17:05.000000 demo_sna-0.3.5/docs/history.rst
+-rw-rw-rw-   0        0        0      321 2023-03-28 19:17:05.000000 demo_sna-0.3.5/docs/index.rst
+-rw-rw-rw-   0        0        0     1145 2023-03-28 19:17:05.000000 demo_sna-0.3.5/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-03-28 19:17:05.000000 demo_sna-0.3.5/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-03-28 19:17:05.000000 demo_sna-0.3.5/docs/readme.rst
+-rw-rw-rw-   0        0        0       70 2023-03-28 19:17:05.000000 demo_sna-0.3.5/docs/usage.rst
+-rw-rw-rw-   0        0        0      399 2023-04-10 21:51:16.572979 demo_sna-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     2845 2023-04-10 20:44:59.000000 demo_sna-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:51:16.568241 demo_sna-0.3.5/tests/
+-rw-rw-rw-   0        0        0       35 2023-03-28 19:17:05.000000 demo_sna-0.3.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-04-08 19:53:09.000000 demo_sna-0.3.5/tests/test_demo.py
```

### Comparing `demo_sna-0.3.4/CONTRIBUTING.rst` & `demo_sna-0.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/LICENSE` & `demo_sna-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/PKG-INFO` & `demo_sna-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demo_sna
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/demo
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: demo_sna
 Requires-Python: >=3.7.0, <3.11
```

### Comparing `demo_sna-0.3.4/README.rst` & `demo_sna-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/data/my_data.pickle` & `demo_sna-0.3.5/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/aned.py` & `demo_sna-0.3.5/demo_sna/aned.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/arabiner/bin/infer.py` & `demo_sna-0.3.5/demo_sna/arabiner/bin/infer.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/arabiner/utils/data.py` & `demo_sna-0.3.5/demo_sna/arabiner/utils/data.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/arabiner/utils/helpers.py` & `demo_sna-0.3.5/demo_sna/arabiner/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/jaccard/jaccardFunction.py` & `demo_sna-0.3.5/demo_sna/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/morph/charsets.py` & `demo_sna-0.3.5/demo_sna/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/morph/lemmatizeSentence.py` & `demo_sna-0.3.5/demo_sna/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/morph/morph_tagger.py` & `demo_sna-0.3.5/demo_sna/morph/morph_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 
 
 
 
 
-def load_ALMA_dic(file_path):
+def load_ALMA_dic():
     """
     Load the ALMA dictionary from a binary pickle file.
 
     Args:
     - file_path: str - The path of the binary pickle file containing the ALMA dictionary.
 
     Returns:
@@ -31,23 +31,24 @@
     - pickle.UnpicklingError: If an error occurred while unpickling the data.
     """
     # URL of the .pickle file on GitHub
     url = 'https://github.com/eng-aomar/ts/blob/main/my_data.pickle'
 
     try:
                 # Download the file from the URL
-        data  = requests.get(url)
+        response = requests.get(url)
+        data = response.content
         # Load the data from the file into a Python object
         # data = pickle.loads(response.content)
         # with open(file_path, 'rb') as f:
         #     ALMA_dic = pickle.load(f)
-        ALMA_dic= dict(data)
-        return ALMA_dic
+        my_dict = pickle.loads(data)
+        return my_dict
     except FileNotFoundError as e:
-        print(f"File not found: {file_path}")
+        print(f"File not found: {url}")
         raise e
     except pickle.UnpicklingError as e:
         print("Error while unpickling the data.")
         raise e
 
 def tag(word, lang, task):
     """
```

### Comparing `demo_sna-0.3.4/demo_sna/morph/tokenizers_words.py` & `demo_sna-0.3.5/demo_sna/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/parser.py` & `demo_sna-0.3.5/demo_sna/parser.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/salma/implication.py` & `demo_sna-0.3.5/demo_sna/salma/implication.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/salma/tokenizers_words.py` & `demo_sna-0.3.5/demo_sna/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/salma/views.py` & `demo_sna-0.3.5/demo_sna/salma/views.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/salma/wsd.py` & `demo_sna-0.3.5/demo_sna/salma/wsd.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna/wsd.py` & `demo_sna-0.3.5/demo_sna/wsd.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/demo_sna.egg-info/PKG-INFO` & `demo_sna-0.3.5/demo_sna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demo-sna
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/demo
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: demo_sna
 Requires-Python: >=3.7.0, <3.11
```

### Comparing `demo_sna-0.3.4/demo_sna.egg-info/SOURCES.txt` & `demo_sna-0.3.5/demo_sna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/docs/Makefile` & `demo_sna-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/docs/conf.py` & `demo_sna-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/docs/installation.rst` & `demo_sna-0.3.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/docs/make.bat` & `demo_sna-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.4/setup.py` & `demo_sna-0.3.5/setup.py`

 * *Files identical despite different names*


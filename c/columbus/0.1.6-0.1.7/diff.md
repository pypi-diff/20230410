# Comparing `tmp/columbus-0.1.6.tar.gz` & `tmp/columbus-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "columbus-0.1.6.tar", max compression
+gzip compressed data, was "columbus-0.1.7.tar", max compression
```

## Comparing `columbus-0.1.6.tar` & `columbus-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0        0 2023-02-17 00:47:49.660143 columbus-0.1.6/columbus/__init__.py
--rw-r--r--   0        0        0        0 2023-02-17 00:32:14.678096 columbus-0.1.6/columbus/framework/__init__.py
--rw-r--r--   0        0        0      223 2023-04-10 15:58:51.572616 columbus-0.1.6/columbus/framework/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6322 2023-02-17 00:32:14.678464 columbus-0.1.6/columbus/framework/__pycache__/parse_yaml.cpython-311.pyc
--rw-r--r--   0        0        0     2799 2023-04-08 14:19:29.565716 columbus-0.1.6/columbus/framework/application.py
--rw-r--r--   0        0        0     1694 2023-04-09 16:27:49.132207 columbus-0.1.6/columbus/framework/constants.py
--rw-r--r--   0        0        0     2390 2023-04-09 16:28:33.627425 columbus-0.1.6/columbus/framework/requests.py
--rw-r--r--   0        0        0     1542 2023-04-06 20:59:46.976691 columbus-0.1.6/columbus/framework/utils.py
--rw-r--r--   0        0        0     3806 2023-04-08 14:27:28.056489 columbus-0.1.6/columbus/framework/validators.py
--rw-r--r--   0        0        0     1207 2023-04-06 20:59:27.259465 columbus-0.1.6/columbus/main.py
--rw-r--r--   0        0        0      274 2023-04-08 14:46:28.337726 columbus-0.1.6/columbus/run.py
--rw-r--r--   0        0        0      601 2023-04-08 14:46:07.165675 columbus-0.1.6/columbus/start.py
--rw-r--r--   0        0        0      613 2023-04-10 16:02:34.910463 columbus-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1030 2023-04-10 16:03:30.324673 columbus-0.1.6/setup.py
--rw-r--r--   0        0        0      830 2023-04-10 16:03:30.324888 columbus-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3211 2023-04-10 15:19:14.177154 columbus-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-02-17 00:47:49.660143 columbus-0.1.7/columbus/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-17 00:32:14.678096 columbus-0.1.7/columbus/framework/__init__.py
+-rw-r--r--   0        0        0      223 2023-04-10 15:58:51.572616 columbus-0.1.7/columbus/framework/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6322 2023-02-17 00:32:14.678464 columbus-0.1.7/columbus/framework/__pycache__/parse_yaml.cpython-311.pyc
+-rw-r--r--   0        0        0     2799 2023-04-08 14:19:29.565716 columbus-0.1.7/columbus/framework/application.py
+-rw-r--r--   0        0        0     1694 2023-04-09 16:27:49.132207 columbus-0.1.7/columbus/framework/constants.py
+-rw-r--r--   0        0        0     2390 2023-04-09 16:28:33.627425 columbus-0.1.7/columbus/framework/requests.py
+-rw-r--r--   0        0        0     1542 2023-04-06 20:59:46.976691 columbus-0.1.7/columbus/framework/utils.py
+-rw-r--r--   0        0        0     3806 2023-04-08 14:27:28.056489 columbus-0.1.7/columbus/framework/validators.py
+-rw-r--r--   0        0        0     1207 2023-04-06 20:59:27.259465 columbus-0.1.7/columbus/main.py
+-rw-r--r--   0        0        0      274 2023-04-08 14:46:28.337726 columbus-0.1.7/columbus/run.py
+-rw-r--r--   0        0        0      601 2023-04-08 14:46:07.165675 columbus-0.1.7/columbus/start.py
+-rw-r--r--   0        0        0      675 2023-04-10 16:06:27.553952 columbus-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4401 2023-04-10 16:06:42.454283 columbus-0.1.7/setup.py
+-rw-r--r--   0        0        0     4124 2023-04-10 16:06:42.454772 columbus-0.1.7/PKG-INFO
```

### Comparing `columbus-0.1.6/columbus/framework/__pycache__/parse_yaml.cpython-311.pyc` & `columbus-0.1.7/columbus/framework/__pycache__/parse_yaml.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `columbus-0.1.6/columbus/framework/application.py` & `columbus-0.1.7/columbus/framework/application.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.6/columbus/framework/constants.py` & `columbus-0.1.7/columbus/framework/constants.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.6/columbus/framework/requests.py` & `columbus-0.1.7/columbus/framework/requests.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.6/columbus/framework/utils.py` & `columbus-0.1.7/columbus/framework/utils.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.6/columbus/framework/validators.py` & `columbus-0.1.7/columbus/framework/validators.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.6/columbus/main.py` & `columbus-0.1.7/columbus/main.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.6/columbus/start.py` & `columbus-0.1.7/columbus/start.py`

 * *Files identical despite different names*


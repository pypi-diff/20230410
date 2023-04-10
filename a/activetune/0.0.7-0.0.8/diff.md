# Comparing `tmp/activetune-0.0.7.tar.gz` & `tmp/activetune-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activetune-0.0.7.tar", last modified: Sat Apr  8 21:49:21 2023, max compression
+gzip compressed data, was "activetune-0.0.8.tar", last modified: Mon Apr 10 10:54:25 2023, max compression
```

## Comparing `activetune-0.0.7.tar` & `activetune-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 21:49:21.719337 activetune-0.0.7/
--rw-rw-rw-   0        0        0       89 2023-04-08 21:49:21.719337 activetune-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      969 2023-03-24 12:36:44.000000 activetune-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 21:49:21.719337 activetune-0.0.7/activetune/
--rw-rw-rw-   0        0        0       47 2023-04-08 21:48:44.000000 activetune-0.0.7/activetune/__init__.py
--rw-rw-rw-   0        0        0     2782 2023-04-08 21:47:01.000000 activetune-0.0.7/activetune/api.py
-drwxrwxrwx   0        0        0        0 2023-04-08 21:49:21.719337 activetune-0.0.7/activetune.egg-info/
--rw-rw-rw-   0        0        0       89 2023-04-08 21:49:21.000000 activetune-0.0.7/activetune.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-08 21:49:21.000000 activetune-0.0.7/activetune.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 21:49:21.000000 activetune-0.0.7/activetune.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-20 12:09:14.000000 activetune-0.0.7/activetune.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-04-08 21:49:21.000000 activetune-0.0.7/activetune.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-08 21:49:21.000000 activetune-0.0.7/activetune.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 21:49:21.719337 activetune-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      350 2023-04-08 21:48:55.000000 activetune-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:54:25.817835 activetune-0.0.8/
+-rw-rw-rw-   0        0        0       89 2023-04-10 10:54:25.817835 activetune-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2023-03-24 12:36:44.000000 activetune-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 10:54:25.801507 activetune-0.0.8/activetune/
+-rw-rw-rw-   0        0        0       47 2023-04-10 10:53:34.000000 activetune-0.0.8/activetune/__init__.py
+-rw-rw-rw-   0        0        0     2783 2023-04-10 10:53:10.000000 activetune-0.0.8/activetune/api.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:54:25.817835 activetune-0.0.8/activetune.egg-info/
+-rw-rw-rw-   0        0        0       89 2023-04-10 10:54:25.000000 activetune-0.0.8/activetune.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-10 10:54:25.000000 activetune-0.0.8/activetune.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 10:54:25.000000 activetune-0.0.8/activetune.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-20 12:09:14.000000 activetune-0.0.8/activetune.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-04-10 10:54:25.000000 activetune-0.0.8/activetune.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-10 10:54:25.000000 activetune-0.0.8/activetune.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 10:54:25.817835 activetune-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      350 2023-04-10 10:53:38.000000 activetune-0.0.8/setup.py
```

### Comparing `activetune-0.0.7/README.md` & `activetune-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `activetune-0.0.7/activetune/api.py` & `activetune-0.0.8/activetune/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         return requests.get(
             self.url + "/api/get_data", {"token": self.token, "dataset_id": dataset_id}
         ).json()
 
     def set_feedback(self, sample_id: str, value: int):
         return requests.get(
             self.url + "/api/set_feedback",
-            {"token": self.token, "sample_id": sample_id, "value": self},
+            {"token": self.token, "sample_id": sample_id, "value": value},
         )
 
     def set_meta(self, sample_id: str, meta):
         return requests.get(
             self.url + "/api/set_meta",
             {
                 "token": self.token,
```


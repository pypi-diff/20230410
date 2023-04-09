# Comparing `tmp/atprototools-0.0.6.tar.gz` & `tmp/atprototools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atprototools-0.0.6.tar", last modified: Sat Apr  8 21:35:05 2023, max compression
+gzip compressed data, was "atprototools-0.0.7.tar", last modified: Sun Apr  9 22:15:56 2023, max compression
```

## Comparing `atprototools-0.0.6.tar` & `atprototools-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 21:35:05.348036 atprototools-0.0.6/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 21:35:05.348036 atprototools-0.0.6/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-08 20:12:15.000000 atprototools-0.0.6/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 21:35:05.348036 atprototools-0.0.6/atprototools/
--rw-r--r--   0 user      (1000) user      (1000)     1885 2023-04-08 21:28:47.000000 atprototools-0.0.6/atprototools/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 21:35:05.348036 atprototools-0.0.6/atprototools.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 21:35:05.000000 atprototools-0.0.6/atprototools.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      222 2023-04-08 21:35:05.000000 atprototools-0.0.6/atprototools.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-08 21:35:05.000000 atprototools-0.0.6/atprototools.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-08 21:35:05.000000 atprototools-0.0.6/atprototools.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2023-04-08 21:35:05.000000 atprototools-0.0.6/atprototools.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-08 21:35:05.348036 atprototools-0.0.6/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-08 21:34:58.000000 atprototools-0.0.6/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 22:15:56.184135 atprototools-0.0.7/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-09 22:15:56.184135 atprototools-0.0.7/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      567 2023-04-09 22:14:50.000000 atprototools-0.0.7/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 22:15:56.184135 atprototools-0.0.7/atprototools/
+-rw-r--r--   0 user      (1000) user      (1000)     2965 2023-04-09 22:14:34.000000 atprototools-0.0.7/atprototools/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 22:15:56.184135 atprototools-0.0.7/atprototools.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-09 22:15:56.000000 atprototools-0.0.7/atprototools.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      222 2023-04-09 22:15:56.000000 atprototools-0.0.7/atprototools.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-09 22:15:56.000000 atprototools-0.0.7/atprototools.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-09 22:15:56.000000 atprototools-0.0.7/atprototools.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       13 2023-04-09 22:15:56.000000 atprototools-0.0.7/atprototools.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-09 22:15:56.184135 atprototools-0.0.7/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-09 22:13:54.000000 atprototools-0.0.7/setup.py
```

### Comparing `atprototools-0.0.6/PKG-INFO` & `atprototools-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.6
+Version: 0.0.7
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.6/atprototools/__init__.py` & `atprototools-0.0.7/atprototools/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import requests
 import datetime
+import os
 
 ATP_HOST = "https://bsky.social"
 ATP_AUTH_TOKEN = ""
 DID = "" # leave blank
 
+# TODO annotate all requests.get/post with auth header
+
 
 def login(username, password):
     data = {"identifier": username, "password": password}
     resp = requests.post(
         ATP_HOST + "/xrpc/com.atproto.server.createSession",
         json=data
     )
@@ -64,10 +67,47 @@
     headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
     resp = requests.get(
         ATP_HOST + "/xrpc/app.bsky.feed.getAuthorFeed?actor={}&limit=1".format(accountname),
         headers = headers
     )
     return resp
 
+def get_car_file(did_of_car_to_fetch=None):
+    '''
+    Get a .car file contain all skoots.
+    TODO is there a putRepo?
+    TODO save to file
+    '''
+
+    if did_of_car_to_fetch == None:
+        did_of_car_to_fetch = DID
+
+    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
+
+    resp = requests.get(
+        ATP_HOST + "/xrpc/com.atproto.sync.getRepo?did={}".format(did_of_car_to_fetch),
+        headers = headers
+    )
+
+    return resp
+
+def get_latest_n_skoots(username, n=5):
+    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
+    resp = requests.get(
+        ATP_HOST + "/xrpc/app.bsky.feed.getAuthorFeed?actor={}&limit={}".format(username, n),
+        headers = headers
+    )
+
+    return resp
+
+if __name__ == "__main__":
+    # This code will only be executed if the script is run directly
+    login(os.environ.get("BSKY_USERNAME"), os.environ.get("BSKY_PASSWORD"))
+    # f = get_latest_n_skoots('klatz.co',1).content
+    # print(f)
+    resp = get_car_file()
+    import pdb; pdb.set_trace()
+
+
 
 # resp = login()
 # post("test post")
```

### Comparing `atprototools-0.0.6/atprototools.egg-info/PKG-INFO` & `atprototools-0.0.7/atprototools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.6
+Version: 0.0.7
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.6/setup.py` & `atprototools-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='atprototools',
-    version='0.0.6',
+    version='0.0.7',
     description='tools for posting / deleting things from bsky, in python',
     author='Ian Klatzco',
     author_email='iklatzco@gmail.com',
     url='https://github.com/ianklatzco/atprototools',
     packages=find_packages(),
     install_requires=[
         'requests>=2.22.0'
```


# Comparing `tmp/paybybot3-0.0.31.tar.gz` & `tmp/paybybot3-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paybybot3-0.0.31.tar", last modified: Sun Apr  9 12:53:02 2023, max compression
+gzip compressed data, was "paybybot3-0.0.32.tar", last modified: Mon Apr 10 09:47:23 2023, max compression
```

## Comparing `paybybot3-0.0.31.tar` & `paybybot3-0.0.32.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-09 12:53:02.605243 paybybot3-0.0.31/
--rw-r--r--   0 rayhan     (503) staff       (20)     1080 2023-04-08 11:47:44.000000 paybybot3-0.0.31/LICENSE
--rw-r--r--   0 rayhan     (503) staff       (20)     2544 2023-04-09 12:53:02.605098 paybybot3-0.0.31/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)     2168 2023-04-09 12:44:56.000000 paybybot3-0.0.31/README.md
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-09 12:53:02.604171 paybybot3-0.0.31/paybybot3/
--rw-r--r--   0 rayhan     (503) staff       (20)      177 2023-04-09 12:44:56.000000 paybybot3-0.0.31/paybybot3/__init__.py
--rw-r--r--   0 rayhan     (503) staff       (20)     5649 2023-04-09 12:44:56.000000 paybybot3-0.0.31/paybybot3/__main__.py
--rw-r--r--   0 rayhan     (503) staff       (20)     8033 2023-04-09 12:44:56.000000 paybybot3-0.0.31/paybybot3/bot.py
--rw-r--r--   0 rayhan     (503) staff       (20)      614 2023-04-09 12:44:56.000000 paybybot3-0.0.31/paybybot3/config.py
--rw-r--r--   0 rayhan     (503) staff       (20)      608 2023-04-09 12:44:56.000000 paybybot3-0.0.31/paybybot3/notifs.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-09 12:53:02.604929 paybybot3-0.0.31/paybybot3.egg-info/
--rw-r--r--   0 rayhan     (503) staff       (20)     2544 2023-04-09 12:53:02.000000 paybybot3-0.0.31/paybybot3.egg-info/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)      327 2023-04-09 12:53:02.000000 paybybot3-0.0.31/paybybot3.egg-info/SOURCES.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-04-09 12:53:02.000000 paybybot3-0.0.31/paybybot3.egg-info/dependency_links.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       53 2023-04-09 12:53:02.000000 paybybot3-0.0.31/paybybot3.egg-info/entry_points.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       22 2023-04-09 12:53:02.000000 paybybot3-0.0.31/paybybot3.egg-info/requires.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       10 2023-04-09 12:53:02.000000 paybybot3-0.0.31/paybybot3.egg-info/top_level.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-04-09 12:53:02.605288 paybybot3-0.0.31/setup.cfg
--rw-r--r--   0 rayhan     (503) staff       (20)      761 2023-04-09 12:52:57.000000 paybybot3-0.0.31/setup.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-10 09:47:23.088106 paybybot3-0.0.32/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1080 2023-04-08 11:47:44.000000 paybybot3-0.0.32/LICENSE
+-rw-r--r--   0 rayhan     (503) staff       (20)     2544 2023-04-10 09:47:23.087895 paybybot3-0.0.32/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)     2168 2023-04-10 09:46:12.000000 paybybot3-0.0.32/README.md
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-10 09:47:23.086604 paybybot3-0.0.32/paybybot3/
+-rw-r--r--   0 rayhan     (503) staff       (20)      177 2023-04-10 09:46:12.000000 paybybot3-0.0.32/paybybot3/__init__.py
+-rw-r--r--   0 rayhan     (503) staff       (20)     5649 2023-04-10 09:46:12.000000 paybybot3-0.0.32/paybybot3/__main__.py
+-rw-r--r--   0 rayhan     (503) staff       (20)     8197 2023-04-10 09:46:12.000000 paybybot3-0.0.32/paybybot3/bot.py
+-rw-r--r--   0 rayhan     (503) staff       (20)      614 2023-04-10 09:46:12.000000 paybybot3-0.0.32/paybybot3/config.py
+-rw-r--r--   0 rayhan     (503) staff       (20)      608 2023-04-10 09:46:12.000000 paybybot3-0.0.32/paybybot3/notifs.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-10 09:47:23.087665 paybybot3-0.0.32/paybybot3.egg-info/
+-rw-r--r--   0 rayhan     (503) staff       (20)     2544 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)      327 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       53 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/entry_points.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       22 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/requires.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       10 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/top_level.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-04-10 09:47:23.088156 paybybot3-0.0.32/setup.cfg
+-rw-r--r--   0 rayhan     (503) staff       (20)      761 2023-04-10 09:47:12.000000 paybybot3-0.0.32/setup.py
```

### Comparing `paybybot3-0.0.31/LICENSE` & `paybybot3-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `paybybot3-0.0.31/PKG-INFO` & `paybybot3-0.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paybybot3
-Version: 0.0.31
+Version: 0.0.32
 Summary: CLI interface to https://www.paybyphone.fr/
 Home-page: https://github.com/rklf/paybybot3
 Author: Louis Abraham (louisabraham) and updated by rklf
 Author-email: louis.abraham@yahoo.fr
 License: MIT
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
```

### Comparing `paybybot3-0.0.31/README.md` & `paybybot3-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `paybybot3-0.0.31/paybybot3/__main__.py` & `paybybot3-0.0.32/paybybot3/__main__.py`

 * *Files identical despite different names*

### Comparing `paybybot3-0.0.31/paybybot3/bot.py` & `paybybot3-0.0.32/paybybot3/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,23 @@
         "Referer": "https://m2.paybyphone.fr/",
         "Origin": "https://m2.paybyphone.fr",
         "DNT": "1",
         "Connection": "keep-alive",
     }
 
     def __init__(self, username, password):
-        resp = requests.get("https://m2.paybyphone.fr/static/js/main.0aec44c0.chunk.js")
-        pattern = r'paymentService:{[^}]*apiKey:\"(.*?)\"'
-        result = re.search(pattern, resp.text, flags=re.MULTILINE) or None
-        self.apiKey = result.group(1) if result else None
+        url = "https://m2.paybyphone.fr/static/js/main.0aec44c0.chunk.js"
+        try:
+            resp = requests.get(url)
+            resp.raise_for_status()
+            pattern = r'paymentService:{[^}]*apiKey:\"(.*?)\"'
+            result = re.search(pattern, resp.text, flags=re.MULTILINE)
+            self.apiKey = result.group(1) if result else None
+        except (requests.exceptions.HTTPError, KeyError):
+            self.apiKey = None
 
         r = requests.post(
             "https://auth.paybyphoneapis.com/token",
             headers={
                 **self.base_headers,
                 "Accept": "application/json, text/plain, */*",
                 "X-Pbp-ClientType": "WebApp",
```

### Comparing `paybybot3-0.0.31/paybybot3/config.py` & `paybybot3-0.0.32/paybybot3/config.py`

 * *Files identical despite different names*

### Comparing `paybybot3-0.0.31/paybybot3/notifs.py` & `paybybot3-0.0.32/paybybot3/notifs.py`

 * *Files identical despite different names*

### Comparing `paybybot3-0.0.31/paybybot3.egg-info/PKG-INFO` & `paybybot3-0.0.32/paybybot3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paybybot3
-Version: 0.0.31
+Version: 0.0.32
 Summary: CLI interface to https://www.paybyphone.fr/
 Home-page: https://github.com/rklf/paybybot3
 Author: Louis Abraham (louisabraham) and updated by rklf
 Author-email: louis.abraham@yahoo.fr
 License: MIT
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
```

### Comparing `paybybot3-0.0.31/setup.py` & `paybybot3-0.0.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="paybybot3",
-    version="0.0.31",
+    version="0.0.32",
     author="Louis Abraham (louisabraham) and updated by rklf",
     license="MIT",
     author_email="louis.abraham@yahoo.fr",
     description="CLI interface to https://www.paybyphone.fr/",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/rklf/paybybot3",
```


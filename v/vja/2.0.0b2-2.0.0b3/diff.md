# Comparing `tmp/vja-2.0.0b2.tar.gz` & `tmp/vja-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vja-2.0.0b2.tar", last modified: Sun Apr  2 20:49:46 2023, max compression
+gzip compressed data, was "vja-2.0.0b3.tar", last modified: Mon Apr 10 07:45:01 2023, max compression
```

## Comparing `vja-2.0.0b2.tar` & `vja-2.0.0b3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 20:49:46.306614 vja-2.0.0b2/
--rw-r--r--   0 root         (0) root         (0)     8295 2023-04-02 20:49:46.306614 vja-2.0.0b2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-02 20:49:46.306614 vja-2.0.0b2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      919 2023-04-02 20:48:38.000000 vja-2.0.0b2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 20:49:46.299613 vja-2.0.0b2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 20:48:38.000000 vja-2.0.0b2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-04-02 20:48:38.000000 vja-2.0.0b2/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2847 2023-04-02 20:48:38.000000 vja-2.0.0b2/tests/test_basic.py
--rw-rw-rw-   0 root         (0) root         (0)     9497 2023-04-02 20:48:38.000000 vja-2.0.0b2/tests/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)     8844 2023-04-02 20:48:38.000000 vja-2.0.0b2/tests/test_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 20:49:46.304613 vja-2.0.0b2/vja/
--rwxrwxrwx   0 root         (0) root         (0)      220 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6802 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/apiclient.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/authenticate.py
--rwxrwxrwx   0 root         (0) root         (0)    17567 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/cli.py
--rwxrwxrwx   0 root         (0) root         (0)     1967 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3736 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2572 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/list_service.py
--rwxrwxrwx   0 root         (0) root         (0)     6008 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3289 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/output.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/parse.py
--rw-rw-rw-   0 root         (0) root         (0)    10031 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/service_command.py
--rw-rw-rw-   0 root         (0) root         (0)     3043 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/service_query.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/task_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2892 2023-04-02 20:48:38.000000 vja-2.0.0b2/vja/urgency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 20:49:46.305613 vja-2.0.0b2/vja.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8295 2023-04-02 20:49:46.000000 vja-2.0.0b2/vja.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      511 2023-04-02 20:49:46.000000 vja-2.0.0b2/vja.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 20:49:46.000000 vja-2.0.0b2/vja.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-02 20:49:46.000000 vja-2.0.0b2/vja.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-02 20:49:46.000000 vja-2.0.0b2/vja.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-02 20:49:46.000000 vja-2.0.0b2/vja.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:45:01.706604 vja-2.0.0b3/
+-rw-r--r--   0 root         (0) root         (0)     8295 2023-04-10 07:45:01.706604 vja-2.0.0b3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-10 07:45:01.707604 vja-2.0.0b3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-04-10 07:43:50.000000 vja-2.0.0b3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:45:01.702604 vja-2.0.0b3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 07:43:50.000000 vja-2.0.0b3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-04-10 07:43:50.000000 vja-2.0.0b3/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2847 2023-04-10 07:43:50.000000 vja-2.0.0b3/tests/test_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)     9497 2023-04-10 07:43:50.000000 vja-2.0.0b3/tests/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     8844 2023-04-10 07:43:50.000000 vja-2.0.0b3/tests/test_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:45:01.705604 vja-2.0.0b3/vja/
+-rwxrwxrwx   0 root         (0) root         (0)      220 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6802 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/apiclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/authenticate.py
+-rwxrwxrwx   0 root         (0) root         (0)    17567 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     1967 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3736 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2572 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/list_service.py
+-rwxrwxrwx   0 root         (0) root         (0)     6008 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3289 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)    10031 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/service_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/service_query.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/task_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/urgency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:45:01.706604 vja-2.0.0b3/vja.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8295 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      511 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/top_level.txt
```

### Comparing `vja-2.0.0b2/PKG-INFO` & `vja-2.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
```

### Comparing `vja-2.0.0b2/setup.py` & `vja-2.0.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/tests/conftest.py` & `vja-2.0.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/tests/test_basic.py` & `vja-2.0.0b3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/tests/test_command.py` & `vja-2.0.0b3/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/tests/test_query.py` & `vja-2.0.0b3/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/apiclient.py` & `vja-2.0.0b3/vja/apiclient.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/authenticate.py` & `vja-2.0.0b3/vja/authenticate.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
 
     def logout(self):
         if os.path.isfile(self._token_file):
             os.remove(self._token_file)
 
     def _post_login_request(self, username, password, totp_passcode):
         login_url = self._create_url('/login')
-        payload = {'username': username,
+        payload = {'long_token': True,
+                   'username': username,
                    'password': password,
                    'totp_passcode': totp_passcode}
         return requests.post(login_url, json=payload, timeout=30)
 
     @staticmethod
     def _to_json(response: requests.Response):
         try:
```

### Comparing `vja-2.0.0b2/vja/cli.py` & `vja-2.0.0b3/vja/cli.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/config.py` & `vja-2.0.0b3/vja/config.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/filter.py` & `vja-2.0.0b3/vja/filter.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/list_service.py` & `vja-2.0.0b3/vja/list_service.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/model.py` & `vja-2.0.0b3/vja/model.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/output.py` & `vja-2.0.0b3/vja/output.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/parse.py` & `vja-2.0.0b3/vja/parse.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/service_command.py` & `vja-2.0.0b3/vja/service_command.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/service_query.py` & `vja-2.0.0b3/vja/service_query.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/task_service.py` & `vja-2.0.0b3/vja/task_service.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja/urgency.py` & `vja-2.0.0b3/vja/urgency.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b2/vja.egg-info/PKG-INFO` & `vja-2.0.0b3/vja.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
```


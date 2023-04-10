# Comparing `tmp/robotframework-kubelibrary-0.8.3.tar.gz` & `tmp/robotframework-kubelibrary-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-kubelibrary-0.8.3.tar", last modified: Mon Dec 19 09:48:11 2022, max compression
+gzip compressed data, was "robotframework-kubelibrary-0.8.4.tar", last modified: Mon Apr 10 17:43:06 2023, max compression
```

## Comparing `robotframework-kubelibrary-0.8.3.tar` & `robotframework-kubelibrary-0.8.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-19 09:48:11.469678 robotframework-kubelibrary-0.8.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2022-12-19 09:48:04.000000 robotframework-kubelibrary-0.8.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2022-12-19 09:48:11.469678 robotframework-kubelibrary-0.8.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6213 2022-12-19 09:48:04.000000 robotframework-kubelibrary-0.8.3/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2022-12-19 09:48:11.469678 robotframework-kubelibrary-0.8.3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2022-12-19 09:48:04.000000 robotframework-kubelibrary-0.8.3/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-19 09:48:11.469678 robotframework-kubelibrary-0.8.3/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-19 09:48:11.469678 robotframework-kubelibrary-0.8.3/src/KubeLibrary/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60653 2022-12-19 09:48:04.000000 robotframework-kubelibrary-0.8.3/src/KubeLibrary/KubeLibrary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2022-12-19 09:48:04.000000 robotframework-kubelibrary-0.8.3/src/KubeLibrary/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2022-12-19 09:48:04.000000 robotframework-kubelibrary-0.8.3/src/KubeLibrary/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2022-12-19 09:48:04.000000 robotframework-kubelibrary-0.8.3/src/KubeLibrary/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-19 09:48:11.469678 robotframework-kubelibrary-0.8.3/src/robotframework_kubelibrary.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2022-12-19 09:48:11.000000 robotframework-kubelibrary-0.8.3/src/robotframework_kubelibrary.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2022-12-19 09:48:11.000000 robotframework-kubelibrary-0.8.3/src/robotframework_kubelibrary.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2022-12-19 09:48:11.000000 robotframework-kubelibrary-0.8.3/src/robotframework_kubelibrary.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2022-12-19 09:48:11.000000 robotframework-kubelibrary-0.8.3/src/robotframework_kubelibrary.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2022-12-19 09:48:11.000000 robotframework-kubelibrary-0.8.3/src/robotframework_kubelibrary.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-19 09:48:11.469678 robotframework-kubelibrary-0.8.3/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42996 2022-12-19 09:48:04.000000 robotframework-kubelibrary-0.8.3/test/test_KubeLibrary.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6213 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/src/KubeLibrary/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60866 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/src/KubeLibrary/KubeLibrary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/src/KubeLibrary/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/src/KubeLibrary/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/src/KubeLibrary/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2023-04-10 17:43:06.000000 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-04-10 17:43:06.000000 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-10 17:43:06.000000 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2023-04-10 17:43:06.000000 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-04-10 17:43:06.000000 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42996 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/test/test_KubeLibrary.py
```

### Comparing `robotframework-kubelibrary-0.8.3/LICENSE` & `robotframework-kubelibrary-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-kubelibrary-0.8.3/PKG-INFO` & `robotframework-kubelibrary-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-kubelibrary
-Version: 0.8.3
+Version: 0.8.4
 Summary: Kubernetes library for Robot Framework
 Home-page: https://github.com/devopsspiral/KubeLibrary
 Author: Michał Wcisło
 Author-email: mwcislo999@gmail.com
 License: MIT
 Keywords: robotframework testing test automation kubernetes
 Platform: UNKNOWN
```

### Comparing `robotframework-kubelibrary-0.8.3/README.md` & `robotframework-kubelibrary-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-kubelibrary-0.8.3/setup.py` & `robotframework-kubelibrary-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-kubelibrary-0.8.3/src/KubeLibrary/KubeLibrary.py` & `robotframework-kubelibrary-0.8.4/src/KubeLibrary/KubeLibrary.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,18 @@
         """
         if "1" == environ.get('INIT_FOR_LIBDOC_ONLY', "0"):
             return
         self.reload_config(kube_config=kube_config, context=context, api_url=api_url, bearer_token=bearer_token,
                            ca_cert=ca_cert, incluster=incluster, cert_validation=cert_validation)
 
     @staticmethod
+    def get_proxy():
+        return environ.get('https_proxy') or environ.get('HTTPS_PROXY') or environ.get('http_proxy') or environ.get('HTTP_PROXY')
+
+    @staticmethod
     def generate_alphanumeric_str(size):
         """Generates a random alphanumeric string with given size.
 
         Returns a string.
 
         - ``size``:
           Desired size of the output string
@@ -243,30 +247,30 @@
             except config.config_exception.ConfigException as e:
                 logger.error('Are you sure tests are executed from within k8s cluster?')
                 raise e
         elif api_url and bearer_token:
             if bearer_token.startswith('Bearer '):
                 raise BearerTokenWithPrefixException
             configuration = client.Configuration()
+            configuration._default.proxy = KubeLibrary.get_proxy()
             configuration.api_key["authorization"] = bearer_token
             configuration.api_key_prefix['authorization'] = 'Bearer'
             configuration.host = api_url
             configuration.ssl_ca_cert = ca_cert
             self.api_client = client.ApiClient(configuration)
         else:
             try:
                 config.load_kube_config(kube_config, context)
+                client.Configuration._default.proxy = KubeLibrary.get_proxy()
             except TypeError:
                 logger.error('Neither KUBECONFIG nor ~/.kube/config available.')
 
         if not self.api_client:
             self.api_client = client.ApiClient(configuration=client.Configuration().get_default_copy())
 
-        self.api_client.configuration.proxy = environ.get('http_proxy') or environ.get('HTTP_PROXY')
-
         self._add_api('v1', client.CoreV1Api)
         self._add_api('networkingv1api', client.NetworkingV1Api)
         self._add_api('batchv1', client.BatchV1Api)
         self._add_api('appsv1', client.AppsV1Api)
         # self._add_api('batchv1_beta1', client.BatchV1Api)
         self._add_api('custom_object', client.CustomObjectsApi)
         self._add_api('rbac_authv1_api', client.RbacAuthorizationV1Api)
```

### Comparing `robotframework-kubelibrary-0.8.3/src/robotframework_kubelibrary.egg-info/PKG-INFO` & `robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-kubelibrary
-Version: 0.8.3
+Version: 0.8.4
 Summary: Kubernetes library for Robot Framework
 Home-page: https://github.com/devopsspiral/KubeLibrary
 Author: Michał Wcisło
 Author-email: mwcislo999@gmail.com
 License: MIT
 Keywords: robotframework testing test automation kubernetes
 Platform: UNKNOWN
```

### Comparing `robotframework-kubelibrary-0.8.3/test/test_KubeLibrary.py` & `robotframework-kubelibrary-0.8.4/test/test_KubeLibrary.py`

 * *Files identical despite different names*


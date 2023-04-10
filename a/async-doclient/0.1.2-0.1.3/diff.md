# Comparing `tmp/async_doclient-0.1.2.tar.gz` & `tmp/async_doclient-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_doclient-0.1.2.tar", max compression
+gzip compressed data, was "async_doclient-0.1.3.tar", max compression
```

## Comparing `async_doclient-0.1.2.tar` & `async_doclient-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-01-10 15:12:27.771380 async_doclient-0.1.2/LICENSE
--rw-r--r--   0        0        0       38 2023-01-14 12:39:34.470175 async_doclient-0.1.2/README.md
--rw-r--r--   0        0        0       63 2023-01-11 17:37:36.043709 async_doclient-0.1.2/doclient/clients/__init__.py
--rw-r--r--   0        0        0     9815 2023-04-02 06:10:06.356580 async_doclient-0.1.2/doclient/clients/k8s_client.py
--rw-r--r--   0        0        0       42 2023-01-11 14:47:37.355774 async_doclient-0.1.2/doclient/exceptions/apiexceptions.py
--rw-r--r--   0        0        0     2241 2023-04-01 09:52:37.418659 async_doclient-0.1.2/doclient/resources/k8s/schemas.py
--rw-r--r--   0        0        0      175 2023-03-19 13:43:41.639860 async_doclient-0.1.2/doclient/resources/vpc/schemas.py
--rw-r--r--   0        0        0      956 2023-04-06 14:40:29.348414 async_doclient-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 async_doclient-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-01-10 15:12:27.771380 async_doclient-0.1.3/LICENSE
+-rw-r--r--   0        0        0       38 2023-01-14 12:39:34.470175 async_doclient-0.1.3/README.md
+-rw-r--r--   0        0        0       63 2023-01-11 17:37:36.043709 async_doclient-0.1.3/doclient/clients/__init__.py
+-rw-r--r--   0        0        0     9807 2023-04-10 15:36:52.819802 async_doclient-0.1.3/doclient/clients/k8s_client.py
+-rw-r--r--   0        0        0     1473 2023-04-10 15:36:52.784251 async_doclient-0.1.3/doclient/clients/vpc_client.py
+-rw-r--r--   0        0        0       42 2023-01-11 14:47:37.355774 async_doclient-0.1.3/doclient/exceptions/apiexceptions.py
+-rw-r--r--   0        0        0     2241 2023-04-01 09:52:37.418659 async_doclient-0.1.3/doclient/resources/k8s/schemas.py
+-rw-r--r--   0        0        0      433 2023-04-10 15:36:46.170262 async_doclient-0.1.3/doclient/resources/vpc/schemas.py
+-rw-r--r--   0        0        0      956 2023-04-10 15:37:04.625517 async_doclient-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 async_doclient-0.1.3/PKG-INFO
```

### Comparing `async_doclient-0.1.2/LICENSE` & `async_doclient-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async_doclient-0.1.2/doclient/clients/k8s_client.py` & `async_doclient-0.1.3/doclient/clients/k8s_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Kubernetes1clickApps,
 )
 
 
 class DoK8Sclient:
     def __init__(self, api_key: str = None) -> None:
         self.api_key = api_key or os.getenv("DO_TOKEN")
-        
+
         self.api_url = "https://api.digitalocean.com"
         self.base_url = f"{self.api_url}/v2/kubernetes"
         self.addon_apps_url = f"{self.api_url}/v2/1-clicks/kubernetes"
         self.headers = {"Authorization": f"Bearer {self.api_key}"}
 
     async def create_k8s_cluster(self, payload: KubernetesPayload) -> dict:
         async with aiohttp.ClientSession() as session:
```

### Comparing `async_doclient-0.1.2/doclient/resources/k8s/schemas.py` & `async_doclient-0.1.3/doclient/resources/k8s/schemas.py`

 * *Files identical despite different names*

### Comparing `async_doclient-0.1.2/pyproject.toml` & `async_doclient-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-doclient"
-version = "0.1.2"
+version = "0.1.3"
 description = "Digitalocean client for python"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/Turall/doclient"
 repository = "https://github.com/Turall/doclient"
 authors = ["Tural Muradov <tural_m@hotmail.com>"]
 packages = [
```

### Comparing `async_doclient-0.1.2/PKG-INFO` & `async_doclient-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-doclient
-Version: 0.1.2
+Version: 0.1.3
 Summary: Digitalocean client for python
 Home-page: https://github.com/Turall/doclient
 License: MIT
 Author: Tural Muradov
 Author-email: tural_m@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```


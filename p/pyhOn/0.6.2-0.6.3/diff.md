# Comparing `tmp/pyhOn-0.6.2.tar.gz` & `tmp/pyhOn-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.6.2.tar", last modified: Mon Apr 10 16:51:00 2023, max compression
+gzip compressed data, was "pyhOn-0.6.3.tar", last modified: Mon Apr 10 18:35:11 2023, max compression
```

## Comparing `pyhOn-0.6.2.tar` & `pyhOn-0.6.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:51:00.737891 pyhOn-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 16:50:51.000000 pyhOn-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 16:51:00.737891 pyhOn-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-10 16:50:51.000000 pyhOn-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:51:00.737891 pyhOn-0.6.2/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:51:00.737891 pyhOn-0.6.2/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4839 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:51:00.737891 pyhOn-0.6.2/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:51:00.737891 pyhOn-0.6.2/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/connection/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/connection/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:51:00.737891 pyhOn-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-10 16:50:51.000000 pyhOn-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:11.378888 pyhOn-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 18:35:01.000000 pyhOn-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 18:35:11.378888 pyhOn-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-10 18:35:01.000000 pyhOn-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:11.374888 pyhOn-0.6.3/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:11.378888 pyhOn-0.6.3/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4839 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:11.378888 pyhOn-0.6.3/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:11.378888 pyhOn-0.6.3/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/connection/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/connection/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:35:11.378888 pyhOn-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-10 18:35:01.000000 pyhOn-0.6.3/setup.py
```

### Comparing `pyhOn-0.6.2/LICENSE` & `pyhOn-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/PKG-INFO` & `pyhOn-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.6.2
+Version: 0.6.3
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.6.2/README.md` & `pyhOn-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.6.3/pyhOn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.6.2
+Version: 0.6.3
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.6.2/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.6.3/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/pyhon/__main__.py` & `pyhOn-0.6.3/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/pyhon/appliance.py` & `pyhOn-0.6.3/pyhon/appliance.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/pyhon/appliances/ov.py` & `pyhOn-0.6.3/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/pyhon/commands.py` & `pyhOn-0.6.3/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/pyhon/connection/api.py` & `pyhOn-0.6.3/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/pyhon/connection/auth.py` & `pyhOn-0.6.3/pyhon/connection/auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 import logging
 import re
 import secrets
+import sys
 import urllib
 from pprint import pformat
 from urllib import parse
 
 from yarl import URL
 
 from pyhon import const
 
-_LOGGER = logging.getLogger()
+_LOGGER = logging.getLogger(__name__)
 
 
 class HonAuth:
     def __init__(self, session, email, password, device) -> None:
         self._session = session
         self._email = email
         self._password = password
@@ -52,27 +53,31 @@
             "display": "touch",
             "scope": "api openid refresh_token web",
             "nonce": nonce,
         }
         params = "&".join([f"{k}={v}" for k, v in params.items()])
         async with self._session.get(
             f"{const.AUTH_API}/services/oauth2/authorize/expid_Login?{params}"
-        ) as resp:
-            if not (login_url := re.findall("url = '(.+?)'", await resp.text())):
+        ) as response:
+            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+            if not (login_url := re.findall("url = '(.+?)'", await response.text())):
                 return False
         async with self._session.get(login_url[0], allow_redirects=False) as redirect1:
+            _LOGGER.debug("%s - %s", redirect1.status, redirect1.request_info.url)
             if not (url := redirect1.headers.get("Location")):
                 return False
         async with self._session.get(url, allow_redirects=False) as redirect2:
+            _LOGGER.debug("%s - %s", redirect2.status, redirect2.request_info.url)
             if not (
                 url := redirect2.headers.get("Location")
                 + "&System=IoT_Mobile_App&RegistrationSubChannel=hOn"
             ):
                 return False
         async with self._session.get(URL(url, encoded=True)) as login_screen:
+            _LOGGER.debug("%s - %s", login_screen.status, login_screen.request_info.url)
             if context := re.findall(
                 '"fwuid":"(.*?)","loaded":(\\{.*?})', await login_screen.text()
             ):
                 fw_uid, loaded_str = context[0]
                 loaded = json.loads(loaded_str)
                 login_url = login_url[0].replace(
                     "/".join(const.AUTH_API.split("/")[:-1]), ""
@@ -113,14 +118,15 @@
         params = {"r": 3, "other.LightningLoginCustom.login": 1}
         async with self._session.post(
             const.AUTH_API + "/s/sfsites/aura",
             headers={"Content-Type": "application/x-www-form-urlencoded"},
             data="&".join(f"{k}={json.dumps(v)}" for k, v in data.items()),
             params=params,
         ) as response:
+            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
             if response.status == 200:
                 try:
                     data = await response.json()
                     return data["events"][0]["attributes"]["values"]["url"]
                 except json.JSONDecodeError:
                     pass
                 except KeyError:
@@ -129,33 +135,39 @@
                     )
             _LOGGER.error(
                 "Unable to login: %s\n%s", response.status, await response.text()
             )
             return ""
 
     async def _get_token(self, url):
-        async with self._session.get(url) as resp:
-            if resp.status != 200:
-                _LOGGER.error("Unable to get token: %s", resp.status)
-                return False
-            url = re.findall("href\\s*=\\s*[\"'](http.+?)[\"']", await resp.text())
-            if not url:
-                _LOGGER.error("Can't get login url - \n%s", await resp.text())
-                raise PermissionError
-        async with self._session.get(url[0]) as resp:
-            if resp.status != 200:
-                _LOGGER.error("Unable to get token: %s", resp.status)
-                return False
-            url = re.findall("href\\s*=\\s*[\"'](.*?)[\"']", await resp.text())
-            url = "/".join(const.AUTH_API.split("/")[:-1]) + url[0]
-        async with self._session.get(url) as resp:
-            if resp.status != 200:
-                _LOGGER.error("Unable to connect to the login service: %s", resp.status)
+        async with self._session.get(url) as response:
+            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+            if response.status != 200:
+                _LOGGER.error("Unable to get token: %s", response.status)
+                return False
+            url = re.findall("href\\s*=\\s*[\"'](.+?)[\"']", await response.text())
+        if not url:
+            _LOGGER.error("Can't get login url - \n%s", await response.text())
+            raise PermissionError
+        if "ProgressiveLogin" in url[0]:
+            async with self._session.get(url[0]) as response:
+                _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+                if response.status != 200:
+                    _LOGGER.error("Unable to get token: %s", response.status)
+                    return False
+                url = re.findall("href\\s*=\\s*[\"'](.*?)[\"']", await response.text())
+        url = "/".join(const.AUTH_API.split("/")[:-1]) + url[0]
+        async with self._session.get(url) as response:
+            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+            if response.status != 200:
+                _LOGGER.error(
+                    "Unable to connect to the login service: %s", response.status
+                )
                 return False
-            text = await resp.text()
+            text = await response.text()
         if access_token := re.findall("access_token=(.*?)&", text):
             self._access_token = access_token[0]
         if refresh_token := re.findall("refresh_token=(.*?)&", text):
             self._refresh_token = refresh_token[0]
         if id_token := re.findall("id_token=(.*?)&", text):
             self._id_token = id_token[0]
         return True
@@ -170,31 +182,33 @@
         if not await self._get_token(url):
             return False
 
         post_headers = {"id-token": self._id_token}
         data = self._device.get()
         async with self._session.post(
             f"{const.API_URL}/auth/v1/login", headers=post_headers, json=data
-        ) as resp:
+        ) as response:
+            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
             try:
-                json_data = await resp.json()
+                json_data = await response.json()
             except json.JSONDecodeError:
-                _LOGGER.error("No JSON Data after POST: %s", await resp.text())
+                _LOGGER.error("No JSON Data after POST: %s", await response.text())
                 return False
             self._cognito_token = json_data["cognitoUser"]["Token"]
         return True
 
     async def refresh(self):
         params = {
             "client_id": const.CLIENT_ID,
             "refresh_token": self._refresh_token,
             "grant_type": "refresh_token",
         }
         async with self._session.post(
             f"{const.AUTH_API}/services/oauth2/token", params=params
-        ) as resp:
-            if resp.status >= 400:
+        ) as response:
+            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+            if response.status >= 400:
                 return False
-            data = await resp.json()
+            data = await response.json()
         self._id_token = data["id_token"]
         self._access_token = data["access_token"]
         return True
```

### Comparing `pyhOn-0.6.2/pyhon/connection/device.py` & `pyhOn-0.6.3/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/pyhon/connection/handler.py` & `pyhOn-0.6.3/pyhon/connection/handler.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/pyhon/hon.py` & `pyhOn-0.6.3/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/pyhon/parameter.py` & `pyhOn-0.6.3/pyhon/parameter.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.2/setup.py` & `pyhOn-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.6.2",
+    version="0.6.3",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```


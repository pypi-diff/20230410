# Comparing `tmp/tonplay-sdk-0.0.4.tar.gz` & `tmp/tonplay-sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonplay-sdk-0.0.4.tar", last modified: Fri Apr  7 13:38:04 2023, max compression
+gzip compressed data, was "tonplay-sdk-0.0.5.tar", last modified: Mon Apr 10 04:04:49 2023, max compression
```

## Comparing `tonplay-sdk-0.0.4.tar` & `tonplay-sdk-0.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-07 13:38:04.881357 tonplay-sdk-0.0.4/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1067 2023-04-04 16:07:16.000000 tonplay-sdk-0.0.4/LICENSE.md
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       31 2023-04-04 17:12:11.000000 tonplay-sdk-0.0.4/MANIFEST.in
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1177 2023-04-07 13:38:04.881470 tonplay-sdk-0.0.4/PKG-INFO
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      856 2023-04-06 05:35:46.000000 tonplay-sdk-0.0.4/README.md
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-07 13:38:04.877888 tonplay-sdk-0.0.4/examples/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-05 11:15:02.000000 tonplay-sdk-0.0.4/examples/__init__.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-07 13:38:04.878733 tonplay-sdk-0.0.4/examples/api/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-05 11:39:44.000000 tonplay-sdk-0.0.4/examples/api/__init__.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      215 2023-04-05 11:27:56.000000 tonplay-sdk-0.0.4/examples/api/asset.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1830 2023-04-06 04:59:01.000000 tonplay-sdk-0.0.4/examples/api/asset_deploy.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      966 2023-04-05 11:28:42.000000 tonplay-sdk-0.0.4/examples/api/auth.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      238 2023-04-07 13:37:32.000000 tonplay-sdk-0.0.4/examples/api/game.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1167 2023-04-06 05:40:30.000000 tonplay-sdk-0.0.4/examples/api/market.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      841 2023-04-06 04:49:44.000000 tonplay-sdk-0.0.4/examples/api/ton.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      387 2023-04-06 04:05:39.000000 tonplay-sdk-0.0.4/examples/api/user.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-07 13:38:04.878903 tonplay-sdk-0.0.4/requirements/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-04 16:16:05.000000 tonplay-sdk-0.0.4/requirements/common.txt
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      106 2023-04-07 13:38:04.881801 tonplay-sdk-0.0.4/setup.cfg
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1059 2023-04-06 05:35:46.000000 tonplay-sdk-0.0.4/setup.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-07 13:38:04.879035 tonplay-sdk-0.0.4/tests/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       76 2023-04-06 05:04:17.000000 tonplay-sdk-0.0.4/tests/test_api.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-07 13:38:04.879524 tonplay-sdk-0.0.4/tonplay/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-04 07:17:37.000000 tonplay-sdk-0.0.4/tonplay/__init__.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       22 2023-04-07 13:35:13.000000 tonplay-sdk-0.0.4/tonplay/__version__.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     3268 2023-04-05 12:24:06.000000 tonplay-sdk-0.0.4/tonplay/api.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1473 2023-04-03 13:03:23.000000 tonplay-sdk-0.0.4/tonplay/error.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-07 13:38:04.879843 tonplay-sdk-0.0.4/tonplay/lib/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-04 08:07:09.000000 tonplay-sdk-0.0.4/tonplay/lib/__init__.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       87 2023-04-04 08:08:15.000000 tonplay-sdk-0.0.4/tonplay/lib/enums.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1273 2023-04-06 04:17:04.000000 tonplay-sdk-0.0.4/tonplay/lib/utils.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-07 13:38:04.880665 tonplay-sdk-0.0.4/tonplay/methods/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1391 2023-04-07 13:29:36.000000 tonplay-sdk-0.0.4/tonplay/methods/__init__.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      293 2023-04-04 11:34:18.000000 tonplay-sdk-0.0.4/tonplay/methods/_asset.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      260 2023-04-04 11:34:18.000000 tonplay-sdk-0.0.4/tonplay/methods/_auth.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1044 2023-04-07 13:37:15.000000 tonplay-sdk-0.0.4/tonplay/methods/_game.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     3026 2023-04-05 11:59:01.000000 tonplay-sdk-0.0.4/tonplay/methods/_market.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     6373 2023-04-07 13:20:42.000000 tonplay-sdk-0.0.4/tonplay/methods/_ton.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      628 2023-04-05 12:26:07.000000 tonplay-sdk-0.0.4/tonplay/methods/_user.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-07 13:38:04.881254 tonplay-sdk-0.0.4/tonplay_sdk.egg-info/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1177 2023-04-07 13:38:04.000000 tonplay-sdk-0.0.4/tonplay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      791 2023-04-07 13:38:04.000000 tonplay-sdk-0.0.4/tonplay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        1 2023-04-07 13:38:04.000000 tonplay-sdk-0.0.4/tonplay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-07 13:38:04.000000 tonplay-sdk-0.0.4/tonplay_sdk.egg-info/requires.txt
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-07 13:38:04.000000 tonplay-sdk-0.0.4/tonplay_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-10 04:04:49.812919 tonplay-sdk-0.0.5/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1067 2023-04-04 16:07:16.000000 tonplay-sdk-0.0.5/LICENSE.md
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       31 2023-04-04 17:12:11.000000 tonplay-sdk-0.0.5/MANIFEST.in
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1205 2023-04-10 04:04:49.812988 tonplay-sdk-0.0.5/PKG-INFO
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      884 2023-04-10 04:04:10.000000 tonplay-sdk-0.0.5/README.md
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-10 04:04:49.806335 tonplay-sdk-0.0.5/examples/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-05 11:15:02.000000 tonplay-sdk-0.0.5/examples/__init__.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-10 04:04:49.808223 tonplay-sdk-0.0.5/examples/api/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-05 11:39:44.000000 tonplay-sdk-0.0.5/examples/api/__init__.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      215 2023-04-05 11:27:56.000000 tonplay-sdk-0.0.5/examples/api/asset.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1830 2023-04-06 04:59:01.000000 tonplay-sdk-0.0.5/examples/api/asset_deploy.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      966 2023-04-05 11:28:42.000000 tonplay-sdk-0.0.5/examples/api/auth.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      238 2023-04-07 13:37:32.000000 tonplay-sdk-0.0.5/examples/api/game.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1167 2023-04-06 05:40:30.000000 tonplay-sdk-0.0.5/examples/api/market.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      841 2023-04-06 04:49:44.000000 tonplay-sdk-0.0.5/examples/api/ton.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      387 2023-04-06 04:05:39.000000 tonplay-sdk-0.0.5/examples/api/user.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-10 04:04:49.808517 tonplay-sdk-0.0.5/requirements/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-04 16:16:05.000000 tonplay-sdk-0.0.5/requirements/common.txt
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      106 2023-04-10 04:04:49.813314 tonplay-sdk-0.0.5/setup.cfg
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1059 2023-04-06 05:35:46.000000 tonplay-sdk-0.0.5/setup.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-10 04:04:49.808630 tonplay-sdk-0.0.5/tests/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       76 2023-04-06 05:04:17.000000 tonplay-sdk-0.0.5/tests/test_api.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-10 04:04:49.809270 tonplay-sdk-0.0.5/tonplay/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-04 07:17:37.000000 tonplay-sdk-0.0.5/tonplay/__init__.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       22 2023-04-10 04:04:10.000000 tonplay-sdk-0.0.5/tonplay/__version__.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     3268 2023-04-05 12:24:06.000000 tonplay-sdk-0.0.5/tonplay/api.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1473 2023-04-03 13:03:23.000000 tonplay-sdk-0.0.5/tonplay/error.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-10 04:04:49.810125 tonplay-sdk-0.0.5/tonplay/lib/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-04 08:07:09.000000 tonplay-sdk-0.0.5/tonplay/lib/__init__.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       87 2023-04-04 08:08:15.000000 tonplay-sdk-0.0.5/tonplay/lib/enums.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1273 2023-04-06 04:17:04.000000 tonplay-sdk-0.0.5/tonplay/lib/utils.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-10 04:04:49.812001 tonplay-sdk-0.0.5/tonplay/methods/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1391 2023-04-07 13:29:36.000000 tonplay-sdk-0.0.5/tonplay/methods/__init__.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      293 2023-04-04 11:34:18.000000 tonplay-sdk-0.0.5/tonplay/methods/_asset.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      260 2023-04-04 11:34:18.000000 tonplay-sdk-0.0.5/tonplay/methods/_auth.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1044 2023-04-07 13:37:15.000000 tonplay-sdk-0.0.5/tonplay/methods/_game.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     3026 2023-04-05 11:59:01.000000 tonplay-sdk-0.0.5/tonplay/methods/_market.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     6373 2023-04-07 13:20:42.000000 tonplay-sdk-0.0.5/tonplay/methods/_ton.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      628 2023-04-05 12:26:07.000000 tonplay-sdk-0.0.5/tonplay/methods/_user.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-10 04:04:49.812806 tonplay-sdk-0.0.5/tonplay_sdk.egg-info/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1205 2023-04-10 04:04:49.000000 tonplay-sdk-0.0.5/tonplay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      791 2023-04-10 04:04:49.000000 tonplay-sdk-0.0.5/tonplay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        1 2023-04-10 04:04:49.000000 tonplay-sdk-0.0.5/tonplay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-10 04:04:49.000000 tonplay-sdk-0.0.5/tonplay_sdk.egg-info/requires.txt
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-10 04:04:49.000000 tonplay-sdk-0.0.5/tonplay_sdk.egg-info/top_level.txt
```

### Comparing `tonplay-sdk-0.0.4/LICENSE.md` & `tonplay-sdk-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/PKG-INFO` & `tonplay-sdk-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: tonplay-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is a lightweight library that works as a connector to TON Play public API
 Author: TON Play
 License: MIT
 Keywords: TON Play,Ton Play API,Tonplay API,ton sdk,ton
 Requires-Python: >=3.11.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # TON Play Public API Connector Python
 
 [![PyPI version](https://img.shields.io/pypi/v/tonplay-sdk)](https://pypi.python.org/pypi/tonplay-sdk)
 
-This is a lightweight library that works as a connector to [TON Play public API](https://github.com/90K2/tonplay-sdk)
+This is a [lightweight library](https://github.com/90K2/tonplay-sdk) that works as a connector to [TON Play public API](https://docs.tonplay.io/)
 ## Installation
 
 ```bash
 pip install tonplay-connector
 ```
 
 ## Get API Key
```

### Comparing `tonplay-sdk-0.0.4/README.md` & `tonplay-sdk-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # TON Play Public API Connector Python
 
 [![PyPI version](https://img.shields.io/pypi/v/tonplay-sdk)](https://pypi.python.org/pypi/tonplay-sdk)
 
-This is a lightweight library that works as a connector to [TON Play public API](https://github.com/90K2/tonplay-sdk)
+This is a [lightweight library](https://github.com/90K2/tonplay-sdk) that works as a connector to [TON Play public API](https://docs.tonplay.io/)
 ## Installation
 
 ```bash
 pip install tonplay-connector
 ```
 
 ## Get API Key
```

### Comparing `tonplay-sdk-0.0.4/examples/api/asset_deploy.py` & `tonplay-sdk-0.0.5/examples/api/asset_deploy.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/examples/api/auth.py` & `tonplay-sdk-0.0.5/examples/api/auth.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/examples/api/market.py` & `tonplay-sdk-0.0.5/examples/api/market.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/examples/api/ton.py` & `tonplay-sdk-0.0.5/examples/api/ton.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/setup.py` & `tonplay-sdk-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/tonplay/api.py` & `tonplay-sdk-0.0.5/tonplay/api.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/tonplay/error.py` & `tonplay-sdk-0.0.5/tonplay/error.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/tonplay/lib/utils.py` & `tonplay-sdk-0.0.5/tonplay/lib/utils.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/tonplay/methods/__init__.py` & `tonplay-sdk-0.0.5/tonplay/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/tonplay/methods/_game.py` & `tonplay-sdk-0.0.5/tonplay/methods/_game.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/tonplay/methods/_market.py` & `tonplay-sdk-0.0.5/tonplay/methods/_market.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/tonplay/methods/_ton.py` & `tonplay-sdk-0.0.5/tonplay/methods/_ton.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/tonplay/methods/_user.py` & `tonplay-sdk-0.0.5/tonplay/methods/_user.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.4/tonplay_sdk.egg-info/PKG-INFO` & `tonplay-sdk-0.0.5/tonplay_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: tonplay-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is a lightweight library that works as a connector to TON Play public API
 Author: TON Play
 License: MIT
 Keywords: TON Play,Ton Play API,Tonplay API,ton sdk,ton
 Requires-Python: >=3.11.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # TON Play Public API Connector Python
 
 [![PyPI version](https://img.shields.io/pypi/v/tonplay-sdk)](https://pypi.python.org/pypi/tonplay-sdk)
 
-This is a lightweight library that works as a connector to [TON Play public API](https://github.com/90K2/tonplay-sdk)
+This is a [lightweight library](https://github.com/90K2/tonplay-sdk) that works as a connector to [TON Play public API](https://docs.tonplay.io/)
 ## Installation
 
 ```bash
 pip install tonplay-connector
 ```
 
 ## Get API Key
```

### Comparing `tonplay-sdk-0.0.4/tonplay_sdk.egg-info/SOURCES.txt` & `tonplay-sdk-0.0.5/tonplay_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


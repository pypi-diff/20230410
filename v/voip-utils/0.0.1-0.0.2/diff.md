# Comparing `tmp/voip-utils-0.0.1.tar.gz` & `tmp/voip-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voip-utils-0.0.1.tar", last modified: Thu Apr  6 19:30:10 2023, max compression
+gzip compressed data, was "voip-utils-0.0.2.tar", last modified: Mon Apr 10 20:29:30 2023, max compression
```

## Comparing `voip-utils-0.0.1.tar` & `voip-utils-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-06 19:30:10.007430 voip-utils-0.0.1/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-11-22 20:23:02.000000 voip-utils-0.0.1/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-06 19:30:10.007430 voip-utils-0.0.1/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-04-06 16:12:50.000000 voip-utils-0.0.1/README.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1935 2023-04-06 18:57:11.000000 voip-utils-0.0.1/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      299 2023-04-06 19:30:10.007430 voip-utils-0.0.1/setup.cfg
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-06 19:30:10.007430 voip-utils-0.0.1/voip_utils/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      158 2023-04-06 17:22:11.000000 voip-utils-0.0.1/voip_utils/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-04-06 15:51:26.000000 voip-utils-0.0.1/voip_utils/error.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7678 2023-04-06 17:20:40.000000 voip-utils-0.0.1/voip_utils/rtp_audio.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5984 2023-04-06 19:25:34.000000 voip-utils-0.0.1/voip_utils/sip.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-04-06 18:58:36.000000 voip-utils-0.0.1/voip_utils/util.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5246 2023-04-06 19:28:21.000000 voip-utils-0.0.1/voip_utils/voip.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-06 19:30:10.007430 voip-utils-0.0.1/voip_utils.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-06 19:30:09.000000 voip-utils-0.0.1/voip_utils.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      333 2023-04-06 19:30:10.000000 voip-utils-0.0.1/voip_utils.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 19:30:09.000000 voip-utils-0.0.1/voip_utils.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       11 2023-04-06 19:30:09.000000 voip-utils-0.0.1/voip_utils.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 18:58:14.000000 voip-utils-0.0.1/voip_utils.egg-info/zip-safe
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-10 20:29:30.002290 voip-utils-0.0.2/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-11-22 20:23:02.000000 voip-utils-0.0.2/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-10 20:29:30.002290 voip-utils-0.0.2/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-04-06 16:12:50.000000 voip-utils-0.0.2/README.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1969 2023-04-10 20:29:17.000000 voip-utils-0.0.2/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      299 2023-04-10 20:29:30.002290 voip-utils-0.0.2/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-10 20:29:29.998290 voip-utils-0.0.2/voip_utils/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      158 2023-04-06 17:22:11.000000 voip-utils-0.0.2/voip_utils/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-04-06 15:51:26.000000 voip-utils-0.0.2/voip_utils/error.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7678 2023-04-06 20:24:07.000000 voip-utils-0.0.2/voip_utils/rtp_audio.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5984 2023-04-06 19:25:34.000000 voip-utils-0.0.2/voip_utils/sip.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-04-06 18:58:36.000000 voip-utils-0.0.2/voip_utils/util.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5246 2023-04-06 19:28:21.000000 voip-utils-0.0.2/voip_utils/voip.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-10 20:29:30.002290 voip-utils-0.0.2/voip_utils.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-10 20:29:29.000000 voip-utils-0.0.2/voip_utils.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      366 2023-04-10 20:29:29.000000 voip-utils-0.0.2/voip_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-10 20:29:29.000000 voip-utils-0.0.2/voip_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-10 20:29:29.000000 voip-utils-0.0.2/voip_utils.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       11 2023-04-10 20:29:29.000000 voip-utils-0.0.2/voip_utils.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 18:58:14.000000 voip-utils-0.0.2/voip_utils.egg-info/zip-safe
```

### Comparing `voip-utils-0.0.1/LICENSE.md` & `voip-utils-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.1/PKG-INFO` & `voip-utils-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voip-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Voice over IP Utilities
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,voip,phone
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `voip-utils-0.0.1/pyproject.toml` & `voip-utils-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "voip-utils"
-version     = "0.0.1"
+version     = "0.0.2"
 license     = {text = "Apache-2.0"}
 description = "Voice over IP Utilities"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "voip", "phone"]
@@ -18,14 +18,15 @@
     "Topic :: Communications :: Internet Phone",
     "Topic :: Communications :: Telephony",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 requires-python = ">=3.9.0"
+dependencies = ["opuslib==3.0.1"]
 
 [project.urls]
 "Source Code" = "https://github.com/home-assistant/intents"
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe  = true
```

### Comparing `voip-utils-0.0.1/voip_utils/rtp_audio.py` & `voip-utils-0.0.2/voip_utils/rtp_audio.py`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.1/voip_utils/sip.py` & `voip-utils-0.0.2/voip_utils/sip.py`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.1/voip_utils/voip.py` & `voip-utils-0.0.2/voip_utils/voip.py`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.1/voip_utils.egg-info/PKG-INFO` & `voip-utils-0.0.2/voip_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voip-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Voice over IP Utilities
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,voip,phone
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```


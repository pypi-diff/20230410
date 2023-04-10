# Comparing `tmp/iplocationchanger-0.0.1.tar.gz` & `tmp/iplocationchanger-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iplocationchanger-0.0.1.tar", last modified: Sun Mar  5 14:06:37 2023, max compression
+gzip compressed data, was "iplocationchanger-0.0.2.tar", last modified: Mon Apr 10 17:17:35 2023, max compression
```

## Comparing `iplocationchanger-0.0.1.tar` & `iplocationchanger-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-03-05 14:06:37.204460 iplocationchanger-0.0.1/
--rw-r--r--   0 faaizz     (501) staff       (20)     1076 2023-03-01 19:20:31.000000 iplocationchanger-0.0.1/LICENSE
--rw-r--r--   0 faaizz     (501) staff       (20)     3918 2023-03-05 14:06:37.203648 iplocationchanger-0.0.1/PKG-INFO
--rw-r--r--   0 faaizz     (501) staff       (20)     2045 2023-03-05 14:00:35.000000 iplocationchanger-0.0.1/README.md
--rw-r--r--   0 faaizz     (501) staff       (20)      923 2023-03-05 13:43:24.000000 iplocationchanger-0.0.1/pyproject.toml
--rw-r--r--   0 faaizz     (501) staff       (20)       38 2023-03-05 14:06:37.204605 iplocationchanger-0.0.1/setup.cfg
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-03-05 14:06:37.189997 iplocationchanger-0.0.1/src/
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-03-05 14:06:37.193492 iplocationchanger-0.0.1/src/iplocationchanger/
--rw-r--r--   0 faaizz     (501) staff       (20)       22 2023-03-05 11:44:17.000000 iplocationchanger-0.0.1/src/iplocationchanger/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)     2128 2023-03-05 13:31:21.000000 iplocationchanger-0.0.1/src/iplocationchanger/__main__.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-03-05 14:06:37.197489 iplocationchanger-0.0.1/src/iplocationchanger/model/
--rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:14.000000 iplocationchanger-0.0.1/src/iplocationchanger/model/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)      570 2023-03-02 21:42:30.000000 iplocationchanger-0.0.1/src/iplocationchanger/model/openvpn_credentials.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-03-05 14:06:37.201035 iplocationchanger-0.0.1/src/iplocationchanger/service/
--rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:19.000000 iplocationchanger-0.0.1/src/iplocationchanger/service/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)     1665 2023-03-05 13:31:46.000000 iplocationchanger-0.0.1/src/iplocationchanger/service/location_changer_service.py
--rw-r--r--   0 faaizz     (501) staff       (20)     1639 2023-03-05 13:31:53.000000 iplocationchanger-0.0.1/src/iplocationchanger/service/openvpn_service.py
--rw-r--r--   0 faaizz     (501) staff       (20)     1505 2023-03-05 13:31:58.000000 iplocationchanger-0.0.1/src/iplocationchanger/service/whatismyip_service.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-03-05 14:06:37.202540 iplocationchanger-0.0.1/src/iplocationchanger/utils/
--rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:22.000000 iplocationchanger-0.0.1/src/iplocationchanger/utils/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)     1163 2023-03-04 21:12:26.000000 iplocationchanger-0.0.1/src/iplocationchanger/utils/utils.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-03-05 14:06:37.196477 iplocationchanger-0.0.1/src/iplocationchanger.egg-info/
--rw-r--r--   0 faaizz     (501) staff       (20)     3918 2023-03-05 14:06:37.000000 iplocationchanger-0.0.1/src/iplocationchanger.egg-info/PKG-INFO
--rw-r--r--   0 faaizz     (501) staff       (20)      693 2023-03-05 14:06:37.000000 iplocationchanger-0.0.1/src/iplocationchanger.egg-info/SOURCES.txt
--rw-r--r--   0 faaizz     (501) staff       (20)        1 2023-03-05 14:06:37.000000 iplocationchanger-0.0.1/src/iplocationchanger.egg-info/dependency_links.txt
--rw-r--r--   0 faaizz     (501) staff       (20)       40 2023-03-05 14:06:37.000000 iplocationchanger-0.0.1/src/iplocationchanger.egg-info/requires.txt
--rw-r--r--   0 faaizz     (501) staff       (20)       18 2023-03-05 14:06:37.000000 iplocationchanger-0.0.1/src/iplocationchanger.egg-info/top_level.txt
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.650354 iplocationchanger-0.0.2/
+-rw-r--r--   0 faaizz     (501) staff       (20)     1076 2023-03-01 19:20:31.000000 iplocationchanger-0.0.2/LICENSE
+-rw-r--r--   0 faaizz     (501) staff       (20)     4140 2023-04-10 17:17:35.649622 iplocationchanger-0.0.2/PKG-INFO
+-rw-r--r--   0 faaizz     (501) staff       (20)     2267 2023-03-31 20:37:55.000000 iplocationchanger-0.0.2/README.md
+-rw-r--r--   0 faaizz     (501) staff       (20)      923 2023-04-10 17:13:33.000000 iplocationchanger-0.0.2/pyproject.toml
+-rw-r--r--   0 faaizz     (501) staff       (20)       38 2023-04-10 17:17:35.650546 iplocationchanger-0.0.2/setup.cfg
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.635991 iplocationchanger-0.0.2/src/
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.639912 iplocationchanger-0.0.2/src/iplocationchanger/
+-rw-r--r--   0 faaizz     (501) staff       (20)       22 2023-03-05 11:44:17.000000 iplocationchanger-0.0.2/src/iplocationchanger/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     2136 2023-04-10 17:02:45.000000 iplocationchanger-0.0.2/src/iplocationchanger/__main__.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.643853 iplocationchanger-0.0.2/src/iplocationchanger/model/
+-rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:14.000000 iplocationchanger-0.0.2/src/iplocationchanger/model/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      570 2023-03-02 21:42:30.000000 iplocationchanger-0.0.2/src/iplocationchanger/model/openvpn_credentials.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.647151 iplocationchanger-0.0.2/src/iplocationchanger/service/
+-rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:19.000000 iplocationchanger-0.0.2/src/iplocationchanger/service/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     1665 2023-04-10 16:40:59.000000 iplocationchanger-0.0.2/src/iplocationchanger/service/location_changer_service.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     1639 2023-03-05 13:31:53.000000 iplocationchanger-0.0.2/src/iplocationchanger/service/openvpn_service.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     1505 2023-04-09 14:25:52.000000 iplocationchanger-0.0.2/src/iplocationchanger/service/whatismyip_service.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.648610 iplocationchanger-0.0.2/src/iplocationchanger/utils/
+-rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:22.000000 iplocationchanger-0.0.2/src/iplocationchanger/utils/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     1492 2023-04-10 17:06:15.000000 iplocationchanger-0.0.2/src/iplocationchanger/utils/utils.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.642970 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/
+-rw-r--r--   0 faaizz     (501) staff       (20)     4140 2023-04-10 17:17:35.000000 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/PKG-INFO
+-rw-r--r--   0 faaizz     (501) staff       (20)      693 2023-04-10 17:17:35.000000 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/SOURCES.txt
+-rw-r--r--   0 faaizz     (501) staff       (20)        1 2023-04-10 17:17:35.000000 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/dependency_links.txt
+-rw-r--r--   0 faaizz     (501) staff       (20)       40 2023-04-10 17:17:35.000000 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/requires.txt
+-rw-r--r--   0 faaizz     (501) staff       (20)       18 2023-04-10 17:17:35.000000 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/top_level.txt
```

### Comparing `iplocationchanger-0.0.1/LICENSE` & `iplocationchanger-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.1/PKG-INFO` & `iplocationchanger-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iplocationchanger
-Version: 0.0.1
+Version: 0.0.2
 Summary: Reliable IP location changer using OpenVPN and WhatIsMyIP
 Author-email: Faizudeen Kajogbola <faizudeen@codecreek.cc>
 License: MIT License
         
         Copyright (c) 2023 Faizudeen Kajogbola
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -104,14 +104,15 @@
 ```shell
 coverage run --rcfile .coveragerc  -m unittest discover -t src/ -s src/tests/unit
 
 coverage report -m
 ```
 
 ## Config
-Sample config file:
+Config files are JSON-formatted files with 2-letter [ISO 3166](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country codes as `keys` and paths to corresponding OpenVPN configuration files as `values`.
+A sample config file is shown below:
 ```json
 {
   "TR": "/assets/NCVPN-TR-Istanbul-TCP.ovpn",
   "AR": "/assets/NCVPN-AR-Buenos-Aires-TCP.ovpn"
 }
 ```
```

### Comparing `iplocationchanger-0.0.1/README.md` & `iplocationchanger-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 ```shell
 coverage run --rcfile .coveragerc  -m unittest discover -t src/ -s src/tests/unit
 
 coverage report -m
 ```
 
 ## Config
-Sample config file:
+Config files are JSON-formatted files with 2-letter [ISO 3166](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country codes as `keys` and paths to corresponding OpenVPN configuration files as `values`.
+A sample config file is shown below:
 ```json
 {
   "TR": "/assets/NCVPN-TR-Istanbul-TCP.ovpn",
   "AR": "/assets/NCVPN-AR-Buenos-Aires-TCP.ovpn"
 }
 ```
```

### Comparing `iplocationchanger-0.0.1/pyproject.toml` & `iplocationchanger-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iplocationchanger"
-version = "0.0.1"
+version = "0.0.2"
 description = "Reliable IP location changer using OpenVPN and WhatIsMyIP"
 readme = "README.md"
 authors = [{ name = "Faizudeen Kajogbola", email = "faizudeen@codecreek.cc" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
```

### Comparing `iplocationchanger-0.0.1/src/iplocationchanger/__main__.py` & `iplocationchanger-0.0.2/src/iplocationchanger/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
   except AttributeError:
     pass
   
   lcs = LocationChangerService(
     args.api_key,
     config_to_country_map,
     args.openvpn,
-    credentials_path=ovnc_path,
+    openvpn_credentials_path=ovnc_path,
   )
   atexit.register(lcs.disconnect_region)
 
   success, msg = lcs.connect_region(args.country)
   if not success:
     logging.error(msg)
     exit(1)
```

### Comparing `iplocationchanger-0.0.1/src/iplocationchanger/model/openvpn_credentials.py` & `iplocationchanger-0.0.2/src/iplocationchanger/model/openvpn_credentials.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.1/src/iplocationchanger/service/location_changer_service.py` & `iplocationchanger-0.0.2/src/iplocationchanger/service/location_changer_service.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.1/src/iplocationchanger/service/openvpn_service.py` & `iplocationchanger-0.0.2/src/iplocationchanger/service/openvpn_service.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.1/src/iplocationchanger/service/whatismyip_service.py` & `iplocationchanger-0.0.2/src/iplocationchanger/service/whatismyip_service.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.1/src/iplocationchanger.egg-info/PKG-INFO` & `iplocationchanger-0.0.2/src/iplocationchanger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iplocationchanger
-Version: 0.0.1
+Version: 0.0.2
 Summary: Reliable IP location changer using OpenVPN and WhatIsMyIP
 Author-email: Faizudeen Kajogbola <faizudeen@codecreek.cc>
 License: MIT License
         
         Copyright (c) 2023 Faizudeen Kajogbola
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -104,14 +104,15 @@
 ```shell
 coverage run --rcfile .coveragerc  -m unittest discover -t src/ -s src/tests/unit
 
 coverage report -m
 ```
 
 ## Config
-Sample config file:
+Config files are JSON-formatted files with 2-letter [ISO 3166](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country codes as `keys` and paths to corresponding OpenVPN configuration files as `values`.
+A sample config file is shown below:
 ```json
 {
   "TR": "/assets/NCVPN-TR-Istanbul-TCP.ovpn",
   "AR": "/assets/NCVPN-AR-Buenos-Aires-TCP.ovpn"
 }
 ```
```

### Comparing `iplocationchanger-0.0.1/src/iplocationchanger.egg-info/SOURCES.txt` & `iplocationchanger-0.0.2/src/iplocationchanger.egg-info/SOURCES.txt`

 * *Files identical despite different names*


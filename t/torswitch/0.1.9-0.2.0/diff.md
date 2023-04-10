# Comparing `tmp/torswitch-0.1.9.tar.gz` & `tmp/torswitch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torswitch-0.1.9.tar", last modified: Mon Apr  3 12:17:06 2023, max compression
+gzip compressed data, was "torswitch-0.2.0.tar", last modified: Mon Apr 10 13:33:35 2023, max compression
```

## Comparing `torswitch-0.1.9.tar` & `torswitch-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-03 12:17:06.817778 torswitch-0.1.9/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1070 2023-01-16 10:35:56.000000 torswitch-0.1.9/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     1769 2023-04-03 12:17:06.817778 torswitch-0.1.9/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1260 2023-01-18 07:29:44.000000 torswitch-0.1.9/README.md
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-03 12:17:06.817778 torswitch-0.1.9/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1231 2023-04-03 12:16:53.000000 torswitch-0.1.9/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-03 12:17:06.817778 torswitch-0.1.9/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-03 11:31:52.000000 torswitch-0.1.9/tests/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1792 2023-04-04 10:58:09.000000 torswitch-0.1.9/tests/tor_test.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-03 12:17:06.817778 torswitch-0.1.9/torswitch/
--rw-rw-r--   0 alex      (1000) alex      (1000)      113 2023-01-16 10:35:56.000000 torswitch-0.1.9/torswitch/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      892 2023-01-16 10:35:56.000000 torswitch-0.1.9/torswitch/logger.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      238 2023-01-16 10:35:56.000000 torswitch-0.1.9/torswitch/status.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3320 2023-04-03 12:09:03.000000 torswitch-0.1.9/torswitch/tor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-03 12:17:06.817778 torswitch-0.1.9/torswitch.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1769 2023-04-03 12:17:06.000000 torswitch-0.1.9/torswitch.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      305 2023-04-03 12:17:06.000000 torswitch-0.1.9/torswitch.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-03 12:17:06.000000 torswitch-0.1.9/torswitch.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      130 2023-04-03 12:17:06.000000 torswitch-0.1.9/torswitch.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       16 2023-04-03 12:17:06.000000 torswitch-0.1.9/torswitch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:33:35.497881 torswitch-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 13:33:16.000000 torswitch-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-10 13:33:35.497881 torswitch-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-10 13:33:16.000000 torswitch-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 13:33:35.497881 torswitch-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-10 13:33:16.000000 torswitch-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:33:35.493881 torswitch-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 13:33:16.000000 torswitch-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-10 13:33:16.000000 torswitch-0.2.0/tests/tor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:33:35.493881 torswitch-0.2.0/torswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-10 13:33:16.000000 torswitch-0.2.0/torswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-10 13:33:16.000000 torswitch-0.2.0/torswitch/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 13:33:16.000000 torswitch-0.2.0/torswitch/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-10 13:33:16.000000 torswitch-0.2.0/torswitch/tor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:33:35.493881 torswitch-0.2.0/torswitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-10 13:33:35.000000 torswitch-0.2.0/torswitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-10 13:33:35.000000 torswitch-0.2.0/torswitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:33:35.000000 torswitch-0.2.0/torswitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 13:33:35.000000 torswitch-0.2.0/torswitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 13:33:35.000000 torswitch-0.2.0/torswitch.egg-info/top_level.txt
```

### Comparing `torswitch-0.1.9/LICENSE` & `torswitch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torswitch-0.1.9/PKG-INFO` & `torswitch-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: torswitch
-Version: 0.1.9
-Summary: A basic package for using tor proxy with python.
+Version: 0.2.0
+Summary: Python package for an easy-to-use interaction with the Tor proxy and controlling IP address rotations.
+Home-page: UNKNOWN
 Author: Alex Deathway
 Author-email: <alexdeathway@gmail.com>
+License: UNKNOWN
 Keywords: python,tor,pythontor,iprotation,ipaddress
-Classifier: Development Status :: 4 - Beta
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-﻿# Tor Switch (unstable release )
+﻿# Tor Switch
 
 <div align="center">
-<img width="300" src="./assets/logo/ProjectLogo.png"  alt="logo"/>
+<img width="300" src="https://github.com/alexdeathway/torswitch/blob/master/assets/logo/ProjectLogo.png"  alt="logo"/>
+
+[![Python Package Test](https://github.com/alexdeathway/torswitch/actions/workflows/test.yaml/badge.svg)](https://github.com/alexdeathway/torswitch/actions/workflows/test.yaml)
+[![PyPI version](https://img.shields.io/badge/dynamic/json?color=brightgreen&label=PyPI&query=$.info.version&url=https://pypi.org/pypi/torswitch/json)](https://pypi.org/project/torswitch/) [![License](https://img.shields.io/github/license/alexdeathway/torswitch.svg)](https://github.com/alexdeathway/torswitch/blob/main/LICENSE)
+
+
 </div>
 
 Python package to interact with tor and control IP address rotations.
 
 ## installation 
  - install tor
  
@@ -66,15 +74,15 @@
 
 
 #finally to stop tor
 thisnetwork.stop()
 
 ```
 
-use tor proxy
+## Use tor as proxy
 ```python 
 
 import requests
 from torswitch import TorProtocol
 
 thisnetwork=TorProtocol()
 thisnetwork.Start()
@@ -85,7 +93,10 @@
 }
 
 proxy=requests.get('https://api.ipify.org',proxies=proxies).text
 print(proxy)
 thisnetwork.Stop()
 
 ```
+--- 
+
+
```

### Comparing `torswitch-0.1.9/setup.py` & `torswitch-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,29 +14,30 @@
     return requirements   
 
 def get_version():
     with open("version.txt") as ver:
         Version=ver.read()
     return Version    
 
-DESCRIPTION = 'A basic package for using tor proxy with python.'
+DESCRIPTION = 'Python package for an easy-to-use interaction with the Tor proxy and controlling IP address rotations.'
 
 # Setting up
 setup(
     name="torswitch",
     version=get_version(),
     author="Alex Deathway",
     author_email="<alexdeathway@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=read_requirements(),
     keywords=['python', 'tor', 'pythontor', 'iprotation','ipaddress'],
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
+    #    "Operating System :: Microsoft :: Windows",
     ]
 )
```

### Comparing `torswitch-0.1.9/tests/tor_test.py` & `torswitch-0.2.0/tests/tor_test.py`

 * *Files identical despite different names*

### Comparing `torswitch-0.1.9/torswitch/logger.py` & `torswitch-0.2.0/torswitch/logger.py`

 * *Files identical despite different names*

### Comparing `torswitch-0.1.9/torswitch/tor.py` & `torswitch-0.2.0/torswitch/tor.py`

 * *Files identical despite different names*

### Comparing `torswitch-0.1.9/torswitch.egg-info/PKG-INFO` & `torswitch-0.2.0/torswitch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: torswitch
-Version: 0.1.9
-Summary: A basic package for using tor proxy with python.
+Version: 0.2.0
+Summary: Python package for an easy-to-use interaction with the Tor proxy and controlling IP address rotations.
+Home-page: UNKNOWN
 Author: Alex Deathway
 Author-email: <alexdeathway@gmail.com>
+License: UNKNOWN
 Keywords: python,tor,pythontor,iprotation,ipaddress
-Classifier: Development Status :: 4 - Beta
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-﻿# Tor Switch (unstable release )
+﻿# Tor Switch
 
 <div align="center">
-<img width="300" src="./assets/logo/ProjectLogo.png"  alt="logo"/>
+<img width="300" src="https://github.com/alexdeathway/torswitch/blob/master/assets/logo/ProjectLogo.png"  alt="logo"/>
+
+[![Python Package Test](https://github.com/alexdeathway/torswitch/actions/workflows/test.yaml/badge.svg)](https://github.com/alexdeathway/torswitch/actions/workflows/test.yaml)
+[![PyPI version](https://img.shields.io/badge/dynamic/json?color=brightgreen&label=PyPI&query=$.info.version&url=https://pypi.org/pypi/torswitch/json)](https://pypi.org/project/torswitch/) [![License](https://img.shields.io/github/license/alexdeathway/torswitch.svg)](https://github.com/alexdeathway/torswitch/blob/main/LICENSE)
+
+
 </div>
 
 Python package to interact with tor and control IP address rotations.
 
 ## installation 
  - install tor
  
@@ -66,15 +74,15 @@
 
 
 #finally to stop tor
 thisnetwork.stop()
 
 ```
 
-use tor proxy
+## Use tor as proxy
 ```python 
 
 import requests
 from torswitch import TorProtocol
 
 thisnetwork=TorProtocol()
 thisnetwork.Start()
@@ -85,7 +93,10 @@
 }
 
 proxy=requests.get('https://api.ipify.org',proxies=proxies).text
 print(proxy)
 thisnetwork.Stop()
 
 ```
+--- 
+
+
```


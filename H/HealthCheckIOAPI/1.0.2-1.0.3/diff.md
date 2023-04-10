# Comparing `tmp/HealthCheckIOAPI-1.0.2.tar.gz` & `tmp/HealthCheckIOAPI-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HealthCheckIOAPI-1.0.2.tar", last modified: Mon Apr 10 13:49:54 2023, max compression
+gzip compressed data, was "HealthCheckIOAPI-1.0.3.tar", last modified: Mon Apr 10 13:54:38 2023, max compression
```

## Comparing `HealthCheckIOAPI-1.0.2.tar` & `HealthCheckIOAPI-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 13:49:54.189880 HealthCheckIOAPI-1.0.2/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 13:49:54.189880 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/
--rw-r--r--   0 felix     (1000) felix     (1000)     1224 2023-04-10 13:49:54.000000 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)      300 2023-04-10 13:49:54.000000 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/SOURCES.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        1 2023-04-10 13:49:54.000000 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/dependency_links.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        9 2023-04-10 13:49:54.000000 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/requires.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       14 2023-04-10 13:49:54.000000 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/top_level.txt
--rw-r--r--   0 felix     (1000) felix     (1000)     1069 2023-03-31 22:59:32.000000 HealthCheckIOAPI-1.0.2/LICENSE
--rw-r--r--   0 felix     (1000) felix     (1000)     1224 2023-04-10 13:49:54.189880 HealthCheckIOAPI-1.0.2/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)      951 2023-04-02 13:44:54.000000 HealthCheckIOAPI-1.0.2/README.md
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 13:49:54.189880 HealthCheckIOAPI-1.0.2/healthcheckio/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2023-03-31 23:02:59.000000 HealthCheckIOAPI-1.0.2/healthcheckio/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2368 2023-04-01 15:34:59.000000 HealthCheckIOAPI-1.0.2/healthcheckio/hc_log.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2853 2023-04-02 12:51:55.000000 HealthCheckIOAPI-1.0.2/healthcheckio/hc_ping.py
--rw-r--r--   0 felix     (1000) felix     (1000)       38 2023-04-10 13:49:54.189880 HealthCheckIOAPI-1.0.2/setup.cfg
--rw-r--r--   0 felix     (1000) felix     (1000)      629 2023-04-10 13:49:23.000000 HealthCheckIOAPI-1.0.2/setup.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 13:54:38.399787 HealthCheckIOAPI-1.0.3/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 13:54:38.399787 HealthCheckIOAPI-1.0.3/HealthCheckIOAPI.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1264 2023-04-10 13:54:38.000000 HealthCheckIOAPI-1.0.3/HealthCheckIOAPI.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      300 2023-04-10 13:54:38.000000 HealthCheckIOAPI-1.0.3/HealthCheckIOAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2023-04-10 13:54:38.000000 HealthCheckIOAPI-1.0.3/HealthCheckIOAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        9 2023-04-10 13:54:38.000000 HealthCheckIOAPI-1.0.3/HealthCheckIOAPI.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       14 2023-04-10 13:54:38.000000 HealthCheckIOAPI-1.0.3/HealthCheckIOAPI.egg-info/top_level.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)     1069 2023-03-31 22:59:32.000000 HealthCheckIOAPI-1.0.3/LICENSE
+-rw-r--r--   0 felix     (1000) felix     (1000)     1264 2023-04-10 13:54:38.399787 HealthCheckIOAPI-1.0.3/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      951 2023-04-02 13:44:54.000000 HealthCheckIOAPI-1.0.3/README.md
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 13:54:38.399787 HealthCheckIOAPI-1.0.3/healthcheckio/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2023-03-31 23:02:59.000000 HealthCheckIOAPI-1.0.3/healthcheckio/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2368 2023-04-01 15:34:59.000000 HealthCheckIOAPI-1.0.3/healthcheckio/hc_log.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2853 2023-04-02 12:51:55.000000 HealthCheckIOAPI-1.0.3/healthcheckio/hc_ping.py
+-rw-r--r--   0 felix     (1000) felix     (1000)       38 2023-04-10 13:54:38.399787 HealthCheckIOAPI-1.0.3/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)      629 2023-04-10 13:54:34.000000 HealthCheckIOAPI-1.0.3/setup.py
```

### Comparing `HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/PKG-INFO` & `HealthCheckIOAPI-1.0.3/HealthCheckIOAPI.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: HealthCheckIOAPI
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple Python Tooling to interact with Healthcheck.io projects.
 Home-page: https://github.com/basegodfelix/healthcheckioapi
 Author: Felix Hernandez
 License: MIT
 Platform: UNKNOWN
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # healthcheckioapi
 # Description
 Simple API binding to assist with using the HealthCheck.IO Ping functionality.
 The whole purpose of this project is to simplify the and minimize the amount of code necessary
 to perform all the ping functionality available from HealthCheck.IO
```

### Comparing `HealthCheckIOAPI-1.0.2/LICENSE` & `HealthCheckIOAPI-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HealthCheckIOAPI-1.0.2/PKG-INFO` & `HealthCheckIOAPI-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: HealthCheckIOAPI
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple Python Tooling to interact with Healthcheck.io projects.
 Home-page: https://github.com/basegodfelix/healthcheckioapi
 Author: Felix Hernandez
 License: MIT
 Platform: UNKNOWN
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # healthcheckioapi
 # Description
 Simple API binding to assist with using the HealthCheck.IO Ping functionality.
 The whole purpose of this project is to simplify the and minimize the amount of code necessary
 to perform all the ping functionality available from HealthCheck.IO
```

### Comparing `HealthCheckIOAPI-1.0.2/README.md` & `HealthCheckIOAPI-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `HealthCheckIOAPI-1.0.2/healthcheckio/hc_log.py` & `HealthCheckIOAPI-1.0.3/healthcheckio/hc_log.py`

 * *Files identical despite different names*

### Comparing `HealthCheckIOAPI-1.0.2/healthcheckio/hc_ping.py` & `HealthCheckIOAPI-1.0.3/healthcheckio/hc_ping.py`

 * *Files identical despite different names*

### Comparing `HealthCheckIOAPI-1.0.2/setup.py` & `HealthCheckIOAPI-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     path = os.path.dirname(os.path.abspath(__file__))
     with open(os.path.join(path, 'README.md'), encoding='utf-8') as f:
         tmp = f.read()
     return tmp
 
 setuptools.setup(
     name="HealthCheckIOAPI",
-    version="1.0.2",
+    version="1.0.3",
     author="Felix Hernandez",
     description="Simple Python Tooling to interact with Healthcheck.io projects.",
     packages=["healthcheckio"],
     install_requires=["requests"],
     url="https://github.com/basegodfelix/healthcheckioapi",
     long_description = read(),
-    long_description_context_type = 'text/markdown',
+    long_description_content_type = 'text/markdown',
     license="MIT"
 )
```


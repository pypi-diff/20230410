# Comparing `tmp/gptdeploy-0.18.3.tar.gz` & `tmp/gptdeploy-0.18.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gptdeploy-0.18.3.tar", last modified: Mon Apr 10 00:22:47 2023, max compression
+gzip compressed data, was "dist/gptdeploy-0.18.4.tar", last modified: Mon Apr 10 00:25:45 2023, max compression
```

## Comparing `gptdeploy-0.18.3.tar` & `gptdeploy-0.18.4.tar`

### file list

```diff
@@ -1,14 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:22:47.000000 gptdeploy-0.18.3/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 00:22:26.000000 gptdeploy-0.18.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:22:47.000000 gptdeploy-0.18.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-04-10 00:22:26.000000 gptdeploy-0.18.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:22:47.000000 gptdeploy-0.18.3/gptdeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:22:47.000000 gptdeploy-0.18.3/gptdeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-10 00:22:47.000000 gptdeploy-0.18.3/gptdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:22:47.000000 gptdeploy-0.18.3/gptdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 00:22:47.000000 gptdeploy-0.18.3/gptdeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 00:22:47.000000 gptdeploy-0.18.3/gptdeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:22:47.000000 gptdeploy-0.18.3/gptdeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 00:22:26.000000 gptdeploy-0.18.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:22:47.000000 gptdeploy-0.18.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-10 00:22:26.000000 gptdeploy-0.18.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/key_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/prompt_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/prompt_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/utils/string_tools.py
```

### Comparing `gptdeploy-0.18.3/PKG-INFO` & `gptdeploy-0.18.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.18.3
+Version: 0.18.4
 Summary: Use natural language interface to create, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/gptdeploy
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Description: <h1 align="center">
         GPT Deploy: One line to create them all 🧙🚀
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.3 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.4 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
```

### Comparing `gptdeploy-0.18.3/README.md` & `gptdeploy-0.18.4/README.md`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.3/gptdeploy.egg-info/PKG-INFO` & `gptdeploy-0.18.4/gptdeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.18.3
+Version: 0.18.4
 Summary: Use natural language interface to create, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/gptdeploy
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Description: <h1 align="center">
         GPT Deploy: One line to create them all 🧙🚀
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.3 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.4 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
```

### Comparing `gptdeploy-0.18.3/setup.py` & `gptdeploy-0.18.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def read_requirements():
     with open('requirements.txt', 'r', encoding='utf-8') as f:
         return [line.strip() for line in f.readlines() if not line.startswith('#')]
 
 
 setup(
     name='gptdeploy',
-    version='0.18.3',
+    version='0.18.4',
     description='Use natural language interface to create, deploy and update your microservice infrastructure.',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Florian Hönicke',
     author_email='florian.hoenicke@jina.ai',
     url='https://github.com/jina-ai/gptdeploy',
     packages=find_packages(),
```


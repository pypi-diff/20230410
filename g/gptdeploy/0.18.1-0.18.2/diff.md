# Comparing `tmp/gptdeploy-0.18.1.tar.gz` & `tmp/gptdeploy-0.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gptdeploy-0.18.1.tar", last modified: Mon Apr 10 00:06:39 2023, max compression
+gzip compressed data, was "dist/gptdeploy-0.18.2.tar", last modified: Mon Apr 10 00:11:46 2023, max compression
```

## Comparing `gptdeploy-0.18.1.tar` & `gptdeploy-0.18.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/key_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/prompt_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/prompt_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/gptdeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/gptdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/gptdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/gptdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/gptdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/gptdeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/gptdeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/key_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/prompt_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/prompt_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:11:46.000000 gptdeploy-0.18.2/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-10 00:11:33.000000 gptdeploy-0.18.2/src/utils/string_tools.py
```

### Comparing `gptdeploy-0.18.1/PKG-INFO` & `gptdeploy-0.18.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.18.1
+Version: 0.18.2
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
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.1 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.2 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
```

### Comparing `gptdeploy-0.18.1/README.md` & `gptdeploy-0.18.2/README.md`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.1/gptdeploy.egg-info/PKG-INFO` & `gptdeploy-0.18.2/gptdeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.18.1
+Version: 0.18.2
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
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.1 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.2 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
```

### Comparing `gptdeploy-0.18.1/setup.py` & `gptdeploy-0.18.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from setuptools import setup, find_packages
-import sys
-from os.path import dirname, abspath
 
-sys.path.append(dirname(abspath(__file__)))
 def read_requirements():
     with open('requirements.txt', 'r', encoding='utf-8') as f:
         return [line.strip() for line in f.readlines() if not line.startswith('#')]
 
 
 setup(
     name='gptdeploy',
-    version='0.18.1',
+    version='0.18.2',
     description='Use natural language interface to create, deploy and update your microservice infrastructure.',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Florian Hönicke',
     author_email='florian.hoenicke@jina.ai',
     url='https://github.com/jina-ai/gptdeploy',
     packages=find_packages(),
     install_requires=read_requirements(),
     entry_points={
         'console_scripts': [
-            'gptdeploy=main:main',
+            'gptdeploy=gptdeploy:main',
         ],
     },
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `gptdeploy-0.18.1/src/constants.py` & `gptdeploy-0.18.2/src/constants.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.1/src/gpt.py` & `gptdeploy-0.18.2/src/gpt.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.1/src/jina_cloud.py` & `gptdeploy-0.18.2/src/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.1/src/key_handling.py` & `gptdeploy-0.18.2/src/key_handling.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.1/src/prompt_system.py` & `gptdeploy-0.18.2/src/prompt_system.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.1/src/prompt_tasks.py` & `gptdeploy-0.18.2/src/prompt_tasks.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.1/src/server.py` & `gptdeploy-0.18.2/src/server.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.1/src/utils/io.py` & `gptdeploy-0.18.2/src/utils/io.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.1/src/utils/string_tools.py` & `gptdeploy-0.18.2/src/utils/string_tools.py`

 * *Files identical despite different names*


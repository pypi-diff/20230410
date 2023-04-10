# Comparing `tmp/gptdeploy-0.18.6.tar.gz` & `tmp/gptdeploy-0.18.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gptdeploy-0.18.6.tar", last modified: Mon Apr 10 19:30:00 2023, max compression
+gzip compressed data, was "dist/gptdeploy-0.18.7.tar", last modified: Mon Apr 10 19:59:51 2023, max compression
```

## Comparing `gptdeploy-0.18.6.tar` & `gptdeploy-0.18.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:00.000000 gptdeploy-0.18.6/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-10 19:30:00.000000 gptdeploy-0.18.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/gptdeploy.cmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:00.000000 gptdeploy-0.18.6/gptdeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-10 19:29:59.000000 gptdeploy-0.18.6/gptdeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-10 19:30:00.000000 gptdeploy-0.18.6/gptdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:29:59.000000 gptdeploy-0.18.6/gptdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 19:29:59.000000 gptdeploy-0.18.6/gptdeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 19:29:59.000000 gptdeploy-0.18.6/gptdeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 19:29:59.000000 gptdeploy-0.18.6/gptdeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:30:00.000000 gptdeploy-0.18.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:00.000000 gptdeploy-0.18.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/executor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/key_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/prompt_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/prompt_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:00.000000 gptdeploy-0.18.6/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-10 19:29:48.000000 gptdeploy-0.18.6/src/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/gptdeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/gptdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/gptdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/gptdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/gptdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/gptdeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/gptdeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/gptdeploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/executor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/key_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/prompt_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/prompt_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:59:51.000000 gptdeploy-0.18.7/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-10 19:59:39.000000 gptdeploy-0.18.7/src/utils/string_tools.py
```

### Comparing `gptdeploy-0.18.6/PKG-INFO` & `gptdeploy-0.18.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.18.6
+Version: 0.18.7
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
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.6 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.7 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
```

### Comparing `gptdeploy-0.18.6/README.md` & `gptdeploy-0.18.7/README.md`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.6/gptdeploy.egg-info/PKG-INFO` & `gptdeploy-0.18.7/gptdeploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.18.6
+Version: 0.18.7
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
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.6 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.7 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
```

### Comparing `gptdeploy-0.18.6/setup.py` & `gptdeploy-0.18.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 def read_requirements():
     with open('requirements.txt', 'r', encoding='utf-8') as f:
         return [line.strip() for line in f.readlines() if not line.startswith('#')]
 
 
 setup(
     name='gptdeploy',
-    version='0.18.6',
+    version='0.18.7',
     description='Use natural language interface to create, deploy and update your microservice infrastructure.',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Florian Hönicke',
     author_email='florian.hoenicke@jina.ai',
     url='https://github.com/jina-ai/gptdeploy',
     packages=find_packages(),
     install_requires=read_requirements(),
-    scripts=['gptdeploy.cmd'],
+    scripts=['gptdeploy.py'],
     entry_points={
         'console_scripts': [
             'gptdeploy = src:main',
         ],
     },
 
     classifiers=[
```

### Comparing `gptdeploy-0.18.6/src/cli.py` & `gptdeploy-0.18.7/src/cli.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.6/src/constants.py` & `gptdeploy-0.18.7/src/constants.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.6/src/executor_factory.py` & `gptdeploy-0.18.7/src/executor_factory.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.6/src/gpt.py` & `gptdeploy-0.18.7/src/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,26 @@
     def get_openai_api_key(self):
         if 'OPENAI_API_KEY' not in os.environ:
             raise Exception('You need to set OPENAI_API_KEY in your environment')
         openai.api_key = os.environ['OPENAI_API_KEY']
 
     def is_gpt4_available(self):
         try:
-            openai.ChatCompletion.create(
-                model="gpt-4",
-                messages=[{
-                    "role": 'system',
-                    "content": 'test'
-                }]
-            )
+            for i in range(5):
+                try:
+                    openai.ChatCompletion.create(
+                        model="gpt-4",
+                        messages=[{
+                            "role": 'system',
+                            "content": 'test'
+                        }]
+                    )
+                except RateLimitError:
+                    sleep(1)
+                    continue
             return True
         except openai.error.InvalidRequestError:
             return False
 
     def cost_callback(self, chars_prompt, chars_generation):
         self.chars_prompt_so_far += chars_prompt
         self.chars_generation_so_far += chars_generation
```

### Comparing `gptdeploy-0.18.6/src/jina_cloud.py` & `gptdeploy-0.18.7/src/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.6/src/key_handling.py` & `gptdeploy-0.18.7/src/key_handling.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.6/src/prompt_system.py` & `gptdeploy-0.18.7/src/prompt_system.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.6/src/prompt_tasks.py` & `gptdeploy-0.18.7/src/prompt_tasks.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.6/src/server.py` & `gptdeploy-0.18.7/src/server.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.6/src/utils/io.py` & `gptdeploy-0.18.7/src/utils/io.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.6/src/utils/string_tools.py` & `gptdeploy-0.18.7/src/utils/string_tools.py`

 * *Files identical despite different names*


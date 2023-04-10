# Comparing `tmp/voai-0.0.2.tar.gz` & `tmp/voai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voai-0.0.2.tar", last modified: Mon Apr 10 08:58:41 2023, max compression
+gzip compressed data, was "voai-0.0.3.tar", last modified: Mon Apr 10 10:36:57 2023, max compression
```

## Comparing `voai-0.0.2.tar` & `voai-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 08:58:41.961879 voai-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-04-09 17:36:21.000000 voai-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      915 2023-04-10 08:58:41.961879 voai-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-04-10 08:58:33.000000 voai-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 08:58:41.961879 voai-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-04-10 08:53:54.000000 voai-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:58:41.954864 voai-0.0.2/voai/
-drwxrwxrwx   0        0        0        0 2023-04-10 08:58:41.961879 voai-0.0.2/voai/voai.egg-info/
--rw-rw-rw-   0        0        0      915 2023-04-10 08:58:41.000000 voai-0.0.2/voai/voai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-10 08:58:41.000000 voai-0.0.2/voai/voai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 08:58:41.000000 voai-0.0.2/voai/voai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-10 08:58:41.000000 voai-0.0.2/voai/voai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-10 08:58:41.000000 voai-0.0.2/voai/voai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1756 2023-04-09 18:08:06.000000 voai-0.0.2/voai/voai.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:36:57.533541 voai-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-09 17:36:21.000000 voai-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      947 2023-04-10 10:36:57.532542 voai-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-04-10 10:36:02.000000 voai-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 10:36:57.533541 voai-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2023-04-10 10:36:09.000000 voai-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:36:57.528043 voai-0.0.3/voai/
+drwxrwxrwx   0        0        0        0 2023-04-10 10:36:57.531548 voai-0.0.3/voai/voai.egg-info/
+-rw-rw-rw-   0        0        0      947 2023-04-10 10:36:57.000000 voai-0.0.3/voai/voai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 10:36:57.000000 voai-0.0.3/voai/voai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 10:36:57.000000 voai-0.0.3/voai/voai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-10 10:36:57.000000 voai-0.0.3/voai/voai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-10 10:36:57.000000 voai-0.0.3/voai/voai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2848 2023-04-10 10:31:17.000000 voai-0.0.3/voai/voai.py
```

### Comparing `voai-0.0.2/LICENSE` & `voai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `voai-0.0.2/PKG-INFO` & `voai-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: voai
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool designed for working with 🧑‍💻ChatGPT API🧑‍💻
 Home-page: https://github.com/CURVoid/voai
 Author: VOID
 License: APACHE 2.0
 Keywords: chatgpt,gpt,chat,voai,openai,ai
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## VoAI v0.0.2 - tool designed for working with ChatGPT API
+## VoAI v0.0.3 - tool designed for working with ChatGPT API
 ## Change log
-- Renamed python file from `vogpt` to `voai`, in v0.0.1 you should import `vogpt` not `voai`
+- Added `ask_with_context` method for `GPT35Turbo` that will do same as just `ask` method but will remember previous context
 ## Usage
 ```python
 import voai
 
 KEY = "your-api-key"
 
 chat = voai.GPT35Turbo(KEY)
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: voai Version: 0.0.2 Summary: A tool designed for
+Metadata-Version: 2.1 Name: voai Version: 0.0.3 Summary: A tool designed for
 working with ð§âð»ChatGPT APIð§âð» Home-page: https://github.com/
 CURVoid/voai Author: VOID License: APACHE 2.0 Keywords:
 chatgpt,gpt,chat,voai,openai,ai Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Description-Content-Type: text/markdown
-License-File: LICENSE ## VoAI v0.0.2 - tool designed for working with ChatGPT
-API ## Change log - Renamed python file from `vogpt` to `voai`, in v0.0.1 you
-should import `vogpt` not `voai` ## Usage ```python import voai KEY = "your-
-api-key" chat = voai.GPT35Turbo(KEY) while True: query = input("> ") response =
-chat.ask(query) print(response) ``` ## Using libraries - requests
+License-File: LICENSE ## VoAI v0.0.3 - tool designed for working with ChatGPT
+API ## Change log - Added `ask_with_context` method for `GPT35Turbo` that will
+do same as just `ask` method but will remember previous context ## Usage
+```python import voai KEY = "your-api-key" chat = voai.GPT35Turbo(KEY) while
+True: query = input("> ") response = chat.ask(query) print(response) ``` ##
+Using libraries - requests
```

### Comparing `voai-0.0.2/setup.py` & `voai-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     sys.stderr.write(
         f"""Current python version ({CURRENT_VERSION[0]}.{CURRENT_VERSION[1]}) is lower than required ({REQUIRED_VERSION[0]}.{REQUIRED_VERSION[1]})
         """
     )
 
 setup(
     name="voai",
-    version="0.0.2",
+    version="0.0.3",
     description="A tool designed for working with 🧑‍💻ChatGPT API🧑‍💻",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/CURVoid/voai",
     author="VOID",
     license="APACHE 2.0", 
     keywords=["chatgpt", "gpt", "chat", "voai", "openai", "ai"],
```

### Comparing `voai-0.0.2/voai/voai.egg-info/PKG-INFO` & `voai-0.0.3/voai/voai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: voai
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool designed for working with 🧑‍💻ChatGPT API🧑‍💻
 Home-page: https://github.com/CURVoid/voai
 Author: VOID
 License: APACHE 2.0
 Keywords: chatgpt,gpt,chat,voai,openai,ai
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## VoAI v0.0.2 - tool designed for working with ChatGPT API
+## VoAI v0.0.3 - tool designed for working with ChatGPT API
 ## Change log
-- Renamed python file from `vogpt` to `voai`, in v0.0.1 you should import `vogpt` not `voai`
+- Added `ask_with_context` method for `GPT35Turbo` that will do same as just `ask` method but will remember previous context
 ## Usage
 ```python
 import voai
 
 KEY = "your-api-key"
 
 chat = voai.GPT35Turbo(KEY)
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: voai Version: 0.0.2 Summary: A tool designed for
+Metadata-Version: 2.1 Name: voai Version: 0.0.3 Summary: A tool designed for
 working with ð§âð»ChatGPT APIð§âð» Home-page: https://github.com/
 CURVoid/voai Author: VOID License: APACHE 2.0 Keywords:
 chatgpt,gpt,chat,voai,openai,ai Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Description-Content-Type: text/markdown
-License-File: LICENSE ## VoAI v0.0.2 - tool designed for working with ChatGPT
-API ## Change log - Renamed python file from `vogpt` to `voai`, in v0.0.1 you
-should import `vogpt` not `voai` ## Usage ```python import voai KEY = "your-
-api-key" chat = voai.GPT35Turbo(KEY) while True: query = input("> ") response =
-chat.ask(query) print(response) ``` ## Using libraries - requests
+License-File: LICENSE ## VoAI v0.0.3 - tool designed for working with ChatGPT
+API ## Change log - Added `ask_with_context` method for `GPT35Turbo` that will
+do same as just `ask` method but will remember previous context ## Usage
+```python import voai KEY = "your-api-key" chat = voai.GPT35Turbo(KEY) while
+True: query = input("> ") response = chat.ask(query) print(response) ``` ##
+Using libraries - requests
```


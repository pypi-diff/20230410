# Comparing `tmp/shell_gpt-0.8.6.tar.gz` & `tmp/shell_gpt-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_gpt-0.8.6.tar", last modified: Sun Apr  9 17:11:12 2023, max compression
+gzip compressed data, was "shell_gpt-0.8.7.tar", last modified: Mon Apr 10 10:10:10 2023, max compression
```

## Comparing `shell_gpt-0.8.6.tar` & `shell_gpt-0.8.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-09 17:11:12.009149 shell_gpt-0.8.6/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.6/LICENSE
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15147 2023-04-09 17:11:12.008934 shell_gpt-0.8.6/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14799 2023-04-09 15:13:49.000000 shell_gpt-0.8.6/README.md
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-09 17:11:12.009186 shell_gpt-0.8.6/setup.cfg
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      829 2023-04-08 20:27:13.000000 shell_gpt-0.8.6/setup.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-09 17:11:12.007262 shell_gpt-0.8.6/sgpt/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      445 2023-04-04 16:16:05.000000 shell_gpt-0.8.6/sgpt/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.6/sgpt/__main__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4398 2023-04-09 17:01:36.000000 shell_gpt-0.8.6/sgpt/app.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.6/sgpt/cache.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3069 2023-04-08 20:21:44.000000 shell_gpt-0.8.6/sgpt/client.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2726 2023-04-09 15:07:44.000000 shell_gpt-0.8.6/sgpt/config.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-09 17:11:12.008001 shell_gpt-0.8.6/sgpt/handlers/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.6/sgpt/handlers/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-04 16:16:05.000000 shell_gpt-0.8.6/sgpt/handlers/chat_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.6/sgpt/handlers/default_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1121 2023-04-06 23:34:58.000000 shell_gpt-0.8.6/sgpt/handlers/handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1839 2023-04-07 18:29:19.000000 shell_gpt-0.8.6/sgpt/handlers/repl_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2092 2023-04-07 18:29:19.000000 shell_gpt-0.8.6/sgpt/make_prompt.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1877 2023-04-07 22:52:58.000000 shell_gpt-0.8.6/sgpt/utils.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-09 17:11:12.008752 shell_gpt-0.8.6/shell_gpt.egg-info/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15147 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/entry_points.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       97 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/requires.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 10:10:10.242655 shell_gpt-0.8.7/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.7/LICENSE
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15413 2023-04-10 10:10:10.242432 shell_gpt-0.8.7/PKG-INFO
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15065 2023-04-09 21:48:47.000000 shell_gpt-0.8.7/README.md
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-10 10:10:10.242696 shell_gpt-0.8.7/setup.cfg
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      829 2023-04-09 21:48:47.000000 shell_gpt-0.8.7/setup.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 10:10:10.240763 shell_gpt-0.8.7/sgpt/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      451 2023-04-09 21:20:27.000000 shell_gpt-0.8.7/sgpt/__init__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.7/sgpt/__main__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4398 2023-04-09 19:35:59.000000 shell_gpt-0.8.7/sgpt/app.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.7/sgpt/cache.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3069 2023-04-09 19:35:59.000000 shell_gpt-0.8.7/sgpt/client.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2857 2023-04-09 21:52:14.000000 shell_gpt-0.8.7/sgpt/config.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 10:10:10.241465 shell_gpt-0.8.7/sgpt/handlers/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.7/sgpt/handlers/__init__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-04 16:16:05.000000 shell_gpt-0.8.7/sgpt/handlers/chat_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.7/sgpt/handlers/default_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1195 2023-04-09 21:48:13.000000 shell_gpt-0.8.7/sgpt/handlers/handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1839 2023-04-07 18:29:19.000000 shell_gpt-0.8.7/sgpt/handlers/repl_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2092 2023-04-07 18:29:19.000000 shell_gpt-0.8.7/sgpt/make_prompt.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1877 2023-04-09 19:35:59.000000 shell_gpt-0.8.7/sgpt/utils.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 10:10:10.242240 shell_gpt-0.8.7/shell_gpt.egg-info/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15413 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       97 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/requires.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/top_level.txt
```

### Comparing `shell_gpt-0.8.6/LICENSE` & `shell_gpt-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.6/PKG-INFO` & `shell_gpt-0.8.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,17 @@
-Metadata-Version: 2.1
-Name: shell_gpt
-Version: 0.8.6
-Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
-Home-page: https://github.com/ther1d/shell_gpt
-Author: Farkhod Sadykov
-Author-email: farkhod@sadykov.dev
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Shell GPT
 A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.6
+pip install shell-gpt==0.8.7
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -257,15 +247,18 @@
 CACHE_LENGTH=100
 # Request cache folder.
 CACHE_PATH=/tmp/shell_gpt/cache
 # Request timeout in seconds.
 REQUEST_TIMEOUT=60
 # Default OpenAI model to use.
 DEFAULT_MODEL=gpt-3.5-turbo
+# Default color for OpenAI completions.
+DEFAULT_COLOR=magenta
 ```
+Possible options for `DEFAULT_COLOR`: black, red, green, yellow, blue, magenta, cyan, white, bright_black, bright_red, bright_green, bright_yellow, bright_blue, bright_magenta, bright_cyan, bright_white.
 
 ### Full list of arguments
 ```text
 ╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────╮
 │   prompt      [PROMPT]  The prompt to generate completions for.                                            │
 ╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────╮
```

### Comparing `shell_gpt-0.8.6/README.md` & `shell_gpt-0.8.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,27 @@
+Metadata-Version: 2.1
+Name: shell_gpt
+Version: 0.8.7
+Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
+Home-page: https://github.com/ther1d/shell_gpt
+Author: Farkhod Sadykov
+Author-email: farkhod@sadykov.dev
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Shell GPT
 A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.6
+pip install shell-gpt==0.8.7
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -247,15 +257,18 @@
 CACHE_LENGTH=100
 # Request cache folder.
 CACHE_PATH=/tmp/shell_gpt/cache
 # Request timeout in seconds.
 REQUEST_TIMEOUT=60
 # Default OpenAI model to use.
 DEFAULT_MODEL=gpt-3.5-turbo
+# Default color for OpenAI completions.
+DEFAULT_COLOR=magenta
 ```
+Possible options for `DEFAULT_COLOR`: black, red, green, yellow, blue, magenta, cyan, white, bright_black, bright_red, bright_green, bright_yellow, bright_blue, bright_magenta, bright_cyan, bright_white.
 
 ### Full list of arguments
 ```text
 ╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────╮
 │   prompt      [PROMPT]  The prompt to generate completions for.                                            │
 ╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────╮
```

### Comparing `shell_gpt-0.8.6/setup.py` & `shell_gpt-0.8.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # pylint: disable=consider-using-with
 setup(
     name="shell_gpt",
-    version="0.8.6",
+    version="0.8.7",
     packages=find_packages(),
     install_requires=[
         "typer~=0.7.0",
         "requests~=2.28.2",
         "rich==13.3.1",
         "distro~=1.8.0",
     ],
```

### Comparing `shell_gpt-0.8.6/sgpt/app.py` & `shell_gpt-0.8.7/sgpt/app.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.6/sgpt/cache.py` & `shell_gpt-0.8.7/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.6/sgpt/client.py` & `shell_gpt-0.8.7/sgpt/client.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.6/sgpt/handlers/chat_handler.py` & `shell_gpt-0.8.7/sgpt/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.6/sgpt/handlers/default_handler.py` & `shell_gpt-0.8.7/sgpt/handlers/default_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.6/sgpt/handlers/handler.py` & `shell_gpt-0.8.7/sgpt/handlers/handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import List, Dict, Generator
 
 import typer
 
 from sgpt import OpenAIClient
+from sgpt import config
 
 
 class Handler:
     def __init__(self, client: OpenAIClient) -> None:
         self.client = client
+        self.color = config.get("DEFAULT_COLOR")
 
     def make_prompt(self, prompt) -> str:
         raise NotImplementedError
 
     def get_completion(  # pylint: disable=too-many-arguments
         self,
         messages: List[Dict[str, str]],
@@ -29,11 +31,11 @@
         )
 
     def handle(self, prompt: str, **kwargs) -> str:
         prompt = self.make_prompt(prompt)
         messages = [{"role": "user", "content": prompt}]
         full_completion = ""
         for word in self.get_completion(messages=messages, **kwargs):
-            typer.secho(word, fg="magenta", bold=True, nl=False)
+            typer.secho(word, fg=self.color, bold=True, nl=False)
             full_completion += word
         typer.echo()
         return full_completion
```

### Comparing `shell_gpt-0.8.6/sgpt/handlers/repl_handler.py` & `shell_gpt-0.8.7/sgpt/handlers/repl_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.6/sgpt/make_prompt.py` & `shell_gpt-0.8.7/sgpt/make_prompt.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.6/sgpt/utils.py` & `shell_gpt-0.8.7/sgpt/utils.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.6/shell_gpt.egg-info/PKG-INFO` & `shell_gpt-0.8.7/shell_gpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-gpt
-Version: 0.8.6
+Version: 0.8.7
 Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
 Home-page: https://github.com/ther1d/shell_gpt
 Author: Farkhod Sadykov
 Author-email: farkhod@sadykov.dev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.6
+pip install shell-gpt==0.8.7
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -257,15 +257,18 @@
 CACHE_LENGTH=100
 # Request cache folder.
 CACHE_PATH=/tmp/shell_gpt/cache
 # Request timeout in seconds.
 REQUEST_TIMEOUT=60
 # Default OpenAI model to use.
 DEFAULT_MODEL=gpt-3.5-turbo
+# Default color for OpenAI completions.
+DEFAULT_COLOR=magenta
 ```
+Possible options for `DEFAULT_COLOR`: black, red, green, yellow, blue, magenta, cyan, white, bright_black, bright_red, bright_green, bright_yellow, bright_blue, bright_magenta, bright_cyan, bright_white.
 
 ### Full list of arguments
 ```text
 ╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────╮
 │   prompt      [PROMPT]  The prompt to generate completions for.                                            │
 ╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────╮
```


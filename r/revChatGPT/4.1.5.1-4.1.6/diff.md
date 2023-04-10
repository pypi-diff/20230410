# Comparing `tmp/revChatGPT-4.1.5.1.tar.gz` & `tmp/revChatGPT-4.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-4.1.5.1.tar", last modified: Sun Apr  9 16:38:42 2023, max compression
+gzip compressed data, was "revChatGPT-4.1.6.tar", last modified: Mon Apr 10 03:31:17 2023, max compression
```

## Comparing `revChatGPT-4.1.5.1.tar` & `revChatGPT-4.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:38:42.160083 revChatGPT-4.1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-04-09 16:38:42.160083 revChatGPT-4.1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-09 16:38:41.000000 revChatGPT-4.1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-09 16:38:42.160083 revChatGPT-4.1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:38:42.152083 revChatGPT-4.1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:38:42.156083 revChatGPT-4.1.5.1/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    34481 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:38:42.160083 revChatGPT-4.1.5.1/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:38:42.160083 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-04-09 16:38:42.000000 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-09 16:38:42.000000 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:38:42.000000 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 16:38:42.000000 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 16:38:42.000000 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:17.148262 revChatGPT-4.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-10 03:31:17.148262 revChatGPT-4.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-10 03:31:16.000000 revChatGPT-4.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 03:31:17.148262 revChatGPT-4.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:17.140262 revChatGPT-4.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:17.144262 revChatGPT-4.1.6/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    34518 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23144 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:17.148262 revChatGPT-4.1.6/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:17.148262 revChatGPT-4.1.6/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-10 03:31:17.000000 revChatGPT-4.1.6/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 03:31:17.000000 revChatGPT-4.1.6/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 03:31:17.000000 revChatGPT-4.1.6/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 03:31:17.000000 revChatGPT-4.1.6/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 03:31:17.000000 revChatGPT-4.1.6/src/revChatGPT.egg-info/top_level.txt
```

### Comparing `revChatGPT-4.1.5.1/LICENSE` & `revChatGPT-4.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5.1/PKG-INFO` & `revChatGPT-4.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.1.5.1
+Version: 4.1.6
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -29,64 +29,71 @@
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
 [![](./view.gif)](https://pypi.python.org/pypi/revChatGPT)
 
 > ## Support my work
+>
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
 
 > #### Discord Server: https://discord.gg/9K2BvbXEHT
 
 # Installation
 
 ```
 python -m pip install --upgrade revChatGPT
 ```
 
 ### Suport Python Version
+
 - Minimum - Python3.9
 - Recommend - Python3.11+
 
-
 <details>
 
 <summary>
 
 # V1 Standard ChatGPT
+
 > > 3:35 PM - Rate limit at 5 requests / 10 seconds due to small server (I ran out of budget.)
 
 > ### [Privacy policy](./PRIVACY.md)
+>
 > <br>
 
 > ### !!! Server is now open source at https://github.com/acheong08/ChatGPT-Proxy-V4 for personal use (requires ChatGPT plus)
 
 </summary>
 
 ## Configuration
 
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
-> *Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`*
-Not supported for Google/Microsoft accounts.
+
+> _Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`_
+> Not supported for Google/Microsoft accounts.
+
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
+
 https://chat.openai.com/api/auth/session
+
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
 
 #### - Optional configuration:
@@ -97,18 +104,19 @@
   "parent_id": "UUID...",
   "proxy": "...",
   "paid": false,
   "collect_analytics": true,
   "model": "gpt-4"
 }
 ```
+
 Analytics is disabled by default. Set `collect_analytics` to `true` to enable it.
 
 3. Save this as `$HOME/.config/revChatGPT/config.json`
-4. If you are using Windows, you will need to create an environment variable named ```HOME``` and set it to your home profile for the script to be able to locate the config.json file.
+4. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 ## Usage
 
 ### Command line
 
 `python3 -m revChatGPT.V1`
 
@@ -124,18 +132,18 @@
 (Press Esc followed by Enter to finish)
 ```
 
 The command line interface supports multi-line inputs and allows navigation using arrow keys. Besides, you can also edit history inputs by arrow keys when the prompt is empty. It also completes your input if it finds matched previous prompts. To finish input, press `Esc` and then `Enter` as solely `Enter` itself is used for creating new line in multi-line mode.
 
 Set the environment variable `NO_COLOR` to `true` to disable color output.
 
-
 ### Developer API
 
 #### Basic example (streamed):
+
 ```python
 from revChatGPT.V1 import Chatbot
 
 chatbot = Chatbot(config={
   "access_token": "<your access_token>"
 })
 
@@ -165,49 +173,52 @@
 for data in chatbot.ask(
   prompt
 ):
     response = data["message"]
 
 print(response)
 ```
+
 #### All API methods
+
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
-
 <details>
 
 <summary>
 
 # V3 Official Chat API
+
 > Recently released by OpenAI
+>
 > - Paid
 
 </summary>
 
 Get API key from https://platform.openai.com/account/api-keys
 
 ## Command line
+
 `python3 -m revChatGPT.V3 --api_key <api_key>`
 
 ```
- $ python3 -m revChatGPT.V3 -h
+  $ python3 -m revChatGPT.V3 --help
 
     ChatGPT - Official ChatGPT API
     Repo: github.com/acheong08/ChatGPT
 
 Type '!help' to show a full list of commands
 Press Esc followed by Enter or Alt+Enter to send a message.
 
-usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream]
-             [--base_prompt BASE_PROMPT] [--proxy PROXY] [--top_p TOP_P]
-             [--reply_count REPLY_COUNT] [--enable_internet] [--config CONFIG]
-             [--submit_key SUBMIT_KEY]
-             [--model {gpt-3.5-turbo,gpt-4,gpt-4-32k}]
+usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream] [--base_prompt BASE_PROMPT]
+             [--proxy PROXY] [--top_p TOP_P] [--reply_count REPLY_COUNT] [--enable_internet]
+             [--config CONFIG] [--submit_key SUBMIT_KEY] [--model {gpt-3.5-turbo,gpt-4,gpt-4-32k}]
+             [--truncate_limit TRUNCATE_LIMIT]
 
 options:
   -h, --help            show this help message and exit
   --api_key API_KEY     OpenAI API key
   --temperature TEMPERATURE
                         Temperature for response
   --no_stream           Disable streaming
@@ -216,28 +227,31 @@
   --proxy PROXY         Proxy address
   --top_p TOP_P         Top p for response
   --reply_count REPLY_COUNT
                         Number of replies for each prompt
   --enable_internet     Allow ChatGPT to search the internet
   --config CONFIG       Path to V3 config json file
   --submit_key SUBMIT_KEY
-                        Custom submit key for chatbot. For more information on keys, see https://python-prompt-toolkit.readthedocs.io/en/stable/pages/advanced_topics/key_bindings.html#list-of-special-keys
+                        Custom submit key for chatbot. For more information on keys, see README
   --model {gpt-3.5-turbo,gpt-4,gpt-4-32k}
+  --truncate_limit TRUNCATE_LIMIT
 ```
 
 ## Developer API
 
 ### Basic example
+
 ```python
 from revChatGPT.V3 import Chatbot
 chatbot = Chatbot(api_key="<api_key>")
 chatbot.ask("Hello world")
 ```
 
 ### Streaming example
+
 ```python
 from revChatGPT.V3 import Chatbot
 chatbot = Chatbot(api_key="<api_key>")
 for data in chatbot.ask_stream("Hello world"):
     print(data, end="", flush=True)
 ```
 
@@ -249,15 +263,14 @@
 
 If you have a cool project you want added to the list, open an issue.
 
 # Disclaimers
 
 This is not an official OpenAI product. This is a personal project and is not affiliated with OpenAI in any way. Don't sue me.
 
-
 ## Contributors
 
 This project exists thanks to all the people who contribute.
 
 <a href="https://github.com/acheong08/ChatGPT/graphs/contributors">
 <img src="https://contrib.rocks/image?repo=acheong08/ChatGPT" />
 </a>
```

### Comparing `revChatGPT-4.1.5.1/README.md` & `revChatGPT-4.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,64 +7,71 @@
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
 [![](./view.gif)](https://pypi.python.org/pypi/revChatGPT)
 
 > ## Support my work
+>
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
 
 > #### Discord Server: https://discord.gg/9K2BvbXEHT
 
 # Installation
 
 ```
 python -m pip install --upgrade revChatGPT
 ```
 
 ### Suport Python Version
+
 - Minimum - Python3.9
 - Recommend - Python3.11+
 
-
 <details>
 
 <summary>
 
 # V1 Standard ChatGPT
+
 > > 3:35 PM - Rate limit at 5 requests / 10 seconds due to small server (I ran out of budget.)
 
 > ### [Privacy policy](./PRIVACY.md)
+>
 > <br>
 
 > ### !!! Server is now open source at https://github.com/acheong08/ChatGPT-Proxy-V4 for personal use (requires ChatGPT plus)
 
 </summary>
 
 ## Configuration
 
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
-> *Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`*
-Not supported for Google/Microsoft accounts.
+
+> _Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`_
+> Not supported for Google/Microsoft accounts.
+
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
+
 https://chat.openai.com/api/auth/session
+
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
 
 #### - Optional configuration:
@@ -75,18 +82,19 @@
   "parent_id": "UUID...",
   "proxy": "...",
   "paid": false,
   "collect_analytics": true,
   "model": "gpt-4"
 }
 ```
+
 Analytics is disabled by default. Set `collect_analytics` to `true` to enable it.
 
 3. Save this as `$HOME/.config/revChatGPT/config.json`
-4. If you are using Windows, you will need to create an environment variable named ```HOME``` and set it to your home profile for the script to be able to locate the config.json file.
+4. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 ## Usage
 
 ### Command line
 
 `python3 -m revChatGPT.V1`
 
@@ -102,18 +110,18 @@
 (Press Esc followed by Enter to finish)
 ```
 
 The command line interface supports multi-line inputs and allows navigation using arrow keys. Besides, you can also edit history inputs by arrow keys when the prompt is empty. It also completes your input if it finds matched previous prompts. To finish input, press `Esc` and then `Enter` as solely `Enter` itself is used for creating new line in multi-line mode.
 
 Set the environment variable `NO_COLOR` to `true` to disable color output.
 
-
 ### Developer API
 
 #### Basic example (streamed):
+
 ```python
 from revChatGPT.V1 import Chatbot
 
 chatbot = Chatbot(config={
   "access_token": "<your access_token>"
 })
 
@@ -143,49 +151,52 @@
 for data in chatbot.ask(
   prompt
 ):
     response = data["message"]
 
 print(response)
 ```
+
 #### All API methods
+
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
-
 <details>
 
 <summary>
 
 # V3 Official Chat API
+
 > Recently released by OpenAI
+>
 > - Paid
 
 </summary>
 
 Get API key from https://platform.openai.com/account/api-keys
 
 ## Command line
+
 `python3 -m revChatGPT.V3 --api_key <api_key>`
 
 ```
- $ python3 -m revChatGPT.V3 -h
+  $ python3 -m revChatGPT.V3 --help
 
     ChatGPT - Official ChatGPT API
     Repo: github.com/acheong08/ChatGPT
 
 Type '!help' to show a full list of commands
 Press Esc followed by Enter or Alt+Enter to send a message.
 
-usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream]
-             [--base_prompt BASE_PROMPT] [--proxy PROXY] [--top_p TOP_P]
-             [--reply_count REPLY_COUNT] [--enable_internet] [--config CONFIG]
-             [--submit_key SUBMIT_KEY]
-             [--model {gpt-3.5-turbo,gpt-4,gpt-4-32k}]
+usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream] [--base_prompt BASE_PROMPT]
+             [--proxy PROXY] [--top_p TOP_P] [--reply_count REPLY_COUNT] [--enable_internet]
+             [--config CONFIG] [--submit_key SUBMIT_KEY] [--model {gpt-3.5-turbo,gpt-4,gpt-4-32k}]
+             [--truncate_limit TRUNCATE_LIMIT]
 
 options:
   -h, --help            show this help message and exit
   --api_key API_KEY     OpenAI API key
   --temperature TEMPERATURE
                         Temperature for response
   --no_stream           Disable streaming
@@ -194,28 +205,31 @@
   --proxy PROXY         Proxy address
   --top_p TOP_P         Top p for response
   --reply_count REPLY_COUNT
                         Number of replies for each prompt
   --enable_internet     Allow ChatGPT to search the internet
   --config CONFIG       Path to V3 config json file
   --submit_key SUBMIT_KEY
-                        Custom submit key for chatbot. For more information on keys, see https://python-prompt-toolkit.readthedocs.io/en/stable/pages/advanced_topics/key_bindings.html#list-of-special-keys
+                        Custom submit key for chatbot. For more information on keys, see README
   --model {gpt-3.5-turbo,gpt-4,gpt-4-32k}
+  --truncate_limit TRUNCATE_LIMIT
 ```
 
 ## Developer API
 
 ### Basic example
+
 ```python
 from revChatGPT.V3 import Chatbot
 chatbot = Chatbot(api_key="<api_key>")
 chatbot.ask("Hello world")
 ```
 
 ### Streaming example
+
 ```python
 from revChatGPT.V3 import Chatbot
 chatbot = Chatbot(api_key="<api_key>")
 for data in chatbot.ask_stream("Hello world"):
     print(data, end="", flush=True)
 ```
 
@@ -227,15 +241,14 @@
 
 If you have a cool project you want added to the list, open an issue.
 
 # Disclaimers
 
 This is not an official OpenAI product. This is a personal project and is not affiliated with OpenAI in any way. Don't sue me.
 
-
 ## Contributors
 
 This project exists thanks to all the people who contribute.
 
 <a href="https://github.com/acheong08/ChatGPT/graphs/contributors">
 <img src="https://contrib.rocks/image?repo=acheong08/ChatGPT" />
 </a>
```

### Comparing `revChatGPT-4.1.5.1/setup.py` & `revChatGPT-4.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="4.1.5.1",
+    version="4.1.6",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-4.1.5.1/src/revChatGPT/V1.py` & `revChatGPT-4.1.6/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 import json
 import logging
 import time
 import uuid
 from functools import wraps
 from os import environ
 from os import getenv
+from pathlib import Path
 from typing import NoReturn
 
 import requests
-from pathlib import Path
 from httpx import AsyncClient
 from OpenAIAuth import Authenticator
 from OpenAIAuth import Error as AuthError
 
 from . import typings as t
 from .utils import create_completer
 from .utils import create_session
@@ -105,14 +105,15 @@
             session_client (_type_, optional): _description_. Defaults to None.
 
         Raises:
             Exception: _description_
         """
         user_home = getenv("HOME")
         if user_home is None:
+            user_home = Path().cwd()
             self.cache_path = Path(Path().cwd(), ".chatgpt_cache.json")
         else:
             # mkdir ~/.config/revChatGPT
             if not Path(user_home, ".config").exists():
                 Path(user_home, ".config").mkdir()
             if not Path(user_home, ".config", "revChatGPT").exists():
                 Path(user_home, ".config", "revChatGPT").mkdir()
```

### Comparing `revChatGPT-4.1.5.1/src/revChatGPT/V3.py` & `revChatGPT-4.1.6/src/revChatGPT/V3.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,26 +35,27 @@
         timeout: float = None,
         max_tokens: int = None,
         temperature: float = 0.5,
         top_p: float = 1.0,
         presence_penalty: float = 0.0,
         frequency_penalty: float = 0.0,
         reply_count: int = 1,
+        truncate_limit: int = None,
         system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
     ) -> None:
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
         self.engine: str = engine
         self.api_key: str = api_key
         self.system_prompt: str = system_prompt
         self.max_tokens: int = max_tokens or (
             31000 if engine == "gpt-4-32k" else 7000 if engine == "gpt-4" else 4000
         )
-        self.truncate_limit: int = (
+        self.truncate_limit: int = truncate_limit or (
             30500 if engine == "gpt-4-32k" else 6500 if engine == "gpt-4" else 3500
         )
         self.temperature: float = temperature
         self.top_p: float = top_p
         self.presence_penalty: float = presence_penalty
         self.frequency_penalty: float = frequency_penalty
         self.reply_count: int = reply_count
@@ -582,14 +583,20 @@
     parser.add_argument(
         "--model",
         type=str,
         default="gpt-3.5-turbo",
         choices=["gpt-3.5-turbo", "gpt-4", "gpt-4-32k"],
     )
 
+    parser.add_argument(
+        "--truncate_limit",
+        type=int,
+        default=None,
+    )
+
     args, _ = parser.parse_known_args()
 
     # Initialize chatbot
     if config := args.config or os.environ.get("GPT_CONFIG_PATH"):
         chatbot = ChatbotCLI(args.api_key)
         try:
             chatbot.load(config)
@@ -601,14 +608,15 @@
             api_key=args.api_key,
             system_prompt=args.base_prompt,
             proxy=args.proxy,
             temperature=args.temperature,
             top_p=args.top_p,
             reply_count=args.reply_count,
             engine=args.model,
+            truncate_limit=args.truncate_limit,
         )
     # Check if internet is enabled
     if args.enable_internet:
         config = path("revChatGPT", "config").__str__()
         chatbot.load(Path(config, "enable_internet.json"), "conversation")
 
     session = create_session()
```

### Comparing `revChatGPT-4.1.5.1/src/revChatGPT/__init__.py` & `revChatGPT-4.1.6/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5.1/src/revChatGPT/__main__.py` & `revChatGPT-4.1.6/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5.1/src/revChatGPT/config/enable_internet.json` & `revChatGPT-4.1.6/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5.1/src/revChatGPT/typings.py` & `revChatGPT-4.1.6/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5.1/src/revChatGPT/utils.py` & `revChatGPT-4.1.6/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5.1/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-4.1.6/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.1.5.1
+Version: 4.1.6
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -29,64 +29,71 @@
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
 [![](./view.gif)](https://pypi.python.org/pypi/revChatGPT)
 
 > ## Support my work
+>
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
 
 > #### Discord Server: https://discord.gg/9K2BvbXEHT
 
 # Installation
 
 ```
 python -m pip install --upgrade revChatGPT
 ```
 
 ### Suport Python Version
+
 - Minimum - Python3.9
 - Recommend - Python3.11+
 
-
 <details>
 
 <summary>
 
 # V1 Standard ChatGPT
+
 > > 3:35 PM - Rate limit at 5 requests / 10 seconds due to small server (I ran out of budget.)
 
 > ### [Privacy policy](./PRIVACY.md)
+>
 > <br>
 
 > ### !!! Server is now open source at https://github.com/acheong08/ChatGPT-Proxy-V4 for personal use (requires ChatGPT plus)
 
 </summary>
 
 ## Configuration
 
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
-> *Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`*
-Not supported for Google/Microsoft accounts.
+
+> _Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`_
+> Not supported for Google/Microsoft accounts.
+
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
+
 https://chat.openai.com/api/auth/session
+
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
 
 #### - Optional configuration:
@@ -97,18 +104,19 @@
   "parent_id": "UUID...",
   "proxy": "...",
   "paid": false,
   "collect_analytics": true,
   "model": "gpt-4"
 }
 ```
+
 Analytics is disabled by default. Set `collect_analytics` to `true` to enable it.
 
 3. Save this as `$HOME/.config/revChatGPT/config.json`
-4. If you are using Windows, you will need to create an environment variable named ```HOME``` and set it to your home profile for the script to be able to locate the config.json file.
+4. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 ## Usage
 
 ### Command line
 
 `python3 -m revChatGPT.V1`
 
@@ -124,18 +132,18 @@
 (Press Esc followed by Enter to finish)
 ```
 
 The command line interface supports multi-line inputs and allows navigation using arrow keys. Besides, you can also edit history inputs by arrow keys when the prompt is empty. It also completes your input if it finds matched previous prompts. To finish input, press `Esc` and then `Enter` as solely `Enter` itself is used for creating new line in multi-line mode.
 
 Set the environment variable `NO_COLOR` to `true` to disable color output.
 
-
 ### Developer API
 
 #### Basic example (streamed):
+
 ```python
 from revChatGPT.V1 import Chatbot
 
 chatbot = Chatbot(config={
   "access_token": "<your access_token>"
 })
 
@@ -165,49 +173,52 @@
 for data in chatbot.ask(
   prompt
 ):
     response = data["message"]
 
 print(response)
 ```
+
 #### All API methods
+
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
-
 <details>
 
 <summary>
 
 # V3 Official Chat API
+
 > Recently released by OpenAI
+>
 > - Paid
 
 </summary>
 
 Get API key from https://platform.openai.com/account/api-keys
 
 ## Command line
+
 `python3 -m revChatGPT.V3 --api_key <api_key>`
 
 ```
- $ python3 -m revChatGPT.V3 -h
+  $ python3 -m revChatGPT.V3 --help
 
     ChatGPT - Official ChatGPT API
     Repo: github.com/acheong08/ChatGPT
 
 Type '!help' to show a full list of commands
 Press Esc followed by Enter or Alt+Enter to send a message.
 
-usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream]
-             [--base_prompt BASE_PROMPT] [--proxy PROXY] [--top_p TOP_P]
-             [--reply_count REPLY_COUNT] [--enable_internet] [--config CONFIG]
-             [--submit_key SUBMIT_KEY]
-             [--model {gpt-3.5-turbo,gpt-4,gpt-4-32k}]
+usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream] [--base_prompt BASE_PROMPT]
+             [--proxy PROXY] [--top_p TOP_P] [--reply_count REPLY_COUNT] [--enable_internet]
+             [--config CONFIG] [--submit_key SUBMIT_KEY] [--model {gpt-3.5-turbo,gpt-4,gpt-4-32k}]
+             [--truncate_limit TRUNCATE_LIMIT]
 
 options:
   -h, --help            show this help message and exit
   --api_key API_KEY     OpenAI API key
   --temperature TEMPERATURE
                         Temperature for response
   --no_stream           Disable streaming
@@ -216,28 +227,31 @@
   --proxy PROXY         Proxy address
   --top_p TOP_P         Top p for response
   --reply_count REPLY_COUNT
                         Number of replies for each prompt
   --enable_internet     Allow ChatGPT to search the internet
   --config CONFIG       Path to V3 config json file
   --submit_key SUBMIT_KEY
-                        Custom submit key for chatbot. For more information on keys, see https://python-prompt-toolkit.readthedocs.io/en/stable/pages/advanced_topics/key_bindings.html#list-of-special-keys
+                        Custom submit key for chatbot. For more information on keys, see README
   --model {gpt-3.5-turbo,gpt-4,gpt-4-32k}
+  --truncate_limit TRUNCATE_LIMIT
 ```
 
 ## Developer API
 
 ### Basic example
+
 ```python
 from revChatGPT.V3 import Chatbot
 chatbot = Chatbot(api_key="<api_key>")
 chatbot.ask("Hello world")
 ```
 
 ### Streaming example
+
 ```python
 from revChatGPT.V3 import Chatbot
 chatbot = Chatbot(api_key="<api_key>")
 for data in chatbot.ask_stream("Hello world"):
     print(data, end="", flush=True)
 ```
 
@@ -249,15 +263,14 @@
 
 If you have a cool project you want added to the list, open an issue.
 
 # Disclaimers
 
 This is not an official OpenAI product. This is a personal project and is not affiliated with OpenAI in any way. Don't sue me.
 
-
 ## Contributors
 
 This project exists thanks to all the people who contribute.
 
 <a href="https://github.com/acheong08/ChatGPT/graphs/contributors">
 <img src="https://contrib.rocks/image?repo=acheong08/ChatGPT" />
 </a>
```


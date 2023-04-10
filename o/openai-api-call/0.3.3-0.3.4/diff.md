# Comparing `tmp/openai_api_call-0.3.3.tar.gz` & `tmp/openai_api_call-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.3.3.tar", last modified: Fri Mar 31 06:38:39 2023, max compression
+gzip compressed data, was "openai_api_call-0.3.4.tar", last modified: Mon Apr 10 08:31:09 2023, max compression
```

## Comparing `openai_api_call-0.3.3.tar` & `openai_api_call-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:38:39.869632 openai_api_call-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-31 06:38:31.000000 openai_api_call-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-03-31 06:38:39.869632 openai_api_call-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-03-31 06:38:31.000000 openai_api_call-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:38:39.869632 openai_api_call-0.3.3/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-31 06:38:31.000000 openai_api_call-0.3.3/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-03-31 06:38:31.000000 openai_api_call-0.3.3/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-31 06:38:31.000000 openai_api_call-0.3.3/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-03-31 06:38:31.000000 openai_api_call-0.3.3/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-31 06:38:31.000000 openai_api_call-0.3.3/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-03-31 06:38:31.000000 openai_api_call-0.3.3/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:38:39.869632 openai_api_call-0.3.3/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-03-31 06:38:39.000000 openai_api_call-0.3.3/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-31 06:38:39.000000 openai_api_call-0.3.3/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 06:38:39.000000 openai_api_call-0.3.3/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-31 06:38:39.000000 openai_api_call-0.3.3/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 06:38:39.000000 openai_api_call-0.3.3/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-31 06:38:39.000000 openai_api_call-0.3.3/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 06:38:39.000000 openai_api_call-0.3.3/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 06:38:39.869632 openai_api_call-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-31 06:38:31.000000 openai_api_call-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:31:09.677534 openai_api_call-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-10 08:31:09.677534 openai_api_call-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:31:09.677534 openai_api_call-0.3.4/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:31:09.677534 openai_api_call-0.3.4/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:31:09.677534 openai_api_call-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/setup.py
```

### Comparing `openai_api_call-0.3.3/LICENSE` & `openai_api_call-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.3/PKG-INFO` & `openai_api_call-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.3.3
+Version: 0.3.4
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/RexWzh/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -13,34 +13,32 @@
         [![Tests](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/)
         [![Documentation Status](https://img.shields.io/badge/docs-github_pages-blue.svg)](https://apicall.wzhecnu.cn)
         
         <!-- 
         [![Updates](https://pyup.io/repos/github/RexWzh/openai_api_call/shield.svg)](https://pyup.io/repos/github/RexWzh/openai_api_call/) 
         -->
         
-        A simple wrapper for OpenAI API, which can send prompt message and return response.
+        A simple wrapper for OpenAI API, which can be used to send requests and get responses.
         
         ## Installation
         
         ```bash
         pip install openai-api-call --upgrade
         ```
         
-        > Note: Since version `0.2.0`, `Chat` type is used to handle data, which is not compatible with previous versions.
-        
         ## Usage
         
         ### Set API Key
         
         ```py
-        import openai_api_call
-        openai_api_call.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+        import openai_api_call as apicall
+        apicall.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         ```
         
-        Or set `OPENAI_API_KEY` in `~/.bashrc` to automatically set it when you start the terminal:
+        Or set `OPENAI_API_KEY` in `~/.bashrc` to avoid setting the API key every time:
         
         ```bash
         # Add the following code to ~/.bashrc
         export OPENAI_API_KEY="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         ```
         
         ### Set Proxy (Optional)
@@ -56,17 +54,27 @@
         # Check the updated proxy
         proxy_status()
         
         # Turn off proxy
         proxy_off() 
         ```
         
+        Alternatively, you can use a proxy URL to send requests from restricted network, as shown below:
+        
+        ```py
+        from openai_api_call import request
+        
+        # set request url
+        alt_url = "https://api.example.com/v1/chat/completions"
+        request.url = alt_url
+        ```
+        
         ### Basic Usage
         
-        Example 1, send prompt and return information:
+        Example 1, send prompt and return response:
         
         ```python
         from openai_api_call import Chat, show_apikey
         
         # Check if API key is set
         show_apikey()
         
@@ -77,18 +85,18 @@
         chat = Chat("Hello, GPT-3.5!")
         resp = chat.getresponse(update=False) # Not update the chat history, default to True
         ```
         
         Example 2, customize the message template and return the information and the number of consumed tokens:
         
         ```python
-        import openai_api_call
+        import openai_api_call as apicall
         
         # Customize the sending template
-        openai_api_call.default_prompt = lambda msg: [
+        apicall.default_prompt = lambda msg: [
             {"role": "system", "content": "帮我翻译这段文字"},
             {"role": "user", "content": msg}
         ]
         chat = Chat("Hello!")
         # Set the number of retries to Inf
         # The timeout for each request is 10 seconds
         response = chat.getresponse(temperature=0.5, max_requests=-1, timeout=10)
@@ -111,14 +119,17 @@
         next_resp = chat.getresponse()
         print(next_resp.content)
         
         # fake response
         chat.user("What's your name?")
         chat.assistant("My name is GPT-3.5.")
         
+        # get the last result
+        print(chat[-1])
+        
         # print chat history
         chat.print_log()
         ```
         
         ## License
         
         This package is licensed under the MIT license. See the LICENSE file for more details.
```

### Comparing `openai_api_call-0.3.3/README.md` & `openai_api_call-0.3.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,34 +5,32 @@
 [![Tests](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/)
 [![Documentation Status](https://img.shields.io/badge/docs-github_pages-blue.svg)](https://apicall.wzhecnu.cn)
 
 <!-- 
 [![Updates](https://pyup.io/repos/github/RexWzh/openai_api_call/shield.svg)](https://pyup.io/repos/github/RexWzh/openai_api_call/) 
 -->
 
-A simple wrapper for OpenAI API, which can send prompt message and return response.
+A simple wrapper for OpenAI API, which can be used to send requests and get responses.
 
 ## Installation
 
 ```bash
 pip install openai-api-call --upgrade
 ```
 
-> Note: Since version `0.2.0`, `Chat` type is used to handle data, which is not compatible with previous versions.
-
 ## Usage
 
 ### Set API Key
 
 ```py
-import openai_api_call
-openai_api_call.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+import openai_api_call as apicall
+apicall.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
 ```
 
-Or set `OPENAI_API_KEY` in `~/.bashrc` to automatically set it when you start the terminal:
+Or set `OPENAI_API_KEY` in `~/.bashrc` to avoid setting the API key every time:
 
 ```bash
 # Add the following code to ~/.bashrc
 export OPENAI_API_KEY="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
 ```
 
 ### Set Proxy (Optional)
@@ -48,17 +46,27 @@
 # Check the updated proxy
 proxy_status()
 
 # Turn off proxy
 proxy_off() 
 ```
 
+Alternatively, you can use a proxy URL to send requests from restricted network, as shown below:
+
+```py
+from openai_api_call import request
+
+# set request url
+alt_url = "https://api.example.com/v1/chat/completions"
+request.url = alt_url
+```
+
 ### Basic Usage
 
-Example 1, send prompt and return information:
+Example 1, send prompt and return response:
 
 ```python
 from openai_api_call import Chat, show_apikey
 
 # Check if API key is set
 show_apikey()
 
@@ -69,18 +77,18 @@
 chat = Chat("Hello, GPT-3.5!")
 resp = chat.getresponse(update=False) # Not update the chat history, default to True
 ```
 
 Example 2, customize the message template and return the information and the number of consumed tokens:
 
 ```python
-import openai_api_call
+import openai_api_call as apicall
 
 # Customize the sending template
-openai_api_call.default_prompt = lambda msg: [
+apicall.default_prompt = lambda msg: [
     {"role": "system", "content": "帮我翻译这段文字"},
     {"role": "user", "content": msg}
 ]
 chat = Chat("Hello!")
 # Set the number of retries to Inf
 # The timeout for each request is 10 seconds
 response = chat.getresponse(temperature=0.5, max_requests=-1, timeout=10)
@@ -103,14 +111,17 @@
 next_resp = chat.getresponse()
 print(next_resp.content)
 
 # fake response
 chat.user("What's your name?")
 chat.assistant("My name is GPT-3.5.")
 
+# get the last result
+print(chat[-1])
+
 # print chat history
 chat.print_log()
 ```
 
 ## License
 
 This package is licensed under the MIT license. See the LICENSE file for more details.
```

### Comparing `openai_api_call-0.3.3/openai_api_call/__init__.py` & `openai_api_call-0.3.4/openai_api_call/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 
 import os
 from .chattool import Chat, Resp, chat_completion
 from .proxy import proxy_on, proxy_off, proxy_status
 
 # read API key from the environment variable
 if os.environ.get('OPENAI_API_KEY') is not None:
```

### Comparing `openai_api_call-0.3.3/openai_api_call/chattool.py` & `openai_api_call-0.3.4/openai_api_call/chattool.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,14 +73,15 @@
                 # Set the alarm to trigger after `timeout` seconds
                 signal.alarm(timeout)
                 # Make the API call
                 response = chat_completion(
                     api_key=api_key, messages=msg, model=model, **options)
                 time.sleep(random.random() * timeinterval)
                 resp = Resp(response, strip=strip)
+                assert resp.is_valid(), "Invalid response with message: " + resp.error_message
                 break
             except Exception as e:
                 max_requests -= 1
                 numoftries += 1
                 print(f"API call failed with message: {e}\nTry again ({numoftries})")
             finally:
                 # Disable the alarm after execution
@@ -124,18 +125,18 @@
             print(sep, d['role'], sep, d['content'])
     
     @property
     def chat_log(self):
         """Chat history"""
         return self._chat_log
     
-    def pop(self):
+    def pop(self, ind:int=-1):
         """Pop the last message"""
-        return self._chat_log.pop()
-    
+        return self._chat_log.pop(ind)
+
     def __len__(self):
         """Length of the chat log"""
         return len(self._chat_log)
     
     def __repr__(self) -> str:
         return f"<Chat with {len(self)} messages>"
```

### Comparing `openai_api_call-0.3.3/openai_api_call/proxy.py` & `openai_api_call-0.3.4/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.3/openai_api_call/request.py` & `openai_api_call-0.3.4/openai_api_call/request.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.3/openai_api_call/response.py` & `openai_api_call-0.3.4/openai_api_call/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     
     @property
     def created(self):
         return self.response['created']
     
     def is_valid(self):
         """Check if the response is an error"""
-        return 'error' not in self.response
+        return 'error' not in self.response and 'choices' in self.response
     
     @property
     def error_message(self):
         """Error message"""
         return self.response['error']['message']
     
     @property
```

### Comparing `openai_api_call-0.3.3/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.3.4/openai_api_call.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.3.3
+Version: 0.3.4
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/RexWzh/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -13,34 +13,32 @@
         [![Tests](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/)
         [![Documentation Status](https://img.shields.io/badge/docs-github_pages-blue.svg)](https://apicall.wzhecnu.cn)
         
         <!-- 
         [![Updates](https://pyup.io/repos/github/RexWzh/openai_api_call/shield.svg)](https://pyup.io/repos/github/RexWzh/openai_api_call/) 
         -->
         
-        A simple wrapper for OpenAI API, which can send prompt message and return response.
+        A simple wrapper for OpenAI API, which can be used to send requests and get responses.
         
         ## Installation
         
         ```bash
         pip install openai-api-call --upgrade
         ```
         
-        > Note: Since version `0.2.0`, `Chat` type is used to handle data, which is not compatible with previous versions.
-        
         ## Usage
         
         ### Set API Key
         
         ```py
-        import openai_api_call
-        openai_api_call.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+        import openai_api_call as apicall
+        apicall.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         ```
         
-        Or set `OPENAI_API_KEY` in `~/.bashrc` to automatically set it when you start the terminal:
+        Or set `OPENAI_API_KEY` in `~/.bashrc` to avoid setting the API key every time:
         
         ```bash
         # Add the following code to ~/.bashrc
         export OPENAI_API_KEY="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         ```
         
         ### Set Proxy (Optional)
@@ -56,17 +54,27 @@
         # Check the updated proxy
         proxy_status()
         
         # Turn off proxy
         proxy_off() 
         ```
         
+        Alternatively, you can use a proxy URL to send requests from restricted network, as shown below:
+        
+        ```py
+        from openai_api_call import request
+        
+        # set request url
+        alt_url = "https://api.example.com/v1/chat/completions"
+        request.url = alt_url
+        ```
+        
         ### Basic Usage
         
-        Example 1, send prompt and return information:
+        Example 1, send prompt and return response:
         
         ```python
         from openai_api_call import Chat, show_apikey
         
         # Check if API key is set
         show_apikey()
         
@@ -77,18 +85,18 @@
         chat = Chat("Hello, GPT-3.5!")
         resp = chat.getresponse(update=False) # Not update the chat history, default to True
         ```
         
         Example 2, customize the message template and return the information and the number of consumed tokens:
         
         ```python
-        import openai_api_call
+        import openai_api_call as apicall
         
         # Customize the sending template
-        openai_api_call.default_prompt = lambda msg: [
+        apicall.default_prompt = lambda msg: [
             {"role": "system", "content": "帮我翻译这段文字"},
             {"role": "user", "content": msg}
         ]
         chat = Chat("Hello!")
         # Set the number of retries to Inf
         # The timeout for each request is 10 seconds
         response = chat.getresponse(temperature=0.5, max_requests=-1, timeout=10)
@@ -111,14 +119,17 @@
         next_resp = chat.getresponse()
         print(next_resp.content)
         
         # fake response
         chat.user("What's your name?")
         chat.assistant("My name is GPT-3.5.")
         
+        # get the last result
+        print(chat[-1])
+        
         # print chat history
         chat.print_log()
         ```
         
         ## License
         
         This package is licensed under the MIT license. See the LICENSE file for more details.
```

### Comparing `openai_api_call-0.3.3/setup.py` & `openai_api_call-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.3.3'
+VERSION = '0.3.4'
 
 requirements = ['Click>=7.0', 'requests>=2.20']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
```


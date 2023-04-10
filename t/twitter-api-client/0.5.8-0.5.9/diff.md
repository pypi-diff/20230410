# Comparing `tmp/twitter-api-client-0.5.8.tar.gz` & `tmp/twitter-api-client-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.5.8.tar", last modified: Fri Apr  7 23:59:01 2023, max compression
+gzip compressed data, was "twitter-api-client-0.5.9.tar", last modified: Mon Apr 10 18:45:23 2023, max compression
```

## Comparing `twitter-api-client-0.5.8.tar` & `twitter-api-client-0.5.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-07 23:59:01.255188 twitter-api-client-0.5.8/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-07 23:06:22.000000 twitter-api-client-0.5.8/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6087 2023-04-07 23:59:01.255188 twitter-api-client-0.5.8/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-07 23:59:01.255188 twitter-api-client-0.5.8/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     7056 2023-04-07 23:58:41.000000 twitter-api-client-0.5.8/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-07 23:59:01.254188 twitter-api-client-0.5.8/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.5.8/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    22554 2023-04-07 23:51:36.000000 twitter-api-client-0.5.8/twitter/account.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-07 23:59:01.254188 twitter-api-client-0.5.8/twitter/config/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.5.8/twitter/config/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)      909 2023-04-07 23:06:22.000000 twitter-api-client-0.5.8/twitter/config/log.py
--rw-r--r--   0 x         (1000) x         (1000)   148071 2023-04-07 23:06:22.000000 twitter-api-client-0.5.8/twitter/config/operations.py
--rw-r--r--   0 x         (1000) x         (1000)     5858 2023-04-07 23:06:22.000000 twitter-api-client-0.5.8/twitter/config/settings.py
--rw-r--r--   0 x         (1000) x         (1000)     2432 2023-04-07 23:06:22.000000 twitter-api-client-0.5.8/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     3984 2023-04-07 23:06:22.000000 twitter-api-client-0.5.8/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    12640 2023-04-07 23:57:38.000000 twitter-api-client-0.5.8/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5035 2023-04-07 23:06:22.000000 twitter-api-client-0.5.8/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     2235 2023-04-07 23:06:22.000000 twitter-api-client-0.5.8/twitter/utils.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-07 23:59:01.255188 twitter-api-client-0.5.8/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6087 2023-04-07 23:59:01.000000 twitter-api-client-0.5.8/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      461 2023-04-07 23:59:01.000000 twitter-api-client-0.5.8/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-07 23:59:01.000000 twitter-api-client-0.5.8/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       82 2023-04-07 23:59:01.000000 twitter-api-client-0.5.8/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-07 23:59:01.000000 twitter-api-client-0.5.8/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 18:45:23.827640 twitter-api-client-0.5.9/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-10 18:45:23.827640 twitter-api-client-0.5.9/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-10 18:45:23.827640 twitter-api-client-0.5.9/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     7094 2023-04-10 18:45:10.000000 twitter-api-client-0.5.9/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 18:45:23.825640 twitter-api-client-0.5.9/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    22979 2023-04-10 18:34:38.000000 twitter-api-client-0.5.9/twitter/account.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 18:45:23.826640 twitter-api-client-0.5.9/twitter/config/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/config/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)      909 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/config/log.py
+-rw-r--r--   0 x         (1000) x         (1000)   148071 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/config/operations.py
+-rw-r--r--   0 x         (1000) x         (1000)     5858 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/config/settings.py
+-rw-r--r--   0 x         (1000) x         (1000)     2456 2023-04-10 18:10:09.000000 twitter-api-client-0.5.9/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5001 2023-04-10 18:35:58.000000 twitter-api-client-0.5.9/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    12811 2023-04-10 18:38:31.000000 twitter-api-client-0.5.9/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     5035 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     2235 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/utils.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 18:45:23.827640 twitter-api-client-0.5.9/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-10 18:45:23.000000 twitter-api-client-0.5.9/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      461 2023-04-10 18:45:23.000000 twitter-api-client-0.5.9/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-10 18:45:23.000000 twitter-api-client-0.5.9/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       82 2023-04-10 18:45:23.000000 twitter-api-client-0.5.9/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-10 18:45:23.000000 twitter-api-client-0.5.9/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.5.8/LICENSE` & `twitter-api-client-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.8/PKG-INFO` & `twitter-api-client-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.5.8
+Version: 0.5.9
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
@@ -16,16 +16,16 @@
  Includes tools to **scrape**, **automate**, and **search** twitter
 
  ### Installation
 
 ```python
  from twitter.account import Account
 
- username, password = ..., ...
- account = Account(username, password)
+ email, username, password = ..., ..., ...
+ account = Account(email, username, password)
 
  account.create_poll('test poll 123', ['hello', 'world', 'foo', 'bar'], 10080)
 
  # DM 1 user
  account.dm([123], 'hello world', filename='test.png')
 
  # DM group of users
@@ -156,16 +156,16 @@
  ### Scraping
 
  #### Get all user/tweet data
 
  ```python
  from twitter.scraper import Scraper
 
- username, password = ..., ...
- scraper = Scraper(username, password)  # session
+ email, username, password = ..., ..., ...
+ scraper = Scraper(email, username, password)  # session
 
  ####### User Data ########
  users = scraper.user_by_screen_name(['bob123', 'jim456', 'stanley789'])
  tweets = scraper.tweets([123, 234, 345])
  likes = scraper.likes([123, 234, 345])
  tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
  media = scraper.media([123, 234, 345])
```

### Comparing `twitter-api-client-0.5.8/setup.py` & `twitter-api-client-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.5.8",
+    version="0.5.9",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
     
     ### Installation
     
    ```python
     from twitter.account import Account
     
-    username, password = ..., ...
-    account = Account(username, password)
+    email, username, password = ..., ..., ...
+    account = Account(email, username, password)
     
     account.create_poll('test poll 123', ['hello', 'world', 'foo', 'bar'], 10080)
     
     # DM 1 user
     account.dm([123], 'hello world', filename='test.png')
     
     # DM group of users
@@ -162,16 +162,16 @@
     ### Scraping
     
     #### Get all user/tweet data
     
     ```python
     from twitter.scraper import Scraper
     
-    username, password = ..., ...
-    scraper = Scraper(username, password)  # session
+    email, username, password = ..., ..., ...
+    scraper = Scraper(email, username, password)  # session
     
     ####### User Data ########
     users = scraper.user_by_screen_name(['bob123', 'jim456', 'stanley789'])
     tweets = scraper.tweets([123, 234, 345])
     likes = scraper.likes([123, 234, 345])
     tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
     media = scraper.media([123, 234, 345])
```

### Comparing `twitter-api-client-0.5.8/twitter/account.py` & `twitter-api-client-0.5.9/twitter/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import hashlib
 import inspect
 import logging.config
 import mimetypes
 import platform
 import random
+import re
 import time
 from copy import deepcopy
 from datetime import datetime
 from functools import wraps, partial
 from pathlib import Path
 from urllib.parse import urlencode
 from uuid import uuid1, getnode
@@ -58,42 +59,48 @@
         limits = {k: v for k, v in r.headers.items() if 'x-rate-limit' in k}
         current_time = int(time.time())
         wait = int(r.headers.get('x-rate-limit-reset', current_time)) - current_time
         logger.log(level, f'{wait // 60} minutes until rate-limit reset. {limits = }')
 
         try:
             if 200 <= r.status_code < 300:
-                message = f'[{SUCCESS}SUCCESS{RESET}] {r.status_code} ({BOLD}{fn.__name__}{RESET}) {args_info}'
+                typenames = find_key(r.json(), '__typename')
+                errors = ','.join([t for t in typenames if re.search('fail|error', t, flags=re.I)])
+                if errors:
+                    message = f'[{ERROR}error{RESET}] {r.status_code} ({BOLD}{fn.__name__}{RESET}) {args_info} {WARN}{errors}{RESET}'
+                else:
+                    message = f'[{SUCCESS}success{RESET}] {r.status_code} ({BOLD}{fn.__name__}{RESET}) {args_info}'
+
                 if info:
                     for k in info:
                         if callable(k):
                             logger.log(level, f'{message} {k(r)}')
                         else:
                             attr = getattr(r, k)
                             v = attr() if callable(attr) else attr
                             d = {f"{k}": v}
                             logger.log(level, f'{message} {d}')
                 else:
                     logger.log(level, f'{message}')
             else:
-                logger.log(level, f'[{WARN}ERROR{RESET}] ({fn.__name__}) {args_info} {r.status_code} {r.text}')
+                logger.log(level, f'[{ERROR}error{RESET}] ({fn.__name__}) {args_info} {r.status_code} {r.text}')
         except Exception as e:
-            logger.log(level, f'[{WARN}FAILED{RESET}] ({fn.__name__}) {args_info} {r.status_code} {e}')
+            logger.log(level, f'[{ERROR}error{RESET}] ({fn.__name__}) {args_info} {r.status_code} {e}')
         return r
 
     return wrapper
 
 
 class Account:
     V1_URL = 'https://api.twitter.com/1.1'
     V2_URL = 'https://api.twitter.com/2'  # /search
     GRAPHQL_URL = 'https://api.twitter.com/graphql'
 
-    def __init__(self, username: str, password: str):
-        self.session = login(username, password)
+    def __init__(self, email: str, username: str, password: str):
+        self.session = login(email, username, password)
 
     def gql(self, operation: tuple, variables: dict) -> Response:
         name, _ = operation
         payload = deepcopy(operations[name])
         qid = payload['queryId']
         payload['variables'] |= variables
         url = f"{self.GRAPHQL_URL}/{qid}/{name}"
@@ -243,15 +250,15 @@
                 i = 0
                 while chunk := f.read(UPLOAD_CHUNK_SIZE):  # todo: arbitrary max size for now
                     data = {'command': 'APPEND', 'media_id': media_id, 'segment_index': i}
                     files = {'media': chunk}
                     r = self.session.post(url=url, headers=headers, data=data, files=files)
                     if r.status_code < 200 or r.status_code > 299:
                         logger.debug(f'{r.status_code} {r.text}')
-                        raise Exception('Upload failed')
+                        raise Exception(f'[{ERROR}error{RESET}] upload failed')
                     i += 1
                     pbar.update(f.tell() - pbar.n)
 
         data = {'command': 'FINALIZE', 'media_id': media_id, 'allow_async': 'true'}
         if is_dm:
             data |= {'original_md5': hashlib.md5(file.read_bytes()).hexdigest()}
         r = self.session.post(url=url, headers=headers, data=data)
@@ -260,15 +267,15 @@
         processing_info = r.json().get('processing_info')
         while processing_info:
             state = processing_info['state']
             logger.debug(f'{processing_info = }')
             if state == MEDIA_UPLOAD_SUCCEED:
                 break
             if state == MEDIA_UPLOAD_FAIL:
-                raise Exception('Media processing failed')
+                raise Exception(f'[{ERROR}error{RESET}] media processing failed')
             check_after_secs = processing_info.get('check_after_secs', random.randint(1, 5))
             time.sleep(check_after_secs)
             params = {'command': 'STATUS', 'media_id': media_id}
             r = self.session.get(url=url, headers=headers, params=params)
             processing_info = r.json().get('processing_info')
         logger.debug('processing complete')
 
@@ -551,8 +558,8 @@
         return r
 
     @staticmethod
     def check_response(r):
         if r.status_code == 429:
             raise Exception(f'rate limit exceeded: {r.url}')
         if find_key(data := r.json(), 'errors'):
-            logger.debug(f'[{WARN}ERROR{RESET}]: {data}')
+            logger.debug(f'[{ERROR}error{RESET}] {data}')
```

### Comparing `twitter-api-client-0.5.8/twitter/config/log.py` & `twitter-api-client-0.5.9/twitter/config/log.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.8/twitter/config/operations.py` & `twitter-api-client-0.5.9/twitter/config/operations.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.8/twitter/config/settings.py` & `twitter-api-client-0.5.9/twitter/config/settings.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.8/twitter/constants.py` & `twitter-api-client-0.5.9/twitter/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum  # todo:add back in python 3.13 , member
 
 BOLD = '\u001b[1m'
 SUCCESS = '\u001b[32m'
-WARN = '\u001b[31m'
+ERROR = '\u001b[31m'
+WARN = '\u001b[33m'
 RESET = '\u001b[0m'
 
 UPLOAD_CHUNK_SIZE = 4 * 1024 * 1024
 MEDIA_UPLOAD_SUCCEED = 'succeeded'
 MEDIA_UPLOAD_FAIL = 'failed'
 
 
@@ -22,23 +23,23 @@
         if item != "_value_":
             attr = getattr(self.value, item)
             return attr.name, attr.value.value
         raise AttributeError
 
 
 class Media(CustomEnum):
-    #@member
+    # @member
     class Type(Enum):
         image = Value(5_242_880)  # ~5 MB
         gif = Value(15_728_640)  # ~15 MB
         video = Value(536_870_912)  # ~530 MB
 
 
 class Operation(CustomEnum):
-    #@member
+    # @member
     class Data(Enum):
         # tweet
         Favoriters = Value('tweetId')
         Retweeters = Value('tweetId')
         TweetDetail = Value('focalTweetId')
         TweetResultByRestId = Value('tweetId')
         # user
@@ -49,15 +50,15 @@
         Followers = Value('userId')
         Following = Value('userId')
         UserByScreenName = Value('screen_name')
         UserByRestId = Value('userId')
         # batch-user
         UsersByRestIds = Value('userIds')
 
-    #@member
+    # @member
     class Account(Enum):
         # tweet
         CreateTweet = Value()
         CreateScheduledTweet = Value()
         DeleteScheduledTweet = Value()
         FetchScheduledTweets = Value()
         DeleteTweet = Value()
```

### Comparing `twitter-api-client-0.5.8/twitter/login.py` & `twitter-api-client-0.5.9/twitter/login.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 import sys
+
 from requests import Session
-from .constants import SUCCESS, WARN, BOLD, RESET
+
+from .constants import SUCCESS, WARN, ERROR, BOLD, RESET
+from .utils import find_key
 
 
 def update_token(session: Session, key: str, url: str, payload: dict) -> Session:
+    caller_name = sys._getframe(1).f_code.co_name
     try:
         headers = {
             "authorization": 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
             "content-type": "application/json",
             "user-agent": 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36',
             "x-guest-token": session.cookies.get('guest_token'),
             "x-csrf-token": session.cookies.get("ct0"),
             "x-twitter-auth-type": "OAuth2Session" if session.cookies.get("auth_token") else '',
             "x-twitter-active-user": "yes",
             "x-twitter-client-language": 'en',
         }
-        r = session.post(url, headers=headers, json=payload).json()
-        session.cookies.set(key, r[key])
+        r = session.post(url, headers=headers, json=payload)
+        info = r.json()
+
+        for s in info.get('subtasks', []):
+            if s.get('enter_text', {}).get('keyboard_type') == 'email':
+                print(f"[{WARN}warning{RESET}] {' '.join(find_key(s, 'text'))}")
+                session.cookies.set('confirm_email', 'true')  # signal that email challenge must be solved
+
+        session.cookies.set(key, info[key])
     except KeyError as e:
-        print(f'[{WARN}FAILED{RESET}] failed to update token at {BOLD}{sys._getframe(1).f_code.co_name}{RESET}\n{e}')
+        print(f'[{ERROR}error{RESET}] failed to update token at {BOLD}{caller_name}{RESET}\n{e}')
     return session
 
 
 def init_guest_token(session: Session) -> Session:
     return update_token(session, 'guest_token', 'https://api.twitter.com/1.1/guest/activate.json', {})
 
 
@@ -72,25 +83,45 @@
         "subtask_inputs": [{
             "subtask_id": "AccountDuplicationCheck",
             "check_logged_in_account": {"link": "AccountDuplicationCheck_false"},
         }],
     })
 
 
+def confirm_email(session: Session) -> Session:
+    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', {
+        "flow_token": session.cookies.get('flow_token'),
+        "subtask_inputs": [
+            {
+                "subtask_id": "LoginAcid",
+                "enter_text": {
+                    "text": session.cookies.get('email'),
+                    "link": "next_link"
+                }
+            }]
+    })
+
+
 def execute_login_flow(session: Session) -> Session:
     session = init_guest_token(session)
     for fn in [flow_start, flow_instrumentation, flow_username, flow_password, flow_duplication_check]:
         session = fn(session)
+
+    # solve email challenge
+    if session.cookies.get('confirm_email') == 'true':
+        session = confirm_email(session)
+
     return session
 
 
-def login(username: str, password: str) -> Session:
+def login(email: str, username: str, password: str) -> Session:
     session = Session()
     session.cookies.update({
+        "email": email,
         "username": username,
         "password": password,
         "guest_token": None,
         "flow_token": None,
     })
     session = execute_login_flow(session)
-    print(f'[{SUCCESS}SUCCESS{RESET}] {BOLD}{username}{RESET} logged in successfully')
+    print(f'[{SUCCESS}success{RESET}] {BOLD}{username}{RESET} logged in successfully')
     return session
```

### Comparing `twitter-api-client-0.5.8/twitter/scraper.py` & `twitter-api-client-0.5.9/twitter/scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 logging.config.dictConfig(log_config)
 logger = logging.getLogger(__name__)
 
 
 class Scraper:
     GRAPHQL_URL = 'https://api.twitter.com/graphql'
 
-    def __init__(self, username: str, password: str):
-        self.session = login(username, password)
+    def __init__(self, email: str, username: str, password: str):
+        self.session = login(email, username, password)
 
     def tweets(self, ids: list[int], limit=math.inf):
         return self.run(ids, Operation.Data.UserTweets, limit)
 
     def tweets_and_replies(self, ids: list[int], limit=math.inf):
         return self.run(ids, Operation.Data.UserTweetsAndReplies, limit)
 
@@ -115,15 +115,15 @@
             urls.append((_id, f"{self.GRAPHQL_URL}/{qid}/{name}?{q}"))
         headers = get_headers(self.session)
         headers['content-type'] = "application/json"
         res = asyncio.run(self.process(urls, headers))
         self.save_data(res, name)
         return res
 
-    async def process(self, urls: list, headers: dict) -> tuple:
+    async def process(self, urls: list, headers: dict) -> list:
         conn = TCPConnector(limit=100, ssl=False, ttl_dns_cache=69)
         async with ClientSession(headers=headers, connector=conn) as s:
             # add cookies from logged-in session
             s.cookie_jar.update_cookies(self.session.cookies)
             return await asyncio.gather(*(self.get(s, u) for u in urls))
 
     async def get(self, session: ClientSession, url: tuple) -> dict:
@@ -135,17 +135,17 @@
             logger.debug(f'{limits = }')
             if r.status == 429:
                 logger.debug(f'rate limit exceeded: {url}')
                 return {}
             data = await r.json()
             return {ID: identifier, **data}
         except Exception as e:
-            logger.debug(f'failed to download {url}: {e}')
+            logger.debug(f'[{ERROR}error{RESET}] failed to download {url}: {e}')
 
-    async def pagination(self, res: list, operation: tuple, limit: int) -> tuple:
+    async def pagination(self, res: list, operation: tuple, limit: int) -> list:
         conn = TCPConnector(limit=100, ssl=False, ttl_dns_cache=69)
         headers = get_headers(self.session)
         headers['content-type'] = "application/json"
         async with ClientSession(headers=headers, connector=conn) as s:
             # add cookies from logged-in session
             s.cookie_jar.update_cookies(self.session.cookies)
             return await asyncio.gather(*(self.paginate(s, data, operation, limit) for data in res))
@@ -190,60 +190,60 @@
                 all_data.append(tagged_data)
                 cursor = get_cursor(_data)
                 logger.debug(f'{cursor = }')
                 ids |= set(find_key(tagged_data, 'rest_id'))
                 logger.debug(f'({data[ID]})\t{len(ids)} unique results')
                 counts.append(len(ids))
 
-                success_message = f'[{SUCCESS}SUCCESS{RESET}] done pagination'
+                success_message = f'[{SUCCESS}success{RESET}] done pagination'
                 # followers/following have "0|"
                 if not cursor or cursor.startswith('0|'):
                     logger.debug(f'{success_message}\tlast cursor: {cursor}')
                     break
                 if len(ids) >= limit:
                     logger.debug(f'{success_message}\tsurpassed limit of {limit} results')
                     break
                 # did last 5 requests return duplicate data?
                 if len(counts) > DUP_LIMIT and len(set(counts[-1:-DUP_LIMIT:-1])) == 1:
                     logger.debug(f'{success_message}\tpast {DUP_LIMIT} requests returned duplicate data')
                     break
         except Exception as e:
-            logger.debug(f'paginate falied: {e}')
+            logger.debug(f'[{ERROR}error{RESET}] paginate falied: {e}')
         # save_data(all_data, name)
         return all_data
 
     async def backoff(self, fn, retries=12):
         for i in range(retries + 1):
             try:
                 r = await fn()
                 data = await r.json()
                 if r.status == 429:
-                    logger.debug(f'rate limit exceeded: {r.url}')
+                    logger.debug(f'[{ERROR}error{RESET}] rate limit exceeded: {r.url}')
                     return r, {}
                 if find_key(data, 'errors'):
-                    logger.debug(f'[{WARN}ERROR{RESET}]: {data}')
+                    logger.debug(f'[{ERROR}error{RESET}] twitter errors: {data}')
                 return r, data
             except Exception as e:
                 if i == retries:
-                    logger.debug(f'{WARN} Max retries exceeded{RESET}\n{e}')
+                    logger.debug(f'[{ERROR}error{RESET}] max retries exceeded{RESET}\n{e}')
                     return
                 t = 2 ** i + random.random()
-                logger.debug(f'retrying in {f"{t:.2f}"} seconds\t\t{e}')
+                logger.debug(f'{WARN}retrying in {f"{t:.2f}"} seconds{RESET}\t\t{e}')
                 time.sleep(t)
 
     def save_data(self, data: list, name: str = ''):
         try:
             for d in data:
                 path = Path(f'data/raw/{d[ID]}')
                 path.mkdir(parents=True, exist_ok=True)
                 (path / f'{time.time_ns()}_{name}.json').write_text(
                     orjson.dumps(d, option=orjson.OPT_INDENT_2).decode())
 
         except KeyError as e:
-            logger.debug(f'failed to save data: {e}')
+            logger.debug(f'[{ERROR}error{RESET}] failed to save data: {e}')
 
     def download(self, post_url: str, cdn_url: str, path: str = 'media', chunk_size: int = 4096) -> None:
         """
         Download file
     
         @param post_url: the actual post url
         @param cdn_url: the cdn url
@@ -260,15 +260,15 @@
             desc = f'downloading: {name}'
             with tqdm(total=total_bytes, desc=desc, unit='B', unit_scale=True, unit_divisor=1024) as pbar:
                 with open(f'{path}/{name}_{ext}', 'wb') as f:
                     for chunk in r.iter_content(chunk_size=chunk_size):
                         f.write(chunk)
                         pbar.update(f.tell() - pbar.n)
         except Exception as e:
-            logger.debug(f'FAILED to download media: {post_url} {e}')
+            logger.debug(f'[{ERROR}error{RESET}] failed to download media: {post_url} {e}')
 
     def download_media(self, ids: list[int], photos: bool = True, videos: bool = True) -> None:
         res = self.tweet_by_rest_id(ids)
         for r in res:
             user_id = find_key(r, 'user_results')[0]['result']['rest_id']
             url = f'https://twitter.com/{user_id}/status/{r[ID]}'  # evaluates to username in browser
             media = [y for x in find_key(r, 'media') for y in x]  # in case of arbitrary schema
```

### Comparing `twitter-api-client-0.5.8/twitter/search.py` & `twitter-api-client-0.5.9/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.8/twitter/utils.py` & `twitter-api-client-0.5.9/twitter/utils.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.8/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.5.9/twitter_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.5.8
+Version: 0.5.9
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
@@ -16,16 +16,16 @@
  Includes tools to **scrape**, **automate**, and **search** twitter
 
  ### Installation
 
 ```python
  from twitter.account import Account
 
- username, password = ..., ...
- account = Account(username, password)
+ email, username, password = ..., ..., ...
+ account = Account(email, username, password)
 
  account.create_poll('test poll 123', ['hello', 'world', 'foo', 'bar'], 10080)
 
  # DM 1 user
  account.dm([123], 'hello world', filename='test.png')
 
  # DM group of users
@@ -156,16 +156,16 @@
  ### Scraping
 
  #### Get all user/tweet data
 
  ```python
  from twitter.scraper import Scraper
 
- username, password = ..., ...
- scraper = Scraper(username, password)  # session
+ email, username, password = ..., ..., ...
+ scraper = Scraper(email, username, password)  # session
 
  ####### User Data ########
  users = scraper.user_by_screen_name(['bob123', 'jim456', 'stanley789'])
  tweets = scraper.tweets([123, 234, 345])
  likes = scraper.likes([123, 234, 345])
  tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
  media = scraper.media([123, 234, 345])
```


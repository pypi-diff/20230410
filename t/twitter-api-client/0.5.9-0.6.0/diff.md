# Comparing `tmp/twitter-api-client-0.5.9.tar.gz` & `tmp/twitter-api-client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.5.9.tar", last modified: Mon Apr 10 18:45:23 2023, max compression
+gzip compressed data, was "twitter-api-client-0.6.0.tar", last modified: Mon Apr 10 19:12:07 2023, max compression
```

## Comparing `twitter-api-client-0.5.9.tar` & `twitter-api-client-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 18:45:23.827640 twitter-api-client-0.5.9/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-10 18:45:23.827640 twitter-api-client-0.5.9/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-10 18:45:23.827640 twitter-api-client-0.5.9/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     7094 2023-04-10 18:45:10.000000 twitter-api-client-0.5.9/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 18:45:23.825640 twitter-api-client-0.5.9/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    22979 2023-04-10 18:34:38.000000 twitter-api-client-0.5.9/twitter/account.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 18:45:23.826640 twitter-api-client-0.5.9/twitter/config/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/config/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)      909 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/config/log.py
--rw-r--r--   0 x         (1000) x         (1000)   148071 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/config/operations.py
--rw-r--r--   0 x         (1000) x         (1000)     5858 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/config/settings.py
--rw-r--r--   0 x         (1000) x         (1000)     2456 2023-04-10 18:10:09.000000 twitter-api-client-0.5.9/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5001 2023-04-10 18:35:58.000000 twitter-api-client-0.5.9/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    12811 2023-04-10 18:38:31.000000 twitter-api-client-0.5.9/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5035 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     2235 2023-04-07 23:06:22.000000 twitter-api-client-0.5.9/twitter/utils.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 18:45:23.827640 twitter-api-client-0.5.9/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-10 18:45:23.000000 twitter-api-client-0.5.9/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      461 2023-04-10 18:45:23.000000 twitter-api-client-0.5.9/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-10 18:45:23.000000 twitter-api-client-0.5.9/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       82 2023-04-10 18:45:23.000000 twitter-api-client-0.5.9/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-10 18:45:23.000000 twitter-api-client-0.5.9/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 19:12:07.854313 twitter-api-client-0.6.0/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-10 19:12:07.854313 twitter-api-client-0.6.0/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-10 19:12:07.854313 twitter-api-client-0.6.0/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     7094 2023-04-10 19:12:02.000000 twitter-api-client-0.6.0/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 19:12:07.853313 twitter-api-client-0.6.0/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    22979 2023-04-10 18:34:38.000000 twitter-api-client-0.6.0/twitter/account.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 19:12:07.853313 twitter-api-client-0.6.0/twitter/config/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/config/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)      909 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/config/log.py
+-rw-r--r--   0 x         (1000) x         (1000)   148071 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/config/operations.py
+-rw-r--r--   0 x         (1000) x         (1000)     5858 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/config/settings.py
+-rw-r--r--   0 x         (1000) x         (1000)     2456 2023-04-10 18:10:09.000000 twitter-api-client-0.6.0/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5242 2023-04-10 19:10:29.000000 twitter-api-client-0.6.0/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    12811 2023-04-10 18:38:31.000000 twitter-api-client-0.6.0/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     5035 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     2235 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/utils.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 19:12:07.854313 twitter-api-client-0.6.0/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-10 19:12:07.000000 twitter-api-client-0.6.0/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      461 2023-04-10 19:12:07.000000 twitter-api-client-0.6.0/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-10 19:12:07.000000 twitter-api-client-0.6.0/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       82 2023-04-10 19:12:07.000000 twitter-api-client-0.6.0/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-10 19:12:07.000000 twitter-api-client-0.6.0/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.5.9/LICENSE` & `twitter-api-client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.9/PKG-INFO` & `twitter-api-client-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.5.9
+Version: 0.6.0
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.5.9/setup.py` & `twitter-api-client-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.5.9",
+    version="0.6.0",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
```

### Comparing `twitter-api-client-0.5.9/twitter/account.py` & `twitter-api-client-0.6.0/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.9/twitter/config/log.py` & `twitter-api-client-0.6.0/twitter/config/log.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.9/twitter/config/operations.py` & `twitter-api-client-0.6.0/twitter/config/operations.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.9/twitter/config/settings.py` & `twitter-api-client-0.6.0/twitter/config/settings.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.9/twitter/constants.py` & `twitter-api-client-0.6.0/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.9/twitter/login.py` & `twitter-api-client-0.6.0/twitter/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         for s in info.get('subtasks', []):
             if s.get('enter_text', {}).get('keyboard_type') == 'email':
                 print(f"[{WARN}warning{RESET}] {' '.join(find_key(s, 'text'))}")
                 session.cookies.set('confirm_email', 'true')  # signal that email challenge must be solved
 
         session.cookies.set(key, info[key])
     except KeyError as e:
+        session.cookies.set('flow_errors', 'true')  # signal that an error occurred somewhere in the flow
         print(f'[{ERROR}error{RESET}] failed to update token at {BOLD}{caller_name}{RESET}\n{e}')
     return session
 
 
 def init_guest_token(session: Session) -> Session:
     return update_token(session, 'guest_token', 'https://api.twitter.com/1.1/guest/activate.json', {})
 
@@ -119,9 +120,12 @@
         "email": email,
         "username": username,
         "password": password,
         "guest_token": None,
         "flow_token": None,
     })
     session = execute_login_flow(session)
-    print(f'[{SUCCESS}success{RESET}] {BOLD}{username}{RESET} logged in successfully')
+    if session.cookies.get('flow_errors') == 'true':
+        print(f'[{ERROR}error{RESET}] {BOLD}{username}{RESET} login failed')
+    else:
+        print(f'[{SUCCESS}success{RESET}] {BOLD}{username}{RESET} login success')
     return session
```

### Comparing `twitter-api-client-0.5.9/twitter/scraper.py` & `twitter-api-client-0.6.0/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.9/twitter/search.py` & `twitter-api-client-0.6.0/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.9/twitter/utils.py` & `twitter-api-client-0.6.0/twitter/utils.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.5.9/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.6.0/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.5.9
+Version: 0.6.0
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```


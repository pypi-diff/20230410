# Comparing `tmp/discordapiwebhooks-1.0.0.tar.gz` & `tmp/discordapiwebhooks-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordapiwebhooks-1.0.0.tar", last modified: Mon Apr 10 11:46:04 2023, max compression
+gzip compressed data, was "discordapiwebhooks-1.0.1.tar", last modified: Mon Apr 10 13:25:17 2023, max compression
```

## Comparing `discordapiwebhooks-1.0.0.tar` & `discordapiwebhooks-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 11:46:04.256434 discordapiwebhooks-1.0.0/
--rw-rw----   0 root         (0) everybody  (9997)      219 2023-04-10 11:46:04.248434 discordapiwebhooks-1.0.0/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 11:46:04.184434 discordapiwebhooks-1.0.0/discordapiwebhooks/
--rw-rw----   0 root         (0) everybody  (9997)     2049 2023-04-10 10:56:07.000000 discordapiwebhooks-1.0.0/discordapiwebhooks/discordapiwebhooks.py
--rw-rw----   0 root         (0) everybody  (9997)      243 2023-04-10 10:58:30.000000 discordapiwebhooks-1.0.0/discordapiwebhooks/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 11:46:04.240434 discordapiwebhooks-1.0.0/discordapiwebhooks.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      219 2023-04-10 11:46:03.000000 discordapiwebhooks-1.0.0/discordapiwebhooks.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      245 2023-04-10 11:46:04.000000 discordapiwebhooks-1.0.0/discordapiwebhooks.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-10 11:46:03.000000 discordapiwebhooks-1.0.0/discordapiwebhooks.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       19 2023-04-10 11:46:03.000000 discordapiwebhooks-1.0.0/discordapiwebhooks.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-10 11:46:04.256434 discordapiwebhooks-1.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      243 2023-04-10 10:58:30.000000 discordapiwebhooks-1.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 13:25:17.354673 discordapiwebhooks-1.0.1/
+-rw-rw----   0 root         (0) everybody  (9997)      344 2023-04-10 13:25:17.346673 discordapiwebhooks-1.0.1/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1439 2023-04-10 13:24:56.000000 discordapiwebhooks-1.0.1/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 13:25:17.286672 discordapiwebhooks-1.0.1/discordapiwebhooks/
+-rw-rw----   0 root         (0) everybody  (9997)     2498 2023-04-10 13:17:43.000000 discordapiwebhooks-1.0.1/discordapiwebhooks/discordapiwebhooks.py
+-rw-rw----   0 root         (0) everybody  (9997)     1693 2023-04-10 12:10:56.000000 discordapiwebhooks-1.0.1/discordapiwebhooks/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 13:25:17.342672 discordapiwebhooks-1.0.1/discordapiwebhooks.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      344 2023-04-10 13:25:17.000000 discordapiwebhooks-1.0.1/discordapiwebhooks.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      255 2023-04-10 13:25:17.000000 discordapiwebhooks-1.0.1/discordapiwebhooks.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-10 13:25:17.000000 discordapiwebhooks-1.0.1/discordapiwebhooks.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       19 2023-04-10 13:25:17.000000 discordapiwebhooks-1.0.1/discordapiwebhooks.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-10 13:25:17.354673 discordapiwebhooks-1.0.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      368 2023-04-10 13:22:19.000000 discordapiwebhooks-1.0.1/setup.py
```

### Comparing `discordapiwebhooks-1.0.0/discordapiwebhooks/discordapiwebhooks.py` & `discordapiwebhooks-1.0.1/discordapiwebhooks/discordapiwebhooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import requests
 import json
 
-def send_message(webhook_url, message, username=None, avatar_url=None, custom_id=None, default=None, label=None, max_length=None, min_length=None, placeholder=None, required=None, style=None, type=None, value=None):
+def send_message(webhook_url, message, username=None, avatar_url=None, custom_id=None, default=None, label=None, max_length=None, min_length=None, placeholder=None, required=None, style=None, type=None, value=None, emoji_id=None, emoji_name=None, emoji_react=None, emoji_add=None):
     payload = {'content': message}
     if username:
         payload['username'] = username
     if avatar_url:
-payload['avatar_url'] = avatar_url
+        payload['avatar_url'] = avatar_url
     if custom_id:
         payload['custom_id'] = custom_id
     if default:
         payload['default'] = default
     if label:
         payload['label'] = label
     if max_length:
@@ -23,14 +23,24 @@
         payload['required'] = required
     if style:
         payload['style']  = style
     if type:
         payload['type'] = type
     if value:
         payload['value'] = value
+    if emoji_id or emoji_name or emoji_react or emoji_add:
+        payload['emoji'] = {}
+        if emoji_id:
+            payload['emoji']['id'] = emoji_id
+        if emoji_name:
+            payload['emoji']['name'] = emoji_name
+        if emoji_react:
+            payload['emoji']['react'] = emoji_react
+        if emoji_add:
+            payload['emoji']['add'] = emoji_add
     headers = {'Content-Type': 'application/json'}
     response = requests.post(webhook_url, data=json.dumps(payload), headers=headers)
     if response.status_code != 204:
         print('Request failed with status code', response.status_code)
 
 def send_embed(webhook_url, embed, username=None, avatar_url=None):
     payload = {'embeds': [embed.to_dict()]}
```


# Comparing `tmp/poe-web-client-0.0.3.tar.gz` & `tmp/poe-web-client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe-web-client-0.0.3.tar", last modified: Mon Apr 10 12:14:40 2023, max compression
+gzip compressed data, was "poe-web-client-0.0.4.tar", last modified: Mon Apr 10 15:13:37 2023, max compression
```

## Comparing `poe-web-client-0.0.3.tar` & `poe-web-client-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 12:14:40.603580 poe-web-client-0.0.3/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)    35149 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/LICENSE
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-10 12:14:40.602916 poe-web-client-0.0.3/PKG-INFO
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     8459 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/README.md
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 12:14:40.566961 poe-web-client-0.0.3/poe-api/
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 12:14:40.570108 poe-web-client-0.0.3/poe-api/src/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)    11885 2023-04-10 12:13:08.000000 poe-web-client-0.0.3/poe-api/src/poe.py
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 12:14:40.599123 poe-web-client-0.0.3/poe-api/src/poe_graphql/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1093 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      373 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       97 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/BioFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       73 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      100 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/ChatFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     6971 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      686 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      154 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      160 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      123 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      103 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/HandleFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      306 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1885 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      135 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      194 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/MessageFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      145 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      216 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      710 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      263 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      213 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      308 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      159 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      162 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       95 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      147 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      368 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      400 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1038 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      657 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)        0 2023-04-09 00:01:12.000000 poe-web-client-0.0.3/poe-api/src/poe_graphql/__init__.py
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 12:14:40.602110 poe-web-client-0.0.3/poe-api/src/poe_web_client.egg-info/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-10 12:14:40.000000 poe-web-client-0.0.3/poe-api/src/poe_web_client.egg-info/PKG-INFO
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     2035 2023-04-10 12:14:40.000000 poe-web-client-0.0.3/poe-api/src/poe_web_client.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)        1 2023-04-10 12:14:40.000000 poe-web-client-0.0.3/poe-api/src/poe_web_client.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       46 2023-04-10 12:14:40.000000 poe-web-client-0.0.3/poe-api/src/poe_web_client.egg-info/requires.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       16 2023-04-10 12:14:40.000000 poe-web-client-0.0.3/poe-api/src/poe_web_client.egg-info/top_level.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       38 2023-04-10 12:14:40.603748 poe-web-client-0.0.3/setup.cfg
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1044 2023-04-10 12:14:22.000000 poe-web-client-0.0.3/setup.py
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 15:13:37.181334 poe-web-client-0.0.4/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)    35149 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/LICENSE
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-10 15:13:37.180673 poe-web-client-0.0.4/PKG-INFO
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     8459 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/README.md
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 15:13:37.116973 poe-web-client-0.0.4/poe-api/
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 15:13:37.120050 poe-web-client-0.0.4/poe-api/src/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)    12107 2023-04-10 15:11:50.000000 poe-web-client-0.0.4/poe-api/src/poe.py
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 15:13:37.173234 poe-web-client-0.0.4/poe-api/src/poe_graphql/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1093 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      373 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       97 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/BioFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       73 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      100 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     6971 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      686 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      154 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      160 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      123 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      103 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      306 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1885 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      135 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      194 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      145 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      216 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      710 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      263 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      213 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      308 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      159 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      162 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       95 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      147 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      368 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      400 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1038 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      657 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)        0 2023-04-09 00:01:12.000000 poe-web-client-0.0.4/poe-api/src/poe_graphql/__init__.py
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 15:13:37.179864 poe-web-client-0.0.4/poe-api/src/poe_web_client.egg-info/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-10 15:13:37.000000 poe-web-client-0.0.4/poe-api/src/poe_web_client.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     2035 2023-04-10 15:13:37.000000 poe-web-client-0.0.4/poe-api/src/poe_web_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)        1 2023-04-10 15:13:37.000000 poe-web-client-0.0.4/poe-api/src/poe_web_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       46 2023-04-10 15:13:37.000000 poe-web-client-0.0.4/poe-api/src/poe_web_client.egg-info/requires.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       16 2023-04-10 15:13:37.000000 poe-web-client-0.0.4/poe-api/src/poe_web_client.egg-info/top_level.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       38 2023-04-10 15:13:37.181501 poe-web-client-0.0.4/setup.cfg
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1044 2023-04-10 15:08:30.000000 poe-web-client-0.0.4/setup.py
```

### Comparing `poe-web-client-0.0.3/LICENSE` & `poe-web-client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.3/PKG-INFO` & `poe-web-client-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-web-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: A reverse engineered API wrapper for Quora's Poe,fork from https://github.com/ading2210/poe-api
 Home-page: https://github.com/libaiabcd/poe-api
 Author: libaiabcd
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `poe-web-client-0.0.3/README.md` & `poe-web-client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.3/poe-api/src/poe.py` & `poe-web-client-0.0.4/poe-api/src/poe.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 
     self.formkey = data["formkey"]
     return data["tchannelData"]
   
   def get_websocket_url(self, channel=None):
     if channel is None:
       channel = self.channel
+    self.ws_domain = f"tch{random.randint(1, 1e6)}"
     query = f'?min_seq={channel["minSeq"]}&channel={channel["channel"]}&hash={channel["channelHash"]}'
     return f'wss://{self.ws_domain}.tch.{channel["baseHost"]}/up/{channel["boxName"]}/updates'+query
 
   def send_query(self, query_name, variables):
     for i in range(20):
       payload = generate_payload(query_name, variables)
       r = request_with_retries(self.session.post, self.gql_url, json=payload, headers=self.gql_headers)
@@ -195,31 +196,35 @@
       on_error=self.on_ws_error,
       on_close=self.on_ws_close
     )
     t = threading.Thread(target=self.ws_run_thread, daemon=True)
     t.start()
     while not self.ws_connected:
       time.sleep(0.01)
+    logger.info(f"connect_ws done")
   
   def disconnect_ws(self):
     logger.info(f"disconnect_ws {self.ws} ")
     if self.ws:
       self.ws.close()
     self.ws_connected = False
   
   def on_ws_connect(self, ws):
+    logger.info(f"on_ws_connect:{ws}")
     self.ws_connected = True
   
   def on_ws_close(self, ws, close_status_code, close_message):
     self.ws_connected = False
     logger.warn(f"Websocket closed with status {close_status_code}: {close_message}")
   
   def on_ws_error(self, ws, error):
+    logger.info(f"on_ws_error:{ws},{error}")
     self.disconnect_ws()
     self.connect_ws()
+    logger.info(f"on_ws_error done:{ws},{error}")
 
   def on_message(self, ws, msg):
     try:
       data = json.loads(msg)
 
       if not "messages" in data:
         return
```

### Comparing `poe-web-client-0.0.3/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql` & `poe-web-client-0.0.4/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.3/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql` & `poe-web-client-0.0.4/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.3/poe-api/src/poe_graphql/ChatPaginationQuery.graphql` & `poe-web-client-0.0.4/poe-api/src/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.3/poe-api/src/poe_graphql/MessageAddedSubscription.graphql` & `poe-web-client-0.0.4/poe-api/src/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.3/poe-api/src/poe_graphql/SendMessageMutation.graphql` & `poe-web-client-0.0.4/poe-api/src/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.3/poe-api/src/poe_graphql/ViewerStateFragment.graphql` & `poe-web-client-0.0.4/poe-api/src/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.3/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `poe-web-client-0.0.4/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.3/poe-api/src/poe_web_client.egg-info/PKG-INFO` & `poe-web-client-0.0.4/poe-api/src/poe_web_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-web-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: A reverse engineered API wrapper for Quora's Poe,fork from https://github.com/ading2210/poe-api
 Home-page: https://github.com/libaiabcd/poe-api
 Author: libaiabcd
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `poe-web-client-0.0.3/poe-api/src/poe_web_client.egg-info/SOURCES.txt` & `poe-web-client-0.0.4/poe-api/src/poe_web_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.3/setup.py` & `poe-web-client-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #pip wheel --no-deps -w dist .
 
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 setuptools.setup(
   name="poe-web-client",
-  version="0.0.3",
+  version="0.0.4",
   author="libaiabcd",
   license="GPLv3",
   description="A reverse engineered API wrapper for Quora's Poe,fork from https://github.com/ading2210/poe-api",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=["poe_graphql"],
   classifiers=[
```


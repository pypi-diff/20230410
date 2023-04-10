# Comparing `tmp/atlassian_api_py-0.4.1-py3-none-any.whl.zip` & `tmp/atlassian_api_py-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13022 bytes, number of entries: 12
--rw-r--r--  2.0 unx      167 b- defN 22-Nov-25 07:21 atlassian/__init__.py
--rw-r--r--  2.0 unx    12925 b- defN 22-Nov-25 07:21 atlassian/bitbucket.py
--rw-r--r--  2.0 unx     3349 b- defN 22-Nov-25 07:21 atlassian/client.py
--rw-r--r--  2.0 unx     2129 b- defN 22-Nov-25 07:21 atlassian/confluence.py
--rw-r--r--  2.0 unx     1608 b- defN 22-Nov-25 07:21 atlassian/error.py
--rw-r--r--  2.0 unx    11439 b- defN 22-Nov-25 07:21 atlassian/jira.py
--rw-r--r--  2.0 unx     1162 b- defN 22-Nov-25 07:21 atlassian/logger.py
--rw-r--r--  2.0 unx     1067 b- defN 22-Nov-25 07:21 atlassian_api_py-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6979 b- defN 22-Nov-25 07:21 atlassian_api_py-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-25 07:21 atlassian_api_py-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 22-Nov-25 07:21 atlassian_api_py-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      970 b- defN 22-Nov-25 07:21 atlassian_api_py-0.4.1.dist-info/RECORD
-12 files, 41897 bytes uncompressed, 11402 bytes compressed:  72.8%
+Zip file size: 12293 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      194 b- defN 23-Apr-10 13:25 atlassian/__init__.py
+-rw-r--r--  2.0 unx    12925 b- defN 23-Apr-10 13:25 atlassian/bitbucket.py
+-rw-r--r--  2.0 unx     3349 b- defN 23-Apr-10 13:25 atlassian/client.py
+-rw-r--r--  2.0 unx     2124 b- defN 23-Apr-10 13:25 atlassian/confluence.py
+-rw-r--r--  2.0 unx     1608 b- defN 23-Apr-10 13:25 atlassian/error.py
+-rw-r--r--  2.0 unx    11448 b- defN 23-Apr-10 13:25 atlassian/jira.py
+-rw-r--r--  2.0 unx     1162 b- defN 23-Apr-10 13:25 atlassian/logger.py
+-rw-r--r--  2.0 unx     1074 b- defN 23-Apr-10 13:25 atlassian_api_py-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3840 b- defN 23-Apr-10 13:25 atlassian_api_py-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 13:25 atlassian_api_py-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-10 13:25 atlassian_api_py-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      970 b- defN 23-Apr-10 13:25 atlassian_api_py-0.5.0.dist-info/RECORD
+12 files, 38796 bytes uncompressed, 10673 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: atlassian/jira.py
 Comment: 
 
 Filename: atlassian/logger.py
 Comment: 
 
-Filename: atlassian_api_py-0.4.1.dist-info/LICENSE
+Filename: atlassian_api_py-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: atlassian_api_py-0.4.1.dist-info/METADATA
+Filename: atlassian_api_py-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: atlassian_api_py-0.4.1.dist-info/WHEEL
+Filename: atlassian_api_py-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: atlassian_api_py-0.4.1.dist-info/top_level.txt
+Filename: atlassian_api_py-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: atlassian_api_py-0.4.1.dist-info/RECORD
+Filename: atlassian_api_py-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atlassian/__init__.py

```diff
@@ -1,6 +1,6 @@
 """Import Jira, Bitbucket"""
-from .jira import Jira
-from .bitbucket import Bitbucket
-from .confluence import Confluence
+from atlassian.jira import Jira
+from atlassian.bitbucket import Bitbucket
+from atlassian.confluence import Confluence
 
 __all__ = ["Jira", "Bitbucket", "Confluence"]
```

## atlassian/confluence.py

```diff
@@ -30,15 +30,15 @@
                 "storage": {"value": f"{body_value}", "representation": "storage"}
             },
         }
         if ancestors_id:
             json = {
                 "type": f"{type}",
                 "title": f"{title}",
-                "ancestors": [{"id": f"{ancestors_id}"}],
+                "ancestors": [{"id": ancestors_id}],
                 "space": {"key": f"{space_key}"},
                 "body": {
                     "storage": {"value": f"{body_value}", "representation": "storage"}
                 },
             }
         return self.post(url, json=json) or {}
```

## atlassian/jira.py

```diff
@@ -243,15 +243,16 @@
         url = f"/rest/api/2/issue/{issue_key}/watchers"
         return self.post(url, json=watcher)
 
     def issue_transition(self, issue_key, transition_id=None):
         """Each Jira project may have different transition_id. You can find your transition_id like below:
         Chose transition Button then right click on the view elements. for example:
         I find Close button's elements is id="action_id_51", so the close transition_id = 51.
-        I find Open button's elements is id="action_id_61", so the open transition_id = 61."""
+        I find Open button's elements is id="action_id_61", so the open transition_id = 61.
+        """
         url = "/rest/api/2/issue/{key}/transitions".format(key=issue_key)
         json = {"transition": {"id": transition_id}}
         return self.post(url, json=json)
 
     def get_transitions(self, issue_id):
         """Get a list of the transitions possible for this issue by the current user"""
         url = f"/rest/api/2/issue/{issue_id}/transitions"
```

## Comparing `atlassian_api_py-0.4.1.dist-info/LICENSE` & `atlassian_api_py-0.5.0.dist-info/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Peter Shen
+Copyright (c) 2021 - 2023 Peter Shen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `atlassian_api_py-0.4.1.dist-info/RECORD` & `atlassian_api_py-0.5.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-atlassian/__init__.py,sha256=Pn5oz1dvGlDBZ3hVBF5OGahX2TCKOgdes9XgcjxY2jQ,167
+atlassian/__init__.py,sha256=bOwS4IT5qBytCyNravdUfLdM4SsCAM1qRWCOQPa_j6I,194
 atlassian/bitbucket.py,sha256=0g9SGkTEwkLWET1J2FxaDODGOSeOH4QY-sJUArHVwU8,12925
 atlassian/client.py,sha256=MmJSGT2RPOxgK_0CA4_jDmoAK4nLpoytRlJeUmDkEDE,3349
-atlassian/confluence.py,sha256=oBI28UKFbuoQsKIflveQ9ykrg1qQaxTqj6GNMQw0vYE,2129
+atlassian/confluence.py,sha256=Xz_pFdsZrv7Df51dnc-uHCS_p8qGsxdwXN_eWRVuj_0,2124
 atlassian/error.py,sha256=6HnhRu1CQLuHjNEj1OmthP8AJqBliwhalHOL76y49Ec,1608
-atlassian/jira.py,sha256=jgHDKdQTkWIlvyArWhtqvC7-RDSbIgTA6sMUx8blS4k,11439
+atlassian/jira.py,sha256=KweXfpIPdxs2BvdtVhO3HoTV1PPGf3lwpID4HudKiSw,11448
 atlassian/logger.py,sha256=L31bRNHMMw4YFZS4_sU5YeK4JGDSj6oRCz7khmL4Sjc,1162
-atlassian_api_py-0.4.1.dist-info/LICENSE,sha256=YuagYNDOVv7t5tzgMszBVyQqgJ2olwxcidRIncjUPLw,1067
-atlassian_api_py-0.4.1.dist-info/METADATA,sha256=XhTrvaBsSezzg7m4iC6yIzhp5rU9vvUH6W90rwvCRwI,6979
-atlassian_api_py-0.4.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-atlassian_api_py-0.4.1.dist-info/top_level.txt,sha256=84-EDv8LNaZx01TCGjBzglwPU1JSRJ7fPSq9uy55Sv0,10
-atlassian_api_py-0.4.1.dist-info/RECORD,,
+atlassian_api_py-0.5.0.dist-info/LICENSE,sha256=0yknWMrerC-pJulAKg6uiNAywvjwHJICz0BZllIeuD8,1074
+atlassian_api_py-0.5.0.dist-info/METADATA,sha256=JuLKbHbWk48aGE6tU5Ga6pcm0jATL7lIoRx_1Fh-NPE,3840
+atlassian_api_py-0.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+atlassian_api_py-0.5.0.dist-info/top_level.txt,sha256=84-EDv8LNaZx01TCGjBzglwPU1JSRJ7fPSq9uy55Sv0,10
+atlassian_api_py-0.5.0.dist-info/RECORD,,
```


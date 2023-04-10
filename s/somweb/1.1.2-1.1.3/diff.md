# Comparing `tmp/somweb-1.1.2.tar.gz` & `tmp/somweb-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somweb-1.1.2.tar", last modified: Sun Jan 16 00:55:55 2022, max compression
+gzip compressed data, was "somweb-1.1.3.tar", last modified: Mon Apr 10 19:06:49 2023, max compression
```

## Comparing `somweb-1.1.2.tar` & `somweb-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-01-16 00:55:55.305186 somweb-1.1.2/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1091 2022-01-01 21:26:14.000000 somweb-1.1.2/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)       27 2022-01-01 19:24:13.000000 somweb-1.1.2/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5556 2022-01-16 00:55:55.305186 somweb-1.1.2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4587 2022-01-02 22:42:33.000000 somweb-1.1.2/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2022-01-16 00:55:55.305186 somweb-1.1.2/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4476 2022-01-01 19:24:13.000000 somweb-1.1.2/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-01-16 00:55:55.305186 somweb-1.1.2/somweb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       99 2022-01-01 22:02:08.000000 somweb-1.1.2/somweb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       85 2022-01-16 00:54:05.000000 somweb-1.1.2/somweb/__version__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12657 2022-01-16 00:51:50.000000 somweb-1.1.2/somweb/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      847 2022-01-01 22:05:30.000000 somweb-1.1.2/somweb/const.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2756 2022-01-15 23:35:19.000000 somweb-1.1.2/somweb/httpclient.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      799 2022-01-02 19:01:23.000000 somweb-1.1.2/somweb/models.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-01-16 00:55:55.305186 somweb-1.1.2/somweb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5556 2022-01-16 00:55:55.000000 somweb-1.1.2/somweb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      299 2022-01-16 00:55:55.000000 somweb-1.1.2/somweb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2022-01-16 00:55:55.000000 somweb-1.1.2/somweb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       17 2022-01-16 00:55:55.000000 somweb-1.1.2/somweb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        7 2022-01-16 00:55:55.000000 somweb-1.1.2/somweb.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-10 19:06:49.036362 somweb-1.1.3/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1091 2023-04-10 18:37:27.000000 somweb-1.1.3/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       27 2022-01-01 19:24:13.000000 somweb-1.1.3/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5556 2023-04-10 19:06:49.036362 somweb-1.1.3/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4587 2022-01-02 22:42:33.000000 somweb-1.1.3/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-10 19:06:49.036362 somweb-1.1.3/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4476 2022-01-01 19:24:13.000000 somweb-1.1.3/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-10 19:06:49.036362 somweb-1.1.3/somweb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       99 2022-01-01 22:02:08.000000 somweb-1.1.3/somweb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       85 2023-04-10 18:37:55.000000 somweb-1.1.3/somweb/__version__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12657 2022-01-16 00:51:50.000000 somweb-1.1.3/somweb/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      849 2022-01-16 02:08:33.000000 somweb-1.1.3/somweb/const.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2800 2023-04-10 17:12:11.000000 somweb-1.1.3/somweb/httpclient.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      799 2022-01-02 19:01:23.000000 somweb-1.1.3/somweb/models.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-10 19:06:49.036362 somweb-1.1.3/somweb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5556 2023-04-10 19:06:48.000000 somweb-1.1.3/somweb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      299 2023-04-10 19:06:48.000000 somweb-1.1.3/somweb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-10 19:06:48.000000 somweb-1.1.3/somweb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       17 2023-04-10 19:06:48.000000 somweb-1.1.3/somweb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        7 2023-04-10 19:06:48.000000 somweb-1.1.3/somweb.egg-info/top_level.txt
```

### Comparing `somweb-1.1.2/LICENSE` & `somweb-1.1.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Trond Aarskog
+Copyright (c) 2023 Trond Aarskog
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `somweb-1.1.2/PKG-INFO` & `somweb-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: somweb
-Version: 1.1.2
+Version: 1.1.3
 Summary: SOMweb client. Open/close Garage doors produced by SOMMER (base+/pro+/tiga/tiga+/barrier systems)
 Home-page: https://github.com/taarskog/pysomweb
 Author: Trond Aarskog
 Author-email: somweb@heiigjen.com
 License: MIT
-Download-URL: https://github.com/taarskog/pysomweb/archive/v1.1.2.tar.gz
+Download-URL: https://github.com/taarskog/pysomweb/archive/v1.1.3.tar.gz
 Keywords: sommer,SOMweb,garage door,home assistant,home automation,heiigjen
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `somweb-1.1.2/README.md` & `somweb-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `somweb-1.1.2/setup.py` & `somweb-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `somweb-1.1.2/somweb/client.py` & `somweb-1.1.3/somweb/client.py`

 * *Files identical despite different names*

### Comparing `somweb-1.1.2/somweb/const.py` & `somweb-1.1.3/somweb/const.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 
 RE_DOORS = re.compile(
     # pylint: disable=line-too-long
     r'<\s*input\s+type\s*=\s*"submit"\s+class\s*=\s*"tab-door[\s\w-]*"\s+name\s*=\s*"tab-door\d+"\s+id\s*=\s*"tab-door(?P<id>\d+)"\s+value="(?P<name>[\w\s]+)"\s*\/?>',
     re.MULTILINE,
 )
 RE_WEBTOKEN = re.compile(
-    r'<\s*input\s+id\s*=\s*"webtoken".*value="(?P<webtoken>\w+)"\/>', re.MULTILINE
+    r'<\s*input\s+id\s*=\s*"webtoken".*value="(?P<webtoken>\w+)".*\/>', re.MULTILINE
 )
```

### Comparing `somweb-1.1.2/somweb/httpclient.py` & `somweb-1.1.3/somweb/httpclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
     async def close(self) -> None:
         """Close underlying session.
 
         Release all acquired resources.
         """
         if not self.closed:
-            await self.__session.close()
+            if self.__private_session:
+                await self.__session.close()
             self.__session = None
 
     @property
     def closed(self) -> bool:
         """Is session closed.
 
         A readonly property.
```

### Comparing `somweb-1.1.2/somweb/models.py` & `somweb-1.1.3/somweb/models.py`

 * *Files identical despite different names*

### Comparing `somweb-1.1.2/somweb.egg-info/PKG-INFO` & `somweb-1.1.3/somweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: somweb
-Version: 1.1.2
+Version: 1.1.3
 Summary: SOMweb client. Open/close Garage doors produced by SOMMER (base+/pro+/tiga/tiga+/barrier systems)
 Home-page: https://github.com/taarskog/pysomweb
 Author: Trond Aarskog
 Author-email: somweb@heiigjen.com
 License: MIT
-Download-URL: https://github.com/taarskog/pysomweb/archive/v1.1.2.tar.gz
+Download-URL: https://github.com/taarskog/pysomweb/archive/v1.1.3.tar.gz
 Keywords: sommer,SOMweb,garage door,home assistant,home automation,heiigjen
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```


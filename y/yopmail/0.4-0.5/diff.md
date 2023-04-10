# Comparing `tmp/yopmail-0.4.tar.gz` & `tmp/yopmail-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopmail-0.4.tar", last modified: Sun Jul 10 10:37:11 2022, max compression
+gzip compressed data, was "yopmail-0.5.tar", last modified: Mon Apr 10 11:32:37 2023, max compression
```

## Comparing `yopmail-0.4.tar` & `yopmail-0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2022-07-10 10:37:11.646880 yopmail-0.4/
--rw-r--r--   0 rayhan     (503) staff       (20)     1468 2022-07-10 10:37:11.646959 yopmail-0.4/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)     1169 2022-07-07 17:58:46.000000 yopmail-0.4/README.md
--rw-r--r--   0 rayhan     (503) staff       (20)      125 2022-07-10 10:37:11.647190 yopmail-0.4/setup.cfg
--rw-r--r--   0 rayhan     (503) staff       (20)      672 2022-07-10 10:37:07.000000 yopmail-0.4/setup.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2022-07-10 10:37:11.646768 yopmail-0.4/yopmail.egg-info/
--rw-r--r--   0 rayhan     (503) staff       (20)     1468 2022-07-10 10:37:11.000000 yopmail-0.4/yopmail.egg-info/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)      182 2022-07-10 10:37:11.000000 yopmail-0.4/yopmail.egg-info/SOURCES.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        1 2022-07-10 10:37:11.000000 yopmail-0.4/yopmail.egg-info/dependency_links.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       13 2022-07-10 10:37:11.000000 yopmail-0.4/yopmail.egg-info/requires.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        3 2022-07-10 10:37:11.000000 yopmail-0.4/yopmail.egg-info/top_level.txt
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-10 11:32:37.736312 yopmail-0.5/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-04-10 11:32:37.736376 yopmail-0.5/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-04-10 10:41:06.000000 yopmail-0.5/README.md
+-rw-r--r--   0 rayhan     (503) staff       (20)      125 2023-04-10 11:32:37.736594 yopmail-0.5/setup.cfg
+-rw-r--r--   0 rayhan     (503) staff       (20)      701 2023-04-10 11:30:57.000000 yopmail-0.5/setup.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-10 11:32:37.736212 yopmail-0.5/yopmail.egg-info/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-04-10 11:32:37.000000 yopmail-0.5/yopmail.egg-info/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)      182 2023-04-10 11:32:37.000000 yopmail-0.5/yopmail.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-04-10 11:32:37.000000 yopmail-0.5/yopmail.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       13 2023-04-10 11:32:37.000000 yopmail-0.5/yopmail.egg-info/requires.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        3 2023-04-10 11:32:37.000000 yopmail-0.5/yopmail.egg-info/top_level.txt
```

### Comparing `yopmail-0.4/PKG-INFO` & `yopmail-0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-Metadata-Version: 2.1
-Name: yopmail
-Version: 0.4
-Summary: A Python module to get mails from a Yopmail inbox, save them
-Home-page: https://github.com/rklf/yopmail
-Author: rklf
-License: MIT
-Keywords: yopmail get mails retrieve scrap emails
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 ###### ⚠️ Disclaimer: Reverse engineering process is shown for research purposes only.
 
 # 👏 Get mails from Yopmail inbox
 Get mails from a Yopmail inbox, save them as ``.html``
 
 
 ## 📖 Usage:
+Install the latest version from PyPI by using [pip](https://pip.pypa.io/):
+```
+pip install yopmail
+```
+
 Instantiate ``Yopmail`` class with username as parameter (with ``@`` or not) and provide proxies if needed
 ```python
 y = Yopmail('test', proxies=None)
 ```
 
 Using ``get_mail_ids()`` method you get mail ids. You can provide (optional) ``page`` parameter otherwise page 1 is used as default. You can as well provide ``proxy`` parameter which would override instantiated class proxies.
 ```python
@@ -40,8 +34,7 @@
 Feel free to contribute 🤝
 
 
 ## 📝 TODO:
 - [ ] Add CSS to saved html mail
 
 ###### Feel free to contact me wherever you find me
-
```

### Comparing `yopmail-0.4/README.md` & `yopmail-0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,30 @@
+Metadata-Version: 2.1
+Name: yopmail
+Version: 0.5
+Summary: A Python module to get mails from a Yopmail inbox, save them
+Home-page: https://github.com/rklf/yopmail
+Author: rklf
+License: MIT
+Keywords: yopmail get mails retrieve scrap emails
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 ###### ⚠️ Disclaimer: Reverse engineering process is shown for research purposes only.
 
 # 👏 Get mails from Yopmail inbox
 Get mails from a Yopmail inbox, save them as ``.html``
 
 
 ## 📖 Usage:
+Install the latest version from PyPI by using [pip](https://pip.pypa.io/):
+```
+pip install yopmail
+```
+
 Instantiate ``Yopmail`` class with username as parameter (with ``@`` or not) and provide proxies if needed
 ```python
 y = Yopmail('test', proxies=None)
 ```
 
 Using ``get_mail_ids()`` method you get mail ids. You can provide (optional) ``page`` parameter otherwise page 1 is used as default. You can as well provide ``proxy`` parameter which would override instantiated class proxies.
 ```python
@@ -28,8 +44,8 @@
 
 Feel free to contribute 🤝
 
 
 ## 📝 TODO:
 - [ ] Add CSS to saved html mail
 
-###### Feel free to contact me wherever you find me
+###### Feel free to contact me wherever you find me
```

### Comparing `yopmail-0.4/yopmail.egg-info/PKG-INFO` & `yopmail-0.5/yopmail.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 0.4
+Version: 0.5
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
-Platform: UNKNOWN
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ###### ⚠️ Disclaimer: Reverse engineering process is shown for research purposes only.
 
 # 👏 Get mails from Yopmail inbox
 Get mails from a Yopmail inbox, save them as ``.html``
 
 
 ## 📖 Usage:
+Install the latest version from PyPI by using [pip](https://pip.pypa.io/):
+```
+pip install yopmail
+```
+
 Instantiate ``Yopmail`` class with username as parameter (with ``@`` or not) and provide proxies if needed
 ```python
 y = Yopmail('test', proxies=None)
 ```
 
 Using ``get_mail_ids()`` method you get mail ids. You can provide (optional) ``page`` parameter otherwise page 1 is used as default. You can as well provide ``proxy`` parameter which would override instantiated class proxies.
 ```python
@@ -40,8 +45,7 @@
 Feel free to contribute 🤝
 
 
 ## 📝 TODO:
 - [ ] Add CSS to saved html mail
 
 ###### Feel free to contact me wherever you find me
-
```


# Comparing `tmp/fenrirWeb-0.2.0.tar.gz` & `tmp/fenrirWeb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenrirWeb-0.2.0.tar", last modified: Sun Apr  2 19:10:21 2023, max compression
+gzip compressed data, was "fenrirWeb-0.3.0.tar", last modified: Mon Apr 10 10:36:35 2023, max compression
```

## Comparing `fenrirWeb-0.2.0.tar` & `fenrirWeb-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-02 19:10:21.403770 fenrirWeb-0.2.0/
--rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-04-01 21:52:19.000000 fenrirWeb-0.2.0/LICENSE
--rw-r--r--   0 hannes    (1000) users      (100)       80 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/MANIFEST.in
--rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-02 19:10:21.403770 fenrirWeb-0.2.0/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      676 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/README.md
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-02 19:10:21.399770 fenrirWeb-0.2.0/fenrirWeb/
--rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-02 18:29:40.000000 fenrirWeb-0.2.0/fenrirWeb/__init__.py
--rw-r--r--   0 hannes    (1000) users      (100)    16718 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/lib.py
--rw-r--r--   0 hannes    (1000) users      (100)     1052 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/main.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-02 19:10:21.403770 fenrirWeb-0.2.0/fenrirWeb/static/
--rw-r--r--   0 hannes    (1000) users      (100)    80420 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/static/bootstrap.bundle.min.js
--rw-r--r--   0 hannes    (1000) users      (100)   194901 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/static/bootstrap.min.css
--rw-r--r--   0 hannes    (1000) users      (100)    60404 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/static/bootstrap.min.js
--rw-r--r--   0 hannes    (1000) users      (100)     9369 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/static/disabled.png
--rw-r--r--   0 hannes    (1000) users      (100)    20270 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/static/disabled.svg
--rw-r--r--   0 hannes    (1000) users      (100)     8004 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/static/enabled.png
--rw-r--r--   0 hannes    (1000) users      (100)    28344 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/static/enabled.svg
--rw-r--r--   0 hannes    (1000) users      (100)    93062 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/static/favicon.ico
--rw-r--r--   0 hannes    (1000) users      (100)    13258 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/static/fenrir.js
--rw-r--r--   0 hannes    (1000) users      (100)     2104 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/static/settings.png
--rw-r--r--   0 hannes    (1000) users      (100)     9046 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/view_config.py
--rw-r--r--   0 hannes    (1000) users      (100)     3152 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/view_main.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-02 19:10:21.403770 fenrirWeb-0.2.0/fenrirWeb/views/
--rw-r--r--   0 hannes    (1000) users      (100)     3046 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/views/changepassword.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     2547 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/views/createpassword.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     3064 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/views/index.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     1697 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/views/mappinginput.tpl
--rw-r--r--   0 hannes    (1000) users      (100)      939 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/views/navbar.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     8286 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/views/settings.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     2501 2023-04-02 10:40:52.000000 fenrirWeb-0.2.0/fenrirWeb/views/vpninput.tpl
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-02 19:10:21.403770 fenrirWeb-0.2.0/fenrirWeb.egg-info/
--rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-02 19:10:21.000000 fenrirWeb-0.2.0/fenrirWeb.egg-info/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      903 2023-04-02 19:10:21.000000 fenrirWeb-0.2.0/fenrirWeb.egg-info/SOURCES.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-02 19:10:21.000000 fenrirWeb-0.2.0/fenrirWeb.egg-info/dependency_links.txt
--rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-02 19:10:21.000000 fenrirWeb-0.2.0/fenrirWeb.egg-info/entry_points.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-02 18:30:18.000000 fenrirWeb-0.2.0/fenrirWeb.egg-info/not-zip-safe
--rw-r--r--   0 hannes    (1000) users      (100)       32 2023-04-02 19:10:21.000000 fenrirWeb-0.2.0/fenrirWeb.egg-info/requires.txt
--rw-r--r--   0 hannes    (1000) users      (100)       10 2023-04-02 19:10:21.000000 fenrirWeb-0.2.0/fenrirWeb.egg-info/top_level.txt
--rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-02 19:10:21.403770 fenrirWeb-0.2.0/setup.cfg
--rw-r--r--   0 hannes    (1000) users      (100)      693 2023-04-02 18:29:33.000000 fenrirWeb-0.2.0/setup.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 10:36:35.073625 fenrirWeb-0.3.0/
+-rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/LICENSE
+-rw-r--r--   0 hannes    (1000) users      (100)       80 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/MANIFEST.in
+-rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-10 10:36:35.073625 fenrirWeb-0.3.0/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      676 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/README.md
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 10:36:35.069625 fenrirWeb-0.3.0/fenrirWeb/
+-rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-10 10:35:45.000000 fenrirWeb-0.3.0/fenrirWeb/__init__.py
+-rw-r--r--   0 hannes    (1000) users      (100)    17010 2023-04-10 10:32:49.000000 fenrirWeb-0.3.0/fenrirWeb/lib.py
+-rw-r--r--   0 hannes    (1000) users      (100)     1052 2023-04-10 10:34:59.000000 fenrirWeb-0.3.0/fenrirWeb/main.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 10:36:35.073625 fenrirWeb-0.3.0/fenrirWeb/static/
+-rw-r--r--   0 hannes    (1000) users      (100)    80420 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.bundle.min.js
+-rw-r--r--   0 hannes    (1000) users      (100)   194901 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.min.css
+-rw-r--r--   0 hannes    (1000) users      (100)    60404 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.min.js
+-rw-r--r--   0 hannes    (1000) users      (100)     9369 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/disabled.png
+-rw-r--r--   0 hannes    (1000) users      (100)    20270 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/disabled.svg
+-rw-r--r--   0 hannes    (1000) users      (100)     8004 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/enabled.png
+-rw-r--r--   0 hannes    (1000) users      (100)    28344 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/enabled.svg
+-rw-r--r--   0 hannes    (1000) users      (100)    93062 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/favicon.ico
+-rw-r--r--   0 hannes    (1000) users      (100)    13258 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/fenrir.js
+-rw-r--r--   0 hannes    (1000) users      (100)     2104 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/settings.png
+-rw-r--r--   0 hannes    (1000) users      (100)     9046 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/view_config.py
+-rw-r--r--   0 hannes    (1000) users      (100)     3152 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/view_main.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 10:36:35.073625 fenrirWeb-0.3.0/fenrirWeb/views/
+-rw-r--r--   0 hannes    (1000) users      (100)     3046 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/changepassword.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     2547 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/createpassword.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     3064 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/index.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     1697 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/mappinginput.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)      939 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/navbar.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     8286 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/settings.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     2501 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/vpninput.tpl
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 10:36:35.069625 fenrirWeb-0.3.0/fenrirWeb.egg-info/
+-rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      903 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/entry_points.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 10:16:52.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/not-zip-safe
+-rw-r--r--   0 hannes    (1000) users      (100)       32 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/requires.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       10 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/top_level.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-10 10:36:35.073625 fenrirWeb-0.3.0/setup.cfg
+-rw-r--r--   0 hannes    (1000) users      (100)      693 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/setup.py
```

### Comparing `fenrirWeb-0.2.0/LICENSE` & `fenrirWeb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/README.md` & `fenrirWeb-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/lib.py` & `fenrirWeb-0.3.0/fenrirWeb/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from bcrypt import gensalt, hashpw
 from fenrir.filehandler import filehandler
 from fenrir.fenrir import Fenrir
 from json import loads, dumps
 from os import O_RDWR, O_NONBLOCK, fdopen, open as osopen
 from select import select
 from time import sleep
+from cryptography.fernet import InvalidToken
 
 APPPATH = dirname(realpath(__file__))
 TEMPLATE_PATH[:] = [f'{APPPATH}/views']
 DBPATH = '/var/cache/fenrir/fenrir.sqlite'
 NEEDSPASSWORDCHECK = False
 
 
@@ -241,19 +242,23 @@
             valuedict = {}
             for i, result in enumerate(results):
                 valuedict['profilename'] = result[0]
                 valuedict['description'] = result[1]
                 valuedict['isdefault'] = result[2]
                 valuedict['ondemand'] = result[3]
                 if getauth:
-                    fh = filehandler(passphrase=passphrase)
-                    valuedict['username'] = fh.decode(result[4].decode('utf-8')).decode('utf-8')
-                    valuedict['password'] = fh.decode(result[5].decode('utf-8')).decode('utf-8')
-                    valuedict['vpnconfig'] = fh.decode(result[6].decode('utf-8')).decode('utf-8')
-                    valuedict['vpnprofileid'] = result[7]
+                    try:
+                        fh = filehandler(passphrase=passphrase)
+                        valuedict['username'] = fh.decode(result[4].decode('utf-8')).decode('utf-8')
+                        valuedict['password'] = fh.decode(result[5].decode('utf-8')).decode('utf-8')
+                        valuedict['vpnconfig'] = fh.decode(result[6].decode('utf-8')).decode('utf-8')
+                        valuedict['vpnprofileid'] = result[7]
+                    except InvalidToken:
+                        if passphrase:
+                            return getvpnconfig(profilename=profilename, getauth=getauth, dbpath=dbpath, passphrase=None)
                 returndict[f'profile{i}'] = valuedict.copy()
     except OperationalError as e:
         debug(f'unable to query Database {dbpath}: {e}')
 
     return returndict
```

### Comparing `fenrirWeb-0.2.0/fenrirWeb/main.py` & `fenrirWeb-0.3.0/fenrirWeb/main.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/static/bootstrap.bundle.min.js` & `fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/static/bootstrap.min.css` & `fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/static/bootstrap.min.js` & `fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/static/disabled.png` & `fenrirWeb-0.3.0/fenrirWeb/static/disabled.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/static/disabled.svg` & `fenrirWeb-0.3.0/fenrirWeb/static/disabled.svg`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/static/enabled.png` & `fenrirWeb-0.3.0/fenrirWeb/static/enabled.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/static/enabled.svg` & `fenrirWeb-0.3.0/fenrirWeb/static/enabled.svg`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/static/favicon.ico` & `fenrirWeb-0.3.0/fenrirWeb/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/static/fenrir.js` & `fenrirWeb-0.3.0/fenrirWeb/static/fenrir.js`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/static/settings.png` & `fenrirWeb-0.3.0/fenrirWeb/static/settings.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/view_config.py` & `fenrirWeb-0.3.0/fenrirWeb/view_config.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/view_main.py` & `fenrirWeb-0.3.0/fenrirWeb/view_main.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/views/changepassword.tpl` & `fenrirWeb-0.3.0/fenrirWeb/views/changepassword.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/views/createpassword.tpl` & `fenrirWeb-0.3.0/fenrirWeb/views/createpassword.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/views/index.tpl` & `fenrirWeb-0.3.0/fenrirWeb/views/index.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/views/mappinginput.tpl` & `fenrirWeb-0.3.0/fenrirWeb/views/mappinginput.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/views/navbar.tpl` & `fenrirWeb-0.3.0/fenrirWeb/views/navbar.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/views/settings.tpl` & `fenrirWeb-0.3.0/fenrirWeb/views/settings.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb/views/vpninput.tpl` & `fenrirWeb-0.3.0/fenrirWeb/views/vpninput.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/fenrirWeb.egg-info/SOURCES.txt` & `fenrirWeb-0.3.0/fenrirWeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.2.0/setup.py` & `fenrirWeb-0.3.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/pythonegardia-1.0.8.tar.gz` & `tmp/pythonegardia-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythonegardia-1.0.8.tar", last modified: Sun Jul  9 10:35:01 2017, max compression
+gzip compressed data, was "dist/pythonegardia-1.0.9.tar", last modified: Tue Jul 11 13:49:50 2017, max compression
```

## Comparing `pythonegardia-1.0.8.tar` & `pythonegardia-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2017-07-09 10:35:01.000000 pythonegardia-1.0.8/
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       59 2017-07-09 10:35:01.000000 pythonegardia-1.0.8/setup.cfg
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      275 2017-07-09 10:35:01.000000 pythonegardia-1.0.8/PKG-INFO
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2017-07-09 10:35:01.000000 pythonegardia-1.0.8/pythonegardia/
--rw-r--r--   0 jeroen    (1000) jeroen    (1000)     1341 2017-07-07 15:28:09.000000 pythonegardia-1.0.8/pythonegardia/egardiareportservice.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     3162 2017-07-09 10:32:56.000000 pythonegardia-1.0.8/pythonegardia/egardiadevice.py
--rw-r--r--   0 jeroen    (1000) jeroen    (1000)      127 2017-07-09 10:33:34.000000 pythonegardia-1.0.8/pythonegardia/test.py
--rw-r--r--   0 jeroen    (1000) root         (0)        2 2017-07-06 17:47:33.000000 pythonegardia-1.0.8/pythonegardia/__init__.py
--rw-r--r--   0 jeroen    (1000) jeroen    (1000)      490 2017-07-09 10:34:20.000000 pythonegardia-1.0.8/setup.py
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2017-07-09 10:35:01.000000 pythonegardia-1.0.8/pythonegardia.egg-info/
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        1 2017-07-09 10:35:01.000000 pythonegardia-1.0.8/pythonegardia.egg-info/dependency_links.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       14 2017-07-09 10:35:01.000000 pythonegardia-1.0.8/pythonegardia.egg-info/requires.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      341 2017-07-09 10:35:01.000000 pythonegardia-1.0.8/pythonegardia.egg-info/SOURCES.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      275 2017-07-09 10:35:01.000000 pythonegardia-1.0.8/pythonegardia.egg-info/PKG-INFO
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       14 2017-07-09 10:35:01.000000 pythonegardia-1.0.8/pythonegardia.egg-info/top_level.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        1 2017-07-07 12:41:01.000000 pythonegardia-1.0.8/pythonegardia.egg-info/zip-safe
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2017-07-11 13:49:50.000000 pythonegardia-1.0.9/
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       59 2017-07-11 13:49:50.000000 pythonegardia-1.0.9/setup.cfg
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      275 2017-07-11 13:49:50.000000 pythonegardia-1.0.9/PKG-INFO
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2017-07-11 13:49:50.000000 pythonegardia-1.0.9/pythonegardia/
+-rw-r--r--   0 jeroen    (1000) jeroen    (1000)     1341 2017-07-07 15:28:09.000000 pythonegardia-1.0.9/pythonegardia/egardiareportservice.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     3235 2017-07-11 13:47:40.000000 pythonegardia-1.0.9/pythonegardia/egardiadevice.py
+-rw-r--r--   0 jeroen    (1000) jeroen    (1000)      127 2017-07-09 10:33:34.000000 pythonegardia-1.0.9/pythonegardia/test.py
+-rw-r--r--   0 jeroen    (1000) root         (0)        2 2017-07-06 17:47:33.000000 pythonegardia-1.0.9/pythonegardia/__init__.py
+-rw-r--r--   0 jeroen    (1000) jeroen    (1000)      490 2017-07-11 13:48:29.000000 pythonegardia-1.0.9/setup.py
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2017-07-11 13:49:50.000000 pythonegardia-1.0.9/pythonegardia.egg-info/
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        1 2017-07-11 13:49:50.000000 pythonegardia-1.0.9/pythonegardia.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       14 2017-07-11 13:49:50.000000 pythonegardia-1.0.9/pythonegardia.egg-info/requires.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      341 2017-07-11 13:49:50.000000 pythonegardia-1.0.9/pythonegardia.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      275 2017-07-11 13:49:50.000000 pythonegardia-1.0.9/pythonegardia.egg-info/PKG-INFO
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       14 2017-07-11 13:49:50.000000 pythonegardia-1.0.9/pythonegardia.egg-info/top_level.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        1 2017-07-07 12:41:01.000000 pythonegardia-1.0.9/pythonegardia.egg-info/zip-safe
```

### Comparing `pythonegardia-1.0.8/pythonegardia/egardiareportservice.py` & `pythonegardia-1.0.9/pythonegardia/egardiareportservice.py`

 * *Files identical despite different names*

### Comparing `pythonegardia-1.0.8/pythonegardia/egardiadevice.py` & `pythonegardia-1.0.9/pythonegardia/egardiadevice.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,18 @@
         r = self.sendCondition(0)
         _LOGGER.info("Egardia alarm arming away, result: "+r)
 
     def sendCondition(self, p):
         import requests
         #Send payload to panelCondPost
         payload = {'area': '1', 'mode': p}
-        r = self.doRequest('POST', 'panelCondPost', payload)
+	try:
+            r = self.doRequest('POST', 'panelCondPost', payload)
+        except:
+            raise
+            return "UNKNOWN"
         statustext = r.text
         ind1 = statustext.find('result : ')
         statustext = statustext[ind1+9:]
         ind2 = statustext.find(',')
         statustext = statustext[:ind2]
         return statustext
```


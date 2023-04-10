# Comparing `tmp/Barky-1.0.2.tar.gz` & `tmp/Barky-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Barky-1.0.2.tar", last modified: Mon Apr 10 08:33:25 2023, max compression
+gzip compressed data, was "Barky-1.0.3.tar", last modified: Mon Apr 10 08:57:58 2023, max compression
```

## Comparing `Barky-1.0.2.tar` & `Barky-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 08:33:25.093936 Barky-1.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 08:33:25.093936 Barky-1.0.2/Barky.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1562 2023-04-10 08:33:24.000000 Barky-1.0.2/Barky.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-10 08:33:25.000000 Barky-1.0.2/Barky.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 08:33:24.000000 Barky-1.0.2/Barky.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-10 08:33:24.000000 Barky-1.0.2/Barky.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-10 08:33:24.000000 Barky-1.0.2/Barky.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 04:15:25.000000 Barky-1.0.2/Barky.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     1065 2023-04-10 03:20:32.000000 Barky-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1562 2023-04-10 08:33:25.093936 Barky-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      998 2023-04-10 06:28:33.000000 Barky-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 08:33:25.093936 Barky-1.0.2/barky/
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-10 08:33:02.000000 Barky-1.0.2/barky/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5671 2023-04-10 03:10:19.000000 Barky-1.0.2/barky/barky.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 08:33:25.093936 Barky-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3153 2023-04-10 03:10:38.000000 Barky-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 08:57:58.943936 Barky-1.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 08:57:58.943936 Barky-1.0.3/Barky.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-04-10 08:57:58.000000 Barky-1.0.3/Barky.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-10 08:57:58.000000 Barky-1.0.3/Barky.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 08:57:58.000000 Barky-1.0.3/Barky.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-10 08:57:58.000000 Barky-1.0.3/Barky.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-10 08:57:58.000000 Barky-1.0.3/Barky.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 04:15:25.000000 Barky-1.0.3/Barky.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-10 03:20:32.000000 Barky-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-04-10 08:57:58.943936 Barky-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-10 06:28:33.000000 Barky-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 08:57:58.943936 Barky-1.0.3/barky/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-10 08:49:03.000000 Barky-1.0.3/barky/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5671 2023-04-10 08:47:29.000000 Barky-1.0.3/barky/barky.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 08:57:58.943936 Barky-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3153 2023-04-10 03:10:38.000000 Barky-1.0.3/setup.py
```

### Comparing `Barky-1.0.2/Barky.egg-info/PKG-INFO` & `Barky-1.0.3/Barky.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Barky
-Version: 1.0.2
+Version: 1.0.3
 Summary: Push notifications to your iPhone with Bark.
 Home-page: https://github.com/well-shark/Barky
 Author: WellShark
 Author-email: wellshark.net@gmail.com
 License: MIT
 Keywords: Bark,Push,Notification,iPhone,iOS
 Platform: UNKNOWN
```

### Comparing `Barky-1.0.2/LICENSE` & `Barky-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Barky-1.0.2/PKG-INFO` & `Barky-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Barky
-Version: 1.0.2
+Version: 1.0.3
 Summary: Push notifications to your iPhone with Bark.
 Home-page: https://github.com/well-shark/Barky
 Author: WellShark
 Author-email: wellshark.net@gmail.com
 License: MIT
 Keywords: Bark,Push,Notification,iPhone,iOS
 Platform: UNKNOWN
```

### Comparing `Barky-1.0.2/README.md` & `Barky-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Barky-1.0.2/barky/barky.py` & `Barky-1.0.3/barky/barky.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         if not os.path.exists(self.config_file):
             return None, None
         else:
             config = configparser.ConfigParser()
             config.read(self.config_file)
             server = config['DEFAULT']['server']
             key = config['DEFAULT']['client_key']
-            return key, server
+            return server, key
 
 def main(*argv):
     ''' For build command line tool
     '''
     if not argv:
         argv = list(sys.argv)
```

### Comparing `Barky-1.0.2/setup.py` & `Barky-1.0.3/setup.py`

 * *Files identical despite different names*

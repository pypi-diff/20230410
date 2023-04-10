# Comparing `tmp/pyvosklivesubtitle-0.0.8.tar.gz` & `tmp/pyvosklivesubtitle-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvosklivesubtitle-0.0.8.tar", last modified: Wed Feb  8 03:44:20 2023, max compression
+gzip compressed data, was "pyvosklivesubtitle-0.1.2.tar", last modified: Mon Apr 10 02:10:48 2023, max compression
```

## Comparing `pyvosklivesubtitle-0.0.8.tar` & `pyvosklivesubtitle-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 03:44:20.721623 pyvosklivesubtitle-0.0.8/
--rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1617 2023-02-08 03:44:20.723121 pyvosklivesubtitle-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4177 2022-11-06 07:43:14.000000 pyvosklivesubtitle-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-08 03:44:20.697646 pyvosklivesubtitle-0.0.8/pyvosklivesubtitle/
--rw-rw-rw-   0        0        0    30913 2023-02-08 03:41:11.000000 pyvosklivesubtitle-0.0.8/pyvosklivesubtitle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 03:44:20.719374 pyvosklivesubtitle-0.0.8/pyvosklivesubtitle.egg-info/
--rw-rw-rw-   0        0        0     1617 2023-02-08 03:44:20.000000 pyvosklivesubtitle-0.0.8/pyvosklivesubtitle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-02-08 03:44:20.000000 pyvosklivesubtitle-0.0.8/pyvosklivesubtitle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 03:44:20.000000 pyvosklivesubtitle-0.0.8/pyvosklivesubtitle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-02-08 03:44:20.000000 pyvosklivesubtitle-0.0.8/pyvosklivesubtitle.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-02-08 03:44:20.000000 pyvosklivesubtitle-0.0.8/pyvosklivesubtitle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-02-08 03:44:20.000000 pyvosklivesubtitle-0.0.8/pyvosklivesubtitle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-02-08 03:44:20.726117 pyvosklivesubtitle-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1490 2023-02-08 03:43:17.000000 pyvosklivesubtitle-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:10:48.889864 pyvosklivesubtitle-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1617 2023-04-10 02:10:48.890610 pyvosklivesubtitle-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4177 2022-11-06 07:43:14.000000 pyvosklivesubtitle-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 02:10:48.849403 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle/
+-rw-rw-rw-   0        0        0    90112 2023-04-10 02:09:51.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:10:48.888363 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/
+-rw-rw-rw-   0        0        0     1617 2023-04-10 02:10:47.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-10 02:10:48.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 02:10:47.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-10 02:10:47.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      109 2023-04-10 02:10:47.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-10 02:10:47.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-10 02:10:48.893607 pyvosklivesubtitle-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1556 2023-04-10 02:10:11.000000 pyvosklivesubtitle-0.1.2/setup.py
```

### Comparing `pyvosklivesubtitle-0.0.8/LICENSE` & `pyvosklivesubtitle-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.0.8/PKG-INFO` & `pyvosklivesubtitle-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvosklivesubtitle
-Version: 0.0.8
+Version: 0.1.2
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.0.8/README.md` & `pyvosklivesubtitle-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.0.8/pyvosklivesubtitle.egg-info/PKG-INFO` & `pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvosklivesubtitle
-Version: 0.0.8
+Version: 0.1.2
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.0.8/setup.py` & `pyvosklivesubtitle-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,29 @@
     'pyvosklivesubtitle is a python based desktop aplication which can recognize any live streaming'
     'in 21 languages that supported by VOSK then translate and display it as LIVE SUBTITLES'
     )
 
 setup(
     name="pyvosklivesubtitle",
     description="A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES",
-    version="0.0.8",
+    version="0.1.2",
     include_package_data=True,
     author='Bot Bahlul',
     author_email='bot.bahlul@gmail.com',
     url='https://github.com/botbahlul/pyvosklivesubtitle',
     packages=[str('pyvosklivesubtitle')],
     entry_points={
         'console_scripts': [
             'pyvosklivesubtitle = pyvosklivesubtitle:main',
         ],
     },
     install_requires=[
         'sounddevice>=0.4.4',
         'vosk>=0.3.44',
-        'pygoogletranslation>=2.0.6',
         'pysimplegui>=4.60.1',
+        "httpx>=0.13.3",
+        "streamlink>=5.3.1",
+        "six>=1.16.0",
+        "pysrt>=1.1.2",
     ],
     license=open("LICENSE").read()
 )
```


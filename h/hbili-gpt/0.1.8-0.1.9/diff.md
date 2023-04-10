# Comparing `tmp/hbili-gpt-0.1.8.tar.gz` & `tmp/hbili-gpt-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbili-gpt-0.1.8.tar", last modified: Mon Mar 27 00:56:50 2023, max compression
+gzip compressed data, was "hbili-gpt-0.1.9.tar", last modified: Mon Mar 27 00:57:30 2023, max compression
```

## Comparing `hbili-gpt-0.1.8.tar` & `hbili-gpt-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-03-27 00:56:50.871824 hbili-gpt-0.1.8/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      705 2023-03-27 00:56:50.871824 hbili-gpt-0.1.8/PKG-INFO
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-03-27 00:56:50.871824 hbili-gpt-0.1.8/hbili_gpt/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hbili-gpt-0.1.8/hbili_gpt/__init__.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     4686 2023-03-27 00:56:34.000000 hbili-gpt-0.1.8/hbili_gpt/bilibili.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     3482 2023-03-26 06:56:44.000000 hbili-gpt-0.1.8/hbili_gpt/gpt.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)    12512 2023-03-26 06:56:44.000000 hbili-gpt-0.1.8/hbili_gpt/notion.py
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-03-27 00:56:50.871824 hbili-gpt-0.1.8/hbili_gpt.egg-info/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      705 2023-03-27 00:56:50.000000 hbili-gpt-0.1.8/hbili_gpt.egg-info/PKG-INFO
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      221 2023-03-27 00:56:50.000000 hbili-gpt-0.1.8/hbili_gpt.egg-info/SOURCES.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-03-27 00:56:50.000000 hbili-gpt-0.1.8/hbili_gpt.egg-info/dependency_links.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)       10 2023-03-27 00:56:50.000000 hbili-gpt-0.1.8/hbili_gpt.egg-info/top_level.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-03-27 00:56:50.871824 hbili-gpt-0.1.8/setup.cfg
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      814 2023-03-27 00:56:45.000000 hbili-gpt-0.1.8/setup.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-03-27 00:57:30.412299 hbili-gpt-0.1.9/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      705 2023-03-27 00:57:30.412299 hbili-gpt-0.1.9/PKG-INFO
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-03-27 00:57:30.412299 hbili-gpt-0.1.9/hbili_gpt/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hbili-gpt-0.1.9/hbili_gpt/__init__.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     4683 2023-03-27 00:57:17.000000 hbili-gpt-0.1.9/hbili_gpt/bilibili.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     3482 2023-03-26 06:56:44.000000 hbili-gpt-0.1.9/hbili_gpt/gpt.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)    12512 2023-03-26 06:56:44.000000 hbili-gpt-0.1.9/hbili_gpt/notion.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-03-27 00:57:30.412299 hbili-gpt-0.1.9/hbili_gpt.egg-info/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      705 2023-03-27 00:57:30.000000 hbili-gpt-0.1.9/hbili_gpt.egg-info/PKG-INFO
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      221 2023-03-27 00:57:30.000000 hbili-gpt-0.1.9/hbili_gpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-03-27 00:57:30.000000 hbili-gpt-0.1.9/hbili_gpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)       10 2023-03-27 00:57:30.000000 hbili-gpt-0.1.9/hbili_gpt.egg-info/top_level.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-03-27 00:57:30.412299 hbili-gpt-0.1.9/setup.cfg
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      814 2023-03-27 00:57:26.000000 hbili-gpt-0.1.9/setup.py
```

### Comparing `hbili-gpt-0.1.8/PKG-INFO` & `hbili-gpt-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbili-gpt
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for GPT and Bilibili
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hbili-gpt-0.1.8/hbili_gpt/bilibili.py` & `hbili-gpt-0.1.9/hbili_gpt/bilibili.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.prompt = prompt
         self.notion_database_id = notion_database_id
         self.notion_token = notion_token
 
     def summary(self, blink: str) -> Dict[str, str]:
         if not self.is_valid_bilibili_url(blink):
             return {'status': 'failed', 'url': blink, 'subtitles': [], 'summaries': 'Invalid bilibili url'}
-        bvid = self.parse_bilibili_url(blink)
+        bvid = self.get_bilibili_id(blink)
         logging.info(f'Start processing video information: {bvid}')
         subtitles = self.__bili_subtitle(
             bvid, self.__bili_player_list(bvid)[0])
         if not subtitles:
             return {'status': 'failed', 'url': blink, 'subtitles': [], 'summaries': 'No subtitles found'}
         logging.info('Subtitle obtained successfully')
         seged_text = segTranscipt(subtitles)
```

### Comparing `hbili-gpt-0.1.8/hbili_gpt/gpt.py` & `hbili-gpt-0.1.9/hbili_gpt/gpt.py`

 * *Files identical despite different names*

### Comparing `hbili-gpt-0.1.8/hbili_gpt/notion.py` & `hbili-gpt-0.1.9/hbili_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hbili-gpt-0.1.8/hbili_gpt.egg-info/PKG-INFO` & `hbili-gpt-0.1.9/hbili_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbili-gpt
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for GPT and Bilibili
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hbili-gpt-0.1.8/setup.py` & `hbili-gpt-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hbili-gpt',
-    version='0.1.8',
+    version='0.1.9',
     description='A library for GPT and Bilibili',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```


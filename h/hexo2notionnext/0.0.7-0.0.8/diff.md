# Comparing `tmp/hexo2notionnext-0.0.7.tar.gz` & `tmp/hexo2notionnext-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexo2notionnext-0.0.7.tar", last modified: Mon Apr 10 02:17:51 2023, max compression
+gzip compressed data, was "hexo2notionnext-0.0.8.tar", last modified: Mon Apr 10 05:05:34 2023, max compression
```

## Comparing `hexo2notionnext-0.0.7.tar` & `hexo2notionnext-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 02:17:51.087220 hexo2notionnext-0.0.7/
--rw-r--r--   0 weizhang   (501) staff       (20)     1064 2023-04-06 11:20:35.000000 hexo2notionnext-0.0.7/LICENSE
--rw-r--r--   0 weizhang   (501) staff       (20)     2845 2023-04-10 02:17:51.086547 hexo2notionnext-0.0.7/PKG-INFO
--rw-r--r--   0 weizhang   (501) staff       (20)     2013 2023-04-10 02:11:01.000000 hexo2notionnext-0.0.7/README.md
-drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 02:17:51.081128 hexo2notionnext-0.0.7/hexo2notionnext/
--rw-r--r--   0 weizhang   (501) staff       (20)        0 2023-04-08 08:18:06.000000 hexo2notionnext-0.0.7/hexo2notionnext/__init__.py
--rw-r--r--   0 weizhang   (501) staff       (20)     6469 2023-04-09 10:18:51.000000 hexo2notionnext-0.0.7/hexo2notionnext/hexo2notionnext.py
-drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 02:17:51.085710 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/
--rw-r--r--   0 weizhang   (501) staff       (20)     2845 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/PKG-INFO
--rw-r--r--   0 weizhang   (501) staff       (20)      325 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/SOURCES.txt
--rw-r--r--   0 weizhang   (501) staff       (20)        1 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/dependency_links.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       73 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/entry_points.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       67 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/requires.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       16 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/top_level.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       38 2023-04-10 02:17:51.087508 hexo2notionnext-0.0.7/setup.cfg
--rw-r--r--   0 weizhang   (501) staff       (20)     1256 2023-04-10 02:12:10.000000 hexo2notionnext-0.0.7/setup.py
+drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 05:05:34.031396 hexo2notionnext-0.0.8/
+-rw-r--r--   0 weizhang   (501) staff       (20)     1064 2023-04-06 11:20:35.000000 hexo2notionnext-0.0.8/LICENSE
+-rw-r--r--   0 weizhang   (501) staff       (20)     2845 2023-04-10 05:05:34.030865 hexo2notionnext-0.0.8/PKG-INFO
+-rw-r--r--   0 weizhang   (501) staff       (20)     2013 2023-04-10 02:11:01.000000 hexo2notionnext-0.0.8/README.md
+drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 05:05:34.025493 hexo2notionnext-0.0.8/hexo2notionnext/
+-rw-r--r--   0 weizhang   (501) staff       (20)        0 2023-04-08 08:18:06.000000 hexo2notionnext-0.0.8/hexo2notionnext/__init__.py
+-rw-r--r--   0 weizhang   (501) staff       (20)     6476 2023-04-10 05:02:57.000000 hexo2notionnext-0.0.8/hexo2notionnext/hexo2notionnext.py
+drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 05:05:34.030039 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/
+-rw-r--r--   0 weizhang   (501) staff       (20)     2845 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/PKG-INFO
+-rw-r--r--   0 weizhang   (501) staff       (20)      325 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/SOURCES.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)        1 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/dependency_links.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       73 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/entry_points.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       67 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/requires.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       16 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/top_level.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       38 2023-04-10 05:05:34.031545 hexo2notionnext-0.0.8/setup.cfg
+-rw-r--r--   0 weizhang   (501) staff       (20)     1256 2023-04-10 05:05:17.000000 hexo2notionnext-0.0.8/setup.py
```

### Comparing `hexo2notionnext-0.0.7/LICENSE` & `hexo2notionnext-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hexo2notionnext-0.0.7/PKG-INFO` & `hexo2notionnext-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexo2notionnext
-Version: 0.0.7
+Version: 0.0.8
 Summary: Convert hexo  to notionnext
 Home-page: https://github.com/zhangweidev/hexo2notionnext
 Author: zhangwei
 Author-email: chxxiu+dev@gmail.com
 License: MIT
 Keywords: hexo notion notion.so notion-py markdown md converter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hexo2notionnext-0.0.7/README.md` & `hexo2notionnext-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hexo2notionnext-0.0.7/hexo2notionnext/hexo2notionnext.py` & `hexo2notionnext-0.0.8/hexo2notionnext/hexo2notionnext.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     sulg_dcit["hour"] = page.get("date").strftime("%H")
     sulg_dcit["minute"] = page.get("date").strftime("%M")
     sulg_dcit["second"] = page.get("date").strftime("%S")
     sulg_dcit["title"] = page.get("title","").replace(" ", "")  
     category = page.get("category")  
     sulg_dcit["category"] = "/".join(category) if category else ""
     sulg_dcit["name"] = page.get("name","")
-    sulg_dcit["post_tile"]=page.get("post_title","")
+    sulg_dcit["post_title"]=page.get("post_title","")
     sulg_dcit["hash"] = sulg_hash(sulg_dcit["title"],page.get("date")) 
     return _format_parse(sulg_dcit,s)
  
 
 # read hexo post file,return sorted list
 def read_post_file(hexo_post_path,sulg_format): 
     hexo_post_path = os.path.abspath(hexo_post_path) 
@@ -126,15 +126,15 @@
             
             content = page.get("content") 
             fp = page.get("filepath") 
 
             row = cv.collection.add_row()
             row.type = "Post"
             row.status= "Published"
-            row.title=page.get("name") 
+            row.title=page.get("post_title") 
             row.summary=content[0:200]+"..."
             row.slug= page.get("sulg") 
 
             if typ != "nobelium" :
                 category =  page.get("category")
                 if category:
                     row.category= category[0]
```

### Comparing `hexo2notionnext-0.0.7/hexo2notionnext.egg-info/PKG-INFO` & `hexo2notionnext-0.0.8/hexo2notionnext.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexo2notionnext
-Version: 0.0.7
+Version: 0.0.8
 Summary: Convert hexo  to notionnext
 Home-page: https://github.com/zhangweidev/hexo2notionnext
 Author: zhangwei
 Author-email: chxxiu+dev@gmail.com
 License: MIT
 Keywords: hexo notion notion.so notion-py markdown md converter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hexo2notionnext-0.0.7/setup.py` & `hexo2notionnext-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='hexo2notionnext',
-    version='0.0.7',
+    version='0.0.8',
     description='Convert hexo  to notionnext',
     long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     url='https://github.com/zhangweidev/hexo2notionnext',
     author='zhangwei',
     author_email='chxxiu+dev@gmail.com',
     license='MIT',
```


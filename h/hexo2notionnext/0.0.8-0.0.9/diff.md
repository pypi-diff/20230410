# Comparing `tmp/hexo2notionnext-0.0.8.tar.gz` & `tmp/hexo2notionnext-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexo2notionnext-0.0.8.tar", last modified: Mon Apr 10 05:05:34 2023, max compression
+gzip compressed data, was "hexo2notionnext-0.0.9.tar", last modified: Mon Apr 10 06:34:29 2023, max compression
```

## Comparing `hexo2notionnext-0.0.8.tar` & `hexo2notionnext-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 05:05:34.031396 hexo2notionnext-0.0.8/
--rw-r--r--   0 weizhang   (501) staff       (20)     1064 2023-04-06 11:20:35.000000 hexo2notionnext-0.0.8/LICENSE
--rw-r--r--   0 weizhang   (501) staff       (20)     2845 2023-04-10 05:05:34.030865 hexo2notionnext-0.0.8/PKG-INFO
--rw-r--r--   0 weizhang   (501) staff       (20)     2013 2023-04-10 02:11:01.000000 hexo2notionnext-0.0.8/README.md
-drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 05:05:34.025493 hexo2notionnext-0.0.8/hexo2notionnext/
--rw-r--r--   0 weizhang   (501) staff       (20)        0 2023-04-08 08:18:06.000000 hexo2notionnext-0.0.8/hexo2notionnext/__init__.py
--rw-r--r--   0 weizhang   (501) staff       (20)     6476 2023-04-10 05:02:57.000000 hexo2notionnext-0.0.8/hexo2notionnext/hexo2notionnext.py
-drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 05:05:34.030039 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/
--rw-r--r--   0 weizhang   (501) staff       (20)     2845 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/PKG-INFO
--rw-r--r--   0 weizhang   (501) staff       (20)      325 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/SOURCES.txt
--rw-r--r--   0 weizhang   (501) staff       (20)        1 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/dependency_links.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       73 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/entry_points.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       67 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/requires.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       16 2023-04-10 05:05:33.000000 hexo2notionnext-0.0.8/hexo2notionnext.egg-info/top_level.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       38 2023-04-10 05:05:34.031545 hexo2notionnext-0.0.8/setup.cfg
--rw-r--r--   0 weizhang   (501) staff       (20)     1256 2023-04-10 05:05:17.000000 hexo2notionnext-0.0.8/setup.py
+drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 06:34:29.649578 hexo2notionnext-0.0.9/
+-rw-r--r--   0 weizhang   (501) staff       (20)     1064 2023-04-06 11:20:35.000000 hexo2notionnext-0.0.9/LICENSE
+-rw-r--r--   0 weizhang   (501) staff       (20)     2845 2023-04-10 06:34:29.648902 hexo2notionnext-0.0.9/PKG-INFO
+-rw-r--r--   0 weizhang   (501) staff       (20)     2013 2023-04-10 02:11:01.000000 hexo2notionnext-0.0.9/README.md
+drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 06:34:29.641876 hexo2notionnext-0.0.9/hexo2notionnext/
+-rw-r--r--   0 weizhang   (501) staff       (20)        0 2023-04-08 08:18:06.000000 hexo2notionnext-0.0.9/hexo2notionnext/__init__.py
+-rw-r--r--   0 weizhang   (501) staff       (20)     6458 2023-04-10 06:32:49.000000 hexo2notionnext-0.0.9/hexo2notionnext/hexo2notionnext.py
+drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 06:34:29.647753 hexo2notionnext-0.0.9/hexo2notionnext.egg-info/
+-rw-r--r--   0 weizhang   (501) staff       (20)     2845 2023-04-10 06:34:29.000000 hexo2notionnext-0.0.9/hexo2notionnext.egg-info/PKG-INFO
+-rw-r--r--   0 weizhang   (501) staff       (20)      325 2023-04-10 06:34:29.000000 hexo2notionnext-0.0.9/hexo2notionnext.egg-info/SOURCES.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)        1 2023-04-10 06:34:29.000000 hexo2notionnext-0.0.9/hexo2notionnext.egg-info/dependency_links.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       73 2023-04-10 06:34:29.000000 hexo2notionnext-0.0.9/hexo2notionnext.egg-info/entry_points.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       67 2023-04-10 06:34:29.000000 hexo2notionnext-0.0.9/hexo2notionnext.egg-info/requires.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       16 2023-04-10 06:34:29.000000 hexo2notionnext-0.0.9/hexo2notionnext.egg-info/top_level.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       38 2023-04-10 06:34:29.649733 hexo2notionnext-0.0.9/setup.cfg
+-rw-r--r--   0 weizhang   (501) staff       (20)     1256 2023-04-10 06:33:01.000000 hexo2notionnext-0.0.9/setup.py
```

### Comparing `hexo2notionnext-0.0.8/LICENSE` & `hexo2notionnext-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hexo2notionnext-0.0.8/PKG-INFO` & `hexo2notionnext-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexo2notionnext
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert hexo  to notionnext
 Home-page: https://github.com/zhangweidev/hexo2notionnext
 Author: zhangwei
 Author-email: chxxiu+dev@gmail.com
 License: MIT
 Keywords: hexo notion notion.so notion-py markdown md converter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hexo2notionnext-0.0.8/README.md` & `hexo2notionnext-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hexo2notionnext-0.0.8/hexo2notionnext/hexo2notionnext.py` & `hexo2notionnext-0.0.9/hexo2notionnext/hexo2notionnext.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 
 
 def _format_parse(data: dict, s: str):
     result = s
     for key,value in data.items():
         if value:
             result = result.replace(f':{key}', value)
-    return result.replace("//", "/")
+    return result.replace("//", "/").replace(" ", "")  
 
 def sulg_format_parse(page: dict, s: str): 
     sulg_dcit={} 
 
     sulg_dcit["year"] = page.get("date").strftime("%Y") 
     sulg_dcit["month"] = page.get("date").strftime("%m") 
     sulg_dcit["day"] = '{:02d}'.format(page.get("date").day)
     sulg_dcit["i_month"] = '{:d}'.format( page.get("date").month)
     sulg_dcit["i_day"] = '{:d}'.format(page.get("date").day)
     sulg_dcit["hour"] = page.get("date").strftime("%H")
     sulg_dcit["minute"] = page.get("date").strftime("%M")
     sulg_dcit["second"] = page.get("date").strftime("%S")
-    sulg_dcit["title"] = page.get("title","").replace(" ", "")  
+    sulg_dcit["title"] = page.get("title","")
     category = page.get("category")  
     sulg_dcit["category"] = "/".join(category) if category else ""
     sulg_dcit["name"] = page.get("name","")
     sulg_dcit["post_title"]=page.get("post_title","")
     sulg_dcit["hash"] = sulg_hash(sulg_dcit["title"],page.get("date")) 
     return _format_parse(sulg_dcit,s)
  
@@ -70,15 +70,15 @@
             
                 mdStr = mdFile.read() 
                 mdStr = mdStr.strip('-').strip() 
                 mdChunks = mdStr.split("---",1) 
                 header = yaml.safe_load(mdChunks[0])
                 content = mdChunks[1]
 
-                post_title = header.get('title',"").replace(" ", "") 
+                post_title = header.get('title',"")
                 date = header.get('date')
             
                 if  isinstance(date, str):
                     date = parse(date)
                 if  not isinstance(date, datetime):     
                     f_create_time = os.path.getctime(fp)
                     date= datetime.fromtimestamp(f_create_time)
```

### Comparing `hexo2notionnext-0.0.8/hexo2notionnext.egg-info/PKG-INFO` & `hexo2notionnext-0.0.9/hexo2notionnext.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexo2notionnext
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert hexo  to notionnext
 Home-page: https://github.com/zhangweidev/hexo2notionnext
 Author: zhangwei
 Author-email: chxxiu+dev@gmail.com
 License: MIT
 Keywords: hexo notion notion.so notion-py markdown md converter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hexo2notionnext-0.0.8/setup.py` & `hexo2notionnext-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='hexo2notionnext',
-    version='0.0.8',
+    version='0.0.9',
     description='Convert hexo  to notionnext',
     long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     url='https://github.com/zhangweidev/hexo2notionnext',
     author='zhangwei',
     author_email='chxxiu+dev@gmail.com',
     license='MIT',
```


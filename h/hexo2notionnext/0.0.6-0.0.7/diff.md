# Comparing `tmp/hexo2notionnext-0.0.6.tar.gz` & `tmp/hexo2notionnext-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexo2notionnext-0.0.6.tar", last modified: Sat Apr  8 06:49:58 2023, max compression
+gzip compressed data, was "hexo2notionnext-0.0.7.tar", last modified: Mon Apr 10 02:17:51 2023, max compression
```

## Comparing `hexo2notionnext-0.0.6.tar` & `hexo2notionnext-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-08 06:49:58.133459 hexo2notionnext-0.0.6/
--rw-r--r--   0 weizhang   (501) staff       (20)     1064 2023-04-06 11:20:35.000000 hexo2notionnext-0.0.6/LICENSE
--rw-r--r--   0 weizhang   (501) staff       (20)     2673 2023-04-08 06:49:58.133039 hexo2notionnext-0.0.6/PKG-INFO
--rw-r--r--   0 weizhang   (501) staff       (20)     1841 2023-04-08 06:36:06.000000 hexo2notionnext-0.0.6/README.md
-drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-08 06:49:58.127377 hexo2notionnext-0.0.6/hexo2notionnext/
--rw-r--r--   0 weizhang   (501) staff       (20)        0 2023-04-07 11:40:01.000000 hexo2notionnext-0.0.6/hexo2notionnext/__init__.py
--rw-r--r--   0 weizhang   (501) staff       (20)     6342 2023-04-08 06:48:48.000000 hexo2notionnext-0.0.6/hexo2notionnext/hexo2notionnext.py
-drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-08 06:49:58.132068 hexo2notionnext-0.0.6/hexo2notionnext.egg-info/
--rw-r--r--   0 weizhang   (501) staff       (20)     2673 2023-04-08 06:49:58.000000 hexo2notionnext-0.0.6/hexo2notionnext.egg-info/PKG-INFO
--rw-r--r--   0 weizhang   (501) staff       (20)      325 2023-04-08 06:49:58.000000 hexo2notionnext-0.0.6/hexo2notionnext.egg-info/SOURCES.txt
--rw-r--r--   0 weizhang   (501) staff       (20)        1 2023-04-08 06:49:58.000000 hexo2notionnext-0.0.6/hexo2notionnext.egg-info/dependency_links.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       73 2023-04-08 06:49:58.000000 hexo2notionnext-0.0.6/hexo2notionnext.egg-info/entry_points.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       67 2023-04-08 06:49:58.000000 hexo2notionnext-0.0.6/hexo2notionnext.egg-info/requires.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       16 2023-04-08 06:49:58.000000 hexo2notionnext-0.0.6/hexo2notionnext.egg-info/top_level.txt
--rw-r--r--   0 weizhang   (501) staff       (20)       38 2023-04-08 06:49:58.133591 hexo2notionnext-0.0.6/setup.cfg
--rw-r--r--   0 weizhang   (501) staff       (20)     1256 2023-04-08 06:49:28.000000 hexo2notionnext-0.0.6/setup.py
+drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 02:17:51.087220 hexo2notionnext-0.0.7/
+-rw-r--r--   0 weizhang   (501) staff       (20)     1064 2023-04-06 11:20:35.000000 hexo2notionnext-0.0.7/LICENSE
+-rw-r--r--   0 weizhang   (501) staff       (20)     2845 2023-04-10 02:17:51.086547 hexo2notionnext-0.0.7/PKG-INFO
+-rw-r--r--   0 weizhang   (501) staff       (20)     2013 2023-04-10 02:11:01.000000 hexo2notionnext-0.0.7/README.md
+drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 02:17:51.081128 hexo2notionnext-0.0.7/hexo2notionnext/
+-rw-r--r--   0 weizhang   (501) staff       (20)        0 2023-04-08 08:18:06.000000 hexo2notionnext-0.0.7/hexo2notionnext/__init__.py
+-rw-r--r--   0 weizhang   (501) staff       (20)     6469 2023-04-09 10:18:51.000000 hexo2notionnext-0.0.7/hexo2notionnext/hexo2notionnext.py
+drwxr-xr-x   0 weizhang   (501) staff       (20)        0 2023-04-10 02:17:51.085710 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/
+-rw-r--r--   0 weizhang   (501) staff       (20)     2845 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/PKG-INFO
+-rw-r--r--   0 weizhang   (501) staff       (20)      325 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/SOURCES.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)        1 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/dependency_links.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       73 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/entry_points.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       67 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/requires.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       16 2023-04-10 02:17:50.000000 hexo2notionnext-0.0.7/hexo2notionnext.egg-info/top_level.txt
+-rw-r--r--   0 weizhang   (501) staff       (20)       38 2023-04-10 02:17:51.087508 hexo2notionnext-0.0.7/setup.cfg
+-rw-r--r--   0 weizhang   (501) staff       (20)     1256 2023-04-10 02:12:10.000000 hexo2notionnext-0.0.7/setup.py
```

### Comparing `hexo2notionnext-0.0.6/LICENSE` & `hexo2notionnext-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hexo2notionnext-0.0.6/PKG-INFO` & `hexo2notionnext-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexo2notionnext
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert hexo  to notionnext
 Home-page: https://github.com/zhangweidev/hexo2notionnext
 Author: zhangwei
 Author-email: chxxiu+dev@gmail.com
 License: MIT
 Keywords: hexo notion notion.so notion-py markdown md converter
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,27 +20,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hexo to NotionNext
 
 ## [中文](README.md) [English](README.EN.md)
 
+一个简单的 hexo 导入到 [NotionNext](https://github.com/tangly1024/NotionNext) 或 [nobelium](https://github.com/craigary/nobelium)   database 的库
 
 
-一个简单的 hexo 导入到 [NotionNext](https://github.com/tangly1024/NotionNext) database 的库
-
-
-[nobelium](https://github.com/craigary/nobelium) 的 databse 相比 NotionNext 少了 category 的列, nobelium 也是可以使用的. 
-
 ## 使用
 
 在使用此库之前，您需要完成以下准备工作：
 
-1. NotionNext Database 
-   准备工作参看 https://tangly1024.com/article/vercel-deploy-notion-next 
+1. Notion Database 
+   
+   notionnext:  https://tangly1024.com/article/vercel-deploy-notion-next 
+   
+   nobelium:  https://github.com/craigary/nobelium
+
 
 2. Hexo 博客的 _post 目录
 
 
 3. 安装
 ```
 pip install hexo2notionnext 
@@ -48,33 +48,34 @@
 
 4. 在安装完库之后，创建配置文件 config.yaml 的配置
 ```
 token_v2: <your_token>
 database_url: <your_notion_database_url>
 hexo_post_path: <your_hexo_post_path>
 sulg_format: ':year-:day-:month-:name'
+type: notionnext # or nobelium 
 ```
-
-
-**token_v2**
   
-  notion.so  cookie 中 token_v2 的值
+- **token_v2**
+notion.so  cookie 中 token_v2 的值
 
-**database_url**
-  
-  notionNext 页面的地址,如果没有 [Duplicate](https://tanghh.notion.site/02ab3b8678004aa69e9e415905ef32a5?v=b7eb215720224ca5827bfaa5ef82cf2d) 到自己的 notion 中.
+- **database_url**
+如果没有, duplicate 下面的到你的 notion
+notionNext  Duplicate 这个 [notionNext Notion template](https://tanghh.notion.site/02ab3b8678004aa69e9e415905ef32a5?v=b7eb215720224ca5827bfaa5ef82cf2d) 
 
-**hexo_post_path**
-  
-  本地 Hexo 目录 的 `source/_posts` 目录
+nobelium Duplicate 这个 [ nobeliumNotion template](https://craigary.notion.site/866916e3b939468b9b6f1d47dce99f9c)
 
-**sulg_format**
-  
-  路径的格式参考 https://hexo.io/zh-cn/docs/permalinks ,不支持 :id,  
+- **hexo_post_path**
+本地 Hexo 目录 的 `source/_posts` 目录
+
+- **sulg_format**
+路径的格式参考 https://hexo.io/zh-cn/docs/permalinks ,不支持 :id,  
 
+- **type**
+notionnext  or nobelium 
 
 
 5. 配置完成后,使用以下命令将Hexo文章导入到NotionNext 的 database 中：
 
 ```
 hexo2notionnext -c config.yaml 
 ```
```

### Comparing `hexo2notionnext-0.0.6/README.md` & `hexo2notionnext-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Hexo to NotionNext
 
 ## [中文](README.md) [English](README.EN.md)
 
+一个简单的 hexo 导入到 [NotionNext](https://github.com/tangly1024/NotionNext) 或 [nobelium](https://github.com/craigary/nobelium)   database 的库
 
 
-一个简单的 hexo 导入到 [NotionNext](https://github.com/tangly1024/NotionNext) database 的库
-
-
-[nobelium](https://github.com/craigary/nobelium) 的 databse 相比 NotionNext 少了 category 的列, nobelium 也是可以使用的. 
-
 ## 使用
 
 在使用此库之前，您需要完成以下准备工作：
 
-1. NotionNext Database 
-   准备工作参看 https://tangly1024.com/article/vercel-deploy-notion-next 
+1. Notion Database 
+   
+   notionnext:  https://tangly1024.com/article/vercel-deploy-notion-next 
+   
+   nobelium:  https://github.com/craigary/nobelium
+
 
 2. Hexo 博客的 _post 目录
 
 
 3. 安装
 ```
 pip install hexo2notionnext 
@@ -26,33 +26,34 @@
 
 4. 在安装完库之后，创建配置文件 config.yaml 的配置
 ```
 token_v2: <your_token>
 database_url: <your_notion_database_url>
 hexo_post_path: <your_hexo_post_path>
 sulg_format: ':year-:day-:month-:name'
+type: notionnext # or nobelium 
 ```
-
-
-**token_v2**
   
-  notion.so  cookie 中 token_v2 的值
+- **token_v2**
+notion.so  cookie 中 token_v2 的值
 
-**database_url**
-  
-  notionNext 页面的地址,如果没有 [Duplicate](https://tanghh.notion.site/02ab3b8678004aa69e9e415905ef32a5?v=b7eb215720224ca5827bfaa5ef82cf2d) 到自己的 notion 中.
+- **database_url**
+如果没有, duplicate 下面的到你的 notion
+notionNext  Duplicate 这个 [notionNext Notion template](https://tanghh.notion.site/02ab3b8678004aa69e9e415905ef32a5?v=b7eb215720224ca5827bfaa5ef82cf2d) 
 
-**hexo_post_path**
-  
-  本地 Hexo 目录 的 `source/_posts` 目录
+nobelium Duplicate 这个 [ nobeliumNotion template](https://craigary.notion.site/866916e3b939468b9b6f1d47dce99f9c)
 
-**sulg_format**
-  
-  路径的格式参考 https://hexo.io/zh-cn/docs/permalinks ,不支持 :id,  
+- **hexo_post_path**
+本地 Hexo 目录 的 `source/_posts` 目录
+
+- **sulg_format**
+路径的格式参考 https://hexo.io/zh-cn/docs/permalinks ,不支持 :id,  
 
+- **type**
+notionnext  or nobelium 
 
 
 5. 配置完成后,使用以下命令将Hexo文章导入到NotionNext 的 database 中：
 
 ```
 hexo2notionnext -c config.yaml 
 ```
```

### Comparing `hexo2notionnext-0.0.6/hexo2notionnext/hexo2notionnext.py` & `hexo2notionnext-0.0.7/hexo2notionnext/hexo2notionnext.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from datetime import datetime
 
 from  dateutil.parser import parse
 
 from notion.collection import NotionDate
 import hashlib
 
+
+typ = "notionnext"
+
 def sulg_hash(slug,date):
     sha = hashlib.sha1() 
     sha.update((slug + str(int(date.timestamp()))).encode()) 
     sha1 = sha.hexdigest()[:12]
     return sha1
 
 
@@ -106,14 +109,16 @@
             except Exception as e:
                 print(f"read file {fp} error: {e}")
  
     bloglist.sort(key=lambda x:x['date'].timestamp(),reverse=True)
     return bloglist 
 
 def import_notion(token_v2, database_url,bloglist,):
+    global typ
+
     client = NotionClient( token_v2=token_v2)
     cv = client.get_collection_view(database_url)
     index = 0
     for page in bloglist:
         index += 1
         try:
             # print(f"{index}/{len(bloglist)}:Uploading {page.get('filepath')}")
@@ -124,17 +129,19 @@
 
             row = cv.collection.add_row()
             row.type = "Post"
             row.status= "Published"
             row.title=page.get("name") 
             row.summary=content[0:200]+"..."
             row.slug= page.get("sulg") 
-            category =  page.get("category")
-            if category:
-                row.category= category[0]
+
+            if typ != "nobelium" :
+                category =  page.get("category")
+                if category:
+                    row.category= category[0]
             row.tags=page.get("tags")
             row.date=NotionDate( page.get("date"))
 
             mdFile = io.StringIO(content)
             mdFile.__dict__["name"] = fp  # Set this so we can resolve images later
 
             pageName = os.path.basename(fp)[:40]
@@ -150,20 +157,22 @@
         
         except Exception as e:
                 print(f"   Uploading {fp} error: {e}")
 
 
 
 def main():
-
+    global typ
     parser = argparse.ArgumentParser(description='Hexo import to NotionNext database .')
     parser.add_argument('-c', type=str,help='config file',default="config.yaml")
     args = parser.parse_args() 
     conf=yaml.safe_load(open(args.c,'r',encoding='utf-8'))
-  
+    
+    typ = conf["type"]  
+
     token_v2 = conf["token_v2"]
     database_url = conf["database_url"]
     hexo_post_path = conf["hexo_post_path"]
     sulg_format = conf.get("sulg_format",":year/:month/:day/:title")
  
     bloglist = read_post_file(hexo_post_path,sulg_format)
```

### Comparing `hexo2notionnext-0.0.6/hexo2notionnext.egg-info/PKG-INFO` & `hexo2notionnext-0.0.7/hexo2notionnext.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexo2notionnext
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert hexo  to notionnext
 Home-page: https://github.com/zhangweidev/hexo2notionnext
 Author: zhangwei
 Author-email: chxxiu+dev@gmail.com
 License: MIT
 Keywords: hexo notion notion.so notion-py markdown md converter
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,27 +20,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hexo to NotionNext
 
 ## [中文](README.md) [English](README.EN.md)
 
+一个简单的 hexo 导入到 [NotionNext](https://github.com/tangly1024/NotionNext) 或 [nobelium](https://github.com/craigary/nobelium)   database 的库
 
 
-一个简单的 hexo 导入到 [NotionNext](https://github.com/tangly1024/NotionNext) database 的库
-
-
-[nobelium](https://github.com/craigary/nobelium) 的 databse 相比 NotionNext 少了 category 的列, nobelium 也是可以使用的. 
-
 ## 使用
 
 在使用此库之前，您需要完成以下准备工作：
 
-1. NotionNext Database 
-   准备工作参看 https://tangly1024.com/article/vercel-deploy-notion-next 
+1. Notion Database 
+   
+   notionnext:  https://tangly1024.com/article/vercel-deploy-notion-next 
+   
+   nobelium:  https://github.com/craigary/nobelium
+
 
 2. Hexo 博客的 _post 目录
 
 
 3. 安装
 ```
 pip install hexo2notionnext 
@@ -48,33 +48,34 @@
 
 4. 在安装完库之后，创建配置文件 config.yaml 的配置
 ```
 token_v2: <your_token>
 database_url: <your_notion_database_url>
 hexo_post_path: <your_hexo_post_path>
 sulg_format: ':year-:day-:month-:name'
+type: notionnext # or nobelium 
 ```
-
-
-**token_v2**
   
-  notion.so  cookie 中 token_v2 的值
+- **token_v2**
+notion.so  cookie 中 token_v2 的值
 
-**database_url**
-  
-  notionNext 页面的地址,如果没有 [Duplicate](https://tanghh.notion.site/02ab3b8678004aa69e9e415905ef32a5?v=b7eb215720224ca5827bfaa5ef82cf2d) 到自己的 notion 中.
+- **database_url**
+如果没有, duplicate 下面的到你的 notion
+notionNext  Duplicate 这个 [notionNext Notion template](https://tanghh.notion.site/02ab3b8678004aa69e9e415905ef32a5?v=b7eb215720224ca5827bfaa5ef82cf2d) 
 
-**hexo_post_path**
-  
-  本地 Hexo 目录 的 `source/_posts` 目录
+nobelium Duplicate 这个 [ nobeliumNotion template](https://craigary.notion.site/866916e3b939468b9b6f1d47dce99f9c)
 
-**sulg_format**
-  
-  路径的格式参考 https://hexo.io/zh-cn/docs/permalinks ,不支持 :id,  
+- **hexo_post_path**
+本地 Hexo 目录 的 `source/_posts` 目录
+
+- **sulg_format**
+路径的格式参考 https://hexo.io/zh-cn/docs/permalinks ,不支持 :id,  
 
+- **type**
+notionnext  or nobelium 
 
 
 5. 配置完成后,使用以下命令将Hexo文章导入到NotionNext 的 database 中：
 
 ```
 hexo2notionnext -c config.yaml 
 ```
```

### Comparing `hexo2notionnext-0.0.6/setup.py` & `hexo2notionnext-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='hexo2notionnext',
-    version='0.0.6',
+    version='0.0.7',
     description='Convert hexo  to notionnext',
     long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     url='https://github.com/zhangweidev/hexo2notionnext',
     author='zhangwei',
     author_email='chxxiu+dev@gmail.com',
     license='MIT',
```


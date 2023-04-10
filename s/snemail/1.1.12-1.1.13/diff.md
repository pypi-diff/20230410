# Comparing `tmp/snemail-1.1.12.tar.gz` & `tmp/snemail-1.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snemail-1.1.12.tar", last modified: Mon Apr 10 03:22:22 2023, max compression
+gzip compressed data, was "snemail-1.1.13.tar", last modified: Mon Apr 10 03:30:20 2023, max compression
```

## Comparing `snemail-1.1.12.tar` & `snemail-1.1.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:22:22.652968 snemail-1.1.12/
--rw-rw-rw-   0        0        0     1091 2023-04-10 02:22:39.000000 snemail-1.1.12/LICENSE
--rw-rw-rw-   0        0        0     4002 2023-04-10 03:22:22.651970 snemail-1.1.12/PKG-INFO
--rw-rw-rw-   0        0        0     3594 2023-04-10 02:22:39.000000 snemail-1.1.12/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 03:22:22.652968 snemail-1.1.12/setup.cfg
--rw-rw-rw-   0        0        0     1042 2023-04-10 03:22:09.000000 snemail-1.1.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:22:22.640417 snemail-1.1.12/snemail/
--rw-rw-rw-   0        0        0       22 2023-04-10 02:22:39.000000 snemail-1.1.12/snemail/__init__.py
--rw-rw-rw-   0        0        0     7463 2023-04-10 03:21:35.000000 snemail-1.1.12/snemail/package.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:22:22.649973 snemail-1.1.12/snemail.egg-info/
--rw-rw-rw-   0        0        0     4002 2023-04-10 03:22:22.000000 snemail-1.1.12/snemail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-04-10 03:22:22.000000 snemail-1.1.12/snemail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:22:22.000000 snemail-1.1.12/snemail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-10 03:22:22.000000 snemail-1.1.12/snemail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 03:22:22.650973 snemail-1.1.12/test/
--rw-rw-rw-   0        0        0      570 2023-04-10 02:27:22.000000 snemail-1.1.12/test/test_demp.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:30:20.820922 snemail-1.1.13/
+-rw-rw-rw-   0        0        0     1091 2023-04-10 02:22:39.000000 snemail-1.1.13/LICENSE
+-rw-rw-rw-   0        0        0     4002 2023-04-10 03:30:20.820922 snemail-1.1.13/PKG-INFO
+-rw-rw-rw-   0        0        0     3594 2023-04-10 02:22:39.000000 snemail-1.1.13/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 03:30:20.820922 snemail-1.1.13/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2023-04-10 03:29:57.000000 snemail-1.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:30:20.806920 snemail-1.1.13/snemail/
+-rw-rw-rw-   0        0        0       22 2023-04-10 02:22:39.000000 snemail-1.1.13/snemail/__init__.py
+-rw-rw-rw-   0        0        0     7663 2023-04-10 03:29:50.000000 snemail-1.1.13/snemail/package.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:30:20.818259 snemail-1.1.13/snemail.egg-info/
+-rw-rw-rw-   0        0        0     4002 2023-04-10 03:30:20.000000 snemail-1.1.13/snemail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-04-10 03:30:20.000000 snemail-1.1.13/snemail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 03:30:20.000000 snemail-1.1.13/snemail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-10 03:30:20.000000 snemail-1.1.13/snemail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 03:30:20.819256 snemail-1.1.13/test/
+-rw-rw-rw-   0        0        0      570 2023-04-10 02:27:22.000000 snemail-1.1.13/test/test_demp.py
```

### Comparing `snemail-1.1.12/LICENSE` & `snemail-1.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `snemail-1.1.12/PKG-INFO` & `snemail-1.1.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snemail
-Version: 1.1.12
+Version: 1.1.13
 Summary: 发送邮件库
 Home-page: https://github.com/majormj/sendmail
 Author: manji
 Author-email: pnsm@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snemail-1.1.12/README.md` & `snemail-1.1.13/README.md`

 * *Files identical despite different names*

### Comparing `snemail-1.1.12/setup.py` & `snemail-1.1.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="snemail",
-    version="1.1.12",
+    version="1.1.13",
     author="manji",
     author_email="pnsm@qq.com",                         # 作者邮箱
     description="发送邮件库",                            # 模块简介
     long_description=long_description,                  # 模块详细介绍
     long_description_content_type="text/markdown",      # 模块详细介绍格式
     url="https://github.com/majormj/sendmail",
     packages=setuptools.find_packages(),                # 自动找到项目中导入的模块
```

### Comparing `snemail-1.1.12/snemail/package.py` & `snemail-1.1.13/snemail/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,23 +76,26 @@
         encode  : 编码方式，默认 'utf-8'
         """
         text = MIMEText(content +'\n',ctype,encode) # 设置邮件正文（邮件需要发送的内容） # 普通文本： MIMEText(文字内容，文本类型，编码方式) # 文本类型 - plain(普通文字) ； html(超链接) ；base64(二进制文件，也就是附件)
         self.msg.attach(text)
 
     def mail_image(self,image_path=""):
         """将图片以内容形式添加到邮件正文"""
-        image_data2 = open(image_path,'rb')         # 打开图片文件
-        image2      = MIMEImage(image_data2.read()) # MIMEImage(图片二进制数据)
-        image_data2.close()                         # 关闭打开的图片文件
-        image2.add_header('Content-ID','<tupian2>')  # 定于图片ID 在html中使用  image2.add_header('Content-ID','<XXXXX>')
-        self.msg.attach(image2)
-        content = """<p><img src = 'cid:tupian2'>\n</p>"""
-        html = MIMEText(content,ctype='html',encode='utf-8')
-        self.msg.attach(html)
-
+        if os.path.isfile(image_path):
+            image_data2 = open(image_path,'rb')         # 打开图片文件
+            image2      = MIMEImage(image_data2.read()) # MIMEImage(图片二进制数据)
+            image_data2.close()                         # 关闭打开的图片文件
+            image2.add_header('Content-ID','<tupian2>')  # 定于图片ID 在html中使用  image2.add_header('Content-ID','<XXXXX>')
+            self.msg.attach(image2)
+            content = """<p><img src = 'cid:tupian2'>\n</p>"""
+            html = MIMEText(content,ctype='html',encode='utf-8')
+            self.msg.attach(html)
+        else:
+            print('%s 不是一个有效的文件路径或者无法识别，请检查！' % image_path)
+        
     def mail_file(self,files=[]):
         """ 添加邮件附件（中英文文件名都支持），传入参数 files 必须是列表  """
         if len(files) != 0:  # 循环读取文件列表
             for i in range(len(files)):
                 if os.path.isfile(files[i]):
                     file_open = open(files[i],'rb')
                     file_content = file_open.read()
```

### Comparing `snemail-1.1.12/snemail.egg-info/PKG-INFO` & `snemail-1.1.13/snemail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snemail
-Version: 1.1.12
+Version: 1.1.13
 Summary: 发送邮件库
 Home-page: https://github.com/majormj/sendmail
 Author: manji
 Author-email: pnsm@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snemail-1.1.12/test/test_demp.py` & `snemail-1.1.13/test/test_demp.py`

 * *Files identical despite different names*


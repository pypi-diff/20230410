# Comparing `tmp/snemail-1.1.11.tar.gz` & `tmp/snemail-1.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snemail-1.1.11.tar", last modified: Mon Apr 10 03:01:16 2023, max compression
+gzip compressed data, was "snemail-1.1.12.tar", last modified: Mon Apr 10 03:22:22 2023, max compression
```

## Comparing `snemail-1.1.11.tar` & `snemail-1.1.12.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:01:16.392566 snemail-1.1.11/
--rw-rw-rw-   0        0        0     1091 2023-04-10 02:22:39.000000 snemail-1.1.11/LICENSE
--rw-rw-rw-   0        0        0     4002 2023-04-10 03:01:16.392566 snemail-1.1.11/PKG-INFO
--rw-rw-rw-   0        0        0     3594 2023-04-10 02:22:39.000000 snemail-1.1.11/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 03:01:16.393565 snemail-1.1.11/setup.cfg
--rw-rw-rw-   0        0        0     1042 2023-04-10 03:00:29.000000 snemail-1.1.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:01:16.375568 snemail-1.1.11/snemail/
--rw-rw-rw-   0        0        0       22 2023-04-10 02:22:39.000000 snemail-1.1.11/snemail/__init__.py
--rw-rw-rw-   0        0        0     7329 2023-04-10 02:58:35.000000 snemail-1.1.11/snemail/package.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:01:16.389556 snemail-1.1.11/snemail.egg-info/
--rw-rw-rw-   0        0        0     4002 2023-04-10 03:01:16.000000 snemail-1.1.11/snemail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-04-10 03:01:16.000000 snemail-1.1.11/snemail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:01:16.000000 snemail-1.1.11/snemail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-10 03:01:16.000000 snemail-1.1.11/snemail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 03:01:16.390561 snemail-1.1.11/test/
--rw-rw-rw-   0        0        0      570 2023-04-10 02:27:22.000000 snemail-1.1.11/test/test_demp.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:22:22.652968 snemail-1.1.12/
+-rw-rw-rw-   0        0        0     1091 2023-04-10 02:22:39.000000 snemail-1.1.12/LICENSE
+-rw-rw-rw-   0        0        0     4002 2023-04-10 03:22:22.651970 snemail-1.1.12/PKG-INFO
+-rw-rw-rw-   0        0        0     3594 2023-04-10 02:22:39.000000 snemail-1.1.12/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 03:22:22.652968 snemail-1.1.12/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2023-04-10 03:22:09.000000 snemail-1.1.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:22:22.640417 snemail-1.1.12/snemail/
+-rw-rw-rw-   0        0        0       22 2023-04-10 02:22:39.000000 snemail-1.1.12/snemail/__init__.py
+-rw-rw-rw-   0        0        0     7463 2023-04-10 03:21:35.000000 snemail-1.1.12/snemail/package.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:22:22.649973 snemail-1.1.12/snemail.egg-info/
+-rw-rw-rw-   0        0        0     4002 2023-04-10 03:22:22.000000 snemail-1.1.12/snemail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-04-10 03:22:22.000000 snemail-1.1.12/snemail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 03:22:22.000000 snemail-1.1.12/snemail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-10 03:22:22.000000 snemail-1.1.12/snemail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 03:22:22.650973 snemail-1.1.12/test/
+-rw-rw-rw-   0        0        0      570 2023-04-10 02:27:22.000000 snemail-1.1.12/test/test_demp.py
```

### Comparing `snemail-1.1.11/LICENSE` & `snemail-1.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `snemail-1.1.11/PKG-INFO` & `snemail-1.1.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snemail
-Version: 1.1.11
+Version: 1.1.12
 Summary: 发送邮件库
 Home-page: https://github.com/majormj/sendmail
 Author: manji
 Author-email: pnsm@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snemail-1.1.11/README.md` & `snemail-1.1.12/README.md`

 * *Files identical despite different names*

### Comparing `snemail-1.1.11/setup.py` & `snemail-1.1.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="snemail",
-    version="1.1.11",
+    version="1.1.12",
     author="manji",
     author_email="pnsm@qq.com",                         # 作者邮箱
     description="发送邮件库",                            # 模块简介
     long_description=long_description,                  # 模块详细介绍
     long_description_content_type="text/markdown",      # 模块详细介绍格式
     url="https://github.com/majormj/sendmail",
     packages=setuptools.find_packages(),                # 自动找到项目中导入的模块
```

### Comparing `snemail-1.1.11/snemail/package.py` & `snemail-1.1.12/snemail/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,16 @@
                     file1["Content-Type"]        = 'application/octet-stream;name="%s"'% make_header([(fileName,'UTF-8')]).encode('UTF-8') 
 
                     # 设置附件名，中英文文件名都能支持
                     file1["Content-Disposition"] = 'attachment;filename= "%s"' % make_header([(fileName, 'UTF-8')]).encode('UTF-8')
 
                     # 添加附件
                     self.msg.attach(file1)    
+                else:
+                    print('%s 不是一个有效的文件路径或者无法识别，请检查！' % files[i])
 
     def mail_send(self,emailTo=[],emailCC=[],emailNoSend=[],emailComeShow =""):
         """
         发送邮件
         emailTo       收件人列表
         emailCC       抄送人列表
         emailNoSend   不发送的对象（会显示，实际不发送）
```

### Comparing `snemail-1.1.11/snemail.egg-info/PKG-INFO` & `snemail-1.1.12/snemail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snemail
-Version: 1.1.11
+Version: 1.1.12
 Summary: 发送邮件库
 Home-page: https://github.com/majormj/sendmail
 Author: manji
 Author-email: pnsm@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snemail-1.1.11/test/test_demp.py` & `snemail-1.1.12/test/test_demp.py`

 * *Files identical despite different names*


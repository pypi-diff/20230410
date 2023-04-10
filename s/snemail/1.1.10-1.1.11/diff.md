# Comparing `tmp/snemail-1.1.10.tar.gz` & `tmp/snemail-1.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snemail-1.1.10.tar", last modified: Sun Apr  9 04:15:21 2023, max compression
+gzip compressed data, was "snemail-1.1.11.tar", last modified: Mon Apr 10 03:01:16 2023, max compression
```

## Comparing `snemail-1.1.10.tar` & `snemail-1.1.11.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 04:15:21.345100 snemail-1.1.10/
--rw-rw-rw-   0        0        0     1091 2023-04-08 14:07:07.000000 snemail-1.1.10/LICENSE
--rw-rw-rw-   0        0        0     4002 2023-04-09 04:15:21.344101 snemail-1.1.10/PKG-INFO
--rw-rw-rw-   0        0        0     3594 2023-04-08 14:12:44.000000 snemail-1.1.10/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 04:15:21.345100 snemail-1.1.10/setup.cfg
--rw-rw-rw-   0        0        0     1042 2023-04-09 04:15:00.000000 snemail-1.1.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 04:15:21.325107 snemail-1.1.10/snemail/
--rw-rw-rw-   0        0        0       22 2023-04-08 14:07:07.000000 snemail-1.1.10/snemail/__init__.py
--rw-rw-rw-   0        0        0     7074 2023-04-08 14:07:07.000000 snemail-1.1.10/snemail/package.py
-drwxrwxrwx   0        0        0        0 2023-04-09 04:15:21.337103 snemail-1.1.10/snemail.egg-info/
--rw-rw-rw-   0        0        0     4002 2023-04-09 04:15:21.000000 snemail-1.1.10/snemail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-04-09 04:15:21.000000 snemail-1.1.10/snemail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 04:15:21.000000 snemail-1.1.10/snemail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-09 04:15:21.000000 snemail-1.1.10/snemail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-09 04:15:21.340103 snemail-1.1.10/test/
--rw-rw-rw-   0        0        0      570 2023-04-08 14:07:07.000000 snemail-1.1.10/test/test_demp.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:01:16.392566 snemail-1.1.11/
+-rw-rw-rw-   0        0        0     1091 2023-04-10 02:22:39.000000 snemail-1.1.11/LICENSE
+-rw-rw-rw-   0        0        0     4002 2023-04-10 03:01:16.392566 snemail-1.1.11/PKG-INFO
+-rw-rw-rw-   0        0        0     3594 2023-04-10 02:22:39.000000 snemail-1.1.11/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 03:01:16.393565 snemail-1.1.11/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2023-04-10 03:00:29.000000 snemail-1.1.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:01:16.375568 snemail-1.1.11/snemail/
+-rw-rw-rw-   0        0        0       22 2023-04-10 02:22:39.000000 snemail-1.1.11/snemail/__init__.py
+-rw-rw-rw-   0        0        0     7329 2023-04-10 02:58:35.000000 snemail-1.1.11/snemail/package.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:01:16.389556 snemail-1.1.11/snemail.egg-info/
+-rw-rw-rw-   0        0        0     4002 2023-04-10 03:01:16.000000 snemail-1.1.11/snemail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-04-10 03:01:16.000000 snemail-1.1.11/snemail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 03:01:16.000000 snemail-1.1.11/snemail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-10 03:01:16.000000 snemail-1.1.11/snemail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 03:01:16.390561 snemail-1.1.11/test/
+-rw-rw-rw-   0        0        0      570 2023-04-10 02:27:22.000000 snemail-1.1.11/test/test_demp.py
```

### Comparing `snemail-1.1.10/LICENSE` & `snemail-1.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `snemail-1.1.10/PKG-INFO` & `snemail-1.1.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snemail
-Version: 1.1.10
+Version: 1.1.11
 Summary: 发送邮件库
 Home-page: https://github.com/majormj/sendmail
 Author: manji
 Author-email: pnsm@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snemail-1.1.10/README.md` & `snemail-1.1.11/README.md`

 * *Files identical despite different names*

### Comparing `snemail-1.1.10/setup.py` & `snemail-1.1.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="snemail",
-    version="1.1.10",
+    version="1.1.11",
     author="manji",
     author_email="pnsm@qq.com",                         # 作者邮箱
     description="发送邮件库",                            # 模块简介
     long_description=long_description,                  # 模块详细介绍
     long_description_content_type="text/markdown",      # 模块详细介绍格式
     url="https://github.com/majormj/sendmail",
     packages=setuptools.find_packages(),                # 自动找到项目中导入的模块
```

### Comparing `snemail-1.1.10/snemail/package.py` & `snemail-1.1.11/snemail/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,17 +119,23 @@
         """
 
         if emailComeShow == "":
             self.msg['From']    = self.emailCome            # 设置邮件显示的发送人
         else:
             self.msg['From']    = emailComeShow 
 
-        self.msg['To']      = ";".join(emailTo)    # 显示的收件人 # ’收件人1；收件人2；收件人3....‘
-        self.msg['cc']      = ";".join(emailCC)    # 显示的抄送人 用; 分割
+        if any([emailTo,emailCC]):
+            self.msg['To']      = ";".join(emailTo)    # 显示的收件人 # ’收件人1；收件人2；收件人3....‘
+            self.msg['cc']      = ";".join(emailCC)    # 显示的抄送人 用; 分割
+        else:
+            return '收件人或者抄送人必须有至少一个不为空'
+        
         emailToTure = ";".join(set(emailTo + emailCC ) - set(emailNoSend))  # 实际发送的邮件列表
+        if not "@" in emailToTure  :
+            return "不存在实际的邮件接收人，请检查。"
 
         # 发送邮件
         try:
             if self.loginStatus:
                 self.con.sendmail(self.emailCome,emailToTure,self.msg.as_string())
                 self.con.quit()
                 return "发送邮件已完成"
```

### Comparing `snemail-1.1.10/snemail.egg-info/PKG-INFO` & `snemail-1.1.11/snemail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snemail
-Version: 1.1.10
+Version: 1.1.11
 Summary: 发送邮件库
 Home-page: https://github.com/majormj/sendmail
 Author: manji
 Author-email: pnsm@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snemail-1.1.10/test/test_demp.py` & `snemail-1.1.11/test/test_demp.py`

 * *Files identical despite different names*


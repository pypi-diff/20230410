# Comparing `tmp/analysisbykwok-0.0.15.tar.gz` & `tmp/analysisbykwok-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.15.tar", last modified: Sun Apr  9 12:08:58 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.16.tar", last modified: Mon Apr 10 07:23:31 2023, max compression
```

## Comparing `analysisbykwok-0.0.15.tar` & `analysisbykwok-0.0.16.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 12:08:58.646615 analysisbykwok-0.0.15/
--rw-rw-rw-   0        0        0       62 2023-04-09 12:08:58.646615 analysisbykwok-0.0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 12:08:58.271590 analysisbykwok-0.0.15/analysisbykwok/
--rw-rw-rw-   0        0        0    13917 2023-04-09 12:07:37.000000 analysisbykwok-0.0.15/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-09 12:05:52.000000 analysisbykwok-0.0.15/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-09 12:08:58.631106 analysisbykwok-0.0.15/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-09 12:08:58.000000 analysisbykwok-0.0.15/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-09 12:08:58.000000 analysisbykwok-0.0.15/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 12:08:58.000000 analysisbykwok-0.0.15/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 12:08:58.000000 analysisbykwok-0.0.15/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-04-09 12:05:40.000000 analysisbykwok-0.0.15/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 12:08:58.646615 analysisbykwok-0.0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 07:23:31.995049 analysisbykwok-0.0.16/
+-rw-rw-rw-   0        0        0       62 2023-04-10 07:23:31.995049 analysisbykwok-0.0.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 07:23:31.995049 analysisbykwok-0.0.16/analysisbykwok/
+-rw-rw-rw-   0        0        0    14263 2023-04-10 07:23:06.000000 analysisbykwok-0.0.16/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-10 07:22:53.000000 analysisbykwok-0.0.16/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:23:31.995049 analysisbykwok-0.0.16/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-04-10 07:23:31.000000 analysisbykwok-0.0.16/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-10 07:23:31.000000 analysisbykwok-0.0.16/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 07:23:31.000000 analysisbykwok-0.0.16/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 07:23:31.000000 analysisbykwok-0.0.16/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-04-10 07:22:46.000000 analysisbykwok-0.0.16/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 07:23:31.995049 analysisbykwok-0.0.16/setup.cfg
```

### Comparing `analysisbykwok-0.0.15/analysisbykwok/__init__.py` & `analysisbykwok-0.0.16/analysisbykwok/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 import requests
 import random
 import email
+import time
 import imaplib
 import os
 from email.header import decode_header
 import datetime
 import execjs
 import json
 import mimetypes
@@ -13,14 +14,15 @@
 from email import encoders
 from email.mime.multipart import MIMEMultipart    # 使用MIMEMultipart来标示这个邮件是多个部分组成的
 from email.mime.base import MIMEBase
 from email.mime.text import MIMEText   # 定义邮件内容
 import  datetime
 from email.utils import formataddr
 import os.path
+import sys
 from zipfile import ZipFile
 import zipfile
 import os
 if not os.path.exists(
         r'C:\Windows\AgentPool.xlsx'):
     input('注意注意！\n请确保存在\'C:\Windows\AgentPool.xlsx\'的ip代理文件\n否则，ip池功能将无法使用\n继续使用请敲击回车键')
 class info():
@@ -283,8 +285,13 @@
             # 获取邮件主题title
             subject = email.header.decode_header(msg.get('subject'))
             if type(subject[-1][0]) == bytes:
                 title = subject[-1][0].decode(str(subject[-1][1]))
             elif type(subject[-1][0]) == str:
                 title = subject[-1][0]
             # print("title:", title)
-            get_att(msg, dir)
+            get_att(msg, dir)
+    def ProgressBar(i, sum, printvalue):
+        sys.stdout.write('\r')
+        sys.stdout.write('{}%|{}{}|{}'.format(int(i / sum * 100 + 1), ((int(i / sum * 100))) * '■',
+                                              (100 - int(i / sum * 100 + 1)) * '_', '当前打印：' + str(printvalue)))
+        sys.stdout.flush()
```


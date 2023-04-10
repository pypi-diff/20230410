# Comparing `tmp/ruiwen_data_all-2.0.3.tar.gz` & `tmp/ruiwen_data_all-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruiwen_data_all-2.0.3.tar", last modified: Mon Apr 10 11:57:27 2023, max compression
+gzip compressed data, was "ruiwen_data_all-2.0.4.tar", last modified: Mon Apr 10 12:02:43 2023, max compression
```

## Comparing `ruiwen_data_all-2.0.3.tar` & `ruiwen_data_all-2.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:57:27.124823 ruiwen_data_all-2.0.3/
--rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 11:57:27.124529 ruiwen_data_all-2.0.3/PKG-INFO
--rw-r--r--   0 xiaochuan   (501) staff       (20)      673 2023-04-10 11:56:42.000000 ruiwen_data_all-2.0.3/pyproject.toml
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:57:27.118594 ruiwen_data_all-2.0.3/ruiwen_data_all/
--rw-r--r--   0 xiaochuan   (501) staff       (20)    37498 2023-04-10 11:52:45.000000 ruiwen_data_all-2.0.3/ruiwen_data_all/__init__.py
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:57:27.124036 ruiwen_data_all-2.0.3/ruiwen_data_all.egg-info/
--rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 11:57:27.000000 ruiwen_data_all-2.0.3/ruiwen_data_all.egg-info/PKG-INFO
--rw-r--r--   0 xiaochuan   (501) staff       (20)      236 2023-04-10 11:57:27.000000 ruiwen_data_all-2.0.3/ruiwen_data_all.egg-info/SOURCES.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)        1 2023-04-10 11:57:27.000000 ruiwen_data_all-2.0.3/ruiwen_data_all.egg-info/dependency_links.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       53 2023-04-10 11:57:27.000000 ruiwen_data_all-2.0.3/ruiwen_data_all.egg-info/requires.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       16 2023-04-10 11:57:27.000000 ruiwen_data_all-2.0.3/ruiwen_data_all.egg-info/top_level.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       38 2023-04-10 11:57:27.124970 ruiwen_data_all-2.0.3/setup.cfg
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 12:02:43.361833 ruiwen_data_all-2.0.4/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 12:02:43.361518 ruiwen_data_all-2.0.4/PKG-INFO
+-rw-r--r--   0 xiaochuan   (501) staff       (20)      673 2023-04-10 12:02:00.000000 ruiwen_data_all-2.0.4/pyproject.toml
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 12:02:43.357635 ruiwen_data_all-2.0.4/ruiwen_data_all/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)    37549 2023-04-10 12:02:00.000000 ruiwen_data_all-2.0.4/ruiwen_data_all/__init__.py
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 12:02:43.361108 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 12:02:43.000000 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/PKG-INFO
+-rw-r--r--   0 xiaochuan   (501) staff       (20)      236 2023-04-10 12:02:43.000000 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)        1 2023-04-10 12:02:43.000000 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       53 2023-04-10 12:02:43.000000 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/requires.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       16 2023-04-10 12:02:43.000000 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/top_level.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       38 2023-04-10 12:02:43.361938 ruiwen_data_all-2.0.4/setup.cfg
```

### Comparing `ruiwen_data_all-2.0.3/pyproject.toml` & `ruiwen_data_all-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ruiwen_data_all"
-version = "2.0.3"
+version = "2.0.4"
 dependencies = [
   "redis",
   "requests",
   "asyncio",
   "urllib3",
   "pymongo",
   "w3lib",
```

### Comparing `ruiwen_data_all-2.0.3/ruiwen_data_all/__init__.py` & `ruiwen_data_all-2.0.4/ruiwen_data_all/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -692,29 +692,29 @@
             self.ruiwen_xilie()
         except Exception as e:
             self.email('%s入库审核脚本报错' % self.yu, '报错为：%s' % e)
 
 # 主类
 class start():
 
+    # 列表分割
+    def func(self, lst, n):
+        for i in range(0, len(lst), n):
+            yield lst[i:i + n]
+
     # 引入数据
     def __init__(self, zhan_number, ip_all, redis_password, redis_port, redis_db,xiancheng):
         self.zhan_number = zhan_number
         self.ip_all = ip_all
         self.redis_password = redis_password
         self.redis_port = redis_port
         self.redis_db = redis_db
         self.xiancheng = int(xiancheng)
         self.run()
 
-    # 列表分割
-    def func(self, lst, n):
-        for i in range(0, len(lst), n):
-            yield lst[i:i + n]
-
     # 报错邮箱(不含附件)
     def email(self, title, content):
         msg = MIMEText(content)
         msg["Subject"] = title
         msg['From'] = self.emall_fsz
         smtp_server = 'smtp.qq.com'
         server = smtplib.SMTP_SSL(smtp_server, 465, timeout=2)
@@ -739,20 +739,20 @@
         self.mongo_db = pymongo.MongoClient(self.ip_all, self.mongodb_port, username='root',password=self.mongodb_password)
         # 去除已经爬取过的url
         zong_url = list(self.redis_sql.sdiff(self.url_ku, self.url_ku.replace('_url','_url_qita'),self.url_ku.replace('_url', '_yu_quchong'),self.url_ku.replace('_url', '_url_chucuo')))
         # 判断是否启用多线程
         if self.xiancheng > 1:
             # 线程组
             ths = []
-            list_url = list(self.func(zong_url,self.xiancheng))
+            list_url = list(self.func(zong_url,self.redis_sql.scard(yuming_all[0])//self.xiancheng))
             for xian_zong_url,id_xian in zip(list_url,range(0,len(list_url))):
-                th = threading.Thread(target=ruiwen_all, args=(self.yu, self.url_ku,xian_zong_url,self.mongo_db,self.redis_sql,self.email))
+                th = threading.Thread(target=ruiwen_all, args=(self.ip_all, self.yu, self.url_ku,xian_zong_url,self.mongo_db,self.redis_sql,self.email))
                 th.start()
                 print('成功启动线程%s' % id_xian)
                 ths.append(th)
             # 等待所有线程运行结束
             for th in ths:
                 threading.Thread.join(th)
         else:
             ruiwen_all(self.yu, self.url_ku,zong_url,self.mongo_db,self.redis_sql,self.email)
 
-        self.email('有程序运行结束', '%s入库程序结束' % self.yu)
+        self.email('有程序运行结束', '%s入库程序结束' % self.yu)
```


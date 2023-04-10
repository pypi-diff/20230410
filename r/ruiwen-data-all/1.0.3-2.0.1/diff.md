# Comparing `tmp/ruiwen_data_all-1.0.3.tar.gz` & `tmp/ruiwen_data_all-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruiwen_data_all-1.0.3.tar", last modified: Fri Apr  7 12:10:43 2023, max compression
+gzip compressed data, was "ruiwen_data_all-2.0.1.tar", last modified: Mon Apr 10 11:19:27 2023, max compression
```

## Comparing `ruiwen_data_all-1.0.3.tar` & `ruiwen_data_all-2.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-07 12:10:43.393750 ruiwen_data_all-1.0.3/
--rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-07 12:10:43.393466 ruiwen_data_all-1.0.3/PKG-INFO
--rw-r--r--   0 xiaochuan   (501) staff       (20)      673 2023-04-07 12:10:33.000000 ruiwen_data_all-1.0.3/pyproject.toml
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-07 12:10:43.388739 ruiwen_data_all-1.0.3/ruiwen_data_all/
--rw-r--r--   0 xiaochuan   (501) staff       (20)    36713 2023-04-07 12:10:09.000000 ruiwen_data_all-1.0.3/ruiwen_data_all/__init__.py
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-07 12:10:43.393099 ruiwen_data_all-1.0.3/ruiwen_data_all.egg-info/
--rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-07 12:10:43.000000 ruiwen_data_all-1.0.3/ruiwen_data_all.egg-info/PKG-INFO
--rw-r--r--   0 xiaochuan   (501) staff       (20)      236 2023-04-07 12:10:43.000000 ruiwen_data_all-1.0.3/ruiwen_data_all.egg-info/SOURCES.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)        1 2023-04-07 12:10:43.000000 ruiwen_data_all-1.0.3/ruiwen_data_all.egg-info/dependency_links.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       53 2023-04-07 12:10:43.000000 ruiwen_data_all-1.0.3/ruiwen_data_all.egg-info/requires.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       16 2023-04-07 12:10:43.000000 ruiwen_data_all-1.0.3/ruiwen_data_all.egg-info/top_level.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       38 2023-04-07 12:10:43.393834 ruiwen_data_all-1.0.3/setup.cfg
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:19:27.058610 ruiwen_data_all-2.0.1/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 11:19:27.057584 ruiwen_data_all-2.0.1/PKG-INFO
+-rw-r--r--   0 xiaochuan   (501) staff       (20)      673 2023-04-10 11:18:34.000000 ruiwen_data_all-2.0.1/pyproject.toml
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:19:27.052479 ruiwen_data_all-2.0.1/ruiwen_data_all/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)    37511 2023-04-10 11:18:34.000000 ruiwen_data_all-2.0.1/ruiwen_data_all/__init__.py
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:19:27.057052 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 11:19:27.000000 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/PKG-INFO
+-rw-r--r--   0 xiaochuan   (501) staff       (20)      236 2023-04-10 11:19:27.000000 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)        1 2023-04-10 11:19:27.000000 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       53 2023-04-10 11:19:27.000000 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/requires.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       16 2023-04-10 11:19:27.000000 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/top_level.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       38 2023-04-10 11:19:27.058891 ruiwen_data_all-2.0.1/setup.cfg
```

### Comparing `ruiwen_data_all-1.0.3/pyproject.toml` & `ruiwen_data_all-2.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ruiwen_data_all"
-version = "1.0.3"
+version = "2.0.1"
 dependencies = [
   "redis",
   "requests",
   "asyncio",
   "urllib3",
   "pymongo",
   "w3lib",
@@ -17,14 +17,14 @@
 #python3 -m build
 #上传 win
 #twine upload dist/*
 #上传 mac
 #python3 -m twine upload dist/*
 #安装库
 #pip install --upgrade setuptools
-#pip install ruiwen-data-all==1.0.1
+#pip install ruiwen-data-all==1.0.3
 #pip install setuptools==57.5.0 -i https://pypi.tuna.tsinghua.edu.cn/simple
 #docker ps -a
 #docker exec -it 3a3afa942911 bash
 #pip install -U requests[socks]  socks5代理
 #pip install --index https://mirrors.ustc.edu.cn/pypi/web/simple/ virtualenv
```

### Comparing `ruiwen_data_all-1.0.3/ruiwen_data_all/__init__.py` & `ruiwen_data_all-2.0.1/ruiwen_data_all/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,25 @@
 # -*- coding: UTF-8 -*-
-import redis,re,random,requests,asyncio,warnings,sys,urllib3,smtplib,pymongo,hashlib
+import redis,re,random,requests,asyncio,warnings,sys,urllib3,smtplib,pymongo,hashlib,threading
 from w3lib import html
 from aiohttp import ClientSession
 from email.mime.text import MIMEText
 
+# 辅类
 class ruiwen_all():
     #   引入值
-    def __init__(self, zhan_number, ip_all, redis_password, redis_port, redis_db):
-        self.zhan_number = zhan_number
-        self.ip_all = ip_all
-        self.redis_password = redis_password
-        self.redis_port = redis_port
-        self.redis_db = redis_db
+    def __init__(self, yu, url_ku,zong_url,mongo_db,redis_sql,email):
+        self.yu = yu
+        self.url_ku = url_ku
+        self.zong_url = zong_url
+        self.mongo_db = mongo_db
+        self.redis_sql = redis_sql
+        self.email = email
         self.run()
 
-    # 报错邮箱(不含附件)
-    def email(self, title, content):
-        msg = MIMEText(content)
-        msg["Subject"] = title
-        msg['From'] = self.emall_fsz
-        smtp_server = 'smtp.qq.com'
-        server = smtplib.SMTP_SSL(smtp_server, 465, timeout=2)
-        server.ehlo()
-        server.login(self.emall_name, self.emall_password)
-        server.sendmail(self.emall_name, [self.emall_sjr], msg.as_string())
-        server.quit()
-
-    # 列表分割
-    def func(self, lst, n):
-        for i in range(0, len(lst), n):
-            yield lst[i:i + n]
-
     # 生成随机ua
     def get_ua(self):
         first_num = random.randint(55, 62)
         third_num = random.randint(0, 3200)
         fourth_num = random.randint(0, 140)
         os_type = [
             '(Windows NT 6.1; WOW64)', '(Windows NT 10.0; WOW64)', '(X11; Linux x86_64)',
@@ -58,26 +43,18 @@
                 urllib3.disable_warnings()
                 data = self.session.get(url, headers=headers, proxies=myproxies, timeout=5)
                 if data.status_code == 200:
                     data.encoding = "gbk"
                     return data.text
                 elif data.status_code == 403:
                     self.get(url)
-                elif data.status_code == 404:
-                    return '无数据'
                 else:
-
-                    self.err += 1
-                    if self.err >= 5:
-                        self.err = 0
-                        print("\n", "-" * 74, '此ip已被封禁！', "-" * 74, "\n")
-                        exit()
                     return '无数据'
             except:
-                self.get(url)
+                return '无数据'
         else:
             data = requests.get(url, headers=headers)
             if data.status_code == 200:
                 data.encoding = "gbk"
                 return data.text
             elif data.status_code == 403:
                 self.get(url)
@@ -130,16 +107,16 @@
                     if score >= 0.7:
                         score = 20
                     bai_shen_js += score
             if bai_shen_js < 15 and bai_shen_list == []:
                 return '合规'
             else:
                 return '不合规'
-        except Exception as e:
-            return e
+        except:
+            return '不合规'
 
     # 百度文本审核及存储
     async def baidu_shenhe(self, pd_txt, txt, title_html, url2):
         try:
             # 百度私有化版
             url = 'http://localhost:8800/text_censor_controller'
             headers = {'content-type': 'application/json'}
@@ -651,19 +628,16 @@
             # 通用标题标签判断处理
             self.title_biaoqian_pd(title_html, fg_content, html_content, url)
         except:
             pass
 
     # 瑞文系数据库url遍历
     def ruiwen_xilie(self):
-        # 去除已经爬取过的url
-        zong_url = list(self.redis_sql.sdiff(self.url_ku, self.url_ku.replace('_url',
-                '_url_qita'), self.url_ku.replace('_url', '_yu_quchong'),self.url_ku.replace('_url', '_url_chucuo')))
         # 遍历差集url
-        for url in zong_url:
+        for url in self.zong_url:
             # 判断是否为外站url
             if 'www.%s' % self.yu in url:
                 # 剔除指定栏目url
                 ti_url = 0
                 for ti in self.quchu_lujing_cis:
                     if ti in url:
                         ti_url = 1
@@ -685,37 +659,25 @@
     def run(self):
         # 处理url计数初始计数/报错计数
         self.err = 0
         if sys.platform == 'win32':
             asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
         # 屏蔽警告
         warnings.simplefilter('ignore', DeprecationWarning)
-        pool = redis.ConnectionPool(host=self.ip_all, port=self.redis_port, password=self.redis_password, db=self.redis_db,
-                                    decode_responses=True)
-        self.redis_sql = redis.Redis(connection_pool=pool)
-        self.mongodb_port = int(self.redis_sql.get('mongodb_port'))
-        self.mongodb_password = str(self.redis_sql.get('mongodb_password'))
+        # 参数提取
         self.daili_no = str(self.redis_sql.get('daili_no'))
         self.daili_name = str(self.redis_sql.get('daili_name'))
         self.daili_password = str(self.redis_sql.get('daili_password'))
         self.dali_host = str(self.redis_sql.get('dali_host'))
         self.daili_port = int(self.redis_sql.get('daili_port'))
-        self.emall_fsz = str(self.redis_sql.get('emall_fsz'))
-        self.emall_name = str(self.redis_sql.get('emall_name'))
-        self.emall_password = str(self.redis_sql.get('emall_password'))
-        self.emall_sjr = str(self.redis_sql.get('emall_sjr'))
-        yuming_all = list(self.redis_sql.smembers('fanwen_yuming2'))[self.zhan_number].replace("'", "").replace('[',
-                                                  '').replace(']','').split(', ')
-        self.yu = yuming_all[1]
-        self.url_ku = yuming_all[0]
         # 判断是否开启代理
         if self.daili_no == '1':
             self.session = requests.session()
             self.session.keep_alive = False
-        self.mongo_db = pymongo.MongoClient(self.ip_all, self.mongodb_port, username='root', password=self.mongodb_password)
+        # 提取过滤库
         for biao in ['quchu_title_ci', 'quchu_title_content_ci', 'quchu_lujing_ci', 'quchu_content_ci', 'tag_ciku']:
             # 去除标题内指定词
             if biao == 'quchu_title_ci':
                 self.quchu_title_cis = list(self.redis_sql.smembers(biao))
             # 去除标题含指定词的内容
             elif biao == 'quchu_title_content_ci':
                 self.quchu_title_content_cis = list(self.redis_sql.smembers(biao))
@@ -727,8 +689,70 @@
                 self.quchu_content_cis = list(self.redis_sql.smembers(biao))
         try:
             # 异步运行瑞文系列网站数据
             self.ruiwen_xilie()
         except Exception as e:
             self.email('%s入库审核脚本报错' % self.yu, '报错为：%s' % e)
 
+# 主类
+class start():
+
+    # 列表分割
+    def func(self, lst, n):
+        for i in range(0, len(lst), n):
+            yield lst[i:i + n]
+
+    # 引入数据
+    def __init__(self, zhan_number, ip_all, redis_password, redis_port, redis_db,xiancheng):
+        self.zhan_number = zhan_number
+        self.ip_all = ip_all
+        self.redis_password = redis_password
+        self.redis_port = redis_port
+        self.redis_db = redis_db
+        self.xiancheng = int(xiancheng)
+        self.run()
+
+    # 报错邮箱(不含附件)
+    def email(self, title, content):
+        msg = MIMEText(content)
+        msg["Subject"] = title
+        msg['From'] = self.emall_fsz
+        smtp_server = 'smtp.qq.com'
+        server = smtplib.SMTP_SSL(smtp_server, 465, timeout=2)
+        server.ehlo()
+        server.login(self.emall_name, self.emall_password)
+        server.sendmail(self.emall_name, [self.emall_sjr], msg.as_string())
+        server.quit()
+
+    # 主程序
+    def run(self):
+        pool = redis.ConnectionPool(host=self.ip_all, port=self.redis_port, password=self.redis_password,db=self.redis_db,decode_responses=True)
+        self.redis_sql = redis.Redis(connection_pool=pool)
+        self.mongodb_port = int(self.redis_sql.get('mongodb_port'))
+        self.mongodb_password = str(self.redis_sql.get('mongodb_password'))
+        self.emall_fsz = str(self.redis_sql.get('emall_fsz'))
+        self.emall_name = str(self.redis_sql.get('emall_name'))
+        self.emall_password = str(self.redis_sql.get('emall_password'))
+        self.emall_sjr = str(self.redis_sql.get('emall_sjr'))
+        yuming_all = list(self.redis_sql.smembers('fanwen_yuming2'))[self.zhan_number].replace("'", "").replace('[','').replace(']', '').split(', ')
+        self.yu = yuming_all[1]
+        self.url_ku = yuming_all[0]
+        self.mongo_db = pymongo.MongoClient(self.ip_all, self.mongodb_port, username='root',password=self.mongodb_password)
+        # 去除已经爬取过的url
+        zong_url = list(self.redis_sql.sdiff(self.url_ku, self.url_ku.replace('_url','_url_qita'),self.url_ku.replace('_url', '_yu_quchong'),self.url_ku.replace('_url', '_url_chucuo')))
+        # 判断是否启用多线程
+        if self.xiancheng > 1:
+            # 线程组
+            ths = []
+            list_url = list(self.func(zong_url,self.xiancheng))
+            for xian_zong_url,id_xian in zip(list_url,range(0,len(list_url))):
+                th = threading.Thread(target=ruiwen_all, args=(self.ip_all, self.yu, self.url_ku,xian_zong_url,self.mongo_db,self.redis_sql,self.email))
+                th.start()
+                print('成功启动线程%s' % id_xian)
+                ths.append(th)
+            # 等待所有线程运行结束
+            for th in ths:
+                threading.Thread.join(th)
+        else:
+            ruiwen_all(self.yu, self.url_ku,zong_url,self.mongo_db,self.redis_sql,self.email)
+
         self.email('有程序运行结束', '%s入库程序结束' % self.yu)
```


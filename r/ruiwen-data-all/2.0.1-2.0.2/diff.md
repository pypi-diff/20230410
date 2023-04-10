# Comparing `tmp/ruiwen_data_all-2.0.1.tar.gz` & `tmp/ruiwen_data_all-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruiwen_data_all-2.0.1.tar", last modified: Mon Apr 10 11:19:27 2023, max compression
+gzip compressed data, was "ruiwen_data_all-2.0.2.tar", last modified: Mon Apr 10 11:45:41 2023, max compression
```

## Comparing `ruiwen_data_all-2.0.1.tar` & `ruiwen_data_all-2.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:19:27.058610 ruiwen_data_all-2.0.1/
--rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 11:19:27.057584 ruiwen_data_all-2.0.1/PKG-INFO
--rw-r--r--   0 xiaochuan   (501) staff       (20)      673 2023-04-10 11:18:34.000000 ruiwen_data_all-2.0.1/pyproject.toml
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:19:27.052479 ruiwen_data_all-2.0.1/ruiwen_data_all/
--rw-r--r--   0 xiaochuan   (501) staff       (20)    37511 2023-04-10 11:18:34.000000 ruiwen_data_all-2.0.1/ruiwen_data_all/__init__.py
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:19:27.057052 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/
--rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 11:19:27.000000 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/PKG-INFO
--rw-r--r--   0 xiaochuan   (501) staff       (20)      236 2023-04-10 11:19:27.000000 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/SOURCES.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)        1 2023-04-10 11:19:27.000000 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/dependency_links.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       53 2023-04-10 11:19:27.000000 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/requires.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       16 2023-04-10 11:19:27.000000 ruiwen_data_all-2.0.1/ruiwen_data_all.egg-info/top_level.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       38 2023-04-10 11:19:27.058891 ruiwen_data_all-2.0.1/setup.cfg
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:45:41.810185 ruiwen_data_all-2.0.2/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 11:45:41.809588 ruiwen_data_all-2.0.2/PKG-INFO
+-rw-r--r--   0 xiaochuan   (501) staff       (20)      673 2023-04-10 11:45:31.000000 ruiwen_data_all-2.0.2/pyproject.toml
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:45:41.804667 ruiwen_data_all-2.0.2/ruiwen_data_all/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)    37549 2023-04-10 11:45:31.000000 ruiwen_data_all-2.0.2/ruiwen_data_all/__init__.py
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 11:45:41.808734 ruiwen_data_all-2.0.2/ruiwen_data_all.egg-info/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 11:45:41.000000 ruiwen_data_all-2.0.2/ruiwen_data_all.egg-info/PKG-INFO
+-rw-r--r--   0 xiaochuan   (501) staff       (20)      236 2023-04-10 11:45:41.000000 ruiwen_data_all-2.0.2/ruiwen_data_all.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)        1 2023-04-10 11:45:41.000000 ruiwen_data_all-2.0.2/ruiwen_data_all.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       53 2023-04-10 11:45:41.000000 ruiwen_data_all-2.0.2/ruiwen_data_all.egg-info/requires.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       16 2023-04-10 11:45:41.000000 ruiwen_data_all-2.0.2/ruiwen_data_all.egg-info/top_level.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       38 2023-04-10 11:45:41.810397 ruiwen_data_all-2.0.2/setup.cfg
```

### Comparing `ruiwen_data_all-2.0.1/pyproject.toml` & `ruiwen_data_all-2.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ruiwen_data_all"
-version = "2.0.1"
+version = "2.0.2"
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
-#pip install ruiwen-data-all==1.0.3
+#pip install ruiwen-data-all==2.0.1
 #pip install setuptools==57.5.0 -i https://pypi.tuna.tsinghua.edu.cn/simple
 #docker ps -a
 #docker exec -it 3a3afa942911 bash
 #pip install -U requests[socks]  socks5代理
 #pip install --index https://mirrors.ustc.edu.cn/pypi/web/simple/ virtualenv
```

### Comparing `ruiwen_data_all-2.0.1/ruiwen_data_all/__init__.py` & `ruiwen_data_all-2.0.2/ruiwen_data_all/__init__.py`

 * *Files 1% similar despite different names*

```diff
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
                 th = threading.Thread(target=ruiwen_all, args=(self.ip_all, self.yu, self.url_ku,xian_zong_url,self.mongo_db,self.redis_sql,self.email))
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


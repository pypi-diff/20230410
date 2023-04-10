# Comparing `tmp/ruiwen_data_all-2.0.4.tar.gz` & `tmp/ruiwen_data_all-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruiwen_data_all-2.0.4.tar", last modified: Mon Apr 10 12:02:43 2023, max compression
+gzip compressed data, was "ruiwen_data_all-2.0.5.tar", last modified: Mon Apr 10 12:12:10 2023, max compression
```

## Comparing `ruiwen_data_all-2.0.4.tar` & `ruiwen_data_all-2.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 12:02:43.361833 ruiwen_data_all-2.0.4/
--rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 12:02:43.361518 ruiwen_data_all-2.0.4/PKG-INFO
--rw-r--r--   0 xiaochuan   (501) staff       (20)      673 2023-04-10 12:02:00.000000 ruiwen_data_all-2.0.4/pyproject.toml
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 12:02:43.357635 ruiwen_data_all-2.0.4/ruiwen_data_all/
--rw-r--r--   0 xiaochuan   (501) staff       (20)    37549 2023-04-10 12:02:00.000000 ruiwen_data_all-2.0.4/ruiwen_data_all/__init__.py
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 12:02:43.361108 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/
--rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 12:02:43.000000 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/PKG-INFO
--rw-r--r--   0 xiaochuan   (501) staff       (20)      236 2023-04-10 12:02:43.000000 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/SOURCES.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)        1 2023-04-10 12:02:43.000000 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/dependency_links.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       53 2023-04-10 12:02:43.000000 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/requires.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       16 2023-04-10 12:02:43.000000 ruiwen_data_all-2.0.4/ruiwen_data_all.egg-info/top_level.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       38 2023-04-10 12:02:43.361938 ruiwen_data_all-2.0.4/setup.cfg
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 12:12:10.254580 ruiwen_data_all-2.0.5/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 12:12:10.254149 ruiwen_data_all-2.0.5/PKG-INFO
+-rw-r--r--   0 xiaochuan   (501) staff       (20)      673 2023-04-10 12:12:00.000000 ruiwen_data_all-2.0.5/pyproject.toml
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 12:12:10.248542 ruiwen_data_all-2.0.5/ruiwen_data_all/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)    37536 2023-04-10 12:12:00.000000 ruiwen_data_all-2.0.5/ruiwen_data_all/__init__.py
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 12:12:10.253464 ruiwen_data_all-2.0.5/ruiwen_data_all.egg-info/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 12:12:10.000000 ruiwen_data_all-2.0.5/ruiwen_data_all.egg-info/PKG-INFO
+-rw-r--r--   0 xiaochuan   (501) staff       (20)      236 2023-04-10 12:12:10.000000 ruiwen_data_all-2.0.5/ruiwen_data_all.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)        1 2023-04-10 12:12:10.000000 ruiwen_data_all-2.0.5/ruiwen_data_all.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       53 2023-04-10 12:12:10.000000 ruiwen_data_all-2.0.5/ruiwen_data_all.egg-info/requires.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       16 2023-04-10 12:12:10.000000 ruiwen_data_all-2.0.5/ruiwen_data_all.egg-info/top_level.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       38 2023-04-10 12:12:10.254748 ruiwen_data_all-2.0.5/setup.cfg
```

### Comparing `ruiwen_data_all-2.0.4/pyproject.toml` & `ruiwen_data_all-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ruiwen_data_all"
-version = "2.0.4"
+version = "2.0.5"
 dependencies = [
   "redis",
   "requests",
   "asyncio",
   "urllib3",
   "pymongo",
   "w3lib",
```

### Comparing `ruiwen_data_all-2.0.4/ruiwen_data_all/__init__.py` & `ruiwen_data_all-2.0.5/ruiwen_data_all/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -741,15 +741,15 @@
         zong_url = list(self.redis_sql.sdiff(self.url_ku, self.url_ku.replace('_url','_url_qita'),self.url_ku.replace('_url', '_yu_quchong'),self.url_ku.replace('_url', '_url_chucuo')))
         # 判断是否启用多线程
         if self.xiancheng > 1:
             # 线程组
             ths = []
             list_url = list(self.func(zong_url,self.redis_sql.scard(yuming_all[0])//self.xiancheng))
             for xian_zong_url,id_xian in zip(list_url,range(0,len(list_url))):
-                th = threading.Thread(target=ruiwen_all, args=(self.ip_all, self.yu, self.url_ku,xian_zong_url,self.mongo_db,self.redis_sql,self.email))
+                th = threading.Thread(target=ruiwen_all, args=(self.yu, self.url_ku,xian_zong_url,self.mongo_db,self.redis_sql,self.email))
                 th.start()
                 print('成功启动线程%s' % id_xian)
                 ths.append(th)
             # 等待所有线程运行结束
             for th in ths:
                 threading.Thread.join(th)
         else:
```


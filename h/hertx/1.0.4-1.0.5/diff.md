# Comparing `tmp/hertx-1.0.4.tar.gz` & `tmp/hertx-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hertx-1.0.4.tar", last modified: Wed Jul  6 16:35:03 2022, max compression
+gzip compressed data, was "dist\hertx-1.0.5.tar", last modified: Sun Mar 12 06:06:05 2023, max compression
```

## Comparing `hertx-1.0.4.tar` & `hertx-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,54 @@
-drwxrwxrwx   0        0        0        0 2022-07-06 16:35:03.423638 hertx-1.0.4/
--rw-rw-rw-   0        0        0      210 2022-07-06 16:35:03.423638 hertx-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-07-06 16:35:03.411629 hertx-1.0.4/hertx/
--rw-rw-rw-   0        0        0      330 2022-07-06 16:31:20.000000 hertx-1.0.4/hertx/__init__.py
--rw-rw-rw-   0        0        0      119 2022-07-06 05:10:57.000000 hertx-1.0.4/hertx/excel.py
--rw-rw-rw-   0        0        0    12244 2022-07-06 16:19:14.000000 hertx-1.0.4/hertx/httpx.py
--rw-rw-rw-   0        0        0      118 2022-07-06 05:10:57.000000 hertx-1.0.4/hertx/m3u8.py
--rw-rw-rw-   0        0        0      119 2022-07-06 05:10:57.000000 hertx-1.0.4/hertx/mysql.py
--rw-rw-rw-   0        0        0      117 2022-07-06 05:10:57.000000 hertx-1.0.4/hertx/pdf.py
--rw-rw-rw-   0        0        0      119 2022-07-06 05:10:57.000000 hertx-1.0.4/hertx/redis.py
--rw-rw-rw-   0        0        0      118 2022-07-06 16:31:10.000000 hertx-1.0.4/hertx/video.py
--rw-rw-rw-   0        0        0      119 2022-07-06 05:10:57.000000 hertx-1.0.4/hertx/win32.py
--rw-rw-rw-   0        0        0      118 2022-07-06 05:10:57.000000 hertx-1.0.4/hertx/word.py
-drwxrwxrwx   0        0        0        0 2022-07-06 16:35:03.421635 hertx-1.0.4/hertx.egg-info/
--rw-rw-rw-   0        0        0      210 2022-07-06 16:35:03.000000 hertx-1.0.4/hertx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2022-07-06 16:35:03.000000 hertx-1.0.4/hertx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-06 16:35:03.000000 hertx-1.0.4/hertx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2022-07-06 16:35:03.000000 hertx-1.0.4/hertx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-07-06 16:35:03.000000 hertx-1.0.4/hertx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-06 16:35:03.424637 hertx-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      453 2022-07-06 16:33:52.000000 hertx-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/
+-rw-rw-rw-   0        0        0      282 2023-03-12 06:06:05.000000 hertx-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx/
+-rw-rw-rw-   0        0        0      401 2022-08-21 13:09:38.000000 hertx-1.0.5/hertx/__init__.py
+-rw-rw-rw-   0        0        0     1727 2023-03-12 05:08:25.000000 hertx-1.0.5/hertx/img.py
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx/interface/
+-rw-rw-rw-   0        0        0      122 2022-07-09 09:10:43.000000 hertx-1.0.5/hertx/interface/__init__.py
+-rw-rw-rw-   0        0        0      192 2022-07-24 12:31:17.000000 hertx-1.0.5/hertx/interface/excel.py
+-rw-rw-rw-   0        0        0      304 2022-08-21 13:10:48.000000 hertx-1.0.5/hertx/interface/httpx.py
+-rw-rw-rw-   0        0        0      119 2022-07-08 11:31:29.000000 hertx-1.0.5/hertx/interface/mysql.py
+-rw-rw-rw-   0        0        0      402 2022-08-21 13:01:14.000000 hertx-1.0.5/hertx/interface/pdf.py
+-rw-rw-rw-   0        0        0      376 2022-07-09 11:43:44.000000 hertx-1.0.5/hertx/interface/video.py
+-rw-rw-rw-   0        0        0      119 2022-07-08 11:32:11.000000 hertx-1.0.5/hertx/interface/win32.py
+-rw-rw-rw-   0        0        0      396 2022-07-24 12:55:56.000000 hertx-1.0.5/hertx/interface/word.py
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx/libs/
+-rw-rw-rw-   0        0        0      125 2022-07-07 15:51:23.000000 hertx-1.0.5/hertx/libs/__init__.py
+-rw-rw-rw-   0        0        0     2576 2023-02-14 03:15:20.000000 hertx-1.0.5/hertx/libs/db.py
+-rw-rw-rw-   0        0        0     2424 2023-02-14 03:11:12.000000 hertx-1.0.5/hertx/libs/db2.py
+-rw-rw-rw-   0        0        0     3429 2023-02-14 09:42:01.000000 hertx-1.0.5/hertx/libs/dbmysql.py
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx/libs/excel/
+-rw-rw-rw-   0        0        0      125 2022-07-07 15:51:52.000000 hertx-1.0.5/hertx/libs/excel/__init__.py
+-rw-rw-rw-   0        0        0     2942 2022-07-09 09:36:59.000000 hertx-1.0.5/hertx/libs/excel/excel.py
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx/libs/httpx/
+-rw-rw-rw-   0        0        0      127 2022-07-07 15:51:40.000000 hertx-1.0.5/hertx/libs/httpx/__init__.py
+-rw-rw-rw-   0        0        0      553 2022-08-21 03:37:18.000000 hertx-1.0.5/hertx/libs/httpx/chrome_agent.py
+-rw-rw-rw-   0        0        0     8270 2022-08-21 03:40:42.000000 hertx-1.0.5/hertx/libs/httpx/http.py
+-rw-rw-rw-   0        0        0     3028 2023-02-27 06:41:30.000000 hertx-1.0.5/hertx/libs/httpx/session.py
+-rw-rw-rw-   0        0        0    11292 2023-02-14 03:08:20.000000 hertx-1.0.5/hertx/libs/mysql_helper.py
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx/libs/pdf/
+-rw-rw-rw-   0        0        0      126 2022-07-11 12:07:09.000000 hertx-1.0.5/hertx/libs/pdf/__init__.py
+-rw-rw-rw-   0        0        0     2206 2022-11-09 07:25:40.000000 hertx-1.0.5/hertx/libs/pdf/pdf.py
+-rw-rw-rw-   0        0        0     1543 2023-03-11 04:49:22.000000 hertx-1.0.5/hertx/libs/pdf.py
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx/libs/video/
+-rw-rw-rw-   0        0        0      125 2022-07-07 15:51:17.000000 hertx-1.0.5/hertx/libs/video/__init__.py
+-rw-rw-rw-   0        0        0      761 2022-11-25 08:09:00.000000 hertx-1.0.5/hertx/libs/video/video.py
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx/libs/word/
+-rw-rw-rw-   0        0        0      126 2022-07-11 12:19:06.000000 hertx-1.0.5/hertx/libs/word/__init__.py
+-rw-rw-rw-   0        0        0     1738 2022-07-24 12:53:05.000000 hertx-1.0.5/hertx/libs/word/word.py
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx/utils/
+-rw-rw-rw-   0        0        0      342 2022-08-21 12:46:13.000000 hertx-1.0.5/hertx/utils/__init__.py
+-rw-rw-rw-   0        0        0     1671 2022-10-25 06:07:37.000000 hertx-1.0.5/hertx/utils/common.py
+-rw-rw-rw-   0        0        0     1762 2022-08-21 12:22:58.000000 hertx-1.0.5/hertx/utils/encryption_tools.py
+-rw-rw-rw-   0        0        0      424 2022-08-21 12:20:43.000000 hertx-1.0.5/hertx/utils/image_tools.py
+-rw-rw-rw-   0        0        0     1675 2022-07-09 11:43:26.000000 hertx-1.0.5/hertx/utils/magic_decorator.py
+-rw-rw-rw-   0        0        0      312 2022-08-21 12:29:26.000000 hertx-1.0.5/hertx/utils/random_tools.py
+-rw-rw-rw-   0        0        0     2997 2022-07-08 11:35:33.000000 hertx-1.0.5/hertx/utils/threadx.py
+drwxrwxrwx   0        0        0        0 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx.egg-info/
+-rw-rw-rw-   0        0        0      282 2023-03-12 06:06:04.000000 hertx-1.0.5/hertx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1021 2023-03-12 06:06:05.000000 hertx-1.0.5/hertx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-12 06:06:04.000000 hertx-1.0.5/hertx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      204 2023-03-12 06:06:04.000000 hertx-1.0.5/hertx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-03-12 06:06:04.000000 hertx-1.0.5/hertx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-12 06:06:05.000000 hertx-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-03-12 06:06:00.000000 hertx-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `hertx-1.0.4/hertx/httpx.py` & `hertx-1.0.5/hertx/libs/mysql_helper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,385 +1,325 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2022/6/4 10:33
-# @Author  : hertx
-# @Software: PyCharm
-# @File    : http.py
-import sys
-import time
-import json
-from functools import wraps
+import re
+import threading
 from typing import Union, List
-from requests import Session, Response, exceptions
-from requests.cookies import cookiejar_from_dict, RequestsCookieJar
-from requests.structures import CaseInsensitiveDict
-from requests.packages import urllib3
-from lxml import etree, html
-
-# 关闭错误提示
-urllib3.disable_warnings()
-
-__all__ = [
-    "http",
-    "Http",
-    "random_chrome_version",
-    "func_run_times",
-]
-if sys.version_info >= (3,):
-    from urllib.parse import urlencode
-    from urllib import parse
-else:
-    from urllib import urlencode, parse
-
-
-def random_chrome_version():
-    import random
-    version_list = ['85.0.4183.83', '85.0.4183.87', '86.0.4240.22', '87.0.4280.20', '87.0.4280.88',
-                    '88.0.4324.96', '89.0.4389.23', '90.0.4430.24', '91.0.4472.19', '90.0.4430.212']
-    user_agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/{} ' \
-                 'Safari/537.36 '
-    return user_agent.format(random.choice(version_list))
 
+from dbutils.pooled_db import PooledDB
+from hertx.utils.magic_decorator import except_desc, func_run_times
 
-def func_run_times(lenth: int = 3):
-    """
-    函数运行耗时装饰器
-    :param lenth:默认3位小数
-    :return:
-    """
-    """
-    # @functools.wraps(func),这是python提供的装饰器。
-    # 它能把原函数的元信息拷贝到装饰器里面的 func 函数中。函数的元信息包括docstring,name,参数列表等等
-    # 可以尝试去除@functools.wraps(func),你会发现"func".__name__的输出变成了inter
-    # 经过装饰后实质上是得到的函数体是wrapper
-    @func_run_times()
-    def a():
-        ...
-    print(a.__name__)
-    """
-
-    def wrapper(fn):
-        def print_red(string):
-            print(f"\033[36m{string}\033[0m")
-
-        @wraps(fn)
-        def inter(*args, **kwargs):
-            start = time.time()
-            res = fn(*args, **kwargs)
-            print_red("run time of the func is '%s' %.*f Ms" % (fn.__name__, lenth, (time.time() - start) * 1000))
-            return res
-
-        return inter
 
-    return wrapper
+# 获取根目录地址
+def get_root_path(import_name):
+    import sys
+    import os
+    import pkgutil
+    mod = sys.modules.get(import_name)
+    if mod is not None and hasattr(mod, "__file__"):
+        return os.path.dirname(os.path.abspath(mod.__file__))
+    loader = pkgutil.get_loader(import_name)
+    if loader is None or import_name == "__main__":
+        return os.getcwd()
+    raise RuntimeError(f'{import_name}文件名错误')
 
 
-def requests_catch_exception(func):
-    """
-    requests异常捕获装饰器
-    :param func:
-    :return:
-    """
-
-    @wraps(func)
-    def wrapper(*args, **kwargs) -> Union[HTTPResponse, HTTPError]:
-        try:
-            return func(*args, **kwargs)
-        except exceptions.HTTPError:
-            return HTTPError(1000, 'HTTP错误!')
-        except exceptions.SSLError:
-            return HTTPError(1001, 'SSL错误!')
-        except exceptions.ProxyError:
-            return HTTPError(1002, '代理错误!')
-        except exceptions.ConnectTimeout:
-            return HTTPError(1003, '请求响应超时!')
-        except exceptions.ConnectionError:
-            return HTTPError(1004, '网络连接错误!')
-        except exceptions.ChunkedEncodingError:
-            return HTTPError(1005, 'chunked编码错误!')
-        except exceptions.ContentDecodingError:
-            return HTTPError(1006, '内部解码错误!')
-        except Exception as e:
-            return HTTPError(1007, e)
-
-    return wrapper
-
-
-class HTTPResponse(object):
-
-    def __init__(self, response: Response):
-        """
-        :param response:http响应请求体
-        """
-        self.ok = True
-        self.__html = None
-        self.__response = response
-        self.code = response.status_code
-        if response.encoding and response.encoding.lower() in ['iso-8859-1', 'gb2312']:
-            """
-            部分页面没有编码"说明"，无法检测到编码类型,如果默认编码在常用编码类型之外将强制转化为最常见的gbk编码
-            也可手动更改或使用apparent_encoding做自适应
-            虽然默认编码是GB2312,但是实际上使用的是GBK编码 且 GB2312 是 GBK子集
-            """
-            self.encoding = 'GBK'
-
-    def apparent_encoding(self):
-        """
-        应用自适应检测网页编码,会大幅度降低速度且不能做到完全匹配
-        """
-        self.encoding = self.__response.apparent_encoding
-        if self.encoding.lower() == 'gb2312':
-            self.encoding = 'GBK'
-        return self.encoding
-
-    @property
-    def encoding(self):
-        return self.__response.encoding
-
-    @encoding.setter
-    def encoding(self, encode):
-        self.__response.encoding = encode
-
-    @property
-    def json(self) -> dict:
-        if (3,) <= sys.version_info < (3, 6):
-            return json.loads(self.res.content.decode(self.encoding), encoding=self.encoding)
-        return self.__response.json()
-
-    @property
-    def lxml(self):
-        # 按需install bs4
-        from bs4 import BeautifulSoup
-        return BeautifulSoup(self.__response.text, "lxml")
-
-    def xpath(self, *args) -> List[html.HtmlElement]:
-        self.__html = self.__html if self.__html is not None else etree.HTML(self.text)
-        return self.__html.xpath(*args)
-
-    @property
-    def text(self):
-        return self.__response.text
-
-    @property
-    def content(self):
-        return self.__response.content
-
-    @property
-    def res(self):
-        return self.__response
-
-    @property
-    def cookies(self):
-        return BaseRequest.cookiejar2dict(self.__response.cookies)
-
-    @property
-    def headers(self):
-        return self.__response.headers
-
-    def xml2dict(self, xml_data=None) -> dict:
-        import xmltodict
-        dict_xml = xmltodict.parse(xml_data) if xml_data else xmltodict.parse(self.text.encode("utf-8"))
-        return json.loads(json.dumps(dict_xml))
-
-    def dict2xml(self, json_str: Union[dict, str] = None):
-        json_str = json_str if json_str else self.json
-        if isinstance(json_str, str):
-            json_str = json.loads(json_str)
-        if len(json_str.keys()) > 1:
-            json_str = {'root': json_str}
-        # 按需install xmltodict
-        import xmltodict
-        return xmltodict.unparse(json_str, pretty=1)
-
-    def __str__(self):
-        return "{}:{}".format(self.__response, self.encoding)
-
-
-class HTTPError(object):
-    """请求错误"""
-
-    def __init__(self, code, reason=None):
-        """
-        :param code: http状态码
-        :param reason: http状态原因
-        """
-        super().__init__()
-        self.ok = False
-        self.code = code
-        self.reason = reason
-
-    def __str__(self):
-        return "HTTP {}: {}".format(self.code, self.reason)
-
-
-class BaseRequest:
-
-    @classmethod
-    def get(cls, url, params=None, timeout=None, proxies=None, **kwargs):
-        """
-        GET请求
-        """
-        kwargs.setdefault('allow_redirects', True)
-        return cls.request('GET', url, params=params, timeout=timeout, proxies=proxies, **kwargs)
-
-    @classmethod
-    def post(cls, url, data=None, timeout=None, proxies=None, **kwargs):
+class Config(dict):
+    def __init__(self, defaults=None):
         """
-        POST请求
+        # 初始化默认字典
+        :param defaults:
         """
-        return cls.request('POST', url, data=data, timeout=timeout, proxies=proxies, **kwargs)
+        dict.__init__(self, defaults or {})
 
-    @staticmethod
-    @requests_catch_exception
-    def request(method, url, **kwargs):
+    def from_object(self, obj):
         """
-        :param method: 大小不敏感，在Session内部upper统一转化为大写
-        :param url: 地址
-        :param kwargs:
+         # 规定只导入对象中key所有字母为大写
+        :param obj:
         :return:
         """
-        kwargs.setdefault('ignore_status', True)
-        ignore_status = kwargs.pop('ignore_status')
-        kwargs.setdefault('headers', {"User-Agent": random_chrome_version()})
-        with Session().request(method, url, **kwargs) as r:
-            results = HTTPResponse(r)
-        if not ignore_status and results.code != 200:
-            return HTTPError(results.code, '请求状态错异常!')
-        return results
+        [self.update({key: getattr(obj, key)}) if key.isupper() else '' for key in dir(obj)]
+        return self
 
-    @staticmethod
-    def cookiejar2dict(cookiejar: RequestsCookieJar) -> dict:
-        """
-        CookieJar转dict
-        """
-        return (lambda ck: [[ck.update({k: v}) for k, v in cookiejar.items()], ck][1])(dict())
 
-    @staticmethod
-    def dict2cookiejar(cookie_dict: dict) -> RequestsCookieJar:
-        """
-        dict转CookieJar
-        """
-        return cookiejar_from_dict(cookie_dict)
+class SqlHelper(object):
+    """这是一个简单的数据库连接池类"""
+    _instance_lock = threading.Lock()
+
+    def __new__(cls, *args, **kwargs):  # 构造函数 | __del__析构函数or销毁函数(对象结束其生命周期)
+        """构造函数"""
+        """单例模式"""
+        with cls._instance_lock:
+            if not hasattr(cls, "_instance"):
+                # print('初始化单例模式')
+                cls._instance = object.__new__(cls)
+            return cls._instance
+
+    def __init__(self, config_class=None):
+        """初始化SqlHelper"""
+        if config_class is not None:
+            self.init(config_class)
+        self.local = threading.local()
+        self.config = Config()
+        self.pool = None
+
+    def init(self, config_class):
+        import pymysql
+        # db_type = self.config.setdefault('SQL_CREATOR', 'mysql')
+        # # print(db_type)
+        # if db_type == 'mysql':
+        #     db_creator = importlib.import_module('pymysql')
+        # elif db_type == 'sqlserver':
+        #     db_creator = importlib.import_module('pymssql')
+        # elif db_type == 'oracle':
+        #     db_creator = importlib.import_module('cx_Oracle')
+        # else:
+        #     raise Exception('unsupported database type ' + db_type)
+        #
+        # # pymysql = importlib.import_module('pymysql')
+        if not bool(self.config.from_object(config_class)):
+            raise ValueError('The config of key be None or NULL')
+        if not self.config.get('SQL_DATABASE'):
+            raise ValueError('SQL_DATABASE的值不能为None或NULL')
+        """
+        初始化连接池
+        """
+        self.pool = PooledDB(
+            creator=pymysql,
+            maxconnections=self.config.setdefault('SQL_MAX_CONNECT', 16),
+            mincached=self.config.setdefault('SQL_MIN_CACHED', 1),
+            blocking=self.config.setdefault('SQL_BLOCKING', True),
+            ping=self.config.setdefault('SQL_PING', 0),
+            host=self.config.setdefault('SQL_HOST', '127.0.0.1'),
+            port=self.config.setdefault('SQL_PORT', 3306),
+            user=self.config.setdefault('SQL_USER', 'root'),
+            password=self.config.setdefault('SQL_PASSWORD', '123456'),
+            database=self.config.setdefault('SQL_DATABASE', None),
+            charset=self.config.setdefault('SQL_CHARSET', 'utf8')
+        )
 
-    @staticmethod
-    def _raw_headers_to_dict(this_headers_str: str) -> dict:
-        """
-        抓包raw字符串解析为headers
+    def open(self):
         """
+        打开连接
+        :return:
         """
-        results = {}
-        for item in this_headers_str.strip().split('\n'):
-            if not item.strip():
-                continue
-            items = item.strip().split(':')
-            results[items[0]] = ':'.join(items[1:]).strip()
-        return results
-        """
-        # lambda
-        return (lambda x: [[(lambda xx: (
-            lambda items: [xx.update({items[0].strip(): ':'.join(items[1:]).strip()}), xx][1]))(x)(
-            item.strip().split(':')) for item in this_headers_str.strip().split('\n') if item.strip()], x])(dict())[1]
+        conn = self.pool.connection()  # 创建连接
+        cursor = conn.cursor()  # 获取游标
+        return conn, cursor
+
+    def close(self, conn, cursor):
+        """
+        关闭连接
+        :param conn:
+        :param cursor:
+        :return: 无明显作用
+        """
+        # print('关闭')
+        cursor.close()
+        conn.close()
+        return self
 
     @staticmethod
-    def dict2url(dict_params) -> str:
-        """
-        字典转url
-        :param dict_params:
+    def _tuple2dict(results: list, cursor):
+        """将查询到的元组类型数据转化为字典类型数据"""
+        column_desc = cursor.description  # 获取连接对象的描述信息 column_desc[0][0] 第一个字段的名称
+        column_names = [column_desc[index][0] for index in range(len(column_desc))]  # 字段名称列表
+        return [dict(zip(column_names, item)) for item in results]
+
+    @func_run_times(3)
+    def all(self, sql, *args) -> list:
+        sql = sql.replace('%', '%%')
+        """返回多个数据，字典类型"""
+        with self as f:
+            conn, cur = f
+            cur.execute(sql, args)
+            results = cur.fetchall()
+        return self._tuple2dict(results, cur)
+
+    @func_run_times(3)
+    def first(self, sql, *args):
+        sql = sql.replace('%', '%%')
+        """一条数据"""
+        with self as f:
+            conn, cur = f
+            cur.execute(sql, args)
+            results = cur.fetchone()
+            # print(results)
+        if results:
+            return self._tuple2dict([results], cur)
+
+    @func_run_times(3)
+    def execute(self, sql, *args):
+        sql = sql.replace('%', '%%')
+        """执行sql"""
+        with self as f:
+            conn, cur = f
+            try:
+                cur.execute(sql, args)
+                conn.commit()
+                return True
+            except Exception as e:
+                print('[{}]meet error'.format(sql))
+                print(e.args[-1])
+                conn.rollback()
+                return False
+
+    # @func_run_times(3)
+    # def update(self, sql, *args):
+    #     """一条数据"""
+    #     with self as f:
+    #         conn, cur = f
+    #         f[1].execute(sql, args)
+    #         results = f.fetchone()
+    #     if results:
+    #         return self._tuple2dict([results], f)
+
+    def __enter__(self):
+        """
+        # 实现with obj as f 主动从连接池中拿连接对象 并存放至线程堆中
+        :return: 连接对象cursor
+        """
+        # print('打开')
+        conn, cursor = self.open()
+        # 读取线程堆中存放当前线程sql_helper_stack存放的数据
+        cc = getattr(self.local, 'sql_helper_stack', None)
+        if not cc:
+            self.local.sql_helper_stack = [(conn, cursor)]
+        else:
+            cc.append((conn, cursor))
+            self.local.sql_helper_stack = cc
+        return conn, cursor
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        """
+        # 实现with 结束 从线程堆中获取链接对象，并回收连接至连接池
+        :param exc_type:
+        :param exc_val:
+        :param exc_tb:
         :return:
         """
-        return urlencode(dict_params)
+        cc = getattr(self.local, 'sql_helper_stack', None)
+        if not cc:
+            return
+        self.close(*self.local.sql_helper_stack.pop())
 
-    @staticmethod
-    def quote(content, encoding='utf-8', **kwargs):
-        """
-        url编码
-        """
-        return parse.quote(content, encoding=encoding, **kwargs)
 
-    @staticmethod
-    def unquote(content, encoding='utf-8', **kwargs):
-        """
-        url解码
-        """
-        return parse.unquote(content, encoding=encoding, **kwargs)
+db = SqlHelper()
 
 
-class Http(BaseRequest):
-    """基于requests 方便日常使用的简单二次封装"""
+def query_1z_timeslot_handle_num(startTime, endTime):
+    """
+    密接数据转运_Main
+    """
+    return db.all(f"select * from yqfk_yw where rpa_end_time >= STR_TO_DATE('{startTime}','%Y-%m-%d %H:%i:%S') "
+                  f"and rpa_end_time <= STR_TO_DATE('{endTime}','%Y-%m-%d %H:%i:%S')  "
+                  f"and (message LIKE '一转_条%' or message LIKE '一转__条%')")
 
-    def __init__(self, ignore_status=True):
-        """
-        :param ignore_status: 是否忽略错误状态码
-        """
-        self.__http = Session()
-        self.headers = {"User-Agent": random_chrome_version()}
-        self.ignore_status = ignore_status
 
-    def get(self, url, params=None, timeout=None, proxies=None, **kwargs):
-        """
-        GET请求
-        """
-        kwargs.setdefault('allow_redirects', True)
-        return self.request('GET', url, params=params, timeout=timeout, proxies=proxies, **kwargs)
+def query_2z_timeslot_handle_num(startTime, endTime):
+    """
+    密接数据转运二转_Main
+    """
+    return db.all(f"select * from yqfk_yw where rpa_end_time >= STR_TO_DATE('{startTime}','%Y-%m-%d %H:%i:%S') "
+                  f"and rpa_end_time <= STR_TO_DATE('{endTime}','%Y-%m-%d %H:%i:%S')  "
+                  f"and (message LIKE '二转_条%' or message LIKE '二转__条%')")
 
-    def post(self, url, data=None, timeout=None, proxies=None, **kwargs):
-        """
-        POST请求
-        """
-        return self.request('POST', url, data=data, timeout=timeout, proxies=proxies, **kwargs)
 
-    @requests_catch_exception
-    def request(self, method, url, **kwargs):
-        """
-        :param method: 大小不敏感，在Session内部upper统一转化为大写
-        :param url: 地址
-        :param kwargs:
-        :return:
-        """
-        with self.__http.request(method, url, **kwargs) as r:
-            results = HTTPResponse(r)
-        if not self.ignore_status and results.code != 200:
-            return HTTPError(results.code, '请求状态错异常!')
-        return results
+def query_1zqt_timeslot_handle_num(startTime, endTime):
+    """
+    非密接次密接数据转运_Main
+    """
+    return db.all(f"select * from yqfk_yw where rpa_end_time >= STR_TO_DATE('{startTime}','%Y-%m-%d %H:%i:%S') "
+                  f"and rpa_end_time <= STR_TO_DATE('{endTime}','%Y-%m-%d %H:%i:%S')  "
+                  f"and (message LIKE '一转其他类_条%' or message LIKE '一转其他类__条%')")
+
+
+def query_mj_items(startTime, endTime) -> List[dict]:
+    """ca_transpot_cherck_mj_items"""
+    sql = f"""
+        SELECT
+        item_name,
+        state,
+        COUNT( id ) as count
+    FROM
+        ca_transpot_cherck_mj_items 
+    WHERE
+        rpa_start_time > STR_TO_DATE( '{startTime}', '%Y-%m-%d %H:%i:%S' ) 
+        AND rpa_start_time < STR_TO_DATE( '{endTime}', '%Y-%m-%d %H:%i:%S' ) 
+        AND item_name = '市区密接类型单据复合' 
+    GROUP BY( ISNULL( state ) )
+    """
+    return db.all(sql)
+    # print(
+    #     f"select item_name,state,rpa_start_time from ca_transpot_cherck_mj_items where rpa_start_time > STR_TO_DATE('{startTime}','%Y-%m-%d %H:%i:%S') and rpa_start_time < STR_TO_DATE('{endTime}','%Y-%m-%d %H:%i:%S') and item_name='市区密接类型单据复合'")
+    # return db.all(
+    #     f"select item_name,state,rpa_start_time from ca_transpot_cherck_mj_items where rpa_start_time > STR_TO_DATE('{startTime}','%Y-%m-%d %H:%i:%S') and rpa_start_time < STR_TO_DATE('{endTime}','%Y-%m-%d %H:%i:%S') and item_name='市区密接类型单据复合'")
+
+
+def query_cmj_items(startTime, endTime):
+    """ca_transpot_cherck_cmj_items"""
+    sql = f"""
+        SELECT
+        item_name,
+        state,
+        COUNT( id ) as count
+    FROM
+        ca_transpot_cherck_cmj_items 
+    WHERE
+        rpa_start_time > STR_TO_DATE( '{startTime}', '%Y-%m-%d %H:%i:%S' ) 
+        AND rpa_start_time < STR_TO_DATE( '{endTime}', '%Y-%m-%d %H:%i:%S' ) 
+        AND item_name = '市区次密接类型单据复合' 
+    GROUP BY( ISNULL( state ) )
+    """
 
-    @property
-    def cookies(self) -> dict:
-        """
-        读取cookies
-        # _cookies = {}
-        # [_cookies.update({k: v}) for k, v in self.__http.cookies.items()]
-        """
-        return self.cookiejar2dict(self.__http.cookies)
+    return db.all(sql)
 
-    @cookies.setter
-    def cookies(self, cookie: dict):
-        """
-        设置cookies
-        """
-        self.__http.cookies = self.dict2cookiejar(cookie)
 
-    @property
-    def headers(self) -> CaseInsensitiveDict:
-        """
-        读取当前headers
-        """
-        self.__http.headers.items()
-        return self.__http.headers
+def query_qt_items(startTime, endTime):
+    """ca_transpot_cherck_items"""
+    sql = f"""
+        SELECT
+        item_name,
+        state,
+        COUNT( id ) as count
+    FROM
+        ca_transpot_cherck_items 
+    WHERE
+        rpa_start_time > STR_TO_DATE( '{startTime}', '%Y-%m-%d %H:%i:%S' ) 
+        AND rpa_start_time < STR_TO_DATE( '{endTime}', '%Y-%m-%d %H:%i:%S' ) 
+        AND item_name = '市区其他类型单据复合' 
+    GROUP BY( ISNULL( state ) )
+    """
+    print(sql)
+    return db.all(sql)
 
-    @headers.setter
-    def headers(self, header: dict or str):
-        """
-        设置headers
-        """
-        self.__http.headers.clear()
-        self.add_headers(header)
 
-    def add_headers(self, header: dict or str) -> CaseInsensitiveDict:
-        """
-        追加headers
-        """
-        if isinstance(header, str):
-            header = self._raw_headers_to_dict(header)
-        if isinstance(header, dict):
-            return [self.__http.headers.update({k: v}) for k, v in header.items()].clear() or self.__http.headers
+from config import Development
 
+# db_result = query_1z_timeslot_handle_num(startTime, endTime)
+# print(db_result)
+# count = 0
+# for item in db_result:
+#     print('script_id', end=' , ')
+#     print(item)
+#     message = item.get('message')
+#     icount = int(re.findall(r'\d+', message)[0])
+#     count = count + icount
+# print(count)
+if __name__ == '__main__':
+    db.init(Development)
+    startTime = '2022-09-01  12:00:04'
+    endTime = '2022-09-02  14:00:18'
+    r = query_qt_items(startTime, endTime)
+    run_count = 0
+    count = 0
+    for i in r:
+        count += i['count']
+        if not i['state'] or i['state'] == 'None':
+            continue
+        else:
+            run_count = i['count']
+    print(run_count, count)
+    # message = db_result[0].get('message')
+    # print(message)
+    # print(re.findall(r'\d+', message))
+    # for i in result:
+    #     print(i)
 
-http = BaseRequest
```


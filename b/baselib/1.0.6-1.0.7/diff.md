# Comparing `tmp/baselib-1.0.6.tar.gz` & `tmp/baselib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/baselib-1.0.6.tar", last modified: Tue Apr  4 03:48:32 2023, max compression
+gzip compressed data, was "dist/baselib-1.0.7.tar", last modified: Mon Apr 10 09:46:19 2023, max compression
```

## Comparing `baselib-1.0.6.tar` & `baselib-1.0.7.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/
--rw-r--r--   0 linkerui   (501) staff       (20)      242 2023-04-04 03:48:32.000000 baselib-1.0.6/PKG-INFO
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib/demo/
--rw-r--r--   0 linkerui   (501) staff       (20)       22 2023-01-31 07:45:57.000000 baselib-1.0.6/baselib/demo/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)       86 2023-01-31 07:30:38.000000 baselib-1.0.6/baselib/demo/demo.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib/py/
--rw-r--r--   0 linkerui   (501) staff       (20)      605 2023-04-03 11:42:09.000000 baselib-1.0.6/baselib/py/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib/tests/
--rw-r--r--   0 linkerui   (501) staff       (20)      126 2023-01-31 07:48:07.000000 baselib-1.0.6/baselib/tests/demo_test.py
--rw-r--r--   0 linkerui   (501) staff       (20)      366 2023-04-03 11:24:54.000000 baselib-1.0.6/baselib/tests/httplib_test.py
--rw-r--r--   0 linkerui   (501) staff       (20)      707 2023-01-31 08:33:52.000000 baselib-1.0.6/baselib/tests/json_file_test.py
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-01-31 07:44:54.000000 baselib-1.0.6/baselib/tests/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4989 2023-04-03 11:24:54.000000 baselib-1.0.6/baselib/tests/debug.py
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-01-31 07:17:34.000000 baselib-1.0.6/baselib/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib/time/
--rw-r--r--   0 linkerui   (501) staff       (20)       39 2023-04-04 03:47:58.000000 baselib-1.0.6/baselib/time/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4480 2023-01-31 08:08:46.000000 baselib-1.0.6/baselib/time/period.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib/json/
--rw-r--r--   0 linkerui   (501) staff       (20)     1687 2023-01-31 08:21:43.000000 baselib-1.0.6/baselib/json/json_file.py
--rw-r--r--   0 linkerui   (501) staff       (20)       44 2023-04-04 03:47:39.000000 baselib-1.0.6/baselib/json/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib/log/
--rw-r--r--   0 linkerui   (501) staff       (20)       40 2023-04-04 03:47:30.000000 baselib-1.0.6/baselib/log/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1281 2023-04-03 11:24:54.000000 baselib-1.0.6/baselib/log/file.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib/request/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-04-03 11:35:22.000000 baselib-1.0.6/baselib/request/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib/qywx/
--rw-r--r--   0 linkerui   (501) staff       (20)    11157 2023-04-04 03:37:15.000000 baselib-1.0.6/baselib/qywx/qywx.py
--rw-r--r--   0 linkerui   (501) staff       (20)       38 2023-04-04 03:47:02.000000 baselib-1.0.6/baselib/qywx/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      195 2023-01-31 07:33:12.000000 baselib-1.0.6/README.md
--rw-r--r--   0 linkerui   (501) staff       (20)      460 2023-04-04 03:48:29.000000 baselib-1.0.6/setup.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib.egg-info/
--rw-r--r--   0 linkerui   (501) staff       (20)      242 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib.egg-info/PKG-INFO
--rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-01-31 07:20:51.000000 baselib-1.0.6/baselib.egg-info/not-zip-safe
--rw-r--r--   0 linkerui   (501) staff       (20)      616 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib.egg-info/SOURCES.txt
--rw-r--r--   0 linkerui   (501) staff       (20)        8 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib.egg-info/top_level.txt
--rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-04-04 03:48:32.000000 baselib-1.0.6/baselib.egg-info/dependency_links.txt
--rw-r--r--   0 linkerui   (501) staff       (20)       38 2023-04-04 03:48:32.000000 baselib-1.0.6/setup.cfg
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/
+-rw-r--r--   0 linkerui   (501) staff       (20)      242 2023-04-10 09:46:19.000000 baselib-1.0.7/PKG-INFO
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/baselib/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/baselib/demo/
+-rw-r--r--   0 linkerui   (501) staff       (20)       22 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/demo/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)       86 2023-04-10 04:09:02.000000 baselib-1.0.7/baselib/demo/demo.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/baselib/py/
+-rw-r--r--   0 linkerui   (501) staff       (20)      605 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/py/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/baselib/tests/
+-rw-r--r--   0 linkerui   (501) staff       (20)      126 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/tests/demo_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2800 2023-04-10 04:07:37.000000 baselib-1.0.7/baselib/tests/period_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      494 2023-04-10 02:10:09.000000 baselib-1.0.7/baselib/tests/httplib_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      849 2023-04-10 09:42:38.000000 baselib-1.0.7/baselib/tests/json_file_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/tests/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4989 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/tests/debug.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1838 2023-04-10 02:21:48.000000 baselib-1.0.7/baselib/tests/file_logger_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3154 2023-04-10 02:10:09.000000 baselib-1.0.7/baselib/tests/qywx_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/baselib/time/
+-rw-r--r--   0 linkerui   (501) staff       (20)       39 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/time/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4480 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/time/period.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/baselib/json/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1687 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/json/json_file.py
+-rw-r--r--   0 linkerui   (501) staff       (20)       44 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/json/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/baselib/log/
+-rw-r--r--   0 linkerui   (501) staff       (20)       40 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/log/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2219 2023-04-10 02:11:14.000000 baselib-1.0.7/baselib/log/file.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/baselib/request/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/request/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/baselib/qywx/
+-rw-r--r--   0 linkerui   (501) staff       (20)    13625 2023-04-10 09:39:56.000000 baselib-1.0.7/baselib/qywx/qywx.py
+-rw-r--r--   0 linkerui   (501) staff       (20)       38 2023-04-04 11:38:24.000000 baselib-1.0.7/baselib/qywx/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1024 2023-04-10 02:10:09.000000 baselib-1.0.7/README.md
+-rw-r--r--   0 linkerui   (501) staff       (20)      460 2023-04-10 09:45:44.000000 baselib-1.0.7/setup.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:46:19.000000 baselib-1.0.7/baselib.egg-info/
+-rw-r--r--   0 linkerui   (501) staff       (20)      242 2023-04-10 09:46:18.000000 baselib-1.0.7/baselib.egg-info/PKG-INFO
+-rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-01-31 07:20:51.000000 baselib-1.0.7/baselib.egg-info/not-zip-safe
+-rw-r--r--   0 linkerui   (501) staff       (20)      706 2023-04-10 09:46:18.000000 baselib-1.0.7/baselib.egg-info/SOURCES.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)        8 2023-04-10 09:46:18.000000 baselib-1.0.7/baselib.egg-info/top_level.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-04-10 09:46:18.000000 baselib-1.0.7/baselib.egg-info/dependency_links.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)       38 2023-04-10 09:46:19.000000 baselib-1.0.7/setup.cfg
```

### Comparing `baselib-1.0.6/baselib/py/__init__.py` & `baselib-1.0.7/baselib/py/__init__.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.6/baselib/tests/json_file_test.py` & `baselib-1.0.7/baselib/tests/json_file_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,7 +15,11 @@
         JsonFile.update("test.json", {"msg": "world"})
         data = JsonFile.read("test.json")
         assert data == {"msg": "world"}
         JsonFile.update("test.json", {"info": "hello"})
         data = JsonFile.read("test.json")
         assert data == {"info": "hello", "msg": "world"}
         os.remove("test.json")
+        with open("test.json", "w") as fid:
+            fid.write("test")
+        data = JsonFile.read("test.json")
+        assert data == {}
```

### Comparing `baselib-1.0.6/baselib/tests/debug.py` & `baselib-1.0.7/baselib/tests/debug.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.6/baselib/time/period.py` & `baselib-1.0.7/baselib/time/period.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.6/baselib/json/json_file.py` & `baselib-1.0.7/baselib/json/json_file.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.6/baselib/log/file.py` & `baselib-1.0.7/baselib/tests/file_logger_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,52 @@
-# -*- coding:utf-8 -*- 
+# -*- coding:utf-8 -*-
+from baselib.log import file_logger
 import logging
-import logging.handlers
 
 
-def file_logger(log_path="runtime.log", log_level="DEBUG", log_format=None, time_rotating='D', encoding='utf-8', name=None):
-    """
-    param string name: 
-    param string log_level: 日志级别: ERROR/WARNING/INFO/DEBUG
-    param string log_format: 每条日志输出格式
-    param string time_rotating: 日志切割时间, 可选值: S(秒)/M(分)/H(小时)/D(天)/W(周)/midnight(深夜)
-    param string encoding: 编码
-    """
-    if not name:
-        name = __name__
-    logger = logging.getLogger(name)
-    logger.setLevel(log_level.upper())
-    if log_format is None:
-        log_format = '[%(asctime)s][%(levelname)s][%(filename)s:%(lineno)d-%(module)s] %(message)s'
-
-    formatter = logging.Formatter(log_format)
-    if time_rotating:
-        file_handler = logging.handlers.TimedRotatingFileHandler(
-            log_path, when=time_rotating, encoding=encoding)
-    else:
-        file_handler = logging.FileHandler(
-            log_path, encoding=encoding)
-    file_handler.setLevel(level=log_level)
-    file_handler.setFormatter(formatter)
-    logger.addHandler(file_handler)
-    return logger
-
-
-if __name__ == "__main__":
-    logger = file_logger()
-    logger.info("info")
-    logger.debug("debug")
+class TestFileLogger:
+    test_obj = file_logger()
+
+    def test_default_log_level(self):
+        assert self.test_obj.level == logging.DEBUG
+
+    def test_default_log_format(self):
+        formatter = logging.Formatter(
+            '[%(asctime)s][%(levelname)s][%(filename)s:%(lineno)d-%(module)s] %(message)s')
+        assert self.test_obj.handlers[0].formatter._fmt == formatter._fmt
+
+    def test_default_time_rotating(self):
+        assert isinstance(self.test_obj.handlers[0], logging.FileHandler)
+
+    def test_no_rotating(self):
+        test_obj = file_logger(time_rotating=None)
+        test_obj.info("no time rotating")
+
+    def test_custom_name(self):
+        logger = file_logger(name='test')
+        assert logger.name == 'test'
+
+    def test_custom_log_level(self):
+        logger = file_logger(log_level='WARNING')
+        assert logger.level == logging.WARNING
+
+    # def test_custom_log_format(self):
+    #     log_format = '[%(asctime)s] %(message)s'
+    #     logger = file_logger(log_format=log_format)
+    #     formatter = logging.Formatter(log_format)
+    #     assert logger.handlers[0].formatter._fmt == formatter._fmt
+
+    # def test_time_rotating_Daily_rotation_interval(self):
+    #     handler_class, interval, backup_count, delay, utc, at_time, encoding \
+    #         = type(file_handler), 'D', 0, False, False, None, 'utf-8'
+    #     handler_instance = handler_class(
+    #         filename=log_path,
+    #         when=interval,
+    #         backupCount=backup_count,
+    #         delay=delay,
+    #         utc=utc,
+    #         atTime=at_time,
+    #         encoding=encoding
+    #     )
+    #     assert isinstance(
+    #         handler_instance,
+    #         TimedRotatingFileHandler) and handler_instance.when == 'D'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `baselib-1.0.6/baselib/qywx/qywx.py` & `baselib-1.0.7/baselib/qywx/qywx.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,25 @@
 """
 企业微信机器人消息类封装
 - 消息类型：https://developer.work.weixin.qq.com/document/path/90236
 - 加解密方案说明: https://developer.work.weixin.qq.com/devtool/introduce?id=36388
 @author     : coreylin
 @createTime : 2018/12/22
 """
-from baselib.py import urllib2
 import json
 import base64
 import hashlib
 
+from baselib.py import urllib2
+from baselib.py import IS_PY3
+
+if not IS_PY3:
+    import ssl
+    ssl._create_default_https_context = ssl._create_unverified_context
+
 
 class QyWechat(object):
     """ 企业微信处理类
     """
     font_tmpl = '<font color="{color}">{info}</font>'
 
     class EnumPageType:
@@ -153,17 +159,25 @@
             base64_data = base64.b64encode(f.read())
         self._send(self.format_image(base64_data, md5))
 
     def send_news(self, data):
         pass
 
     def send_markdown(
-            self, msg, page_type=EnumPageType.CUT, limit=4096, post_msg="\n...",
-            to_user=None, to_party=None, to_tag=None, agent_id=None,
-            enable_duplicate_check=None, duplicate_check_interval=None):
+            self,
+            msg,
+            page_type=EnumPageType.CUT,
+            limit=4096,
+            post_msg="\n...",
+            to_user=None,
+            to_party=None,
+            to_tag=None,
+            agent_id=None,
+            enable_duplicate_check=None,
+            duplicate_check_interval=None):
         """ 发送 markdown 格式的数据
         :param string msg: 发送的数据内容（markdown格式）
         :param int limit: 分页参数，每条消息的最大长度（企业微信默认4096），超过该长度报错
         :param string page_type: 分页参数，消息内容超长的处理方法， 取值范围：EnumPageType.CUT
         :param string post_msg: 分页参数，选择截断时，加在消息末尾的补充信息
         :param list to_user: 指定接收消息的成员，成员ID列表（多个接收者用‘|’分隔，最多支持1000个）
             特殊情况：指定为"@all"，则向该企业应用的全部成员发送
@@ -190,16 +204,22 @@
                 msg, to_user, to_party, to_tag, agent_id,
                 enable_duplicate_check, duplicate_check_interval))
         if len(rsp_list) == 1:
             return rsp_list[0]
         return rsp_list
 
     def raw_send_markdown(
-            self, content, to_user=None, to_party=None, to_tag=None, agent_id=None,
-            enable_duplicate_check=None, duplicate_check_interval=None):
+            self,
+            content,
+            to_user=None,
+            to_party=None,
+            to_tag=None,
+            agent_id=None,
+            enable_duplicate_check=None,
+            duplicate_check_interval=None):
         """ 发送 markdown 消息
         """
         data = {
             "msgtype": "markdown",
             "markdown": {
                 "content": content
             }
@@ -227,73 +247,133 @@
             - 如果小于等于 limit，则直接返回
         :param string msg: 消息内容
         :param int limit: 消息长度限制
         :param string post_msg: 截断末尾补充消息
         :rtype: string
         :return: 返回截断后数据
         """
-        msg_len = len(msg.encode("utf-8"))
+
+        msg_unicode, encode = self.__decode_msg(msg)
+        msg_len = len(msg_unicode.encode("utf-8"))
         if msg_len <= limit:
             return msg
-        post_msg_len = len(post_msg.encode("utf-8"))
+        post_msg_unicode, _ = self.__decode_msg(post_msg)
+        post_msg_len = len(post_msg_unicode.encode("utf-8"))
         idx = 0
-        for idx in range(len(msg)):
-            if len(msg[:-1 - idx].encode("utf-8")) <= limit - post_msg_len:
+        for idx in range(len(msg_unicode)):
+            if len(msg_unicode[:-1 - idx].encode("utf-8")
+                   ) <= limit - post_msg_len:
                 break
-        return msg[:-1 - idx] + post_msg
+        ret = msg_unicode[:-1 - idx] + post_msg_unicode
+        return self.__encode_msg(ret, encode)
+
+    def __decode_msg(self, msg):
+        if IS_PY3:
+            print(1, type(msg))
+            return msg, type(msg)
+        try:
+            encode = "utf-8"
+            msg_unicode = msg.decode("utf-8")
+        except UnicodeEncodeError:
+            encode = "unicode"
+            msg_unicode = msg
+        return msg_unicode, encode
+
+    def __encode_msg(self, msg, encode):
+        """ 将字符串 msg 转换成目标编码格式 encode
+        :param msg:
+        :param encode:
+        :return:
+        """
+        # 兼容 python2
+        if not IS_PY3:
+            return msg.encode(encode)
+        # 相同时无需转换
+        if type(msg) == encode:
+            return msg
+        if type(msg) == str:
+            return msg.encode()
+        else:
+            return msg.decode()
 
     def split_msg(self, msg, limit=4096):
         """ 将消息 msg 的长度限制（limit），拆分成多条消息(一条消息即一页）
         :param string msg: 消息内容
         :param int limit: 消息长度限制
         :rtype: list
         :return: 返回分页后的数据列表
         """
-        msg_len = len(msg.encode("utf-8"))
+        msg_unicode, encode = self.__decode_msg(msg)
+        msg_len = len(msg_unicode.encode("utf-8"))
         if msg_len <= limit:
             return [msg]
         lines = [""]
         line_no = 0
-        for char in msg:
+        for char in msg_unicode:
             if len(lines[line_no].encode("utf-8")) <= limit - \
                     len(char.encode("utf-8")):
                 lines[line_no] += char
                 continue
             lines.append(char)
             line_no += 1
-        return lines
+        return [self.__encode_msg(i, encode) for i in lines]
 
     def split_msg_by_line(self, msg, limit=4096):
-        """ 将数据按行分页
-            本函数适用场景： 消息分多行，单行不超过 limit的情况，单行limit会直接截断
-        :param string msg: 消息内容
+        """将数据按行分页
+
+        本函数适用场景：消息分多行，单行不超过 limit 的情况，单行 limit 会直接截断
+
+        :param str msg: 消息内容
         :param int limit: 消息长度限制
-        :rtype: list
         :return: 返回分页后的数据列表
+        :rtype: list
         """
+        # 去除消息内容两端的空格
         msg = msg.strip()
-        msg_len = len(msg.encode("utf-8"))
+        msg_unicode, encode = self.__decode_msg(msg)
+        # 计算消息内容的字节数
+        msg_len = len(msg_unicode.encode("utf-8"))
+        # 如果消息内容的字节数小于限制，则直接返回
         if msg_len < limit:
             return [msg]
+        # 初始化分页长度、页码、页列表
         page_len = page_no = 0
         page_list = [""]
-        for aline in msg.split("\n"):
+        # 遍历消息内容的每一行
+        for aline in msg_unicode.split("\n"):
+            # 计算当前行的字节数
             len_aline = len("{}\n".format(aline).encode("utf-8"))
+            if len_aline >= limit:
+                page_len = 0
+                page_no += 2
+                page_list.append(self.cut_msg(aline, limit, "..."))
+                page_list.append("")
+                continue
+            # 如果当前行加上分页长度小于限制，则将当前行添加到当前页
             if page_len + len_aline <= limit:
                 page_len += len_aline
                 page_list[page_no] += "{}\n".format(aline)
                 continue
+            # 如果当前行加上分页长度大于限制，则将当前行添加到新的一页
             page_len = 0
             page_no += 1
-            page_list.append(self.cut_msg(aline, limit, "..."))
-        return [i.strip() for i in page_list]
+            page_list.append(aline)
+        # 返回分页后的数据列表
+        return [self.__encode_msg(i.strip(), encode) for i in page_list if len(i) > 0]
 
 
 if __name__ == "__main__":
     def demo():
         key = ""  # robot key
         robot = QyWechat(key=key, is_ssl=True, debug=True)
-        aline = "[hello](http://www.baidu.com)"*100
+        aline = "[hello](http://www.baidu.com)" * 100
         print(robot.send_markdown(
             "# test\n" + aline + "\n" + aline + "\n",
             page_type=robot.EnumPageType.SPLIT_BY_LINES))
-    demo()
+    # demo()
+    robot = QyWechat("")
+    msg = "你好，世界"
+    limit = 9
+    expected = ["你好，", "世界"]
+    print(type(msg))
+    print(type(robot.split_msg(msg, limit)[0]))
+    print(type(expected[0]))
```

### Comparing `baselib-1.0.6/baselib.egg-info/SOURCES.txt` & `baselib-1.0.7/baselib.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,11 +15,14 @@
 baselib/py/__init__.py
 baselib/qywx/__init__.py
 baselib/qywx/qywx.py
 baselib/request/__init__.py
 baselib/tests/__init__.py
 baselib/tests/debug.py
 baselib/tests/demo_test.py
+baselib/tests/file_logger_test.py
 baselib/tests/httplib_test.py
 baselib/tests/json_file_test.py
+baselib/tests/period_test.py
+baselib/tests/qywx_test.py
 baselib/time/__init__.py
 baselib/time/period.py
```


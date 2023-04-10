# Comparing `tmp/PrSpiders-0.2.6.tar.gz` & `tmp/PrSpiders-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.2.6.tar", last modified: Fri Apr  7 07:28:59 2023, max compression
+gzip compressed data, was "PrSpiders-0.2.7.tar", last modified: Mon Apr 10 14:07:26 2023, max compression
```

## Comparing `PrSpiders-0.2.6.tar` & `PrSpiders-0.2.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 07:28:59.701983 PrSpiders-0.2.6/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.2.6/LICENSE.txt
--rw-rw-rw-   0        0        0     4511 2023-04-07 07:28:59.699984 PrSpiders-0.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-07 07:28:59.619987 PrSpiders-0.2.6/PrSpider/
--rw-rw-rw-   0        0        0     8777 2023-04-07 07:28:46.000000 PrSpiders-0.2.6/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.2.6/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    10988 2023-04-07 07:28:46.000000 PrSpiders-0.2.6/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3995 2023-04-07 07:28:46.000000 PrSpiders-0.2.6/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.6/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-07 07:28:59.666981 PrSpiders-0.2.6/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4511 2023-04-07 07:28:59.000000 PrSpiders-0.2.6/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2023-04-07 07:28:59.000000 PrSpiders-0.2.6/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 07:28:59.000000 PrSpiders-0.2.6/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-07 07:28:59.000000 PrSpiders-0.2.6/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-07 07:28:59.000000 PrSpiders-0.2.6/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-04-07 07:28:59.000000 PrSpiders-0.2.6/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3999 2023-03-30 07:25:40.000000 PrSpiders-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 07:28:59.684984 PrSpiders-0.2.6/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.2.6/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8883 2023-03-22 07:44:13.000000 PrSpiders-0.2.6/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.2.6/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.6/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-04-07 07:28:59.701983 PrSpiders-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-04-07 07:28:46.000000 PrSpiders-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 07:28:59.695989 PrSpiders-0.2.6/table_parse/
--rw-rw-rw-   0        0        0   282891 2023-03-22 06:00:42.000000 PrSpiders-0.2.6/table_parse/T.py
--rw-rw-rw-   0        0        0        0 2023-03-22 06:03:34.000000 PrSpiders-0.2.6/table_parse/__init__.py
--rw-rw-rw-   0        0        0     3005 2023-03-22 08:01:31.000000 PrSpiders-0.2.6/table_parse/tb_parse.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:07:26.300608 PrSpiders-0.2.7/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.2.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     4469 2023-04-10 14:07:26.296610 PrSpiders-0.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 14:07:26.228608 PrSpiders-0.2.7/PrSpider/
+-rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.2.7/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.2.7/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    10988 2023-04-07 07:28:46.000000 PrSpiders-0.2.7/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3995 2023-04-07 07:28:46.000000 PrSpiders-0.2.7/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.7/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:07:26.260610 PrSpiders-0.2.7/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4469 2023-04-10 14:07:25.000000 PrSpiders-0.2.7/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2023-04-10 14:07:26.000000 PrSpiders-0.2.7/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:07:25.000000 PrSpiders-0.2.7/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-10 14:07:25.000000 PrSpiders-0.2.7/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-10 14:07:25.000000 PrSpiders-0.2.7/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-04-10 14:07:25.000000 PrSpiders-0.2.7/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3957 2023-04-10 01:15:21.000000 PrSpiders-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 14:07:26.274610 PrSpiders-0.2.7/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.2.7/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8883 2023-03-22 07:44:13.000000 PrSpiders-0.2.7/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.2.7/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.7/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:07:26.300608 PrSpiders-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-04-10 14:06:53.000000 PrSpiders-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:07:26.293612 PrSpiders-0.2.7/table_parse/
+-rw-rw-rw-   0        0        0   282891 2023-03-22 06:00:42.000000 PrSpiders-0.2.7/table_parse/T.py
+-rw-rw-rw-   0        0        0        0 2023-03-22 06:03:34.000000 PrSpiders-0.2.7/table_parse/__init__.py
+-rw-rw-rw-   0        0        0     3005 2023-03-22 08:01:31.000000 PrSpiders-0.2.7/table_parse/tb_parse.py
```

### Comparing `PrSpiders-0.2.6/LICENSE.txt` & `PrSpiders-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.6/PKG-INFO` & `PrSpiders-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.2.6
+Version: 0.2.7
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -21,25 +21,26 @@
 and retries*
 
 
 > **ProTip:** Request to carry random useragent by default.
 
 ## *Introduction to Usage*
 
-| Args               | Values                                            | notes                           |
-|--------------------|---------------------------------------------------|---------------------------------|
-| `method`           | `Examle: "get" or "post" Type: string`            | `Request Method`                |
-| `url`              | `Examle: "http://www.example.com" Type: string`   | `Request Url`                   |
-| `headers`          | `Type: dict`                                      | `Default Random Request Header` |
-| `data`             | `Type: dict or string`                            | `Request parameters`            |
-| `encoding`         | `Default: "utf-8" Type: string`                   | `Request Encoding`              |
-| `retry_time`       | `Default: 3 Type: int`                            | `Retry Count`                   |
-| `retry_interval`   | `Default: 1 Type: int`                            | `Retry Interval`                |
-| `timeout`          | `Default: 3 Type: int`                            | `Request timeout`               |
-| `others`           | `*args or **kwargs`                               | `Follow Requests`               | 
+| Args             | Values                                          | notes                           |
+|------------------|-------------------------------------------------|---------------------------------|
+| `method`         | `Examle: "get" or "post" Type: string`          | `Request Method`                |
+| `url`            | `Examle: "http://www.example.com" Type: string` | `Request Url`                   |
+| `headers`        | `Type: dict`                                    | `Default Random Request Header` |
+| `data`           | `Type: dict or string`                          | `Request parameters`            |
+| `encoding`       | `Default: "utf-8" Type: string`                 | `Request Encoding`              |
+| `retry_time`     | `Default: 3 Type: int`                          | `Retry Count`                   |
+| `retry_interval` | `Default: 1 Type: int`                          | `Retry Interval`                |
+| `timeout`        | `Default: 3 Type: int`                          | `Request timeout`               |
+| `others`         | `*args or **kwargs`                             | `Follow Requests`               | 
+
 
 
 ## *Get started*
 
 Install Package: pip install requestXpath
 Make a request:
```

### Comparing `PrSpiders-0.2.6/PrSpider/PrSpiders.py` & `PrSpiders-0.2.7/PrSpider/PrSpiders.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         settions.success_num = self.success_num
         settions.false_num = self.false_num
         settions.retry = self.retry
         settions.workers = self.workers
         settions.download_delay = self.download_delay
         settions.download_num = self.download_num
         logging.info(
-            '****************** @PrSpider Start  @Workers %s  @Retry %s  @Pid %s @Download_Delay %s ******************'
-            % (self.workers, self.retry, self.pid, self.download_delay))
+            '****************** @PrSpider Start  @Workers %s  @Retry %s  @Pid %s @Download_Delay %s @Download_Num %s ******************'
+            % (self.workers, self.retry, self.pid, self.download_delay, self.download_num))
         if not self.start_urls and not hasattr(self, 'start_requests'):
             raise AttributeError(
                 "Crawling could not start: 'start_urls' not found ")
         else:
             self.start_requests()
 
     def start_requests(cls, **kwargs):
@@ -53,17 +53,17 @@
             cls.Requests(callback=cls.parse,
                          url=u, **kwargs)
 
     @classmethod
     def RequestsMap(cls, request=None, callback=None, headers=None, retry_time=3, method='GET', meta=None,
                     encoding='utf-8', retry_interval=1, timeout=10, **kwargs):
         futures = []
-        if isinstance(request, str):
+        if not isinstance(request, list):
             raise AttributeError(
-                "Requests object must be list")
+                "Requests object must be list: [{'url': 1, 'data': 1},{'url': 2, 'params': 2}]")
         else:
             url_dim_list = [request[i:i + cls.download_num]
                             for i in range(0, len(request), cls.download_num)]
             for u in url_dim_list:
                 time.sleep(cls.download_delay)
                 for _u in u:
                     url = _u.get('url')
@@ -88,33 +88,26 @@
 
     @classmethod
     def Requests(cls, url=None, callback=None, headers=None, retry_time=3, method='GET', meta=None,
                  encoding='utf-8', retry_interval=1, timeout=10, **kwargs, ):
         futures = []
         if isinstance(url, str):
             url = [url]
-        if len(url) > 10:
-            url_dim_list = [url[i:i + cls.download_num]
-                            for i in range(0, len(url), cls.download_num)]
-            for u in url_dim_list:
-                time.sleep(cls.download_delay)
-                for _u in u:
-                    futures.append(
-                        ThreadPoolExecutor(cls.workers).submit(cls.fetch, url=_u, callback=callback, headers=headers,
-                                                               timeout=timeout,
-                                                               retry_time=retry_time,
-                                                               method=method, meta=meta, encoding=encoding,
-                                                               retry_interval=retry_interval, **kwargs))
-        else:
-            for _url in url:
+        url_dim_list = [url[i:i + cls.download_num]
+                        for i in range(0, len(url), cls.download_num)]
+        for u in url_dim_list:
+            time.sleep(cls.download_delay)
+            for _u in u:
                 futures.append(
-                    ThreadPoolExecutor(cls.workers).submit(cls.fetch, url=_url, callback=callback, headers=headers,
+                    ThreadPoolExecutor(cls.workers).submit(cls.fetch, url=_u, callback=callback, headers=headers,
+                                                           timeout=timeout,
                                                            retry_time=retry_time,
                                                            method=method, meta=meta, encoding=encoding,
                                                            retry_interval=retry_interval, **kwargs))
+
         for future in as_completed(futures):
             worker_exception = future.exception()
             if worker_exception:
                 current_time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
                 logging.exception(
                     f'{current_time} [PrSpider Exception] %s' % worker_exception)
 
@@ -128,16 +121,26 @@
                                   encoding=encoding, retry_interval=retry_interval, timeout=timeout,
                                   settion=settions, **kwargs)
         if response:
             if response.ok:
                 settions.success_num += 1
                 logging.info(
                     f'{current_time} [PrSpider] True [Method] {method} [Status] {response.code} [Url] {url}')
-            callback(response)
-            return self
+                callback(response)
+                return self
+            else:
+                settions.false_num += 1
+                if response:
+                    logging.error(
+                        f'{current_time} [PrSpider] False [Method] {method} [Status] {response.code} [Url] {url}')
+                else:
+                    logging.error(
+                        f'{current_time} [PrSpider] Error [Method] {method} [Status] Timeout [Url] {url}')
+                callback(response)
+                return self
         else:
             settions.false_num += 1
             if response:
                 logging.error(
                     f'{current_time} [PrSpider] False [Method] {method} [Status] {response.code} [Url] {url}')
             else:
                 logging.error(
@@ -166,22 +169,25 @@
             average_time = spend_time / self.request_num
         except ZeroDivisionError:
             average_time = 0
         m = """
 -->Spider Close Status.
 | ------------------ | ----------------------
 | `Requests`         | `Response Close.`                                 
-| `request_num`      | `%s`                                             
-| `success_num`      | `%s`                                             
-| `false_num`        | `%s`                                              
-| `start_time`       | `%s`                                              
-| `end_time`         | `%s`                                             
-| `spend_time`       | `%.3fs`                                          
-| `average_time`     | `%.3fs`         
-| ------------------ | ----------------------                                  
+| `Workers`          | `%s`                                             
+| `Download Delay`   | `%s`                                             
+| `Download Num`     | `%s`                                             
+| `Request Num`      | `%s`                                             
+| `Success Num`      | `%s`                                             
+| `False Num`        | `%s`                                              
+| `Start Time`       | `%s`                                              
+| `End Time`         | `%s`                                             
+| `Spend Time`       | `%.3fs`                                          
+| `Average Time`     | `%.3fs`         
+| ------------------ | ----------------------                            
         """ % (
-            self.request_num, self.success_num, self.false_num,
+            self.workers, self.download_delay, self.download_num, self.request_num, self.success_num, self.false_num,
             self.process_timestamp(self.start_time), self.process_timestamp(
                 end_time), spend_time,
             average_time
         )
         logging.info(m)
```

### Comparing `PrSpiders-0.2.6/PrSpider/pxpath.py` & `PrSpiders-0.2.7/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.6/PrSpider/requestXpath.py` & `PrSpiders-0.2.7/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.6/PrSpider/useragent.py` & `PrSpiders-0.2.7/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.6/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.2.7/PrSpiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.2.6
+Version: 0.2.7
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -21,25 +21,26 @@
 and retries*
 
 
 > **ProTip:** Request to carry random useragent by default.
 
 ## *Introduction to Usage*
 
-| Args               | Values                                            | notes                           |
-|--------------------|---------------------------------------------------|---------------------------------|
-| `method`           | `Examle: "get" or "post" Type: string`            | `Request Method`                |
-| `url`              | `Examle: "http://www.example.com" Type: string`   | `Request Url`                   |
-| `headers`          | `Type: dict`                                      | `Default Random Request Header` |
-| `data`             | `Type: dict or string`                            | `Request parameters`            |
-| `encoding`         | `Default: "utf-8" Type: string`                   | `Request Encoding`              |
-| `retry_time`       | `Default: 3 Type: int`                            | `Retry Count`                   |
-| `retry_interval`   | `Default: 1 Type: int`                            | `Retry Interval`                |
-| `timeout`          | `Default: 3 Type: int`                            | `Request timeout`               |
-| `others`           | `*args or **kwargs`                               | `Follow Requests`               | 
+| Args             | Values                                          | notes                           |
+|------------------|-------------------------------------------------|---------------------------------|
+| `method`         | `Examle: "get" or "post" Type: string`          | `Request Method`                |
+| `url`            | `Examle: "http://www.example.com" Type: string` | `Request Url`                   |
+| `headers`        | `Type: dict`                                    | `Default Random Request Header` |
+| `data`           | `Type: dict or string`                          | `Request parameters`            |
+| `encoding`       | `Default: "utf-8" Type: string`                 | `Request Encoding`              |
+| `retry_time`     | `Default: 3 Type: int`                          | `Retry Count`                   |
+| `retry_interval` | `Default: 1 Type: int`                          | `Retry Interval`                |
+| `timeout`        | `Default: 3 Type: int`                          | `Request timeout`               |
+| `others`         | `*args or **kwargs`                             | `Follow Requests`               | 
+
 
 
 ## *Get started*
 
 Install Package: pip install requestXpath
 Make a request:
```

### Comparing `PrSpiders-0.2.6/README.md` & `PrSpiders-0.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 and retries*
 
 
 > **ProTip:** Request to carry random useragent by default.
 
 ## *Introduction to Usage*
 
-| Args               | Values                                            | notes                           |
-|--------------------|---------------------------------------------------|---------------------------------|
-| `method`           | `Examle: "get" or "post" Type: string`            | `Request Method`                |
-| `url`              | `Examle: "http://www.example.com" Type: string`   | `Request Url`                   |
-| `headers`          | `Type: dict`                                      | `Default Random Request Header` |
-| `data`             | `Type: dict or string`                            | `Request parameters`            |
-| `encoding`         | `Default: "utf-8" Type: string`                   | `Request Encoding`              |
-| `retry_time`       | `Default: 3 Type: int`                            | `Retry Count`                   |
-| `retry_interval`   | `Default: 1 Type: int`                            | `Retry Interval`                |
-| `timeout`          | `Default: 3 Type: int`                            | `Request timeout`               |
-| `others`           | `*args or **kwargs`                               | `Follow Requests`               | 
+| Args             | Values                                          | notes                           |
+|------------------|-------------------------------------------------|---------------------------------|
+| `method`         | `Examle: "get" or "post" Type: string`          | `Request Method`                |
+| `url`            | `Examle: "http://www.example.com" Type: string` | `Request Url`                   |
+| `headers`        | `Type: dict`                                    | `Default Random Request Header` |
+| `data`           | `Type: dict or string`                          | `Request parameters`            |
+| `encoding`       | `Default: "utf-8" Type: string`                 | `Request Encoding`              |
+| `retry_time`     | `Default: 3 Type: int`                          | `Retry Count`                   |
+| `retry_interval` | `Default: 1 Type: int`                          | `Retry Interval`                |
+| `timeout`        | `Default: 3 Type: int`                          | `Request timeout`               |
+| `others`         | `*args or **kwargs`                             | `Follow Requests`               | 
+
 
 
 ## *Get started*
 
 Install Package: pip install requestXpath
 Make a request:
```

### Comparing `PrSpiders-0.2.6/requestXpath/__init__.py` & `PrSpiders-0.2.7/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.6/requestXpath/pxpath.py` & `PrSpiders-0.2.7/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.6/requestXpath/requestXpath.py` & `PrSpiders-0.2.7/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.6/requestXpath/useragent.py` & `PrSpiders-0.2.7/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.6/setup.py` & `PrSpiders-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
-__version__ = '0.2.6'
+__version__ = '0.2.7'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

### Comparing `PrSpiders-0.2.6/table_parse/T.py` & `PrSpiders-0.2.7/table_parse/T.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.6/table_parse/tb_parse.py` & `PrSpiders-0.2.7/table_parse/tb_parse.py`

 * *Files identical despite different names*


# Comparing `tmp/unicorn-binance-websocket-api-1.45.1.tar.gz` & `tmp/unicorn-binance-websocket-api-1.45.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicorn-binance-websocket-api-1.45.1.tar", last modified: Fri Apr  7 22:27:48 2023, max compression
+gzip compressed data, was "unicorn-binance-websocket-api-1.45.2.tar", last modified: Mon Apr 10 01:47:18 2023, max compression
```

## Comparing `unicorn-binance-websocket-api-1.45.1.tar` & `unicorn-binance-websocket-api-1.45.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-07 22:27:48.930439 unicorn-binance-websocket-api-1.45.1/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     1215 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.1/LICENSE
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    43675 2023-04-07 22:27:48.925920 unicorn-binance-websocket-api-1.45.1/PKG-INFO
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    41825 2023-04-07 22:23:46.000000 unicorn-binance-websocket-api-1.45.1/README.md
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)       38 2023-04-07 22:27:48.932437 unicorn-binance-websocket-api-1.45.1/setup.cfg
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     4904 2023-04-04 00:02:14.000000 unicorn-binance-websocket-api-1.45.1/setup.py
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-07 22:27:48.722990 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      498 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/__init__.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    47042 2023-04-07 22:03:52.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/api.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    26452 2023-04-06 12:13:20.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/connection.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2874 2023-04-06 10:06:24.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/connection_settings.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2168 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/exceptions.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)   208063 2023-04-07 22:26:25.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/manager.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    14327 2023-04-04 08:52:30.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/restclient.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     3673 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/restserver.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    16540 2023-04-07 16:36:46.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/sockets.py
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-07 22:27:48.882751 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api.egg-info/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    43675 2023-04-07 22:27:47.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api.egg-info/PKG-INFO
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      680 2023-04-07 22:27:47.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)        1 2023-04-07 22:27:47.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      144 2023-04-07 22:27:47.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api.egg-info/requires.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)       30 2023-04-07 22:27:47.000000 unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api.egg-info/top_level.txt
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-10 01:47:18.508813 unicorn-binance-websocket-api-1.45.2/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     1215 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.2/LICENSE
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    44007 2023-04-10 01:47:18.504819 unicorn-binance-websocket-api-1.45.2/PKG-INFO
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    42159 2023-04-09 23:44:27.000000 unicorn-binance-websocket-api-1.45.2/README.md
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)       38 2023-04-10 01:47:18.510814 unicorn-binance-websocket-api-1.45.2/setup.cfg
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     4925 2023-04-10 01:41:32.000000 unicorn-binance-websocket-api-1.45.2/setup.py
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-10 01:47:18.311409 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      498 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/__init__.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    47042 2023-04-07 22:03:52.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/api.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    26452 2023-04-06 12:13:20.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/connection.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2836 2023-04-10 01:34:45.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/connection_settings.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2168 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/exceptions.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)   208184 2023-04-10 01:46:50.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/manager.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    14327 2023-04-04 08:52:30.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/restclient.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     3673 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/restserver.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    16540 2023-04-07 16:36:46.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/sockets.py
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-10 01:47:18.473240 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    44007 2023-04-10 01:47:17.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      680 2023-04-10 01:47:17.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)        1 2023-04-10 01:47:17.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      162 2023-04-10 01:47:17.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/requires.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)       30 2023-04-10 01:47:17.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/top_level.txt
```

### Comparing `unicorn-binance-websocket-api-1.45.1/LICENSE` & `unicorn-binance-websocket-api-1.45.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.1/PKG-INFO` & `unicorn-binance-websocket-api-1.45.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicorn-binance-websocket-api
-Version: 1.45.1
+Version: 1.45.2
 Summary: An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, com-isolated_margin+testnet, com-futures+testnet, jersey, us, jex, dex/chain+testnet) in a easy, fast, flexible, robust and fully-featured way.
 Home-page: https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api
 Author: LUCIT Systems and Development
 Author-email: info@lucit.tech
 License: MIT License
 Project-URL: Howto, https://www.lucit.tech/unicorn-binance-websocket-api.html#howto
 Project-URL: Documentation, https://unicorn-binance-websocket-api.docs.lucit.tech
@@ -131,16 +131,16 @@
 from unicorn_binance_websocket_api.manager import BinanceWebSocketApiManager
 
 
 def process_api_responses(stream_data):
     print(str(stream_data))
 
 
-api_key = ""
-api_secret = ""
+api_key = "YOUR BINANCE API KEY"
+api_secret = "YOUR BINANCE API SECRET"
 
 ubwa = BinanceWebSocketApiManager(exchange="binance.com")
 api_stream = ubwa.create_stream(api=True, api_key=api_key, api_secret=api_secret,
                                 process_stream_data=process_api_responses)
                                 
 orig_client_order_id = ubwa.api.create_order(stream_id=api_stream, price=1.1, order_type="LIMIT",
                                              quantity=15.0, side="SELL", symbol="BUSDUSDT")
@@ -403,16 +403,18 @@
 - [example_subscribe.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_subscribe.py)
 - [example_ticker_and_miniticker.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_ticker_and_miniticker.py)
 - [example_trade_stream.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_trade_stream.py)
 - [example_trbinance.com.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_trbinance_com.py)
 - [example_userdata_stream.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_userdata_stream.py)
 - [example_userdata_stream_new_style.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_userdata_stream_new_style.py)
 - [example_version_of_this_package.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_version_of_this_package.py)
+- [example_websocket_api.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_websocket_api.py)
 
 ## Howto
+- [Create and Cancel Orders via WebSocket on Binance](https://medium.lucit.tech/create-and-cancel-orders-via-websocket-on-binance-7f828831404)
 - [How to Download Klines from Binance using Python?](https://medium.lucit.tech/how-to-download-data-from-binance-using-python-8f1b6e8f19f3)
 - [How to Connect to binance.com Websockets using Python via a Socks5 Proxy](https://medium.lucit.tech/how-to-connect-to-binance-com-websockets-using-python-via-a-socks5-proxy-3c5a3e063f12)
 
 ## Project Homepage
 [https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 
 ## Wiki
```

### Comparing `unicorn-binance-websocket-api-1.45.1/README.md` & `unicorn-binance-websocket-api-1.45.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,16 @@
 from unicorn_binance_websocket_api.manager import BinanceWebSocketApiManager
 
 
 def process_api_responses(stream_data):
     print(str(stream_data))
 
 
-api_key = ""
-api_secret = ""
+api_key = "YOUR BINANCE API KEY"
+api_secret = "YOUR BINANCE API SECRET"
 
 ubwa = BinanceWebSocketApiManager(exchange="binance.com")
 api_stream = ubwa.create_stream(api=True, api_key=api_key, api_secret=api_secret,
                                 process_stream_data=process_api_responses)
                                 
 orig_client_order_id = ubwa.api.create_order(stream_id=api_stream, price=1.1, order_type="LIMIT",
                                              quantity=15.0, side="SELL", symbol="BUSDUSDT")
@@ -366,16 +366,18 @@
 - [example_subscribe.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_subscribe.py)
 - [example_ticker_and_miniticker.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_ticker_and_miniticker.py)
 - [example_trade_stream.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_trade_stream.py)
 - [example_trbinance.com.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_trbinance_com.py)
 - [example_userdata_stream.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_userdata_stream.py)
 - [example_userdata_stream_new_style.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_userdata_stream_new_style.py)
 - [example_version_of_this_package.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_version_of_this_package.py)
+- [example_websocket_api.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_websocket_api.py)
 
 ## Howto
+- [Create and Cancel Orders via WebSocket on Binance](https://medium.lucit.tech/create-and-cancel-orders-via-websocket-on-binance-7f828831404)
 - [How to Download Klines from Binance using Python?](https://medium.lucit.tech/how-to-download-data-from-binance-using-python-8f1b6e8f19f3)
 - [How to Connect to binance.com Websockets using Python via a Socks5 Proxy](https://medium.lucit.tech/how-to-connect-to-binance-com-websockets-using-python-via-a-socks5-proxy-3c5a3e063f12)
 
 ## Project Homepage
 [https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 
 ## Wiki
```

### Comparing `unicorn-binance-websocket-api-1.45.1/setup.py` & `unicorn-binance-websocket-api-1.45.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                  "com-isolated_margin+testnet, com-futures+testnet, jersey, us, jex, dex/chain+testnet) in a easy, fast"
                  ", flexible, robust and fully-featured way.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      license='MIT License',
      install_requires=['colorama', 'requests', 'websocket-client', 'websockets==10.4', 'flask_restful',
                        'cheroot', 'flask', 'ujson', 'psutil', 'PySocks', 'unicorn-fy',
-                       'unicorn-binance-rest-api>=1.8.1'],
+                       'unicorn-binance-rest-api>=1.8.1', 'typing_extensions'],
      keywords='binance, asyncio, async, asynchronous, concurrent, websocket-api, webstream-api, '
               'binance-websocket, binance-webstream, webstream, websocket, api, binance-jersey, binance-dex, '
               'binance-futures, binance-margin, binance-us',
      project_urls={
          'Howto': 'https://www.lucit.tech/unicorn-binance-websocket-api.html#howto',
          'Documentation': 'https://unicorn-binance-websocket-api.docs.lucit.tech',
          'Wiki': 'https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki',
```

### Comparing `unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/api.py` & `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/api.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/connection.py` & `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/connection.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/connection_settings.py` & `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/connection_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
+import sys
 from enum import Enum
-from typing import Tuple
 
-# Works only in Python >= 3.9:
-# from typing import Tuple, Type
-# MAX_SUBSCRIPTIONS_PER_STREAM: Type[int] = int
-# RESTFUL_BASE_URI: Type[str] = str
-# RESTFUL_PATH_USERDATA: Type[str] = str
-# WEBSOCKET_BASE_URI: Type[str] = str
-
-# To maintain backward compatibility, we use instead:
-MAX_SUBSCRIPTIONS_PER_STREAM = int
-WEBSOCKET_BASE_URI = str
-WEBSOCKET_API_BASE_URI = str
+if sys.version_info >= (3, 9):
+    from typing import Type
+    MAX_SUBSCRIPTIONS_PER_STREAM: Type[int] = int
+    WEBSOCKET_BASE_URI: Type[str] = str
+    WEBSOCKET_API_BASE_URI: Type[str] = str
+else:
+    MAX_SUBSCRIPTIONS_PER_STREAM = int
+    WEBSOCKET_BASE_URI = str
+    WEBSOCKET_API_BASE_URI = str
 
 
 class Exchanges(str, Enum):
     BINANCE = "binance.com"
     BINANCE_TESTNET = "binance.com-testnet"
     BINANCE_MARGIN = "binance.com-margin"
     BINANCE_MARGIN_TESTNET = "binance.com-margin-testnet"
@@ -43,15 +41,18 @@
     Exchanges.BINANCE_COIN_FUTURES,
     Exchanges.BINANCE_FUTURES_TESTNET,
     Exchanges.BINANCE_US,
     Exchanges.TRBINANCE,
     Exchanges.JEX,
 ]
 
-CONNECTION_SETTINGS: dict[str, Tuple[MAX_SUBSCRIPTIONS_PER_STREAM, WEBSOCKET_BASE_URI, WEBSOCKET_API_BASE_URI]] = {
+# only python 3.9+
+# CONNECTION_SETTINGS: dict[str, Tuple[MAX_SUBSCRIPTIONS_PER_STREAM, WEBSOCKET_BASE_URI, WEBSOCKET_API_BASE_URI]] = {
+
+CONNECTION_SETTINGS = {
     Exchanges.BINANCE: (1024, "wss://stream.binance.com:9443/", "wss://ws-api.binance.com/ws-api/v3"),
     Exchanges.BINANCE_TESTNET: (1024, "wss://testnet.binance.vision/", "wss://testnet.binance.vision/ws-api/v3"),
     Exchanges.BINANCE_MARGIN: (1024, "wss://stream.binance.com:9443/", ""),
     Exchanges.BINANCE_MARGIN_TESTNET: (1024, "wss://testnet.binance.vision/", ""),
     Exchanges.BINANCE_ISOLATED_MARGIN: (1024, "wss://stream.binance.com:9443/", ""),
     Exchanges.BINANCE_ISOLATED_MARGIN_TESTNET: (1024, "wss://testnet.binance.vision/", ""),
     Exchanges.BINANCE_FUTURES: (200, "wss://fstream.binance.com/", ""),
```

### Comparing `unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/exceptions.py` & `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/manager.py` & `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,20 @@
 from unicorn_binance_websocket_api.api import BinanceWebSocketApiApi
 from cheroot import wsgi
 from collections import deque
 from datetime import datetime
 from flask import Flask, redirect
 from flask_restful import Api
 from operator import itemgetter
-from typing import Literal, Optional, Union
+from typing import Optional, Union
+try:
+    # python <=3.7 support
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
 import asyncio
 import colorama
 import copy
 import logging
 import hmac
 import hashlib
 import os
@@ -227,15 +232,15 @@
                  exchange_type: Optional[Literal['cex', 'dex']] = None,
                  socks5_proxy_server: Optional[str] = None,
                  socks5_proxy_user: Optional[str] = None,
                  socks5_proxy_pass: Optional[str] = None,
                  socks5_proxy_ssl_verification: Optional[bool] = True,):
         threading.Thread.__init__(self)
         self.name = "unicorn-binance-websocket-api"
-        self.version = "1.45.1"
+        self.version = "1.45.2"
         logger.info(f"New instance of {self.get_user_agent()} on "
                     f"{str(platform.system())} {str(platform.release())} for exchange {exchange} started ...")
         self.debug = debug
         logger.info(f"Debug is {self.debug}")
         if disable_colorama is not True:
             logger.info(f"Initiating `colorama_{colorama.__version__}`")
             colorama.init()
```

### Comparing `unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/restclient.py` & `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/restclient.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/restserver.py` & `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/restserver.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api/sockets.py` & `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/sockets.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api.egg-info/PKG-INFO` & `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicorn-binance-websocket-api
-Version: 1.45.1
+Version: 1.45.2
 Summary: An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, com-isolated_margin+testnet, com-futures+testnet, jersey, us, jex, dex/chain+testnet) in a easy, fast, flexible, robust and fully-featured way.
 Home-page: https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api
 Author: LUCIT Systems and Development
 Author-email: info@lucit.tech
 License: MIT License
 Project-URL: Howto, https://www.lucit.tech/unicorn-binance-websocket-api.html#howto
 Project-URL: Documentation, https://unicorn-binance-websocket-api.docs.lucit.tech
@@ -131,16 +131,16 @@
 from unicorn_binance_websocket_api.manager import BinanceWebSocketApiManager
 
 
 def process_api_responses(stream_data):
     print(str(stream_data))
 
 
-api_key = ""
-api_secret = ""
+api_key = "YOUR BINANCE API KEY"
+api_secret = "YOUR BINANCE API SECRET"
 
 ubwa = BinanceWebSocketApiManager(exchange="binance.com")
 api_stream = ubwa.create_stream(api=True, api_key=api_key, api_secret=api_secret,
                                 process_stream_data=process_api_responses)
                                 
 orig_client_order_id = ubwa.api.create_order(stream_id=api_stream, price=1.1, order_type="LIMIT",
                                              quantity=15.0, side="SELL", symbol="BUSDUSDT")
@@ -403,16 +403,18 @@
 - [example_subscribe.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_subscribe.py)
 - [example_ticker_and_miniticker.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_ticker_and_miniticker.py)
 - [example_trade_stream.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_trade_stream.py)
 - [example_trbinance.com.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_trbinance_com.py)
 - [example_userdata_stream.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_userdata_stream.py)
 - [example_userdata_stream_new_style.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_userdata_stream_new_style.py)
 - [example_version_of_this_package.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_version_of_this_package.py)
+- [example_websocket_api.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_websocket_api.py)
 
 ## Howto
+- [Create and Cancel Orders via WebSocket on Binance](https://medium.lucit.tech/create-and-cancel-orders-via-websocket-on-binance-7f828831404)
 - [How to Download Klines from Binance using Python?](https://medium.lucit.tech/how-to-download-data-from-binance-using-python-8f1b6e8f19f3)
 - [How to Connect to binance.com Websockets using Python via a Socks5 Proxy](https://medium.lucit.tech/how-to-connect-to-binance-com-websockets-using-python-via-a-socks5-proxy-3c5a3e063f12)
 
 ## Project Homepage
 [https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 
 ## Wiki
```

### Comparing `unicorn-binance-websocket-api-1.45.1/unicorn_binance_websocket_api.egg-info/SOURCES.txt` & `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*


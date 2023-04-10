# Comparing `tmp/py5paisa-0.6.7.tar.gz` & `tmp/py5paisa-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py5paisa-0.6.7.tar", last modified: Fri Jan  6 07:07:17 2023, max compression
+gzip compressed data, was "py5paisa-0.6.9.tar", last modified: Mon Apr 10 07:13:39 2023, max compression
```

## Comparing `py5paisa-0.6.7.tar` & `py5paisa-0.6.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 07:07:17.766852 py5paisa-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-06 07:07:07.000000 py5paisa-0.6.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-01-06 07:07:07.000000 py5paisa-0.6.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-06 07:07:07.000000 py5paisa-0.6.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-06 07:07:07.000000 py5paisa-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14381 2023-01-06 07:07:17.766852 py5paisa-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-01-06 07:07:07.000000 py5paisa-0.6.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 07:07:17.762852 py5paisa-0.6.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 07:07:17.766852 py5paisa-0.6.7/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    48489 2023-01-06 07:07:07.000000 py5paisa-0.6.7/docs/images/5-paisa-img.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 07:07:17.766852 py5paisa-0.6.7/py5paisa/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-06 07:07:07.000000 py5paisa-0.6.7/py5paisa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-01-06 07:07:07.000000 py5paisa-0.6.7/py5paisa/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-06 07:07:07.000000 py5paisa-0.6.7/py5paisa/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-06 07:07:07.000000 py5paisa-0.6.7/py5paisa/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-01-06 07:07:07.000000 py5paisa-0.6.7/py5paisa/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    32384 2023-01-06 07:07:07.000000 py5paisa-0.6.7/py5paisa/py5paisa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-01-06 07:07:07.000000 py5paisa-0.6.7/py5paisa/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-01-06 07:07:07.000000 py5paisa-0.6.7/py5paisa/urlconst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 07:07:17.766852 py5paisa-0.6.7/py5paisa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14381 2023-01-06 07:07:17.000000 py5paisa-0.6.7/py5paisa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-01-06 07:07:17.000000 py5paisa-0.6.7/py5paisa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 07:07:17.000000 py5paisa-0.6.7/py5paisa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 07:07:17.000000 py5paisa-0.6.7/py5paisa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-06 07:07:17.000000 py5paisa-0.6.7/py5paisa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-06 07:07:17.000000 py5paisa-0.6.7/py5paisa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-01-06 07:07:17.770852 py5paisa-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-06 07:07:07.000000 py5paisa-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 07:07:17.766852 py5paisa-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 07:07:07.000000 py5paisa-0.6.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-01-06 07:07:07.000000 py5paisa-0.6.7/tests/test_py5paisa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.989379 py5paisa-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-10 07:13:30.000000 py5paisa-0.6.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-10 07:13:30.000000 py5paisa-0.6.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 07:13:30.000000 py5paisa-0.6.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-10 07:13:30.000000 py5paisa-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-04-10 07:13:39.989379 py5paisa-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-10 07:13:30.000000 py5paisa-0.6.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.985379 py5paisa-0.6.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.985379 py5paisa-0.6.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    48489 2023-04-10 07:13:30.000000 py5paisa-0.6.9/docs/images/5-paisa-img.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.985379 py5paisa-0.6.9/py5paisa/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32425 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/py5paisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/urlconst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.989379 py5paisa-0.6.9/py5paisa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-10 07:13:39.989379 py5paisa-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-10 07:13:30.000000 py5paisa-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.989379 py5paisa-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 07:13:30.000000 py5paisa-0.6.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-10 07:13:30.000000 py5paisa-0.6.9/tests/test_py5paisa.py
```

### Comparing `py5paisa-0.6.7/CONTRIBUTING.rst` & `py5paisa-0.6.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.7/PKG-INFO` & `py5paisa-0.6.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py5paisa
-Version: 0.6.7
+Version: 0.6.9
 Summary:  Python SDK for 5paisa APIs natively written in VB.NET
 Home-page: https://github.com/5paisa/py5paisa
 Author: 5paisa
 Author-email: coreteam@5paisa.com
 Keywords: py5paisa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -40,15 +40,15 @@
 
 `pip install py5paisa`
 
 ### Usage
 
 #### Configuring API keys
 
-Get your API keys from https://invest.5paisa.com/DeveloperAPI/APIKeys
+Get your API keys from https://tradestation.5paisa.com/apidoc
 
 Note:- We have deprecated the existing method which involved the use of login credentials.
        Kindly go through this updated documentation of using Access token for API Access.
 
 #### AUTHENTICATION USING OAUTH
 ```py
 from py5paisa import FivePaisaClient
@@ -140,16 +140,16 @@
 # please use price = 0 for market Order
 #use IsIntraday= true for intraday orders
 
 #Using Scrip Data :-
 
 #Using Scrip Code :-
 client.place_order(OrderType='B',Exchange='N',ExchangeType='C', ScripCode = 1660, Qty=1, Price=260)
-#Sample For SL order
-client.place_order(OrderType='B',Exchange='N',ExchangeType='C', ScripCode = 1660, Qty=1, Price=350, IsIntraday=False, IsStopLossOrder=True, StopLossPrice=345)
+#Sample For SL order (for order to be treated as SL order just pass StopLossPrice)
+client.place_order(OrderType='B',Exchange='N',ExchangeType='C', ScripCode = 1660, Qty=1, Price=350, IsIntraday=False, StopLossPrice=345)
 #Derivative Order
 client.place_order(OrderType='B',Exchange='N',ExchangeType='D', ScripCode = 57633, Qty=50, Price=1.5)
 
 Please refer below documentation link for paramaters to be passed in cleint.place_order function
 https://www.5paisa.com/developerapi/order-request-place-order
 
 ```
@@ -178,46 +178,55 @@
                 "ExchOrderID": "<Exchange Order ID 1>"
             },
             {
                 "ExchOrderID": "<Exchange Order ID 2>"
             },
 client.cancel_bulk_order(cancel_bulk)
 ```
+#### SquareOffAll Orders
+
+```py
+client.squareoff_all()
+```
+
 #### Bracket Order 
 
 
 
 For placing Braket order
 ```py
-test_order=bo_co_order(scrip_code=1660,BuySell='B',Qty=1, LimitPriceInitialOrder=205,TriggerPriceInitialOrder=0,LimitPriceProfitOrder=215.0,TriggerPriceForSL=203,LimitPriceForSL=202,ExchType='C',Exch='N',RequestType='P',AtMarket=False)
+client.bo_order(OrderType='B',Exchange='N',ExchangeType='C', ScripCode = 1660, Qty=1, LimitPrice=330,TargetPrice=345,StopLossPrice=320,LimitPriceForSL=319,TrailingSL=1.5)
 
-client.bo_order(test_order)
 ```
+For placing Cover order
+```py
+client.cover_order(OrderType='B',Exchange='N',ExchangeType='C', ScripCode = 1660, Qty=1, LimitPrice=330,StopLossPrice=320,LimitPriceForSL=319,TrailingSL=1.5)
+```
+
 Note:For placing Bracket order in FNO segment pass ExchType='D'
 
-For Modifying Bracket Order only for Initial order (entry)
+For Modifying Bracket/Cover Order only for Initial order (entry)
 ```py
-test_order=bo_co_order(scrip_code=1660,BuySell='B',Qty=1, LimitPriceInitialOrder=203,TriggerPriceInitialOrder=0,LimitPriceProfitOrder=208.0,TriggerPriceForSL=202,LimitPriceForSL=201,ExchType='C',Exch='N',RequestType='M',AtMarket=False,ExchOrderId='12345678')
 
-client.bo_order(test_order)
+client.modify_bo_order(ExchOrderID="1100000017861430",LimitPrice=330)
+client.modify_cover_order(ExchOrderID="1100000017861430",LimitPrice=330)
 
 #Note : For cover order just pass LimitPriceProfitOrder equal to Zero.
 ```
 
 For Modifying LimitPriceProfitOrder 
 ```py
-test_order=Order(order_type='S', scrip_code=1660, quantity=1, price=208.50,is_intraday=True,exchange='N',exchange_segment='C',atmarket=False,exch_order_id="12345678" ,order_for='M')
-
-client.mod_bo_order(test_order)
+client.modify_bo_order(ExchOrderID="1100000017861430",TargetPrice=330)
+client.modify_cover_order(ExchOrderID="1100000017861430",TargetPrice=330)
 ```
 For Modifying TriggerPriceForSL
 ```py
-test_order=Order(order_type='S', scrip_code=1660, quantity=1, price=0,is_intraday=True,exchange='N',exchange_segment='C',atmarket=True,exch_order_id="123456789" ,stoploss_price=201.50,is_stoploss_order=True,order_for='M')
 
-client.mod_bo_order(test_order)
+client.modify_bo_order(ExchOrderID="1100000017861430",LimitPriceForSL=330)
+client.modify_bo_order(ExchOrderID="1100000017861430",LimitPriceForSL=330)
 
 #Note : You have pass atmarket=true while modifying stoploss price, Pass ExchorderId for the particular leg to modify.
 ```
 
 #### Basket Orders
 
 ```py
```

### Comparing `py5paisa-0.6.7/README.rst` & `py5paisa-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.7/docs/images/5-paisa-img.jpg` & `py5paisa-0.6.9/docs/images/5-paisa-img.jpg`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.7/py5paisa/auth.py` & `py5paisa-0.6.9/py5paisa/auth.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.7/py5paisa/const.py` & `py5paisa-0.6.9/py5paisa/const.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.7/py5paisa/order.py` & `py5paisa-0.6.9/py5paisa/order.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.7/py5paisa/py5paisa.py` & `py5paisa-0.6.9/py5paisa/py5paisa.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,15 +535,16 @@
             timeList=['1m','5m','10m','15m','30m','60m','1d']
             if time not in timeList:
                 return 'Invalid Time Frame. it should be within [1m,5m,10m,15m,30m,60m,1d].'
             else:
                 response = self.session.get(url, headers=self.jwt_headers).json()
                 candleList=response['data']['candles']
                 df=pd.DataFrame(candleList)
-                df.columns=['Datetime','Open','High','Low','Close','Volume']
+                if df.empty != True:
+                    df.columns=['Datetime','Open','High','Low','Close','Volume']
                 return df
 
         except Exception as e:
             log_response(e)
 
     def get_buy(self):
         try:
```

### Comparing `py5paisa-0.6.7/py5paisa/strategy.py` & `py5paisa-0.6.9/py5paisa/strategy.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.7/py5paisa/urlconst.py` & `py5paisa-0.6.9/py5paisa/urlconst.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.7/py5paisa.egg-info/PKG-INFO` & `py5paisa-0.6.9/py5paisa.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py5paisa
-Version: 0.6.7
+Version: 0.6.9
 Summary:  Python SDK for 5paisa APIs natively written in VB.NET
 Home-page: https://github.com/5paisa/py5paisa
 Author: 5paisa
 Author-email: coreteam@5paisa.com
 Keywords: py5paisa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -40,15 +40,15 @@
 
 `pip install py5paisa`
 
 ### Usage
 
 #### Configuring API keys
 
-Get your API keys from https://invest.5paisa.com/DeveloperAPI/APIKeys
+Get your API keys from https://tradestation.5paisa.com/apidoc
 
 Note:- We have deprecated the existing method which involved the use of login credentials.
        Kindly go through this updated documentation of using Access token for API Access.
 
 #### AUTHENTICATION USING OAUTH
 ```py
 from py5paisa import FivePaisaClient
@@ -140,16 +140,16 @@
 # please use price = 0 for market Order
 #use IsIntraday= true for intraday orders
 
 #Using Scrip Data :-
 
 #Using Scrip Code :-
 client.place_order(OrderType='B',Exchange='N',ExchangeType='C', ScripCode = 1660, Qty=1, Price=260)
-#Sample For SL order
-client.place_order(OrderType='B',Exchange='N',ExchangeType='C', ScripCode = 1660, Qty=1, Price=350, IsIntraday=False, IsStopLossOrder=True, StopLossPrice=345)
+#Sample For SL order (for order to be treated as SL order just pass StopLossPrice)
+client.place_order(OrderType='B',Exchange='N',ExchangeType='C', ScripCode = 1660, Qty=1, Price=350, IsIntraday=False, StopLossPrice=345)
 #Derivative Order
 client.place_order(OrderType='B',Exchange='N',ExchangeType='D', ScripCode = 57633, Qty=50, Price=1.5)
 
 Please refer below documentation link for paramaters to be passed in cleint.place_order function
 https://www.5paisa.com/developerapi/order-request-place-order
 
 ```
@@ -178,46 +178,55 @@
                 "ExchOrderID": "<Exchange Order ID 1>"
             },
             {
                 "ExchOrderID": "<Exchange Order ID 2>"
             },
 client.cancel_bulk_order(cancel_bulk)
 ```
+#### SquareOffAll Orders
+
+```py
+client.squareoff_all()
+```
+
 #### Bracket Order 
 
 
 
 For placing Braket order
 ```py
-test_order=bo_co_order(scrip_code=1660,BuySell='B',Qty=1, LimitPriceInitialOrder=205,TriggerPriceInitialOrder=0,LimitPriceProfitOrder=215.0,TriggerPriceForSL=203,LimitPriceForSL=202,ExchType='C',Exch='N',RequestType='P',AtMarket=False)
+client.bo_order(OrderType='B',Exchange='N',ExchangeType='C', ScripCode = 1660, Qty=1, LimitPrice=330,TargetPrice=345,StopLossPrice=320,LimitPriceForSL=319,TrailingSL=1.5)
 
-client.bo_order(test_order)
 ```
+For placing Cover order
+```py
+client.cover_order(OrderType='B',Exchange='N',ExchangeType='C', ScripCode = 1660, Qty=1, LimitPrice=330,StopLossPrice=320,LimitPriceForSL=319,TrailingSL=1.5)
+```
+
 Note:For placing Bracket order in FNO segment pass ExchType='D'
 
-For Modifying Bracket Order only for Initial order (entry)
+For Modifying Bracket/Cover Order only for Initial order (entry)
 ```py
-test_order=bo_co_order(scrip_code=1660,BuySell='B',Qty=1, LimitPriceInitialOrder=203,TriggerPriceInitialOrder=0,LimitPriceProfitOrder=208.0,TriggerPriceForSL=202,LimitPriceForSL=201,ExchType='C',Exch='N',RequestType='M',AtMarket=False,ExchOrderId='12345678')
 
-client.bo_order(test_order)
+client.modify_bo_order(ExchOrderID="1100000017861430",LimitPrice=330)
+client.modify_cover_order(ExchOrderID="1100000017861430",LimitPrice=330)
 
 #Note : For cover order just pass LimitPriceProfitOrder equal to Zero.
 ```
 
 For Modifying LimitPriceProfitOrder 
 ```py
-test_order=Order(order_type='S', scrip_code=1660, quantity=1, price=208.50,is_intraday=True,exchange='N',exchange_segment='C',atmarket=False,exch_order_id="12345678" ,order_for='M')
-
-client.mod_bo_order(test_order)
+client.modify_bo_order(ExchOrderID="1100000017861430",TargetPrice=330)
+client.modify_cover_order(ExchOrderID="1100000017861430",TargetPrice=330)
 ```
 For Modifying TriggerPriceForSL
 ```py
-test_order=Order(order_type='S', scrip_code=1660, quantity=1, price=0,is_intraday=True,exchange='N',exchange_segment='C',atmarket=True,exch_order_id="123456789" ,stoploss_price=201.50,is_stoploss_order=True,order_for='M')
 
-client.mod_bo_order(test_order)
+client.modify_bo_order(ExchOrderID="1100000017861430",LimitPriceForSL=330)
+client.modify_bo_order(ExchOrderID="1100000017861430",LimitPriceForSL=330)
 
 #Note : You have pass atmarket=true while modifying stoploss price, Pass ExchorderId for the particular leg to modify.
 ```
 
 #### Basket Orders
 
 ```py
```

### Comparing `py5paisa-0.6.7/setup.py` & `py5paisa-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,10 +45,10 @@
     keywords='py5paisa',
     name='py5paisa',
     packages=find_packages(include=['py5paisa', 'py5paisa.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/5paisa/py5paisa',
-    version='0.6.7',
+    version='0.6.9',
     zip_safe=False,
 )
```


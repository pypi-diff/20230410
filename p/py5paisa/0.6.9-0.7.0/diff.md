# Comparing `tmp/py5paisa-0.6.9.tar.gz` & `tmp/py5paisa-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py5paisa-0.6.9.tar", last modified: Mon Apr 10 07:13:39 2023, max compression
+gzip compressed data, was "py5paisa-0.7.0.tar", last modified: Mon Apr 10 07:38:21 2023, max compression
```

## Comparing `py5paisa-0.6.9.tar` & `py5paisa-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.989379 py5paisa-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-10 07:13:30.000000 py5paisa-0.6.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-10 07:13:30.000000 py5paisa-0.6.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 07:13:30.000000 py5paisa-0.6.9/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-10 07:13:30.000000 py5paisa-0.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-04-10 07:13:39.989379 py5paisa-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-10 07:13:30.000000 py5paisa-0.6.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.985379 py5paisa-0.6.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.985379 py5paisa-0.6.9/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    48489 2023-04-10 07:13:30.000000 py5paisa-0.6.9/docs/images/5-paisa-img.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.985379 py5paisa-0.6.9/py5paisa/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    32425 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/py5paisa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-10 07:13:30.000000 py5paisa-0.6.9/py5paisa/urlconst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.989379 py5paisa-0.6.9/py5paisa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 07:13:39.000000 py5paisa-0.6.9/py5paisa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-10 07:13:39.989379 py5paisa-0.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-10 07:13:30.000000 py5paisa-0.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:13:39.989379 py5paisa-0.6.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 07:13:30.000000 py5paisa-0.6.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-10 07:13:30.000000 py5paisa-0.6.9/tests/test_py5paisa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.062077 py5paisa-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-10 07:38:12.000000 py5paisa-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-10 07:38:12.000000 py5paisa-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 07:38:12.000000 py5paisa-0.7.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-10 07:38:12.000000 py5paisa-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-04-10 07:38:21.062077 py5paisa-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-10 07:38:12.000000 py5paisa-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.058077 py5paisa-0.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.062077 py5paisa-0.7.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    48489 2023-04-10 07:38:12.000000 py5paisa-0.7.0/docs/images/5-paisa-img.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.062077 py5paisa-0.7.0/py5paisa/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32425 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/py5paisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/urlconst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.062077 py5paisa-0.7.0/py5paisa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-10 07:38:21.062077 py5paisa-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-10 07:38:12.000000 py5paisa-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.062077 py5paisa-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 07:38:12.000000 py5paisa-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-10 07:38:12.000000 py5paisa-0.7.0/tests/test_py5paisa.py
```

### Comparing `py5paisa-0.6.9/CONTRIBUTING.rst` & `py5paisa-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.9/PKG-INFO` & `py5paisa-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py5paisa
-Version: 0.6.9
+Version: 0.7.0
 Summary:  Python SDK for 5paisa APIs natively written in VB.NET
 Home-page: https://github.com/5paisa/py5paisa
 Author: 5paisa
 Author-email: coreteam@5paisa.com
 Keywords: py5paisa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `py5paisa-0.6.9/README.rst` & `py5paisa-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.9/docs/images/5-paisa-img.jpg` & `py5paisa-0.7.0/docs/images/5-paisa-img.jpg`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.9/py5paisa/auth.py` & `py5paisa-0.7.0/py5paisa/auth.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.9/py5paisa/const.py` & `py5paisa-0.7.0/py5paisa/const.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.9/py5paisa/order.py` & `py5paisa-0.7.0/py5paisa/order.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.9/py5paisa/py5paisa.py` & `py5paisa-0.7.0/py5paisa/py5paisa.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.9/py5paisa/strategy.py` & `py5paisa-0.7.0/py5paisa/strategy.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.6.9/py5paisa/urlconst.py` & `py5paisa-0.7.0/py5paisa/urlconst.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 LOGIN_ROUTE = f'{BaseUrl}V4/LoginRequestMobileNewbyEmail'
 
 MARGIN_ROUTE = f'{BaseUrl}V3/Margin'
 ORDER_BOOK_ROUTE = f'{BaseUrl}V2/OrderBook'
-HOLDINGS_ROUTE = f'{BaseUrl}V2/Holding'
+HOLDINGS_ROUTE = f'{BaseUrl}V3/Holding'
 POSITIONS_ROUTE = f'{BaseUrl}V1/NetPositionNetWise'
 
 ORDER_PLACEMENT_ROUTE = f'{BaseUrl}V1/PlaceOrderRequest'
 ORDER_MODIFY_ROUTE= f'{BaseUrl}V1/ModifyOrderRequest'
 ORDER_CANCEL_ROUTE= f'{BaseUrl}V1/CancelOrderRequest'
 ORDER_STATUS_ROUTE = f'{BaseUrl}V1/OrderStatus'
 TRADE_INFO_ROUTE = f'{BaseUrl}TradeInformation'
```

### Comparing `py5paisa-0.6.9/py5paisa.egg-info/PKG-INFO` & `py5paisa-0.7.0/py5paisa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py5paisa
-Version: 0.6.9
+Version: 0.7.0
 Summary:  Python SDK for 5paisa APIs natively written in VB.NET
 Home-page: https://github.com/5paisa/py5paisa
 Author: 5paisa
 Author-email: coreteam@5paisa.com
 Keywords: py5paisa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `py5paisa-0.6.9/setup.py` & `py5paisa-0.7.0/setup.py`

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
-    version='0.6.9',
+    version='0.7.0',
     zip_safe=False,
 )
```


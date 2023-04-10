# Comparing `tmp/xj_finance-1.0.9.tar.gz` & `tmp/xj_finance-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xj_finance-1.0.9.tar", last modified: Fri Sep 16 12:41:50 2022, max compression
+gzip compressed data, was "dist\xj_finance-1.1.1.tar", last modified: Mon Apr 10 05:04:18 2023, max compression
```

## Comparing `xj_finance-1.0.9.tar` & `xj_finance-1.1.1.tar`

### file list

```diff
@@ -1,45 +1,57 @@
-drwxrwxrwx   0        0        0        0 2022-09-16 12:41:50.589600 xj_finance-1.0.9/
--rw-rw-rw-   0        0        0     1990 2022-09-16 12:41:50.587600 xj_finance-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2022-08-24 12:42:59.000000 xj_finance-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2022-09-16 12:41:50.590602 xj_finance-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      912 2022-09-16 12:24:06.000000 xj_finance-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-16 12:41:50.171304 xj_finance-1.0.9/xj_finance/
--rw-rw-rw-   0        0        0        0 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/__init__.py
--rw-rw-rw-   0        0        0     2038 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/admin.py
-drwxrwxrwx   0        0        0        0 2022-09-16 12:41:50.309401 xj_finance-1.0.9/xj_finance/apis/
--rw-rw-rw-   0        0        0        0 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/apis/__init__.py
--rw-rw-rw-   0        0        0     3084 2022-08-28 08:41:22.000000 xj_finance-1.0.9/xj_finance/apis/finance_contact_book.py
--rw-rw-rw-   0        0        0     1012 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/apis/finance_currency.py
--rw-rw-rw-   0        0        0     4772 2022-08-28 08:41:22.000000 xj_finance-1.0.9/xj_finance/apis/finance_export.py
--rw-rw-rw-   0        0        0     1012 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/apis/finance_pay_mode.py
--rw-rw-rw-   0        0        0     1006 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/apis/finance_sand_box.py
--rw-rw-rw-   0        0        0     1549 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/apis/finance_statistic.py
--rw-rw-rw-   0        0        0     3694 2022-08-28 08:41:22.000000 xj_finance-1.0.9/xj_finance/apis/finance_transact.py
--rw-rw-rw-   0        0        0     2341 2022-08-28 08:41:22.000000 xj_finance-1.0.9/xj_finance/apis/finance_transacts.py
--rw-rw-rw-   0        0        0     2133 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/apis/middleware.py
--rw-rw-rw-   0        0        0     4180 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/apis/router.py
--rw-rw-rw-   0        0        0      208 2022-09-16 12:15:01.000000 xj_finance-1.0.9/xj_finance/apps.py
--rw-rw-rw-   0        0        0     6273 2022-09-06 09:05:22.000000 xj_finance-1.0.9/xj_finance/models.py
-drwxrwxrwx   0        0        0        0 2022-09-16 12:41:50.513552 xj_finance-1.0.9/xj_finance/services/
--rw-rw-rw-   0        0        0        0 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/services/__init__.py
--rw-rw-rw-   0        0        0     1296 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/services/finance_currency_service.py
--rw-rw-rw-   0        0        0      454 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/services/finance_list_service.py
--rw-rw-rw-   0        0        0      858 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/services/finance_pay_mode_service.py
--rw-rw-rw-   0        0        0      939 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/services/finance_sand_box_service.py
--rw-rw-rw-   0        0        0    11378 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/services/finance_service.py
--rw-rw-rw-   0        0        0     4787 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/services/finance_statistic_service.py
--rw-rw-rw-   0        0        0    23814 2022-08-28 08:41:22.000000 xj_finance-1.0.9/xj_finance/services/finance_transact_service.py
--rw-rw-rw-   0        0        0     6764 2022-08-28 08:41:22.000000 xj_finance-1.0.9/xj_finance/services/finance_transacts_service.py
--rw-rw-rw-   0        0        0       63 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/tests.py
--rw-rw-rw-   0        0        0     1857 2022-09-06 09:05:22.000000 xj_finance-1.0.9/xj_finance/urls.py
-drwxrwxrwx   0        0        0        0 2022-09-16 12:41:50.576592 xj_finance-1.0.9/xj_finance/utils/
--rw-rw-rw-   0        0        0        0 2022-08-28 08:41:22.000000 xj_finance-1.0.9/xj_finance/utils/__init__.py
--rw-rw-rw-   0        0        0     1350 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/utils/custom_response.py
--rw-rw-rw-   0        0        0     4634 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/utils/jt.py
--rw-rw-rw-   0        0        0     7314 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/utils/model_handle.py
--rw-rw-rw-   0        0        0     3661 2022-08-24 12:42:59.000000 xj_finance-1.0.9/xj_finance/views.py
-drwxrwxrwx   0        0        0        0 2022-09-16 12:41:50.208330 xj_finance-1.0.9/xj_finance.egg-info/
--rw-rw-rw-   0        0        0     1990 2022-09-16 12:41:49.000000 xj_finance-1.0.9/xj_finance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1198 2022-09-16 12:41:50.000000 xj_finance-1.0.9/xj_finance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-16 12:41:49.000000 xj_finance-1.0.9/xj_finance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-09-16 12:41:49.000000 xj_finance-1.0.9/xj_finance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/
+-rw-rw-rw-   0        0        0     1990 2023-04-10 05:04:18.000000 xj_finance-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2022-08-16 02:23:15.000000 xj_finance-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:04:18.000000 xj_finance-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-04-10 02:12:25.000000 xj_finance-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/__init__.py
+-rw-rw-rw-   0        0        0     3227 2023-03-07 08:56:37.000000 xj_finance-1.1.1/xj_finance/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/apis/__init__.py
+-rw-rw-rw-   0        0        0     4422 2023-04-07 01:43:10.000000 xj_finance-1.1.1/xj_finance/apis/finance_apis.py
+-rw-rw-rw-   0        0        0     2233 2023-04-06 05:13:05.000000 xj_finance-1.1.1/xj_finance/apis/finance_balance.py
+-rw-rw-rw-   0        0        0     3084 2022-08-26 08:45:38.000000 xj_finance-1.1.1/xj_finance/apis/finance_contact_book.py
+-rw-rw-rw-   0        0        0     1012 2022-08-26 02:55:22.000000 xj_finance-1.1.1/xj_finance/apis/finance_currency.py
+-rw-rw-rw-   0        0        0     4772 2022-08-26 02:40:58.000000 xj_finance-1.1.1/xj_finance/apis/finance_export.py
+-rw-rw-rw-   0        0        0     1430 2023-01-04 01:15:24.000000 xj_finance-1.1.1/xj_finance/apis/finance_pay_mode.py
+-rw-rw-rw-   0        0        0     1006 2022-08-24 07:41:31.000000 xj_finance-1.1.1/xj_finance/apis/finance_sand_box.py
+-rw-rw-rw-   0        0        0     1549 2022-08-24 09:06:59.000000 xj_finance-1.1.1/xj_finance/apis/finance_statistic.py
+-rw-rw-rw-   0        0        0     1021 2023-01-18 07:58:44.000000 xj_finance-1.1.1/xj_finance/apis/finance_status_code.py
+-rw-rw-rw-   0        0        0     5419 2023-04-06 08:10:44.000000 xj_finance-1.1.1/xj_finance/apis/finance_transact.py
+-rw-rw-rw-   0        0        0     4661 2023-04-07 08:45:23.000000 xj_finance-1.1.1/xj_finance/apis/finance_transacts.py
+-rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/apis/middleware.py
+-rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_finance-1.1.1/xj_finance/apis/router.py
+-rw-rw-rw-   0        0        0      208 2022-09-19 06:40:42.000000 xj_finance-1.1.1/xj_finance/apps.py
+-rw-rw-rw-   0        0        0     9325 2023-04-06 08:07:37.000000 xj_finance-1.1.1/xj_finance/models.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance/services/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/services/__init__.py
+-rw-rw-rw-   0        0        0     1296 2022-08-24 02:05:06.000000 xj_finance-1.1.1/xj_finance/services/finance_currency_service.py
+-rw-rw-rw-   0        0        0      454 2022-08-23 09:51:33.000000 xj_finance-1.1.1/xj_finance/services/finance_list_service.py
+-rw-rw-rw-   0        0        0     1526 2023-01-04 01:25:29.000000 xj_finance-1.1.1/xj_finance/services/finance_pay_mode_service.py
+-rw-rw-rw-   0        0        0      982 2023-03-07 08:57:01.000000 xj_finance-1.1.1/xj_finance/services/finance_sand_box_service.py
+-rw-rw-rw-   0        0        0    15239 2023-04-01 16:10:40.000000 xj_finance-1.1.1/xj_finance/services/finance_service v1.py
+-rw-rw-rw-   0        0        0     9753 2023-04-07 08:55:14.000000 xj_finance-1.1.1/xj_finance/services/finance_service.py
+-rw-rw-rw-   0        0        0     4787 2022-08-24 09:08:36.000000 xj_finance-1.1.1/xj_finance/services/finance_statistic_service.py
+-rw-rw-rw-   0        0        0      934 2023-01-18 08:16:12.000000 xj_finance-1.1.1/xj_finance/services/finance_status_code_service.py
+-rw-rw-rw-   0        0        0    25531 2022-10-25 08:56:34.000000 xj_finance-1.1.1/xj_finance/services/finance_transact_service v1.py
+-rw-rw-rw-   0        0        0    37592 2023-03-30 05:27:34.000000 xj_finance-1.1.1/xj_finance/services/finance_transact_service v2.py
+-rw-rw-rw-   0        0        0    29283 2023-04-07 09:07:47.000000 xj_finance-1.1.1/xj_finance/services/finance_transact_service.py
+-rw-rw-rw-   0        0        0    31989 2023-03-30 07:10:48.000000 xj_finance-1.1.1/xj_finance/services/finance_transacts_service v1.py
+-rw-rw-rw-   0        0        0    16760 2023-04-07 08:48:42.000000 xj_finance-1.1.1/xj_finance/services/finance_transacts_service.py
+-rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/tests.py
+-rw-rw-rw-   0        0        0     2509 2023-04-07 09:10:32.000000 xj_finance-1.1.1/xj_finance/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/utils/__init__.py
+-rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_finance-1.1.1/xj_finance/utils/custom_response.py
+-rw-rw-rw-   0        0        0    10868 2023-03-01 02:16:37.000000 xj_finance-1.1.1/xj_finance/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_finance-1.1.1/xj_finance/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_finance-1.1.1/xj_finance/utils/j_dict.py
+-rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_finance-1.1.1/xj_finance/utils/jt.py
+-rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_finance-1.1.1/xj_finance/utils/model_handle.py
+-rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_finance-1.1.1/xj_finance/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/views.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance.egg-info/
+-rw-rw-rw-   0        0        0     1990 2023-04-10 05:04:17.000000 xj_finance-1.1.1/xj_finance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1672 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:04:17.000000 xj_finance-1.1.1/xj_finance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-10 05:04:17.000000 xj_finance-1.1.1/xj_finance.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `xj_finance-1.0.9/PKG-INFO` & `xj_finance-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_finance
-Version: 1.0.9
+Version: 1.1.1
 Summary: 资金模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: ['莫小瑛', '高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
```

### Comparing `xj_finance-1.0.9/README.md` & `xj_finance-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/setup.py` & `xj_finance-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_finance',  # 模块名称
-    version='1.0.9',  # 模块版本
+    version='1.1.1',  # 模块版本
     description='资金模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='赵向明',  # 作者
     author_email='sieyoo@163.com',  # 作者邮箱
     maintainer=["莫小瑛", "高栋天"],  # 维护者
     maintainer_email="angelvy@foxmail.com",  # 维护者的邮箱地址
```

### Comparing `xj_finance-1.0.9/xj_finance/apis/finance_contact_book.py` & `xj_finance-1.1.1/xj_finance/apis/finance_contact_book.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/apis/finance_currency.py` & `xj_finance-1.1.1/xj_finance/apis/finance_currency.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/apis/finance_export.py` & `xj_finance-1.1.1/xj_finance/apis/finance_export.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/apis/finance_pay_mode.py` & `xj_finance-1.1.1/xj_finance/apis/finance_pay_mode.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,7 +25,18 @@
         params = parse_data(request)
         if not params:
             return util_response(err=6046, msg='至少需要一个请求参数')
         data, err_txt = FinancePayModeService.post(params=params)
         if err_txt is None:
             return util_response(data=data)
         return util_response(err=47767, msg=err_txt)
+
+        # 支付方式修改
+
+    def put(self, request, *args, **kwargs):
+        params = parse_data(request)
+        if not params:
+            return util_response(err=6046, msg='至少需要一个请求参数')
+        data, err_txt = FinancePayModeService.put(params=params)
+        if err_txt is None:
+            return util_response(data=data)
+        return util_response(err=47767, msg=err_txt)
```

### Comparing `xj_finance-1.0.9/xj_finance/apis/finance_sand_box.py` & `xj_finance-1.1.1/xj_finance/apis/finance_sand_box.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/apis/finance_statistic.py` & `xj_finance-1.1.1/xj_finance/apis/finance_statistic.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/apis/middleware.py` & `xj_finance-1.1.1/xj_finance/apis/middleware.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/apis/router.py` & `xj_finance-1.1.1/xj_finance/apis/router.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/services/finance_currency_service.py` & `xj_finance-1.1.1/xj_finance/services/finance_currency_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/services/finance_sand_box_service.py` & `xj_finance-1.1.1/xj_finance/services/finance_sand_box_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class FinanceSandBoxService:
 
     @staticmethod
     def get():
         currencies = SandBox.objects.all().annotate(value=F('sand_box_name'), sand_box=F('sand_box_name'))
 
-        return list(currencies.values('value', 'sand_box', 'sand_box_name'))
+        return list(currencies.values('value', 'sand_box', 'sand_box_name', 'sand_box_label', 'description', 'config'))
 
     @staticmethod
     def post(params):
         sand_box_name = params.get('sand_box_name', '')
         if sand_box_name:
             sand_box_set = SandBox.objects.filter(sand_box_name=sand_box_name).first()
             if sand_box_set is not None:
```

### Comparing `xj_finance-1.0.9/xj_finance/services/finance_service.py` & `xj_finance-1.1.1/xj_finance/services/finance_service v1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,98 +1,119 @@
 import time
 import os
 import datetime
 
 from django.db.models import Q
 from django.db.models import F
-from rest_framework.response import Response
-
-from xj_user.models import *
-from xj_finance.models import *
+from django.forms import model_to_dict
+from xj_user.services.user_platform_service import UserPlatformService
+from ..models import *
+from ..models import StatusCode
 
 from decimal import Decimal
+from ..utils.custom_tool import format_params_handle
 
 
 class FinanceService:
 
     def __init__(self):
         pass
 
     # 检查账号余额是否正确
     @staticmethod
-    def check_balance(account_id='', platform='', currency='', sand_box=''):
-        print("-" * 30, os.path.basename(__file__), "-" * 30)
+    def check_balance(account_id='', platform='', platform_id=None, currency='', sand_box=''):
+        # print("-" * 30, os.path.basename(__file__), "-" * 30)
         # print("check_balance account_id, platform, currency:", account_id, platform, currency, )
 
         # ========== 一、内容的类型准确性检查 ==========
         account_set = BaseInfo.objects.filter(id=account_id).first()
         if not account_set:
-            print('check_balance: account_id不存在', account_id, account_set)
+            # print('check_balance: account_id不存在', account_id, account_set)
             return {'err': 7001, 'msg': 'check_balance: account_id不存在:' + str(account_id)}
 
-        platform_set = Platform.objects.filter(platform_name=platform).first()
-        if not platform_set:
-            print('check_balance: platform不存在', platform, platform_set)
-            return {'err': 7002, 'msg': 'check_balance: platform不存在' + str(platform)}
-
+        # platform_set = Platform.objects.filter(platform_name=platform).first()
+        if platform:
+            platform_info, error = UserPlatformService.get_platform_info(platform_name=platform)
+            if error:
+                # print('check_balance: platform不存在', platform, platform_info)
+                return {'err': 7002, 'msg': 'check_balance: platform不存在' + str(platform)}
+            platform_id = platform_info.get('platform_id')
+        elif platform_id:
+            platform_id = platform_id
         currency_set = Currency.objects.filter(currency=currency).first()
         if not currency_set:
-            print('check_balance: currency不存在', currency, currency_set)
+            # print('check_balance: currency不存在', currency, currency_set)
             return {'err': 7003, 'msg': 'check_balance: currency不存在' + str(currency)}
 
         sand_box = sand_box if sand_box else None
         sand_box_set = None
         if sand_box:
             sand_box_set = SandBox.objects.filter(sand_box_name=sand_box).first()
         if sand_box and not sand_box_set:
-            print('check_balance: sand_box不存在', sand_box, sand_box_set)
+            # print('check_balance: sand_box不存在', sand_box, sand_box_set)
             return {'err': 7004, 'msg': 'check_balance: sand_box不存在' + str(sand_box)}
 
         # ========== 二、相关前置业务逻辑处理 ==========
         transact_set = Transact.objects.filter(
             Q(account_id=account_id) &
-            Q(platform__platform_name=platform) &
+            Q(platform_id=platform_id) &
             Q(currency__currency=currency)
         )
 
         if sand_box is None:
             transact_set = transact_set.filter(Q(sand_box__sand_box_name__isnull=True))
         else:
             transact_set = transact_set.filter(Q(sand_box__sand_box_name=sand_box))
 
         transact_set = transact_set.order_by('transact_time')
-        print(">>> transact_set: ", transact_set)
+        # print(">>> transact_set: ", transact_set)
 
         for i, it in enumerate(transact_set):
             is_inside_pay = True if str(it.pay_mode).upper() == 'BALANCE' else False
             # print(">>>>>> is_inside_pay:", is_inside_pay)
             income = it.income if it.income else Decimal(0.0)
             outgo = it.outgo if it.outgo else Decimal(0.0)
             # outgo = it.outgo if it.outgo and is_inside_pay else Decimal(0.0)
 
-            print('check_balance: for:', i, ': ', income, -outgo, ' = ', it.balance, )
-            print('check_balance: for:', i, type(income), type(outgo), type(it.balance))
+            # print('check_balance: for:', i, ': ', income, -outgo, ' = ', it.balance, )
+            # print('check_balance: for:', i, type(income), type(outgo), type(it.balance))
+            if is_inside_pay:
+                if i == 0:
+                    balance = income - outgo
+                    # print(">>>>>> balance: ", balance)  # -10000.00000000
+                    # print(">>>>>> it.balance: ", it.balance)  # 0E-8   0.00000000
+                    if balance != it.balance:
+                        # print('check_balance: 首条余额不匹配，自动修正:', i, income, -outgo, balance, it.balance)
+                        it.balance = balance
+                        it.save()
+                    continue
 
-            if i == 0:
-                balance = income - outgo
-                print(">>>>>> balance: ", balance)  # -10000.00000000
-                print(">>>>>> it.balance: ", it.balance)  # 0E-8   0.00000000
+                last = transact_set[i - 1]
+                balance = last.balance + income - outgo
                 if balance != it.balance:
-                    print('check_balance: 首条余额不匹配，自动修正:', i, income, -outgo, balance, it.balance)
+                    # print('check_balance: 余额不匹配，自动修正:', i, last.balance, income, -outgo, balance, it.balance)
                     it.balance = balance
                     it.save()
-                continue
+        transact_set_new = Transact.objects.filter(
+            Q(account_id=account_id) &
+            Q(platform_id=platform_id) &
+            Q(currency__currency=currency)
+        )
+        if sand_box is None:
+            transact_set_new = transact_set_new.filter(Q(sand_box__sand_box_name__isnull=True))
+        else:
+            transact_set_new = transact_set_new.filter(Q(sand_box__sand_box_name=sand_box))
+        transact_set_new = transact_set_new.order_by('-transact_time').first()
+        if transact_set_new:
+            transact_set_new = model_to_dict(transact_set_new)
+            return {"balance": transact_set_new['balance']}
+
+        return {"balance": 0}
 
-            last = transact_set[i - 1]
-            balance = last.balance + income - outgo
-            if balance != it.balance:
-                print('check_balance: 余额不匹配，自动修正:', i, last.balance, income, -outgo, balance, it.balance)
-                it.balance = balance
-                it.save()
-        return True
+        # return True
 
     # 生成交易号：2位数（当前年份后2位数字）+8位数（当前时间戳去头2位）+6位数（用户名 经过hash crc16生成的 4位十六进制 转成5位数 然后头为补0）
     @staticmethod
     def make_unicode(salt=''):
         # 当前时间戳
         date_time = time.localtime(time.time())
         # 截取第3位到第4位
@@ -138,18 +159,26 @@
         """
 
         query_dict = {}
 
         # 搜索平台
         platform_name = params.get('platform', '')
         if platform_name:
-            platform_set = Platform.objects.filter(Q(platform_name=platform_name)).first()
-            if not platform_set:
+            platform_set, err = UserPlatformService.get_platform_info(platform_name=platform_name)
+            if err:
                 return {'err': 3001, 'msg': 'platform不存在', }
-            query_dict['platform__platform_name'] = platform_name
+            query_dict['platform_id'] = platform_set['platform_id']
+
+        finance_status_code = params.get('finance_status_code', '')
+        if finance_status_code:
+            sand_box_set = StatusCode.objects.filter(finance_status_code=finance_status_code).first().id
+            # print("1",sand_box_set)
+            if not sand_box_set:
+                return {'err': 3001, 'msg': 'finance_status_code不存在', }
+            query_dict['finance_status_code'] = sand_box_set
 
         # 搜索币种
         currency = params.get('currency', '')
         if currency:
             currency_set = Currency.objects.filter(Q(currency=currency)).first()
             if not currency_set:
                 return {'err': 3002, 'msg': 'currency不存在', }
@@ -159,39 +188,59 @@
         pay_mode = params.get('pay_mode', '')
         if pay_mode:
             pay_mode_set = PayMode.objects.filter(Q(pay_mode=pay_mode)).first()
             if not pay_mode_set:
                 return {'err': 3003, 'msg': 'pay_mode不存在', }
             query_dict['pay_mode__pay_mode'] = pay_mode
 
+        sand_box_list = params.get('sand_box_list', '')
+        if sand_box_list:
+            # print(">>> sand_box_list:", type(sand_box_list), sand_box_list)
+            sand_box_list = sand_box_list.split(',')
+            sand_box_set = SandBox.objects.filter(Q(sand_box_name__in=sand_box_list)).first()
+            if not sand_box_set:
+                return {'err': 3004, 'msg': 'sand_box不存在', }
+            query_dict['sand_box__sand_box_name__in'] = sand_box_list
+
+        # print(sand_box_list)
+
         # 搜索沙盒
         sand_box = params.get('sand_box', '')
         # 如果沙盒为空则搜索全部内容，但沙盒为假值或者0时，则只显示非沙盒
-        sand_box = False if sand_box.lower() == 'false' or sand_box == '0' else sand_box
-        sand_box = True if sand_box.lower() == 'false' or sand_box == '0' else sand_box
+        # sand_box = False if sand_box.lower() == 'false' or sand_box == '0' else sand_box
+        # sand_box = True if sand_box.lower() == 'false' or sand_box == '0' else sand_box
+        # print(">>>sand_box", sand_box)
         # 显示指定沙盒
-        if sand_box and sand_box:
+        # if sand_box and sand_box:
+        if sand_box:
             sand_box_set = SandBox.objects.filter(Q(sand_box_name=sand_box)).first()
             if sand_box and not sand_box_set:
                 return {'err': 3004, 'msg': 'sand_box不存在', }
             query_dict['sand_box__sand_box_name'] = sand_box
-        # 显示非沙盒（即真实交易）
-        if sand_box is False:
+        elif not sand_box and not sand_box_list:
+            # 显示非沙盒（即真实交易）
+            # if sand_box is False:
+
             query_dict['sand_box__sand_box_name__isnull'] = True
 
         # 模糊搜索对方账号
         their_account_name = params.get('their_account_name', '')
         if their_account_name:
             query_dict['their_account__full_name__icontains'] = their_account_name
 
         # 模糊搜索摘要search_word
         search_word = params.get('search_word', '')
         if search_word:
             query_dict['summary__icontains'] = search_word
 
+        # 精确匹配沙盒状态
+        sand_box_status_code = params.get('sand_box_status_code', '')
+        if sand_box_status_code:
+            query_dict['sand_box_status_code'] = sand_box_status_code
+
         return {'err': 0, 'msg': 'OK', 'query_dict': query_dict, }
 
     #
     # # 过滤筛选
     # @staticmethod
     # def transact_filter(params={}, account_id=None, ):
     #     """
@@ -264,7 +313,37 @@
     #     search_word = params.get('search_word', '')
     #     if search_word:
     #         transacts = transacts.filter(Q(summary__icontains=search_word))
     #
     #     transacts = transacts.order_by('-transact_time')
     #
     #     return {'err': 0, 'msg': 'OK', 'query_set': transacts, }
+    @staticmethod
+    def balance_validation(request_params):
+        # transact_set = Transact.objects.filter()
+        account_id = request_params.get("account_id")
+        platform_id = request_params.get("platform_id")
+
+        transact_set = Transact.objects.filter(
+            Q(account_id=account_id) &
+            Q(platform_id=platform_id) &
+            Q(sand_box_id__isnull=True)
+        ).order_by('id')
+
+        transact_set.filter(Q(pay_mode__pay_mode__in=['TRANSFER', 'WECHAT'])).update(balance=0)
+        first_record = transact_set.exclude(pay_mode__pay_mode__in=['TRANSFER', 'WECHAT']).first()
+        first_record = model_to_dict(first_record)
+        if first_record['income'] > first_record['outgo']:
+            balance = first_record['income']
+        else:
+            balance = first_record['outgo']
+        Transact.objects.filter(id=first_record['id']).update(balance=balance)
+        record = transact_set.exclude(pay_mode__pay_mode__in=['TRANSFER', 'WECHAT']).values("id", "income", "outgo")
+        for i in list(record):
+            if i['income'] > i['outgo']:
+                balance += i['income']
+            else:
+                balance -= i['outgo']
+            Transact.objects.filter(id=i['id']).update(balance=balance)
+            # print(balance)
+        return None, None
+        # transact_set.values("income","outgo")
```

### Comparing `xj_finance-1.0.9/xj_finance/services/finance_statistic_service.py` & `xj_finance-1.1.1/xj_finance/services/finance_statistic_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/services/finance_transact_service.py` & `xj_finance-1.1.1/xj_finance/services/finance_transact_service v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pytz
 from django.db.models import Q
 from django.utils import timezone
 from django.utils.datetime_safe import datetime
 from rest_framework import serializers
 
 from xj_user.models import BaseInfo, Platform
+from xj_user.services.user_platform_service import UserPlatformService
 
 from ..utils.jt import Jt
 from ..models import Transact, Currency, PayMode, SandBox
 from .finance_service import FinanceService
 
 
 # 声明用户序列化
@@ -37,15 +38,15 @@
     outgo = serializers.SerializerMethodField()
     balance = serializers.SerializerMethodField()
     sand_box = serializers.SerializerMethodField()
     transact_time = serializers.SerializerMethodField()
     transact_timestamp = serializers.SerializerMethodField()
 
     # 自定义外键字段
-    platform = serializers.ReadOnlyField(source='platform.platform_name')
+    # platform = serializers.ReadOnlyField(source='platform.platform_name')
     account_name = serializers.ReadOnlyField(source='account.full_name')
     their_account_name = serializers.ReadOnlyField(source='their_account.full_name')
     pay_mode = serializers.ReadOnlyField(source='pay_mode.pay_mode')
     currency = serializers.ReadOnlyField(source='currency.currency')
 
     def create(self, validated_data):
         """
@@ -61,16 +62,16 @@
             'transact_id',
             'transact_time',
             'transact_timestamp',
             'account_id',
             'account_name',
             'their_account_id',
             'their_account_name',
-            'platform',
-            'platform_order_id',
+            'platform_id',
+            'order_no',
             'opposite_account',
             'summary',
             'currency',
             'amount',
             'lend',
             'income',
             'outgo',
@@ -144,18 +145,25 @@
         # output = _("Welcome to my site.")
 
         return serializer.data, None
 
         # POST方法，如果无transact_id则是新增，否则为修改
 
     @staticmethod
+    def finance_transact_detailed(transact_id):
+        transact = Transact.objects.filter(transact_id=transact_id).first()
+        if not transact:
+            return None, "不存在"
+        return transact, None
+
+    @staticmethod
     def post(param):
         # param = self.params = request.query_params  # 返回QueryDict类型
         item = serializer_params = {}  # 将要写入的某条数据
-        print(param)
+        # print(param)
         # print(">>> self.params:", self.params)
 
         # ========== 一、验证权限 ==========
 
         # token = self.request.META.get('HTTP_AUTHORIZATION', '')
         # if not token:
         #     return Response({'err': 4001, 'msg': '缺少Token', })
@@ -183,85 +191,99 @@
             return None, '缺少pay_mode'
         if not param.get('summary', ''):
             # return Response({'err': 3306, 'msg': '缺少summary', })
             return None, '缺少summary'
 
         # ========== 三、内容的类型准确性检查 ==========
         # 判断无transact_id为新建，否则为修改
-        is_create = 'transact_id' not in param or param['transact_id'] is ''
-
+        is_create = True
+        transact_has_id = Transact.objects.filter(transact_id=param.get('transact_id', ''))
+        if transact_has_id:
+            is_create = False
+        # is_create = 'transact_id' not in param or param['transact_id'] is ''
         # 检查是否有该id
         if not is_create and param.get('id', ''):
             has_id = Transact.objects.filter(id=param.get('id', '')).count() > 0
             if not has_id:
                 # return Response({'err': 1001, 'msg': 'id不存在', })
                 return None, 'id不存在'
-
         # 判断平台是否存在
         platform_name = param.get('platform', '')
         # item['platform'] = Platform.objects.filter(platform_name=platform_name).first().platform_id
-        item['platform'] = Platform.objects.filter(platform_name=platform_name).first()
-        print("> platform_name:", platform_name, item['platform'], type(item['platform']))
-        if not item['platform']:
+        # item['platform'] = Platform.objects.filter(platform_name=platform_name).first()
+        platform_info, err = UserPlatformService.get_platform_info(platform_name=platform_name)
+        # print("> platform_name:", platform_name, platform_info)
+        if err:
             # return Response({'err': 1002, 'msg': '平台不存在: ' + platform_name, })
             return None, '平台不存在: ' + platform_name
-
+        item['platform_id'] = platform_info.get('platform_id')
         # 发起交易的账号ID，如果没有则默认自己
         # account_id = int(param.get('account_id', '') or user_id)
         account_id = int(param.get('account_id', ''))
         item['account'] = BaseInfo.objects.filter(id=account_id).first()
         # print("> account:", account_id, item['account'], )
         if not item['account']:
             # return Response({'err': 1003, 'msg': '用户account_id不存在', })
             return None, '用户account_id不存在'
-
         # 承受交易的账号，要从数据库判断是否存在
         their_account_id = param.get('their_account_id', '')
         # print("> their_account_id:", their_account_id, )
         # 如果有id需要判断是否为数字
-        if their_account_id and not their_account_id.isdecimal():
-            # return Response({'err': 1004, 'msg': '用户their_account_id必须是数字', })
-            return None, '用户their_account_id必须是数字'
+        # if their_account_id and not their_account_id.isdecimal():
+        #     # return Response({'err': 1004, 'msg': '用户their_account_id必须是数字', })
+        #     return None, '用户their_account_id必须是数字'
         if their_account_id:
             their_account_id = int(their_account_id)
         if their_account_id:
             item['their_account'] = BaseInfo.objects.filter(id=their_account_id).first()
             # print("> their_account_id:", their_account_id, item['their_account'])
             if not item['their_account']:
                 # return Response({'err': 1004, 'msg': '用户their_account_id不存在', })
                 return None, '用户their_account_id不存在'
-
         # 边界检查，自己不能和自己交易
         if account_id == their_account_id:
             # return Response({'err': 1005, 'msg': '自己不能和自己交易', })
             return None, '自己不能和自己交易'
 
         # 生成发起交易的用户名 todo 要不用金额会不会更安全？怎么处理重复的可能性
         username = item['account'].user_name
         # print(">>> username:", username)
-
         # 生成唯一且不可重复的交易ID，且具有校验作用
-        transact_id = param['transact_id'] if not is_create else FinanceService.make_unicode(username)
+        # transact_id = param['transact_id'] if not is_create else FinanceService.make_unicode(username)
+        if is_create and param.get('transact_id', ''):
+
+            transact_id = param.get('transact_id', '')
+        elif is_create and not param.get('transact_id', ''):
+            transact_id = FinanceService.make_unicode(username)
+        else:
+            transact_id = param.get('transact_id', '')
+
         item['transact_id'] = transact_id
+
         # print(">>> transact_id:", transact_id)
         if is_create and Transact.objects.filter(transact_id=transact_id).values().count():
             # return Response({'err': 1007, 'msg': '新增时发现复重交易ID，请检查是否有重复记录: ' + transact_id, })
             return None, '新增时发现复重交易ID，请检查是否有重复记录: ' + transact_id
         if not is_create and Transact.objects.filter(transact_id=transact_id).values().count() == 0:
             # return Response({'err': 1008, 'msg': '修改信息的交易ID不存在: ' + transact_id, })
             return None, '修改信息的交易ID不存在: ' + transact_id
 
+        tz = pytz.timezone('Asia/Shanghai')
+        # 返回datetime格式的时间
+        now_time = timezone.now().astimezone(tz=tz).strftime("%Y-%m-%d %H:%M:%S")
+        now = datetime.strptime(now_time, '%Y-%m-%d %H:%M:%S')
         # 如果没有时间则生成交易时间
         # transact_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
         transact_time = param.get('transact_time', '')
-        print(">>> transact_time:", transact_time, )
+        # print(">>> transact_time:", transact_time, )
+        # if transact_time else timezone.localtime() if is_create TODO USE_TZ = False 时会报错 如果USE_TZ设置为True时，Django会使用系统默认设置的时区，即America/Chicago，此时的TIME_ZONE不管有没有设置都不起作用。
         item['transact_time'] = datetime.strptime(transact_time, '%Y-%m-%d %H:%M:%S') \
-            if transact_time else timezone.localtime() if is_create \
+            if transact_time else now if is_create \
             else Transact.objects.filter(transact_id=transact_id).first().transact_time
-        print(">>> transact_time:", transact_time, item['transact_time'], type(item['transact_time']))
+        # print(">>> transact_time:", transact_time, item['transact_time'], type(item['transact_time']))
         if not item['transact_time']:
             # return Response({'err': 1006, 'msg': '交易时间格式不正确', })
             return None, '交易时间格式不正确'
 
         # 边界检查：币种是否存在
         currency = param.get('currency', '')
         item['currency_set'] = Currency.objects.filter(currency=currency).first()
@@ -302,52 +324,55 @@
         if sand_box_name:
             item['sand_box_set'] = SandBox.objects.filter(sand_box_name=sand_box_name).first()
             # print(">>> sand_box:", sand_box_name, item['sand_box_set'])
             if item['sand_box_set'] is None:
                 # return Response({'err': 1011, 'msg': 'sand_box不存在', })
                 return None, 'sand_box不存在'
             item['sand_box'] = item['sand_box_set'].id
-        print(">>> sand_box_name: ", sand_box_name)
+        # print(">>> sand_box_name: ", sand_box_name)
         # print(">>> item['sand_box']: ", item['sand_box'])
 
         # 查余额 ---------------------------------------------------------------------
         balance_set = Transact.objects.filter(
             Q(account_id=account_id) &
             Q(currency_id=item['currency']) &
+            Q(platform_id=item['platform_id']) &
             Q(transact_time__lt=item['transact_time']) &
             ~Q(transact_id=item['transact_id'])
         )
-
         # 如果有沙盒。
         if sand_box_name:
             balance_set = balance_set.filter(Q(sand_box_id=item['sand_box']))
         else:
             balance_set = balance_set.filter(Q(sand_box_id=None))
 
         balance_set = balance_set.order_by('-transact_time').values().first()
         print(">>> balance_set:", balance_set)
         # print(">>> balance_set['balance'] ", balance_set['balance'])
         last_balance = balance_set['balance'] if balance_set is not None else Decimal(0.0)
-        print(">>> last_balance:", last_balance)
+        # print(">>> last_balance:", last_balance)
 
         # getcontext().rounding = "ROUND_HALF_UP"  # 真正四舍五入
         # getcontext().prec = 2  # //保留两位小数 打开这个后有时候会变成整数，为什么？
         # 如果是余额支付则内部交易，否则是第三方支付，如微信、支付宝等
         # is_inside_pay = True if pay_mode.upper() == 'BALANCE' else False
         # print(">>> is_inside_pay:", is_inside_pay)
         # balance = last_balance + income - (outgo if is_inside_pay else Decimal(0.0))
-        balance = last_balance + income - outgo
-        print(">>> balance:", balance)
-        item['balance'] = balance
+
+        item['balance'] = last_balance
+        if pay_mode == "BALANCE":
+            balance = last_balance + income - outgo
+            # print(">>> balance:", balance)
+            item['balance'] = balance
         # if balance < 0:
         #     return Response({'err': 1014, 'msg': '余额不足，待扣金额为'+str(amount)+'，当前余额为'+str(last_balance)+',差额'+str(balance) })
 
         # 平台订单号是可以允许重复的，如果没有平台订单号则输入交易号
-        platform_order_id = int(param.get('platform_order_id', transact_id))  # 如果没有平台订单号则填交易号
-        item['platform_order_id'] = platform_order_id
+        order_no = int(param.get('order_no', transact_id))  # 如果没有平台订单号则填交易号
+        item['order_no'] = order_no
 
         # 对方科目
         opposite_account = param.get('opposite_account', '')
         item['opposite_account'] = opposite_account
 
         # 摘要
         summary = param.get('summary', '')
@@ -370,51 +395,53 @@
         item['images'] = images
 
         # ========== 四、相关前置业务逻辑处理 ==========
 
         # 在新建订单时：如果平台订单号重复，金额不能重复，收方和支出方不能重复，金额也不能重复。
         if is_create:
             repeat_order_set = Transact.objects.filter(
-                Q(platform_order_id=platform_order_id) &
+                Q(order_no=order_no) &
                 Q(account_id=account_id) &
                 (Q(income=income) | Q(outgo=outgo))
             )
             # 单独判断，当有对方账号ID时才判断，因为在设计上对方账号是可以自动生成的
             if their_account_id:
                 repeat_order_set.filter(Q(their_account_id=their_account_id))
             if repeat_order_set.count() > 0:
-                # return Response({'err': 1015, 'msg': '重复的交易订单号：' + str(platform_order_id), })
-                return None, '重复的交易订单号：' + str(platform_order_id)
-
+                # return Response({'err': 1015, 'msg': '重复的交易订单号：' + str(order_no), })
+                return None, '重复的交易订单号：' + str(order_no)
         # --------------------------------------------------------------------------------------
+
         if not param.get('their_account_id', '') and not param.get('their_account_name', ''):
             # return Response({'err': 1016, 'msg': 'their_account_id或their_account_name 必填', })
             return None, 'their_account_id或their_account_name 必填'
         # 没有对方账户ID时从对方账户名创建一个账户
         # 如果无their_account_id、有their_account_name，则用their_account_name生成一个their_account_id
+        # TODO 貌似该功能不能使用 作废
         if not param.get('their_account_id', '') and param.get('their_account_name', ''):
             their_account_name = param['their_account_name']
-            platform_id = BaseInfo.objects.get(id=account_id).platform_id
-
+            #     platform_id = BaseInfo.objects.get(id=account_id).platform_id
             new_user_param = {
-                "platform_id": platform_id,
+                # "platform_id": platform_id,
                 "full_name": their_account_name,
-                "platform_uid": str(int(time.time())) + FinanceTransactService.random_four_int(),  # 这样写好吗？
+                # "platform_uid": str(int(time.time())) + FinanceTransactService.random_four_int(),  # 这样写好吗？
             }
-            # 增加一个用户
-            user_serializer = UserSerializer(data=new_user_param, context={})
-            print(">>> user_serializer ", user_serializer)
-            if not user_serializer.is_valid():
-                # return Response({'err': 1017, 'msg': user_serializer.errors, })
-                return None, user_serializer.errors
-            user_serializer.validated_data['platform_id'] = platform_id
-            print(">>> user_serializer.validated_data['platform_id']", user_serializer.validated_data['platform_id'])
-            user_serializer.save()
-            # 这是什么写法？传递引用了两次呢
-            item['their_account_id'] = BaseInfo.objects.get(platform_uid=new_user_param['platform_uid']).id
+            new_user = BaseInfo.objects.create(**new_user_param)
+            #     # 增加一个用户
+            #     user_serializer = UserSerializer(data=new_user_param, context={})
+            #     # print(">>> user_serializer ", user_serializer)
+            #     if not user_serializer.is_valid():
+            #         # return Response({'err': 1017, 'msg': user_serializer.errors, })
+            #         return None, user_serializer.errors
+            #     user_serializer.validated_data['platform_id'] = platform_id
+            #     # print(">>> user_serializer.validated_data['platform_id']", user_serializer.validated_data['platform_id'])
+            #     user_serializer.save()
+            #     # 这是什么写法？传递引用了两次呢
+            #     item['their_account_id'] = BaseInfo.objects.get(platform_uid=new_user_param['platform_uid']).id
+            item['their_account_id'] = new_user.id
             item['their_account'] = BaseInfo.objects.get(id=item['their_account_id'])
         # -------------------------------------------------------------------------------------
 
         # 如果有id，则是修改数据
         if is_create:
             response = FinanceTransactService.create(item)
         else:
@@ -427,21 +454,21 @@
     def create(item):
         # print(">>> create:", item, )
         # 增加一个交易记录
         serializer = FinanceTransactSerializer(data=item, context={})
 
         # 验证失败，获取错误信息
         if not serializer.is_valid():
-            print(">>> serializer.errors:", serializer.errors, "\n")
+            # print(">>> serializer.errors:", serializer.errors, "\n")
             # 调用save(), 从而调用序列化对象的create()方法,创建一条数据
             # return Response({'err': 1018, 'msg': serializer.errors, })
             return None, serializer.errors
 
         # 验证成功，获取数据
-        serializer.validated_data['platform'] = item['platform']
+        serializer.validated_data['platform_id'] = item['platform_id']
         serializer.validated_data['account'] = item['account']
         serializer.validated_data['their_account'] = item['their_account']
         serializer.validated_data['pay_mode'] = item['pay_mode_set']
         serializer.validated_data['currency'] = item['currency_set']
         serializer.validated_data['sand_box'] = item.get('sand_box_set', None)
         serializer.validated_data['income'] = item['income']
         serializer.validated_data['outgo'] = item['outgo']
@@ -450,15 +477,15 @@
 
         # print(">>> serializer.validated_data: ", serializer.validated_data,)
         # print(">>> serializer: ", serializer,)
 
         serializer.save()
 
         FinanceService.check_balance(account_id=item['account'].id,
-                                     platform=item['platform'].platform_name,
+                                     platform_id=item['platform_id'],
                                      currency=item['currency_set'].currency,
                                      sand_box=item.get('sand_box_set', None))
 
         # return Response({
         #     'err': 0,
         #     'msg': '新增成功',
         # })
@@ -473,29 +500,29 @@
         update_serializer = FinanceTransactSerializer(data=item, instance=transact)
         if not update_serializer.is_valid():
             # print(">>> serializer.errors:", serializer.errors, "\n")
             # 调用save(), 从而调用序列化对象的create()方法,创建一条数据
             # return Response({'err': 1019, 'msg': update_serializer.errors, })
             return None, update_serializer.errors
         # 验证成功，获取数据
-        update_serializer.validated_data['platform'] = item['platform']
+        update_serializer.validated_data['platform_id'] = item['platform_id']
         update_serializer.validated_data['account'] = item['account']
         update_serializer.validated_data['their_account'] = item['their_account']
         update_serializer.validated_data['pay_mode'] = item['pay_mode_set']
         update_serializer.validated_data['currency'] = item['currency_set']
         update_serializer.validated_data['sand_box'] = item.get('sand_box_set', None)
         update_serializer.validated_data['income'] = item['income']
         update_serializer.validated_data['outgo'] = item['outgo']
         update_serializer.validated_data['balance'] = item['balance']
         update_serializer.validated_data['transact_time'] = item['transact_time']
 
         update_serializer.save()
 
         FinanceService.check_balance(account_id=item['account'].id,
-                                     platform=item['platform'].platform_name,
+                                     platform_id=item['platform_id'],
                                      currency=item['currency_set'].currency,
                                      sand_box=item.get('sand_box_set', None))
 
         # return Response({
         #     'err': 0,
         #     'msg': '更新成功',
         # })
```

### Comparing `xj_finance-1.0.9/xj_finance/utils/jt.py` & `xj_finance-1.1.1/xj_finance/utils/jt.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/utils/model_handle.py` & `xj_finance-1.1.1/xj_finance/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance/views.py` & `xj_finance-1.1.1/xj_finance/views.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.0.9/xj_finance.egg-info/PKG-INFO` & `xj_finance-1.1.1/xj_finance.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-finance
-Version: 1.0.9
+Version: 1.1.1
 Summary: 资金模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: ['莫小瑛', '高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
```

### Comparing `xj_finance-1.0.9/xj_finance.egg-info/SOURCES.txt` & `xj_finance-1.1.1/xj_finance.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,30 +8,42 @@
 xj_finance/urls.py
 xj_finance/views.py
 xj_finance.egg-info/PKG-INFO
 xj_finance.egg-info/SOURCES.txt
 xj_finance.egg-info/dependency_links.txt
 xj_finance.egg-info/top_level.txt
 xj_finance/apis/__init__.py
+xj_finance/apis/finance_apis.py
+xj_finance/apis/finance_balance.py
 xj_finance/apis/finance_contact_book.py
 xj_finance/apis/finance_currency.py
 xj_finance/apis/finance_export.py
 xj_finance/apis/finance_pay_mode.py
 xj_finance/apis/finance_sand_box.py
 xj_finance/apis/finance_statistic.py
+xj_finance/apis/finance_status_code.py
 xj_finance/apis/finance_transact.py
 xj_finance/apis/finance_transacts.py
 xj_finance/apis/middleware.py
 xj_finance/apis/router.py
 xj_finance/services/__init__.py
 xj_finance/services/finance_currency_service.py
 xj_finance/services/finance_list_service.py
 xj_finance/services/finance_pay_mode_service.py
 xj_finance/services/finance_sand_box_service.py
+xj_finance/services/finance_service v1.py
 xj_finance/services/finance_service.py
 xj_finance/services/finance_statistic_service.py
+xj_finance/services/finance_status_code_service.py
+xj_finance/services/finance_transact_service v1.py
+xj_finance/services/finance_transact_service v2.py
 xj_finance/services/finance_transact_service.py
+xj_finance/services/finance_transacts_service v1.py
 xj_finance/services/finance_transacts_service.py
 xj_finance/utils/__init__.py
 xj_finance/utils/custom_response.py
+xj_finance/utils/custom_tool.py
+xj_finance/utils/j_config.py
+xj_finance/utils/j_dict.py
 xj_finance/utils/jt.py
-xj_finance/utils/model_handle.py
+xj_finance/utils/model_handle.py
+xj_finance/utils/user_wrapper.py
```


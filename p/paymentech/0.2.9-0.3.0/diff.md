# Comparing `tmp/paymentech-0.2.9.tar.gz` & `tmp/paymentech-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paymentech-0.2.9.tar", last modified: Fri Jul  1 16:03:22 2022, max compression
+gzip compressed data, was "paymentech-0.3.0.tar", last modified: Mon Apr 10 14:25:10 2023, max compression
```

## Comparing `paymentech-0.2.9.tar` & `paymentech-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 16:03:22.940082 paymentech-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-01 16:03:21.000000 paymentech-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-07-01 16:03:22.940082 paymentech-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-07-01 16:03:21.000000 paymentech-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 16:03:22.940082 paymentech-0.2.9/paymentech/
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 16:03:22.940082 paymentech-0.2.9/paymentech/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/resources/authorization.py
--rw-r--r--   0 runner    (1001) docker     (121)     4163 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/resources/inquiry.py
--rw-r--r--   0 runner    (1001) docker     (121)     8844 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/resources/order.py
--rw-r--r--   0 runner    (1001) docker     (121)     4862 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/resources/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/resources/reversal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/service.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-01 16:03:21.000000 paymentech-0.2.9/paymentech/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 16:03:22.940082 paymentech-0.2.9/paymentech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-07-01 16:03:22.000000 paymentech-0.2.9/paymentech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-07-01 16:03:22.000000 paymentech-0.2.9/paymentech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-01 16:03:22.000000 paymentech-0.2.9/paymentech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-01 16:03:22.000000 paymentech-0.2.9/paymentech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-01 16:03:22.000000 paymentech-0.2.9/paymentech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-07-01 16:03:22.940082 paymentech-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-07-01 16:03:21.000000 paymentech-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 16:03:22.940082 paymentech-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-01 16:03:21.000000 paymentech-0.2.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-07-01 16:03:21.000000 paymentech-0.2.9/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-01 16:03:21.000000 paymentech-0.2.9/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:09.990123 paymentech-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 14:25:04.000000 paymentech-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-10 14:25:09.990123 paymentech-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 14:25:04.000000 paymentech-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:09.990123 paymentech-0.3.0/paymentech/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:09.990123 paymentech-0.3.0/paymentech/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/inquiry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:09.990123 paymentech-0.3.0/paymentech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-10 14:25:09.000000 paymentech-0.3.0/paymentech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-10 14:25:09.000000 paymentech-0.3.0/paymentech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:25:09.000000 paymentech-0.3.0/paymentech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 14:25:09.000000 paymentech-0.3.0/paymentech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-10 14:25:09.000000 paymentech-0.3.0/paymentech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-10 14:25:09.990123 paymentech-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-10 14:25:04.000000 paymentech-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:09.990123 paymentech-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:04.000000 paymentech-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-10 14:25:04.000000 paymentech-0.3.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 14:25:04.000000 paymentech-0.3.0/tests/test_sanity.py
```

### Comparing `paymentech-0.2.9/LICENSE` & `paymentech-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paymentech-0.2.9/PKG-INFO` & `paymentech-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paymentech
-Version: 0.2.9
+Version: 0.3.0
 Summary: Python SDK for Chase Paymentech
 Home-page: https://github.com/SerenitySoftware/paymentech
 Author: Jordan Ambra
 Author-email: jordan@serenity.software
 License: UNKNOWN
 Description: # Chase Paymentech SDK
         Python SDK for Chase Paymentech
```

### Comparing `paymentech-0.2.9/paymentech/__init__.py` & `paymentech-0.3.0/paymentech/__init__.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.2.9/paymentech/resources/authorization.py` & `paymentech-0.3.0/paymentech/resources/authorization.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.2.9/paymentech/resources/base.py` & `paymentech-0.3.0/paymentech/resources/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,38 +75,39 @@
             pass
 
         return None
 
     @staticmethod
     def validate_response(result):
         message = result.get("StatusMsg", result.get("RespMsg", "Error"))
+
+        cvv_resp_code = result.get("CVV2RespCode", None)
+        if cvv_resp_code in ("N", "I", "Y"):
+            cvv_lookup = {
+                "N": "CVV doesn't match",
+                "I": "Invalid CVV",
+                "Y": "Invalid CVV"
+            }
+
+            message = cvv_lookup.get(cvv_resp_code)
+            raise exceptions.PaymentechException(message, "cvv", cvv_resp_code, result)
+
         proc_status = result.get("ProcStatus", None)
         if proc_status not in (None, 0, "0", "00"):
             raise exceptions.PaymentechException(message, "processor", proc_status, result)
 
         approval_status = result.get("ApprovalStatus", None)
         if approval_status in (0, "0"):
             message = message or "Payment declined"
             raise exceptions.PaymentechException(message, "approval", approval_status, result)
 
         if approval_status in (2, "2"):
             message = message or "System error, please try again"
             raise exceptions.PaymentechException(message, "system", approval_status, result)
 
-        cvv_resp_code = result.get("CVV2RespCode", None)
-        if cvv_resp_code in ("N", "I", "Y"):
-            cvv_lookup = {
-                "N": "CVV doesn't match",
-                "I": "Invalid CVV",
-                "Y": "Invalid CVV"
-            }
-
-            message = cvv_lookup.get(cvv_resp_code)
-            raise exceptions.PaymentechException(message, "cvv", cvv_resp_code, result)
-
         profile_proc_status = result.get("ProfileProcStatus", None)
         if profile_proc_status not in (None, 0, "0", "00"):
             message = result.get("CustomerProfileMessage", message)
             raise exceptions.PaymentechException(message, "profile", profile_proc_status, result)
 
     @staticmethod
     def process_result(result):
```

### Comparing `paymentech-0.2.9/paymentech/resources/inquiry.py` & `paymentech-0.3.0/paymentech/resources/inquiry.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.2.9/paymentech/resources/order.py` & `paymentech-0.3.0/paymentech/resources/order.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.2.9/paymentech/resources/profile.py` & `paymentech-0.3.0/paymentech/resources/profile.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.2.9/paymentech/resources/reversal.py` & `paymentech-0.3.0/paymentech/resources/reversal.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.2.9/paymentech/service.py` & `paymentech-0.3.0/paymentech/service.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.2.9/paymentech.egg-info/PKG-INFO` & `paymentech-0.3.0/paymentech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paymentech
-Version: 0.2.9
+Version: 0.3.0
 Summary: Python SDK for Chase Paymentech
 Home-page: https://github.com/SerenitySoftware/paymentech
 Author: Jordan Ambra
 Author-email: jordan@serenity.software
 License: UNKNOWN
 Description: # Chase Paymentech SDK
         Python SDK for Chase Paymentech
```

### Comparing `paymentech-0.2.9/paymentech.egg-info/SOURCES.txt` & `paymentech-0.3.0/paymentech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paymentech-0.2.9/setup.py` & `paymentech-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.2.9/tests/test_configuration.py` & `paymentech-0.3.0/tests/test_configuration.py`

 * *Files identical despite different names*


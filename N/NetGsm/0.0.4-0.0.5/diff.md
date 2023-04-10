# Comparing `tmp/NetGsm-0.0.4.tar.gz` & `tmp/NetGsm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NetGsm-0.0.4.tar", last modified: Sun Nov 20 13:13:35 2022, max compression
+gzip compressed data, was "NetGsm-0.0.5.tar", last modified: Mon Apr 10 19:31:35 2023, max compression
```

## Comparing `NetGsm-0.0.4.tar` & `NetGsm-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2022-11-20 13:13:35.587977 NetGsm-0.0.4/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 NetGsm-0.0.4/LICENSE
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2022-11-20 13:13:35.586785 NetGsm-0.0.4/NetGsm.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1832 2022-11-20 13:13:35.000000 NetGsm-0.0.4/NetGsm.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      232 2022-11-20 13:13:35.000000 NetGsm-0.0.4/NetGsm.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2022-11-20 13:13:35.000000 NetGsm-0.0.4/NetGsm.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2022-11-20 13:13:35.000000 NetGsm-0.0.4/NetGsm.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        7 2022-11-20 13:13:35.000000 NetGsm-0.0.4/NetGsm.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1832 2022-11-20 13:13:35.587816 NetGsm-0.0.4/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1328 2022-11-20 10:57:16.000000 NetGsm-0.0.4/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2022-11-20 13:13:35.587525 NetGsm-0.0.4/netgsm/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       99 2022-11-20 13:13:27.000000 NetGsm-0.0.4/netgsm/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      298 2022-11-20 10:40:53.000000 NetGsm-0.0.4/netgsm/exception.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1686 2022-11-20 13:13:22.000000 NetGsm-0.0.4/netgsm/service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2022-11-20 13:13:35.588024 NetGsm-0.0.4/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      823 2022-11-20 13:13:22.000000 NetGsm-0.0.4/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-10 19:31:35.599268 NetGsm-0.0.5/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 NetGsm-0.0.5/LICENSE
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-10 19:31:35.597733 NetGsm-0.0.5/NetGsm.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1832 2023-04-10 19:31:35.000000 NetGsm-0.0.5/NetGsm.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      253 2023-04-10 19:31:35.000000 NetGsm-0.0.5/NetGsm.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-04-10 19:31:35.000000 NetGsm-0.0.5/NetGsm.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-04-10 19:31:35.000000 NetGsm-0.0.5/NetGsm.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        7 2023-04-10 19:31:35.000000 NetGsm-0.0.5/NetGsm.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1832 2023-04-10 19:31:35.599127 NetGsm-0.0.5/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1328 2022-11-20 10:57:16.000000 NetGsm-0.0.5/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-10 19:31:35.598808 NetGsm-0.0.5/netgsm/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       99 2022-11-20 13:13:27.000000 NetGsm-0.0.5/netgsm/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1096 2023-04-10 19:15:27.000000 NetGsm-0.0.5/netgsm/error_code.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      298 2022-11-20 10:40:53.000000 NetGsm-0.0.5/netgsm/exception.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2492 2023-04-10 19:31:01.000000 NetGsm-0.0.5/netgsm/service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-04-10 19:31:35.599313 NetGsm-0.0.5/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      823 2023-04-10 19:31:01.000000 NetGsm-0.0.5/setup.py
```

### Comparing `NetGsm-0.0.4/LICENSE` & `NetGsm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `NetGsm-0.0.4/NetGsm.egg-info/PKG-INFO` & `NetGsm-0.0.5/NetGsm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetGsm
-Version: 0.0.4
+Version: 0.0.5
 Summary: NetGsm Sms Client Python package
 Home-page: https://github.com/blueromans/netgsm.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/netgsm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NetGsm-0.0.4/PKG-INFO` & `NetGsm-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetGsm
-Version: 0.0.4
+Version: 0.0.5
 Summary: NetGsm Sms Client Python package
 Home-page: https://github.com/blueromans/netgsm.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/netgsm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NetGsm-0.0.4/README.md` & `NetGsm-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `NetGsm-0.0.4/netgsm/service.py` & `NetGsm-0.0.5/netgsm/service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,63 @@
 import os
 import re
 
 import requests
 
+from netgsm.error_code import ErrorCode
 from netgsm.exception import NetGsmException, ErrorCodes
 
 
 class SmsService:
     params = dict()
-    API_URL = 'https://api.netgsm.com.tr/sms/send/get'
-    error_codes = [20, 30, 40, 70]
+    API_URL = 'https://api.netgsm.com.tr'
     is_sms_send = False
 
     def __init__(self, user_code=None, user_password=None, api_url=None):
         self.user_code = os.environ.get('NETGSM_USER_CODE', user_code)
         if self.user_code is None:
             raise ValueError(ErrorCodes.USER_CODE_ERROR)
         self.user_password = os.environ.get('NETGSM_USER_PASSWORD', user_password)
         if self.user_password is None:
             raise ValueError(ErrorCodes.USER_PASSWORD_ERROR)
         if api_url is not None:
             self.API_URL = api_url
         self.params = {'usercode': self.user_code, 'password': self.user_password}
 
-    def send(self, phone, message, header=None):
+    def send_sms(self, phone, message, url='/sms/send/get', header=None):
         try:
             if header is None:
                 header = self.user_code
             self.params.update({'gsmno': phone,
                                 'message': message,
                                 'msgheader': header})
             response = requests.get(
-                self.API_URL,
+                f'{self.API_URL}{url}',
                 params=self.params,
             )
             self.check_sms_status(response)
-            if self.is_sms_send is False:
-                raise NetGsmException(ErrorCodes.SMS_SEND_ERROR)
+            return True
+        except Exception as e:
+            raise NetGsmException(e.__str__())
+
+    def send_otp(self, phone, message, url='/sms/send/otp', header=None):
+        try:
+            if header is None:
+                header = self.user_code
+            xmlData = f'<?xml version="1.0"?><mainbody><header><usercode>{self.user_code}</usercode><password>{self.user_password}</password><msgheader>{header}</msgheader></header><body><msg><![CDATA[{message}]] ></msg><no>{phone}</no></body></mainbody>'
+            headers = {'Content-Type': 'application/xml'}
+            response = requests.post(
+                f'{self.API_URL}{url}',
+                data=xmlData, headers=headers
+            )
+            self.check_sms_status(response)
             return True
         except Exception as e:
             raise NetGsmException(e.__str__())
 
     def check_sms_status(self, response):
         response = response.text
         response_code = re.search('[0-9]+', response).group()
-        self.is_sms_send = int(response_code) not in self.error_codes
+        self.is_sms_send = int(response_code) not in ErrorCode.sms_error_codes
+        if self.is_sms_send:
+            return
+        raise NetGsmException(ErrorCode.sms_error_codes[response_code])
```

### Comparing `NetGsm-0.0.4/setup.py` & `NetGsm-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='NetGsm',
-    version="0.0.4",
+    version="0.0.5",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='NetGsm Sms Client Python package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/netgsm.git',
     project_urls={
```


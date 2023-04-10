# Comparing `tmp/badsecrets-0.1.288.tar.gz` & `tmp/badsecrets-0.1.300.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badsecrets-0.1.288.tar", max compression
+gzip compressed data, was "badsecrets-0.1.300.tar", max compression
```

## Comparing `badsecrets-0.1.288.tar` & `badsecrets-0.1.300.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0    35149 2023-04-07 21:21:13.456259 badsecrets-0.1.288/LICENSE
--rw-r--r--   0        0        0    25793 2023-04-07 21:21:13.456259 badsecrets-0.1.288/README.md
--rw-r--r--   0        0        0      711 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/__init__.py
--rw-r--r--   0        0        0     4485 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/base.py
--rw-r--r--   0        0        0      233 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/errors.py
--rw-r--r--   0        0        0     3570 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/helpers.py
--rw-r--r--   0        0        0        0 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/__init__.py
--rw-r--r--   0        0        0     5865 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/aspnet_viewstate.py
--rw-r--r--   0        0        0     1032 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/django_signedcookies.py
--rw-r--r--   0        0        0     2079 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/express_signedcookies.py
--rw-r--r--   0        0        0      856 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/flask_signedcookies.py
--rw-r--r--   0        0        0     3363 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/generic_jwt.py
--rw-r--r--   0        0        0    13573 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/jsf_viewstate.py
--rw-r--r--   0        0        0     1325 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/peoplesoft_pstoken.py
--rw-r--r--   0        0        0     3058 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/rails_secretkeybase.py
--rw-r--r--   0        0        0     2098 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/symfony_signedurl.py
--rw-r--r--   0        0        0     4943 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/telerik_encryptionkey.py
--rw-r--r--   0        0        0     2961 2023-04-07 21:21:13.456259 badsecrets-0.1.288/badsecrets/modules/telerik_hashkey.py
--rw-r--r--   0        0        0   654111 2023-04-07 21:21:13.464259 badsecrets-0.1.288/badsecrets/resources/aspnet_machinekeys.txt
--rw-r--r--   0        0        0    31178 2023-04-07 21:21:13.464259 badsecrets-0.1.288/badsecrets/resources/django_secret_keys.txt
--rw-r--r--   0        0        0    40993 2023-04-07 21:21:13.464259 badsecrets-0.1.288/badsecrets/resources/express_session_secrets.txt
--rw-r--r--   0        0        0  1777603 2023-04-07 21:21:13.480259 badsecrets-0.1.288/badsecrets/resources/flask_secret_keys.txt
--rw-r--r--   0        0        0       87 2023-04-07 21:21:13.480259 badsecrets-0.1.288/badsecrets/resources/jsf_viewstate_passwords.txt
--rw-r--r--   0        0        0     1257 2023-04-07 21:21:13.480259 badsecrets-0.1.288/badsecrets/resources/jsf_viewstate_passwords_b64.txt
--rw-r--r--   0        0        0     7785 2023-04-07 21:21:13.484259 badsecrets-0.1.288/badsecrets/resources/jwt_rsakeys_private.txt
--rw-r--r--   0        0        0     2122 2023-04-07 21:21:13.484259 badsecrets-0.1.288/badsecrets/resources/jwt_rsakeys_public.txt
--rw-r--r--   0        0        0   113170 2023-04-07 21:21:13.484259 badsecrets-0.1.288/badsecrets/resources/jwt_secrets.txt
--rw-r--r--   0        0        0       78 2023-04-07 21:21:13.484259 badsecrets-0.1.288/badsecrets/resources/peoplesoft_passwords.txt
--rw-r--r--   0        0        0     6184 2023-04-07 21:21:13.484259 badsecrets-0.1.288/badsecrets/resources/rails_secret_key_base.txt
--rw-r--r--   0        0        0     3009 2023-04-07 21:21:13.484259 badsecrets-0.1.288/badsecrets/resources/symfony_appsecret.txt
--rw-r--r--   0        0        0    18037 2023-04-07 21:21:13.484259 badsecrets-0.1.288/badsecrets/resources/telerik_encryption_keys.txt
--rw-r--r--   0        0        0    17990 2023-04-07 21:21:13.484259 badsecrets-0.1.288/badsecrets/resources/telerik_hash_keys.txt
--rw-r--r--   0        0        0    76516 2023-04-07 21:21:13.484259 badsecrets-0.1.288/badsecrets/resources/top_10000_passwords.txt
--rw-r--r--   0        0        0      872 2023-04-07 21:21:40.424153 badsecrets-0.1.288/pyproject.toml
--rw-r--r--   0        0        0    26606 1970-01-01 00:00:00.000000 badsecrets-0.1.288/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 15:03:34.146377 badsecrets-0.1.300/LICENSE
+-rw-r--r--   0        0        0    26452 2023-04-10 15:03:34.146377 badsecrets-0.1.300/README.md
+-rw-r--r--   0        0        0      711 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/__init__.py
+-rw-r--r--   0        0        0     4485 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/base.py
+-rw-r--r--   0        0        0      233 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/errors.py
+-rw-r--r--   0        0        0     3570 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/__init__.py
+-rw-r--r--   0        0        0     5865 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/aspnet_viewstate.py
+-rw-r--r--   0        0        0     1032 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/django_signedcookies.py
+-rw-r--r--   0        0        0     2079 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/express_signedcookies.py
+-rw-r--r--   0        0        0      856 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/flask_signedcookies.py
+-rw-r--r--   0        0        0     3363 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/generic_jwt.py
+-rw-r--r--   0        0        0    13573 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/jsf_viewstate.py
+-rw-r--r--   0        0        0     2169 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/laravel_signedcookies.py
+-rw-r--r--   0        0        0     1325 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/peoplesoft_pstoken.py
+-rw-r--r--   0        0        0     3058 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/rails_secretkeybase.py
+-rw-r--r--   0        0        0     2098 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/symfony_signedurl.py
+-rw-r--r--   0        0        0     4943 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/telerik_encryptionkey.py
+-rw-r--r--   0        0        0     2961 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/telerik_hashkey.py
+-rw-r--r--   0        0        0   654111 2023-04-10 15:03:34.154378 badsecrets-0.1.300/badsecrets/resources/aspnet_machinekeys.txt
+-rw-r--r--   0        0        0    31178 2023-04-10 15:03:34.154378 badsecrets-0.1.300/badsecrets/resources/django_secret_keys.txt
+-rw-r--r--   0        0        0    40993 2023-04-10 15:03:34.154378 badsecrets-0.1.300/badsecrets/resources/express_session_secrets.txt
+-rw-r--r--   0        0        0  1777603 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/flask_secret_keys.txt
+-rw-r--r--   0        0        0       87 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/jsf_viewstate_passwords.txt
+-rw-r--r--   0        0        0     1257 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/jsf_viewstate_passwords_b64.txt
+-rw-r--r--   0        0        0     7785 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/jwt_rsakeys_private.txt
+-rw-r--r--   0        0        0     2122 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/jwt_rsakeys_public.txt
+-rw-r--r--   0        0        0   113170 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/jwt_secrets.txt
+-rw-r--r--   0        0        0    45086 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/laravel_app_keys.txt
+-rw-r--r--   0        0        0       78 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/peoplesoft_passwords.txt
+-rw-r--r--   0        0        0     6184 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/rails_secret_key_base.txt
+-rw-r--r--   0        0        0     3009 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/symfony_appsecret.txt
+-rw-r--r--   0        0        0    18037 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/telerik_encryption_keys.txt
+-rw-r--r--   0        0        0    17990 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/telerik_hash_keys.txt
+-rw-r--r--   0        0        0    76516 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/top_10000_passwords.txt
+-rw-r--r--   0        0        0      872 2023-04-10 15:04:00.163742 badsecrets-0.1.300/pyproject.toml
+-rw-r--r--   0        0        0    27265 1970-01-01 00:00:00.000000 badsecrets-0.1.300/PKG-INFO
```

### Comparing `badsecrets-0.1.288/LICENSE` & `badsecrets-0.1.300/LICENSE`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/README.md` & `badsecrets-0.1.300/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 | Flask_SignedCookies  | Checks for weak Flask cookie signing password. Wrapper for [flask-unsign](https://github.com/Paradoxis/Flask-Unsign) |
 | Peoplesoft_PSToken  | Can check a peoplesoft PS_TOKEN for a bad/weak signing password |
 | Django_SignedCookies   | Checks django's session cookies (when in signed_cookie mode) for known django secret_key |
 | Rails_SecretKeyBase   | Checks Ruby on Rails signed or encrypted session cookies (from multiple major releases) for known secret_key_base |
 | Generic_JWT | Checks JWTs for known HMAC secrets or RSA private keys |
 | Jsf_viewstate | Checks Both Mojarra and Myfaces implimentations of Java Server Faces (JSF) for use of known or weak secret keys | 
 | Symfony_SignedURL | Checks symfony "_fragment" urls for known HMAC key. Operates on Full URL, including hash |
-| Express_SignedCookies | Checks express.js signed cookies and session cookies for session secret |
+| Express_SignedCookies | Checks express.js signed cookies and session cookies for known 'session secret' |
+| Laravel_SignedCookies | Checks 'laravel_session' cookies for known laravel 'APP_KEY' |
 
 ## Installation
 
 We have a [pypi](https://pypi.org/project/badsecrets/) package, so you can just do `pip install badsecrets` to make use of the library.
 
 To use the examples, after doing the pip install just `git clone` the repo and `cd` into the `badsecrets` directory:
 
@@ -137,14 +138,15 @@
 Telerik_HashKey = modules_loaded["telerik_hashkey"]
 Telerik_EncryptionKey = modules_loaded["telerik_encryptionkey"]
 Rails_SecretKeyBase = modules_loaded["rails_secretkeybase"]
 Generic_JWT = modules_loaded["generic_jwt"]
 Jsf_viewstate = modules_loaded["jsf_viewstate"]
 Symfony_SignedURL = modules_loaded["symfony_signedurl"]
 Express_SignedCookies = modules_loaded["express_signedcookies"]
+Laravel_SignedCookies = modules_loaded["laravel_signedcookies"]
 
 x = ASPNET_Viewstate()
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("AgF5WuyVO11CsYJ1K5rjyuLXqUGCITSOapG1cYNiriYQ6VTKochMpn8ws4eJRvft81nQIA==","EDD8C9AE")
 if r:
     print(r)
 else:
@@ -229,14 +231,23 @@
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("s%3A8FnPwdeM9kdGTZlWvdaVtQ0S1BCOhY5G.qys7H2oGSLLdRsEq7sqh7btOohHsaRKqyjV4LiVnBvc")
 if r:
     print(r)
 else:
     print("KEY NOT FOUND :(")
 
+
+x = Laravel_SignedCookies()
+print(f"###{str(x.__class__.__name__)}###")
+r = x.check_secret("eyJpdiI6IlhlNTZ2UjZUQWZKVHdIcG9nZFkwcGc9PSIsInZhbHVlIjoiRlUvY2grU1F1b01lSXdveXJ0T3N1WGJqeVVmZlNRQjNVOWxiSzljL1Z3RDhqYUdDbjZxMU9oSThWRzExT0YvUmthVzVKRE9kL0RvTEw1cFRhQkphOGw4S2loV1ZrMkkwTHd4am9sZkJQd2VCZ3R0VlFSeFo3ay9wTlBMb3lLSG8iLCJtYWMiOiJkMmU3M2ExNDc2NTc5YjAwMGMwMTdkYTQ1NThkMjRkNTY2YTE4OTg2MzY5MzE5NGZmOTM4YWVjOGZmMWU4NTk2IiwidGFnIjoiIn0%3D")
+if r:
+    print(r)
+else:
+    print("KEY NOT FOUND :(")
+
 ```
 
 #### Carve
 An additional layer of abstraction above check_secret, which accepts a python requests.response object or a string
 
 ```python
 import requests
@@ -320,11 +331,11 @@
 
 Nothing would make us happier than getting a pull request with a new module! But the easiest way to contribute would be helping to populate our word lists! If you find publicly available keys help us make Badsecrets more useful by submitting a pull request to add them.
 
 Requests for modules are always very welcome as well!
 
 ### Planned Modules
 
-- Laravel
+- ~~Laravel~~
 -  ~~Express~~
```

### Comparing `badsecrets-0.1.288/badsecrets/__init__.py` & `badsecrets-0.1.300/badsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/base.py` & `badsecrets-0.1.300/badsecrets/base.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/helpers.py` & `badsecrets-0.1.300/badsecrets/helpers.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/aspnet_viewstate.py` & `badsecrets-0.1.300/badsecrets/modules/aspnet_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/django_signedcookies.py` & `badsecrets-0.1.300/badsecrets/modules/django_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/express_signedcookies.py` & `badsecrets-0.1.300/badsecrets/modules/express_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/flask_signedcookies.py` & `badsecrets-0.1.300/badsecrets/modules/flask_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/generic_jwt.py` & `badsecrets-0.1.300/badsecrets/modules/generic_jwt.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/jsf_viewstate.py` & `badsecrets-0.1.300/badsecrets/modules/jsf_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/peoplesoft_pstoken.py` & `badsecrets-0.1.300/badsecrets/modules/peoplesoft_pstoken.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/rails_secretkeybase.py` & `badsecrets-0.1.300/badsecrets/modules/rails_secretkeybase.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/symfony_signedurl.py` & `badsecrets-0.1.300/badsecrets/modules/symfony_signedurl.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/telerik_encryptionkey.py` & `badsecrets-0.1.300/badsecrets/modules/telerik_encryptionkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/modules/telerik_hashkey.py` & `badsecrets-0.1.300/badsecrets/modules/telerik_hashkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/aspnet_machinekeys.txt` & `badsecrets-0.1.300/badsecrets/resources/aspnet_machinekeys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/django_secret_keys.txt` & `badsecrets-0.1.300/badsecrets/resources/django_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/express_session_secrets.txt` & `badsecrets-0.1.300/badsecrets/resources/express_session_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/flask_secret_keys.txt` & `badsecrets-0.1.300/badsecrets/resources/flask_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/jsf_viewstate_passwords_b64.txt` & `badsecrets-0.1.300/badsecrets/resources/jsf_viewstate_passwords_b64.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/jwt_rsakeys_private.txt` & `badsecrets-0.1.300/badsecrets/resources/jwt_rsakeys_private.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/jwt_rsakeys_public.txt` & `badsecrets-0.1.300/badsecrets/resources/jwt_rsakeys_public.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/jwt_secrets.txt` & `badsecrets-0.1.300/badsecrets/resources/jwt_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/rails_secret_key_base.txt` & `badsecrets-0.1.300/badsecrets/resources/rails_secret_key_base.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/symfony_appsecret.txt` & `badsecrets-0.1.300/badsecrets/resources/symfony_appsecret.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/telerik_encryption_keys.txt` & `badsecrets-0.1.300/badsecrets/resources/telerik_encryption_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/telerik_hash_keys.txt` & `badsecrets-0.1.300/badsecrets/resources/telerik_hash_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/badsecrets/resources/top_10000_passwords.txt` & `badsecrets-0.1.300/badsecrets/resources/top_10000_passwords.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.288/pyproject.toml` & `badsecrets-0.1.300/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "badsecrets"
-version = "v0.1.288"
+version = "v0.1.300"
 description = "About"
 authors = ["A library for detecting known or weak secrets on across many platforms"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dev-dependencies]
 requests-mock = "^1.10.0"
```

### Comparing `badsecrets-0.1.288/PKG-INFO` & `badsecrets-0.1.300/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badsecrets
-Version: 0.1.288
+Version: 0.1.300
 Summary: About
 License: GPL-3.0
 Author: A library for detecting known or weak secrets on across many platforms
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -46,15 +46,16 @@
 | Flask_SignedCookies  | Checks for weak Flask cookie signing password. Wrapper for [flask-unsign](https://github.com/Paradoxis/Flask-Unsign) |
 | Peoplesoft_PSToken  | Can check a peoplesoft PS_TOKEN for a bad/weak signing password |
 | Django_SignedCookies   | Checks django's session cookies (when in signed_cookie mode) for known django secret_key |
 | Rails_SecretKeyBase   | Checks Ruby on Rails signed or encrypted session cookies (from multiple major releases) for known secret_key_base |
 | Generic_JWT | Checks JWTs for known HMAC secrets or RSA private keys |
 | Jsf_viewstate | Checks Both Mojarra and Myfaces implimentations of Java Server Faces (JSF) for use of known or weak secret keys | 
 | Symfony_SignedURL | Checks symfony "_fragment" urls for known HMAC key. Operates on Full URL, including hash |
-| Express_SignedCookies | Checks express.js signed cookies and session cookies for session secret |
+| Express_SignedCookies | Checks express.js signed cookies and session cookies for known 'session secret' |
+| Laravel_SignedCookies | Checks 'laravel_session' cookies for known laravel 'APP_KEY' |
 
 ## Installation
 
 We have a [pypi](https://pypi.org/project/badsecrets/) package, so you can just do `pip install badsecrets` to make use of the library.
 
 To use the examples, after doing the pip install just `git clone` the repo and `cd` into the `badsecrets` directory:
 
@@ -158,14 +159,15 @@
 Telerik_HashKey = modules_loaded["telerik_hashkey"]
 Telerik_EncryptionKey = modules_loaded["telerik_encryptionkey"]
 Rails_SecretKeyBase = modules_loaded["rails_secretkeybase"]
 Generic_JWT = modules_loaded["generic_jwt"]
 Jsf_viewstate = modules_loaded["jsf_viewstate"]
 Symfony_SignedURL = modules_loaded["symfony_signedurl"]
 Express_SignedCookies = modules_loaded["express_signedcookies"]
+Laravel_SignedCookies = modules_loaded["laravel_signedcookies"]
 
 x = ASPNET_Viewstate()
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("AgF5WuyVO11CsYJ1K5rjyuLXqUGCITSOapG1cYNiriYQ6VTKochMpn8ws4eJRvft81nQIA==","EDD8C9AE")
 if r:
     print(r)
 else:
@@ -250,14 +252,23 @@
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("s%3A8FnPwdeM9kdGTZlWvdaVtQ0S1BCOhY5G.qys7H2oGSLLdRsEq7sqh7btOohHsaRKqyjV4LiVnBvc")
 if r:
     print(r)
 else:
     print("KEY NOT FOUND :(")
 
+
+x = Laravel_SignedCookies()
+print(f"###{str(x.__class__.__name__)}###")
+r = x.check_secret("eyJpdiI6IlhlNTZ2UjZUQWZKVHdIcG9nZFkwcGc9PSIsInZhbHVlIjoiRlUvY2grU1F1b01lSXdveXJ0T3N1WGJqeVVmZlNRQjNVOWxiSzljL1Z3RDhqYUdDbjZxMU9oSThWRzExT0YvUmthVzVKRE9kL0RvTEw1cFRhQkphOGw4S2loV1ZrMkkwTHd4am9sZkJQd2VCZ3R0VlFSeFo3ay9wTlBMb3lLSG8iLCJtYWMiOiJkMmU3M2ExNDc2NTc5YjAwMGMwMTdkYTQ1NThkMjRkNTY2YTE4OTg2MzY5MzE5NGZmOTM4YWVjOGZmMWU4NTk2IiwidGFnIjoiIn0%3D")
+if r:
+    print(r)
+else:
+    print("KEY NOT FOUND :(")
+
 ```
 
 #### Carve
 An additional layer of abstraction above check_secret, which accepts a python requests.response object or a string
 
 ```python
 import requests
@@ -341,12 +352,12 @@
 
 Nothing would make us happier than getting a pull request with a new module! But the easiest way to contribute would be helping to populate our word lists! If you find publicly available keys help us make Badsecrets more useful by submitting a pull request to add them.
 
 Requests for modules are always very welcome as well!
 
 ### Planned Modules
 
-- Laravel
+- ~~Laravel~~
 -  ~~Express~~
```


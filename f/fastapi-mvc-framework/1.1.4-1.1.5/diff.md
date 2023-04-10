# Comparing `tmp/fastapi_mvc_framework-1.1.4.tar.gz` & `tmp/fastapi_mvc_framework-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mvc_framework-1.1.4.tar", last modified: Mon Apr 10 07:37:51 2023, max compression
+gzip compressed data, was "fastapi_mvc_framework-1.1.5.tar", last modified: Mon Apr 10 14:23:17 2023, max compression
```

## Comparing `fastapi_mvc_framework-1.1.4.tar` & `fastapi_mvc_framework-1.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 07:37:51.651188 fastapi_mvc_framework-1.1.4/
--rw-rw-rw-   0        0        0     7658 2023-04-10 07:37:51.650190 fastapi_mvc_framework-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5526 2023-04-10 07:37:34.000000 fastapi_mvc_framework-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 07:37:51.642209 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/
--rw-rw-rw-   0        0        0      251 2023-04-06 06:00:47.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/__init__.py
--rw-rw-rw-   0        0        0      931 2023-04-07 07:39:59.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/_utils.py
--rw-rw-rw-   0        0        0     9943 2023-04-09 05:56:58.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/auth.py
--rw-rw-rw-   0        0        0     8826 2023-04-08 11:33:08.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/cbv.py
--rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/config.py
--rw-rw-rw-   0        0        0     3733 2023-04-09 05:46:23.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/controller.py
--rw-rw-rw-   0        0        0    12971 2023-04-09 05:48:57.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/controller_utils.py
--rw-rw-rw-   0        0        0    11236 2023-04-09 13:15:31.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/core.py
--rw-rw-rw-   0        0        0     1710 2023-04-10 07:35:52.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/database.py
--rw-rw-rw-   0        0        0     5507 2023-04-07 11:35:06.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware_casbin.py
--rw-rw-rw-   0        0        0     9185 2023-04-08 05:46:03.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware_session.py
--rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/view.py
-drwxrwxrwx   0        0        0        0 2023-04-10 07:37:51.648194 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/
--rw-rw-rw-   0        0        0     7658 2023-04-10 07:37:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      682 2023-04-10 07:37:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 07:37:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-10 07:37:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 07:37:51.651188 fastapi_mvc_framework-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      721 2023-04-10 07:31:04.000000 fastapi_mvc_framework-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:23:17.472672 fastapi_mvc_framework-1.1.5/
+-rw-rw-rw-   0        0        0     6979 2023-04-10 14:23:17.471674 fastapi_mvc_framework-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4959 2023-04-10 07:40:40.000000 fastapi_mvc_framework-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 14:23:17.464692 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/
+-rw-rw-rw-   0        0        0      267 2023-04-10 12:07:43.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-04-07 07:39:59.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/_utils.py
+-rw-rw-rw-   0        0        0     9943 2023-04-09 05:56:58.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/auth.py
+-rw-rw-rw-   0        0        0     9090 2023-04-10 14:04:09.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/cbv.py
+-rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/config.py
+-rw-rw-rw-   0        0        0     3733 2023-04-09 05:46:23.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/controller.py
+-rw-rw-rw-   0        0        0    12971 2023-04-09 05:48:57.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/controller_utils.py
+-rw-rw-rw-   0        0        0    11234 2023-04-10 14:14:04.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/core.py
+-rw-rw-rw-   0        0        0     1905 2023-04-10 14:13:08.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/database.py
+-rw-rw-rw-   0        0        0     5507 2023-04-07 11:35:06.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware_session.py
+-rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/view.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:23:17.469679 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/
+-rw-rw-rw-   0        0        0     6979 2023-04-10 14:23:17.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      682 2023-04-10 14:23:17.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:23:17.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-10 14:23:17.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:23:17.473669 fastapi_mvc_framework-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      721 2023-04-10 14:23:07.000000 fastapi_mvc_framework-1.1.5/setup.py
```

### Comparing `fastapi_mvc_framework-1.1.4/PKG-INFO` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fastapi_mvc_framework
-Version: 1.1.4
+Name: fastapi-mvc-framework
+Version: 1.1.5
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: UNKNOWN
 Description: # fastapi_framework
         A mvc framework used FastApi
@@ -158,18 +158,14 @@
         +---app1
         |   |   __init__.py
         |   |
         |   +---controllers
         |   |   |   test1_controller.py
         |   |   |   __init__.py
         |   |   |
-        |   |   \---__pycache__
-        |   |           test1_controller.cpython-38.pyc
-        |   |           __init__.cpython-38.pyc
-        |   |
         |   +---views
         |   |   +---test1
         |   |   |   \---v1.0
         |   |   |           home.css
         |   |   |           home.html
         |   |   |           home1.css
         |   |   |
@@ -193,24 +189,14 @@
         |   |   +---versions
         |   |   |   |   0d0205db5b39_create_tables.py
         |   |   |   |   0e4e15e67367_autogenerate.py
         |   |   |   |   108dad121227__new_upgrade_operations_detected__add_.py
         |   |   |   |   ac7ce07126b3_autogenerate.py
         |   |   |   |   e51711eb3d84_autogenerate.py
         |   |   |   |
-        |   |   |   \---__pycache__
-        |   |   |           0d0205db5b39_create_tables.cpython-38.pyc
-        |   |   |           0e4e15e67367_autogenerate.cpython-38.pyc
-        |   |   |           108dad121227__new_upgrade_operations_detected__add_.cpython-38.pyc
-        |   |   |           ac7ce07126b3_autogenerate.cpython-38.pyc
-        |   |   |           e51711eb3d84_autogenerate.cpython-38.pyc
-        |   |   |
-        |   |   \---__pycache__
-        |   |           env.cpython-38.pyc
-        |   |
         |   \---db
         |           test.db
         
         ```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.4 Summary:
+Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.5 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
 License: UNKNOWN Description: # fastapi_framework A mvc framework used FastApi
 Simple and elegant use of FastApi in MVC mode ## usage: install: ```bash pip
 install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
@@ -43,26 +43,19 @@
 ``` your project directory structrue like this: ``` +---app | | __init__.py | |
 | +---controllers | | | test_controller.py | | | __init__.py | | | | +---models
 | | | user_model.py | | | __init__.py | | | | +---services | | |
 user_service.py | | | __init__.py | | | | +---views | | +---abc | | | \---2.0 |
 | | css.css | | | home.html | | | | | +---test | | | chatgpt.css | | |
 chatgpt.html | | | chatgpt.js | | | home.html | | | home.js | | | login.html |
 | | | | \---ws | | ws_home.html | | +---app1 | | __init__.py | | | +---
-controllers | | | test1_controller.py | | | __init__.py | | | | | \---
-__pycache__ | | test1_controller.cpython-38.pyc | | __init__.cpython-38.pyc | |
-| +---views | | +---test1 | | | \---v1.0 | | | home.css | | | home.html | | |
-home1.css | | | | | \---test2 | +---configs | alembic.ini | cache.yaml |
-casbin-adapter.csv | casbin-model.conf | database.yaml | general.yaml |
-session.yaml | +---data | +---alembic | | | env.py | | | README | | |
-script.py.mako | | | | | +---versions | | | | 0d0205db5b39_create_tables.py | |
-| | 0e4e15e67367_autogenerate.py | | | |
-108dad121227__new_upgrade_operations_detected__add_.py | | | |
-ac7ce07126b3_autogenerate.py | | | | e51711eb3d84_autogenerate.py | | | | | | |
-\---__pycache__ | | | 0d0205db5b39_create_tables.cpython-38.pyc | | |
-0e4e15e67367_autogenerate.cpython-38.pyc | | |
-108dad121227__new_upgrade_operations_detected__add_.cpython-38.pyc | | |
-ac7ce07126b3_autogenerate.cpython-38.pyc | | |
-e51711eb3d84_autogenerate.cpython-38.pyc | | | | | \---__pycache__ | |
-env.cpython-38.pyc | | | \---db | test.db ``` Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+controllers | | | test1_controller.py | | | __init__.py | | | | +---views | |
++---test1 | | | \---v1.0 | | | home.css | | | home.html | | | home1.css | | | |
+| \---test2 | +---configs | alembic.ini | cache.yaml | casbin-adapter.csv |
+casbin-model.conf | database.yaml | general.yaml | session.yaml | +---data | +-
+--alembic | | | env.py | | | README | | | script.py.mako | | | | | +---versions
+| | | | 0d0205db5b39_create_tables.py | | | | 0e4e15e67367_autogenerate.py | |
+| | 108dad121227__new_upgrade_operations_detected__add_.py | | | |
+ac7ce07126b3_autogenerate.py | | | | e51711eb3d84_autogenerate.py | | | | | \--
+-db | test.db ``` Platform: UNKNOWN Classifier: Programming Language :: Python
+:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown
```

### Comparing `fastapi_mvc_framework-1.1.4/README.md` & `fastapi_mvc_framework-1.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -150,18 +150,14 @@
 +---app1
 |   |   __init__.py
 |   |
 |   +---controllers
 |   |   |   test1_controller.py
 |   |   |   __init__.py
 |   |   |
-|   |   \---__pycache__
-|   |           test1_controller.cpython-38.pyc
-|   |           __init__.cpython-38.pyc
-|   |
 |   +---views
 |   |   +---test1
 |   |   |   \---v1.0
 |   |   |           home.css
 |   |   |           home.html
 |   |   |           home1.css
 |   |   |
@@ -185,21 +181,11 @@
 |   |   +---versions
 |   |   |   |   0d0205db5b39_create_tables.py
 |   |   |   |   0e4e15e67367_autogenerate.py
 |   |   |   |   108dad121227__new_upgrade_operations_detected__add_.py
 |   |   |   |   ac7ce07126b3_autogenerate.py
 |   |   |   |   e51711eb3d84_autogenerate.py
 |   |   |   |
-|   |   |   \---__pycache__
-|   |   |           0d0205db5b39_create_tables.cpython-38.pyc
-|   |   |           0e4e15e67367_autogenerate.cpython-38.pyc
-|   |   |           108dad121227__new_upgrade_operations_detected__add_.cpython-38.pyc
-|   |   |           ac7ce07126b3_autogenerate.cpython-38.pyc
-|   |   |           e51711eb3d84_autogenerate.cpython-38.pyc
-|   |   |
-|   |   \---__pycache__
-|   |           env.cpython-38.pyc
-|   |
 |   \---db
 |           test.db
 
 ```
```

#### html2text {}

```diff
@@ -39,23 +39,16 @@
 ``` your project directory structrue like this: ``` +---app | | __init__.py | |
 | +---controllers | | | test_controller.py | | | __init__.py | | | | +---models
 | | | user_model.py | | | __init__.py | | | | +---services | | |
 user_service.py | | | __init__.py | | | | +---views | | +---abc | | | \---2.0 |
 | | css.css | | | home.html | | | | | +---test | | | chatgpt.css | | |
 chatgpt.html | | | chatgpt.js | | | home.html | | | home.js | | | login.html |
 | | | | \---ws | | ws_home.html | | +---app1 | | __init__.py | | | +---
-controllers | | | test1_controller.py | | | __init__.py | | | | | \---
-__pycache__ | | test1_controller.cpython-38.pyc | | __init__.cpython-38.pyc | |
-| +---views | | +---test1 | | | \---v1.0 | | | home.css | | | home.html | | |
-home1.css | | | | | \---test2 | +---configs | alembic.ini | cache.yaml |
-casbin-adapter.csv | casbin-model.conf | database.yaml | general.yaml |
-session.yaml | +---data | +---alembic | | | env.py | | | README | | |
-script.py.mako | | | | | +---versions | | | | 0d0205db5b39_create_tables.py | |
-| | 0e4e15e67367_autogenerate.py | | | |
-108dad121227__new_upgrade_operations_detected__add_.py | | | |
-ac7ce07126b3_autogenerate.py | | | | e51711eb3d84_autogenerate.py | | | | | | |
-\---__pycache__ | | | 0d0205db5b39_create_tables.cpython-38.pyc | | |
-0e4e15e67367_autogenerate.cpython-38.pyc | | |
-108dad121227__new_upgrade_operations_detected__add_.cpython-38.pyc | | |
-ac7ce07126b3_autogenerate.cpython-38.pyc | | |
-e51711eb3d84_autogenerate.cpython-38.pyc | | | | | \---__pycache__ | |
-env.cpython-38.pyc | | | \---db | test.db ```
+controllers | | | test1_controller.py | | | __init__.py | | | | +---views | |
++---test1 | | | \---v1.0 | | | home.css | | | home.html | | | home1.css | | | |
+| \---test2 | +---configs | alembic.ini | cache.yaml | casbin-adapter.csv |
+casbin-model.conf | database.yaml | general.yaml | session.yaml | +---data | +-
+--alembic | | | env.py | | | README | | | script.py.mako | | | | | +---versions
+| | | | 0d0205db5b39_create_tables.py | | | | 0e4e15e67367_autogenerate.py | |
+| | 108dad121227__new_upgrade_operations_detected__add_.py | | | |
+ac7ce07126b3_autogenerate.py | | | | e51711eb3d84_autogenerate.py | | | | | \--
+-db | test.db ```
```

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/_utils.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/auth.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/base_controller.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/base_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,23 @@
     @flash.setter
     def flash(self,value):
         self._request.state.keep_flash = True
         self._request['session']['flash'] = value
     @property
     def response(self)->Response :
         return self._response
-    @property
-    def params(self):
-        return self._params
      
+    def get_param(self,key):
+        if key in self._form:
+            return self._form[key]
+        if key in self._json:
+            return self._json[key]
+        if key in self._query:
+            return self._query[key]
+        return None 
      
     @property
     def session(self)->Dict:
         return self._session  
     @classmethod
     def redirect(self,url ,statu_code=StateCodes.HTTP_303_SEE_OTHER):
          
@@ -183,17 +188,17 @@
 
         
         try:
             json_params =  await  request.json()
         except:
             pass
         query_params = request.query_params
-        params.update(form_params)
-        params.update(query_params)
-        params.update(json_params)
+        base_controller_class._form = form_params
+        base_controller_class._query = query_params
+        base_controller_class._json = json_params
         base_controller_class._params = params
         def __init_flash(request:Request): 
             request.state.keep_flash = False 
             if 'flash' not in request.session:
                 request.session['flash'] ='' 
             
         __init_flash(request=request) 
@@ -211,15 +216,16 @@
             response.set_cookie(key=_session_key,
                                 value=base_controller_class._request.cookies[_session_key],
                                 max_age = 14 * 24 * 60 * 60,  # 14 days, in seconds
                                 path  = "/",
                                 samesite  = "lax",
                                 httponly  = False ) 
             
-        process_cookies(new_response,base_controller_class._cookies,base_controller_class._request.cookies)
+        if new_response:
+            process_cookies(new_response,base_controller_class._cookies,base_controller_class._request.cookies)
 
         def __clear_flash(request:Request):
             if not request.state.keep_flash:
                 request.session['flash'] = ''
         __clear_flash(base_controller_class._request)
```

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/cbv.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/cbv.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/config.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/controller.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/controller_utils.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/controller_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/core.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,10 +246,11 @@
     return application
 
 def run(app,*args,**kwargs): 
     import uvicorn
     global __is_debug
     host =  "host" in kwargs  and kwargs["host"]  or '0.0.0.0' 
     port = "port" in kwargs  and kwargs["port"] or 8000  
-    __is_debug = kwargs["debug"] if  "debug" in kwargs else False   
+    if  "debug" in kwargs:
+        __is_debug = kwargs["debug"]  
      
     uvicorn.run(app, host=host, port=port)
```

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/database.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,12 +42,17 @@
     except Exception as e: 
         msg = sanitize_path(str(e.args)) 
         command.revision(alembic_cfg, autogenerate=True, message=msg) 
         # 执行数据库迁移
         command.upgrade(alembic_cfg, "head") 
 
 def init_database( uri:str,debug:bool=False,alembic_ini:str=""):
+    '''
+    params :uri sqlalchemy 的连接字符串
+    :params debug 是否调试模式
+    :params alembic_ini alembic的配置文件路径,debug=True时则会执行数据迁移
+    '''
     engine = create_engine(uri, echo=debug)
     if debug and alembic_ini:
         __check_migration(engine,uri,alembic_ini)
     return engine
```

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware_casbin.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware_session.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,18 @@
     def set(self, session_id: str, data ) -> None:
         filename = self.ensure_file_exists(session_id)
         self.cachedData[session_id] = data 
         with open(filename, "wb") as f:
             f.write(data)
 
     def delete(self, session_id: str) -> None:
-        filename = self.ensure_file_exists(session_id)
+        filename = self.ensure_file_exists(session_id,'delete')
         try:
-            os.remove(filename)
+            if filename:
+                os.remove(filename)
         except Exception as e:
             _log.error(e)   
 
 try:
     import redis
     class RedisStorage(SessionStorage):
         def __init__(self, host: str, port: int, password: str, db: int): 
@@ -164,14 +165,16 @@
             else:
                 data = connection.cookies[self.session_cookie_key].encode("utf-8")
             try:
                 data = self.signer.unsign(data, max_age=self.max_age)
                 scope["session"] =  (json.loads(b64decode(data)))
                 initial_session_was_empty = False
             except BadSignature:
+                if self.storage:
+                    self.storage.delete(connection.cookies[self.session_cookie_key])
                 scope["session"] = {}
         else:
             
             scope["session"] = {}
         # old_data = scope["session"].copy()
 
         async def send_wrapper(message: Message) -> None:
```

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/view.py` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/view.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/PKG-INFO` & `fastapi_mvc_framework-1.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fastapi-mvc-framework
-Version: 1.1.4
+Name: fastapi_mvc_framework
+Version: 1.1.5
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: UNKNOWN
 Description: # fastapi_framework
         A mvc framework used FastApi
@@ -158,18 +158,14 @@
         +---app1
         |   |   __init__.py
         |   |
         |   +---controllers
         |   |   |   test1_controller.py
         |   |   |   __init__.py
         |   |   |
-        |   |   \---__pycache__
-        |   |           test1_controller.cpython-38.pyc
-        |   |           __init__.cpython-38.pyc
-        |   |
         |   +---views
         |   |   +---test1
         |   |   |   \---v1.0
         |   |   |           home.css
         |   |   |           home.html
         |   |   |           home1.css
         |   |   |
@@ -193,24 +189,14 @@
         |   |   +---versions
         |   |   |   |   0d0205db5b39_create_tables.py
         |   |   |   |   0e4e15e67367_autogenerate.py
         |   |   |   |   108dad121227__new_upgrade_operations_detected__add_.py
         |   |   |   |   ac7ce07126b3_autogenerate.py
         |   |   |   |   e51711eb3d84_autogenerate.py
         |   |   |   |
-        |   |   |   \---__pycache__
-        |   |   |           0d0205db5b39_create_tables.cpython-38.pyc
-        |   |   |           0e4e15e67367_autogenerate.cpython-38.pyc
-        |   |   |           108dad121227__new_upgrade_operations_detected__add_.cpython-38.pyc
-        |   |   |           ac7ce07126b3_autogenerate.cpython-38.pyc
-        |   |   |           e51711eb3d84_autogenerate.cpython-38.pyc
-        |   |   |
-        |   |   \---__pycache__
-        |   |           env.cpython-38.pyc
-        |   |
         |   \---db
         |           test.db
         
         ```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.4 Summary:
+Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.5 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
 License: UNKNOWN Description: # fastapi_framework A mvc framework used FastApi
 Simple and elegant use of FastApi in MVC mode ## usage: install: ```bash pip
 install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
@@ -43,26 +43,19 @@
 ``` your project directory structrue like this: ``` +---app | | __init__.py | |
 | +---controllers | | | test_controller.py | | | __init__.py | | | | +---models
 | | | user_model.py | | | __init__.py | | | | +---services | | |
 user_service.py | | | __init__.py | | | | +---views | | +---abc | | | \---2.0 |
 | | css.css | | | home.html | | | | | +---test | | | chatgpt.css | | |
 chatgpt.html | | | chatgpt.js | | | home.html | | | home.js | | | login.html |
 | | | | \---ws | | ws_home.html | | +---app1 | | __init__.py | | | +---
-controllers | | | test1_controller.py | | | __init__.py | | | | | \---
-__pycache__ | | test1_controller.cpython-38.pyc | | __init__.cpython-38.pyc | |
-| +---views | | +---test1 | | | \---v1.0 | | | home.css | | | home.html | | |
-home1.css | | | | | \---test2 | +---configs | alembic.ini | cache.yaml |
-casbin-adapter.csv | casbin-model.conf | database.yaml | general.yaml |
-session.yaml | +---data | +---alembic | | | env.py | | | README | | |
-script.py.mako | | | | | +---versions | | | | 0d0205db5b39_create_tables.py | |
-| | 0e4e15e67367_autogenerate.py | | | |
-108dad121227__new_upgrade_operations_detected__add_.py | | | |
-ac7ce07126b3_autogenerate.py | | | | e51711eb3d84_autogenerate.py | | | | | | |
-\---__pycache__ | | | 0d0205db5b39_create_tables.cpython-38.pyc | | |
-0e4e15e67367_autogenerate.cpython-38.pyc | | |
-108dad121227__new_upgrade_operations_detected__add_.cpython-38.pyc | | |
-ac7ce07126b3_autogenerate.cpython-38.pyc | | |
-e51711eb3d84_autogenerate.cpython-38.pyc | | | | | \---__pycache__ | |
-env.cpython-38.pyc | | | \---db | test.db ``` Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+controllers | | | test1_controller.py | | | __init__.py | | | | +---views | |
++---test1 | | | \---v1.0 | | | home.css | | | home.html | | | home1.css | | | |
+| \---test2 | +---configs | alembic.ini | cache.yaml | casbin-adapter.csv |
+casbin-model.conf | database.yaml | general.yaml | session.yaml | +---data | +-
+--alembic | | | env.py | | | README | | | script.py.mako | | | | | +---versions
+| | | | 0d0205db5b39_create_tables.py | | | | 0e4e15e67367_autogenerate.py | |
+| | 108dad121227__new_upgrade_operations_detected__add_.py | | | |
+ac7ce07126b3_autogenerate.py | | | | e51711eb3d84_autogenerate.py | | | | | \--
+-db | test.db ``` Platform: UNKNOWN Classifier: Programming Language :: Python
+:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown
```

### Comparing `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/SOURCES.txt` & `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.4/setup.py` & `fastapi_mvc_framework-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='fastapi_mvc_framework',
-    version='1.1.4',
+    version='1.1.5',
     author='Bruce chou',
     author_email='smjkzsl@gmail.com',
     description='Simple and elegant use of FastApi in MVC mode',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     url='https://github.com/smjkzsl/fastapi_framework',
```


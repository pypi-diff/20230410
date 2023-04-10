# Comparing `tmp/fastapi_mvc_framework-1.1.3.tar.gz` & `tmp/fastapi_mvc_framework-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mvc_framework-1.1.3.tar", last modified: Sun Apr  9 06:40:46 2023, max compression
+gzip compressed data, was "fastapi_mvc_framework-1.1.4.tar", last modified: Mon Apr 10 07:37:51 2023, max compression
```

## Comparing `fastapi_mvc_framework-1.1.3.tar` & `fastapi_mvc_framework-1.1.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:40:46.442270 fastapi_mvc_framework-1.1.3/
--rw-rw-rw-   0        0        0     6265 2023-04-09 06:40:46.441272 fastapi_mvc_framework-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4421 2023-04-09 06:40:13.000000 fastapi_mvc_framework-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:40:46.433295 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/
--rw-rw-rw-   0        0        0      251 2023-04-06 06:00:47.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/__init__.py
--rw-rw-rw-   0        0        0      931 2023-04-07 07:39:59.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/_utils.py
--rw-rw-rw-   0        0        0     9943 2023-04-09 05:56:58.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/auth.py
--rw-rw-rw-   0        0        0     8826 2023-04-08 11:33:08.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/cbv.py
--rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/config.py
--rw-rw-rw-   0        0        0     3733 2023-04-09 05:46:23.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/controller.py
--rw-rw-rw-   0        0        0    12971 2023-04-09 05:48:57.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/controller_utils.py
--rw-rw-rw-   0        0        0    10468 2023-04-09 05:50:46.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/core.py
--rw-rw-rw-   0        0        0     5507 2023-04-07 11:35:06.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware_casbin.py
--rw-rw-rw-   0        0        0     9185 2023-04-08 05:46:03.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware_session.py
--rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/view.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:40:46.440276 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/
--rw-rw-rw-   0        0        0     6265 2023-04-09 06:40:46.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-04-09 06:40:46.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:40:46.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-09 06:40:46.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 06:40:46.442270 fastapi_mvc_framework-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      721 2023-04-09 06:40:34.000000 fastapi_mvc_framework-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:37:51.651188 fastapi_mvc_framework-1.1.4/
+-rw-rw-rw-   0        0        0     7658 2023-04-10 07:37:51.650190 fastapi_mvc_framework-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5526 2023-04-10 07:37:34.000000 fastapi_mvc_framework-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 07:37:51.642209 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/
+-rw-rw-rw-   0        0        0      251 2023-04-06 06:00:47.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-04-07 07:39:59.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/_utils.py
+-rw-rw-rw-   0        0        0     9943 2023-04-09 05:56:58.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/auth.py
+-rw-rw-rw-   0        0        0     8826 2023-04-08 11:33:08.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/cbv.py
+-rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/config.py
+-rw-rw-rw-   0        0        0     3733 2023-04-09 05:46:23.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/controller.py
+-rw-rw-rw-   0        0        0    12971 2023-04-09 05:48:57.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/controller_utils.py
+-rw-rw-rw-   0        0        0    11236 2023-04-09 13:15:31.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/core.py
+-rw-rw-rw-   0        0        0     1710 2023-04-10 07:35:52.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/database.py
+-rw-rw-rw-   0        0        0     5507 2023-04-07 11:35:06.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware_casbin.py
+-rw-rw-rw-   0        0        0     9185 2023-04-08 05:46:03.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware_session.py
+-rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/view.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:37:51.648194 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/
+-rw-rw-rw-   0        0        0     7658 2023-04-10 07:37:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      682 2023-04-10 07:37:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 07:37:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-10 07:37:51.000000 fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 07:37:51.651188 fastapi_mvc_framework-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      721 2023-04-10 07:31:04.000000 fastapi_mvc_framework-1.1.4/setup.py
```

### Comparing `fastapi_mvc_framework-1.1.3/README.md` & `fastapi_mvc_framework-1.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # fastapi_framework
 A mvc framework used FastApi
 Simple and elegant use of FastApi in MVC mode
 
-usage:
-
+## usage:
+install:
+```bash
+pip install fastapi-mvc-framework
+```
 
+controller:
 ```python
-
 from fastapi_mvc_framework import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
-import requests,openai,json
-from typing import Dict
-from fastapi_mvc_framework import Form
- 
+from typing import Dict 
+from app.services import UserService
+
 application._public_auth_url = '/user/login'
 application._user_auth_url = '/user/login'
 
 @api_router(auth='public')
-class TestController(BaseController):
-    # _auth_url = '/user/login'
-    
+class TestController(BaseController): 
     @api.get("/user/login")
     def login(self):
-        """:title Login""" 
-        
-        redirect = self.params['redirect'] if 'redirect' in self.params else '/'
-       
+        """:title Login"""  
+        redirect = self.params['redirect'] if 'redirect' in self.params else '/' 
         return self.view() 
+    
     @api.get("/user/logout")
     def logout(self):
         return self._user_logout()
     
     @api.post("/test/verity_user")
     async def verity_user(self): 
         form = self.params
@@ -46,27 +45,25 @@
     
     @api.get("/" )
     def home(self,request:Request): 
         '''
         :title Home
         '''
         c = self.session.get('home',1)
-        c = c+1 
-        # #setting cookies   
-        # self.response.set_cookie('a',c) 
+        c = c+1  
         self.cookies["a"] = c
         if c>10:
             del self.cookies["a"]
             c = 0
         self.session['home'] = c
         text = "Hello World! I'm in FastapiMvcFramework"
         routers_map = application.routers_map
-        routers = application.routes
-         
+        routers = application.routes 
         return self.view()
+    
     @api.get("/xml",auth='user')
     def get_legacy_data(self):
         """:title XML(Protected)"""
 
         data = """<?xml version="1.0"?>
         <shampoo>
         <Header>
@@ -74,27 +71,23 @@
         </Header>
         <Body>
             You'll have to use soap here.
         </Body>
         </shampoo>
         """
         return self.view(content=data,media_type="application/xml")
-         
-
-     
+          
     @api.get("/chatgpt")
     def chatgpt(self):
         """
         :title Chat
         """
         return self.view()
 
 
- 
-
 ```
 
 home.html:
 
 ```html
 <body>
     <header>
@@ -116,54 +109,97 @@
     </section>
     <footer>
         <p>&copy; 2023 My Website</p>
     </footer>
 </body>
 ```
 
-your project directory structrue:
+your project directory structrue like this:
 ```
 +---app
 |   |   __init__.py
 |   |
 |   +---controllers
 |   |   |   test_controller.py
 |   |   |   __init__.py
 |   |   |
+|   +---models
+|   |   |   user_model.py
+|   |   |   __init__.py
+|   |   |
+|   +---services
+|   |   |   user_service.py
+|   |   |   __init__.py
+|   |   |
 |   +---views
-|   |   +---abc(controller name defined in app/controllers/test_controller.py)
+|   |   +---abc
 |   |   |   \---2.0
 |   |   |           css.css
 |   |   |           home.html
 |   |   |
-|   |   +---test 
+|   |   +---test
 |   |   |       chatgpt.css
 |   |   |       chatgpt.html
 |   |   |       chatgpt.js
 |   |   |       home.html
 |   |   |       home.js
 |   |   |       login.html
 |   |   |
-|   |   \---ws 
+|   |   \---ws
 |   |           ws_home.html
-├─app1
-│  ├─controllers
-│  │  └─...
-│  ├─views
-│  │  ├─test1
-│  │  │  └─v1.0
-│  │  └─test2
+|   |
++---app1
+|   |   __init__.py
+|   |
+|   +---controllers
+|   |   |   test1_controller.py
+|   |   |   __init__.py
+|   |   |
+|   |   \---__pycache__
+|   |           test1_controller.cpython-38.pyc
+|   |           __init__.cpython-38.pyc
+|   |
+|   +---views
+|   |   +---test1
+|   |   |   \---v1.0
+|   |   |           home.css
+|   |   |           home.html
+|   |   |           home1.css
+|   |   |
+|   |   \---test2
+|
 +---configs
+|       alembic.ini
 |       cache.yaml
 |       casbin-adapter.csv
 |       casbin-model.conf
 |       database.yaml
 |       general.yaml
 |       session.yaml
-+---public
-|       error_404.html
-|       error_500.html
-|       js.js
-└─sessions
- 
+|
++---data
+|   +---alembic
+|   |   |   env.py
+|   |   |   README
+|   |   |   script.py.mako
+|   |   |
+|   |   +---versions
+|   |   |   |   0d0205db5b39_create_tables.py
+|   |   |   |   0e4e15e67367_autogenerate.py
+|   |   |   |   108dad121227__new_upgrade_operations_detected__add_.py
+|   |   |   |   ac7ce07126b3_autogenerate.py
+|   |   |   |   e51711eb3d84_autogenerate.py
+|   |   |   |
+|   |   |   \---__pycache__
+|   |   |           0d0205db5b39_create_tables.cpython-38.pyc
+|   |   |           0e4e15e67367_autogenerate.cpython-38.pyc
+|   |   |           108dad121227__new_upgrade_operations_detected__add_.cpython-38.pyc
+|   |   |           ac7ce07126b3_autogenerate.cpython-38.pyc
+|   |   |           e51711eb3d84_autogenerate.cpython-38.pyc
+|   |   |
+|   |   \---__pycache__
+|   |           env.cpython-38.pyc
+|   |
+|   \---db
+|           test.db
 
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
 # fastapi_framework A mvc framework used FastApi Simple and elegant use of
-FastApi in MVC mode usage: ```python from fastapi_mvc_framework import
+FastApi in MVC mode ## usage: install: ```bash pip install fastapi-mvc-
+framework ``` controller: ```python from fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
-import requests,openai,json from typing import Dict from fastapi_mvc_framework
-import Form application._public_auth_url = '/user/login'
-application._user_auth_url = '/user/login' @api_router(auth='public') class
-TestController(BaseController): # _auth_url = '/user/login' @api.get("/user/
-login") def login(self): """:title Login""" redirect = self.params['redirect']
-if 'redirect' in self.params else '/' return self.view() @api.get("/user/
-logout") def logout(self): return self._user_logout() @api.post("/test/
-verity_user") async def verity_user(self): form = self.params username = form
-['username'] password = form['password'] redirect = form['redirect'] if
-username and password: #do veritied if username in ['bruce','alice'] and
-password: return self._verity_successed(username,redirect) else: return
-self._verity_error() return self._verity_error() @api.get("/" ) def home
-(self,request:Request): ''' :title Home ''' c = self.session.get('home',1) c =
-c+1 # #setting cookies # self.response.set_cookie('a',c) self.cookies["a"] = c
-if c>10: del self.cookies["a"] c = 0 self.session['home'] = c text = "Hello
-World! I'm in FastapiMvcFramework" routers_map = application.routers_map
-routers = application.routes return self.view() @api.get("/xml",auth='user')
-def get_legacy_data(self): """:title XML(Protected)""" data = """<?xml
+from typing import Dict from app.services import UserService
+application._public_auth_url = '/user/login' application._user_auth_url = '/
+user/login' @api_router(auth='public') class TestController(BaseController):
+@api.get("/user/login") def login(self): """:title Login""" redirect =
+self.params['redirect'] if 'redirect' in self.params else '/' return self.view
+() @api.get("/user/logout") def logout(self): return self._user_logout()
+@api.post("/test/verity_user") async def verity_user(self): form = self.params
+username = form['username'] password = form['password'] redirect = form
+['redirect'] if username and password: #do veritied if username in
+['bruce','alice'] and password: return self._verity_successed
+(username,redirect) else: return self._verity_error() return self._verity_error
+() @api.get("/" ) def home(self,request:Request): ''' :title Home ''' c =
+self.session.get('home',1) c = c+1 self.cookies["a"] = c if c>10: del
+self.cookies["a"] c = 0 self.session['home'] = c text = "Hello World! I'm in
+FastapiMvcFramework" routers_map = application.routers_map routers =
+application.routes return self.view() @api.get("/xml",auth='user') def
+get_legacy_data(self): """:title XML(Protected)""" data = """<?xml
 version="1.0"?>   Apply shampoo here.
 You'll have to use soap here.
  """ return self.view(content=data,media_type="application/xml") @api.get("/
 chatgpt") def chatgpt(self): """ :title Chat """ return self.view() ```
 home.html: ```html
 ****** My Website ******
   {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %}
@@ -32,17 +32,30 @@
 ***** Welcome to my website *****
 This is an example of a responsive design that works well on both desktop and
 mobile devices.
 here is the `text` variable in class method:{{text}}
 {{flash}}
 
 © 2023 My Website
-``` your project directory structrue: ``` +---app | | __init__.py | | | +---
-controllers | | | test_controller.py | | | __init__.py | | | | +---views | | +-
---abc(controller name defined in app/controllers/test_controller.py) | | | \---
-2.0 | | | css.css | | | home.html | | | | | +---test | | | chatgpt.css | | |
+``` your project directory structrue like this: ``` +---app | | __init__.py | |
+| +---controllers | | | test_controller.py | | | __init__.py | | | | +---models
+| | | user_model.py | | | __init__.py | | | | +---services | | |
+user_service.py | | | __init__.py | | | | +---views | | +---abc | | | \---2.0 |
+| | css.css | | | home.html | | | | | +---test | | | chatgpt.css | | |
 chatgpt.html | | | chatgpt.js | | | home.html | | | home.js | | | login.html |
-| | | | \---ws | | ws_home.html ââapp1 â ââcontrollers â â
-ââ... â ââviews â â ââtest1 â â â ââv1.0 â â
-ââtest2 +---configs | cache.yaml | casbin-adapter.csv | casbin-model.conf |
-database.yaml | general.yaml | session.yaml +---public | error_404.html |
-error_500.html | js.js ââsessions ```
+| | | | \---ws | | ws_home.html | | +---app1 | | __init__.py | | | +---
+controllers | | | test1_controller.py | | | __init__.py | | | | | \---
+__pycache__ | | test1_controller.cpython-38.pyc | | __init__.cpython-38.pyc | |
+| +---views | | +---test1 | | | \---v1.0 | | | home.css | | | home.html | | |
+home1.css | | | | | \---test2 | +---configs | alembic.ini | cache.yaml |
+casbin-adapter.csv | casbin-model.conf | database.yaml | general.yaml |
+session.yaml | +---data | +---alembic | | | env.py | | | README | | |
+script.py.mako | | | | | +---versions | | | | 0d0205db5b39_create_tables.py | |
+| | 0e4e15e67367_autogenerate.py | | | |
+108dad121227__new_upgrade_operations_detected__add_.py | | | |
+ac7ce07126b3_autogenerate.py | | | | e51711eb3d84_autogenerate.py | | | | | | |
+\---__pycache__ | | | 0d0205db5b39_create_tables.cpython-38.pyc | | |
+0e4e15e67367_autogenerate.cpython-38.pyc | | |
+108dad121227__new_upgrade_operations_detected__add_.cpython-38.pyc | | |
+ac7ce07126b3_autogenerate.cpython-38.pyc | | |
+e51711eb3d84_autogenerate.cpython-38.pyc | | | | | \---__pycache__ | |
+env.cpython-38.pyc | | | \---db | test.db ```
```

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/_utils.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/auth.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/base_controller.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/base_controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/cbv.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/cbv.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/config.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/controller.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/controller_utils.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/controller_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/core.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,40 +16,57 @@
 from .controller import create_controller,controller as api,   register_controllers_to_app 
 from .controller_utils import  TEMPLATE_PATH_KEY,AUTH_KEY, VER_KEY,get_docs  
 from .config import config,ROOT_PATH,_log
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
 from . import midware
 from . import auth
+from . import database
 
-
-__is_debug=False
+__is_debug=config.get('debug',False)
 
 class MvcApp(FastAPI):
     def __init__(self,  **kwargs):
         self._authObj:auth.AuthenticationBackend_ = None 
+        self._data_engine:database.Engine = None
         self._user_auth_url=""
         self._public_auth_url=""
         super().__init__(**kwargs)
     @property
     def authObj(self)->auth.AuthenticationBackend_:
         return self._authObj
+    
     @authObj.setter
     def authObj(self,value:auth.AuthenticationBackend_):
         self._authObj = value
     pass
+    @property 
+    def data_engine(self)->database.Engine:
+        return self._data_engine
+    @data_engine.setter
+    def data_engine(self,value):
+        self._data_engine = value
 
- 
 __app = MvcApp( ) 
 
 __app_views_dirs = {} 
 __all_controller__ = []
 
 application = __app
 
+def __init_database(): 
+    db_cfg = config.get("database")
+    db_uri:str = db_cfg.get("uri")
+    alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
+    if db_uri:
+        if db_uri.startswith('sqlite'):
+            db_directory = os.path.dirname(db_uri.split(':///')[1])
+            os.makedirs(db_directory, exist_ok=True) 
+        application.data_engine=database.init_database(db_uri,__is_debug, alembic_ini)
+
 def __init_auth(app,auth_type:str):
     __type_casbin_adapter = config.get("auth").get("casbin_adapter","file")
     casbin_adapter =  auth._adapters[__type_casbin_adapter] if __type_casbin_adapter in auth._adapters else None
     if not casbin_adapter:
         raise f"Not support {__type_casbin_adapter} ,Adapter config error in auth.casbin_adapter"
     
     auth_class = auth._auth_types[auth_type] if auth_type in auth._auth_types else None
@@ -199,15 +216,15 @@
 
 def generate_mvc_app(isDebug):
     if not len(__all_controller__)>0:
         raise "must use @api_route to define a controller class"
     all_routers = []
     all_routers_map = {}
     for ctrl in __all_controller__:
-        all_routers.append(register_controllers_to_app(__app, ctrl))
+        all_routers.append(register_controllers_to_app(application, ctrl))
     for router in all_routers:
         for r in router.routes:
             funcname = str(r.endpoint).split('<function ')[1].split(" at ")[0] 
             end_point_abs = get_wrapped_endpoint(r.endpoint)
             auth_type = getattr(end_point_abs,AUTH_KEY) if hasattr(end_point_abs,AUTH_KEY) else 'None'
             doc_map =  get_docs(r.description) if hasattr(r,'description') else {}
             if hasattr(r,'methods'):
@@ -220,18 +237,19 @@
     application.routers_map = all_routers_map  
     midware.init(app=application,debug=isDebug)
     
     auth_type = config.get("auth",None)
     if auth_type:
         auth_type=auth_type.get("type" )
         if auth_type:
-            application.authObj = __init_auth(__app,auth_type)
+            application.authObj = __init_auth(application,auth_type)
+    __init_database()
     return application
 
 def run(app,*args,**kwargs): 
     import uvicorn
     global __is_debug
     host =  "host" in kwargs  and kwargs["host"]  or '0.0.0.0' 
     port = "port" in kwargs  and kwargs["port"] or 8000  
-    __is_debug = "debug" in kwargs and kwargs["debug"]   
+    __is_debug = kwargs["debug"] if  "debug" in kwargs else False   
      
     uvicorn.run(app, host=host, port=port)
```

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware_casbin.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware_session.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/midware_session.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/view.py` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework/view.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/PKG-INFO` & `fastapi_mvc_framework-1.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
-Name: fastapi-mvc-framework
-Version: 1.1.3
+Name: fastapi_mvc_framework
+Version: 1.1.4
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: UNKNOWN
 Description: # fastapi_framework
         A mvc framework used FastApi
         Simple and elegant use of FastApi in MVC mode
         
-        usage:
-        
+        ## usage:
+        install:
+        ```bash
+        pip install fastapi-mvc-framework
+        ```
         
+        controller:
         ```python
-        
         from fastapi_mvc_framework import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
-        import requests,openai,json
-        from typing import Dict
-        from fastapi_mvc_framework import Form
-         
+        from typing import Dict 
+        from app.services import UserService
+        
         application._public_auth_url = '/user/login'
         application._user_auth_url = '/user/login'
         
         @api_router(auth='public')
-        class TestController(BaseController):
-            # _auth_url = '/user/login'
-            
+        class TestController(BaseController): 
             @api.get("/user/login")
             def login(self):
-                """:title Login""" 
-                
-                redirect = self.params['redirect'] if 'redirect' in self.params else '/'
-               
+                """:title Login"""  
+                redirect = self.params['redirect'] if 'redirect' in self.params else '/' 
                 return self.view() 
+            
             @api.get("/user/logout")
             def logout(self):
                 return self._user_logout()
             
             @api.post("/test/verity_user")
             async def verity_user(self): 
                 form = self.params
@@ -54,27 +53,25 @@
             
             @api.get("/" )
             def home(self,request:Request): 
                 '''
                 :title Home
                 '''
                 c = self.session.get('home',1)
-                c = c+1 
-                # #setting cookies   
-                # self.response.set_cookie('a',c) 
+                c = c+1  
                 self.cookies["a"] = c
                 if c>10:
                     del self.cookies["a"]
                     c = 0
                 self.session['home'] = c
                 text = "Hello World! I'm in FastapiMvcFramework"
                 routers_map = application.routers_map
-                routers = application.routes
-                 
+                routers = application.routes 
                 return self.view()
+            
             @api.get("/xml",auth='user')
             def get_legacy_data(self):
                 """:title XML(Protected)"""
         
                 data = """<?xml version="1.0"?>
                 <shampoo>
                 <Header>
@@ -82,27 +79,23 @@
                 </Header>
                 <Body>
                     You'll have to use soap here.
                 </Body>
                 </shampoo>
                 """
                 return self.view(content=data,media_type="application/xml")
-                 
-        
-             
+                  
             @api.get("/chatgpt")
             def chatgpt(self):
                 """
                 :title Chat
                 """
                 return self.view()
         
         
-         
-        
         ```
         
         home.html:
         
         ```html
         <body>
             <header>
@@ -124,59 +117,102 @@
             </section>
             <footer>
                 <p>&copy; 2023 My Website</p>
             </footer>
         </body>
         ```
         
-        your project directory structrue:
+        your project directory structrue like this:
         ```
         +---app
         |   |   __init__.py
         |   |
         |   +---controllers
         |   |   |   test_controller.py
         |   |   |   __init__.py
         |   |   |
+        |   +---models
+        |   |   |   user_model.py
+        |   |   |   __init__.py
+        |   |   |
+        |   +---services
+        |   |   |   user_service.py
+        |   |   |   __init__.py
+        |   |   |
         |   +---views
-        |   |   +---abc(controller name defined in app/controllers/test_controller.py)
+        |   |   +---abc
         |   |   |   \---2.0
         |   |   |           css.css
         |   |   |           home.html
         |   |   |
-        |   |   +---test 
+        |   |   +---test
         |   |   |       chatgpt.css
         |   |   |       chatgpt.html
         |   |   |       chatgpt.js
         |   |   |       home.html
         |   |   |       home.js
         |   |   |       login.html
         |   |   |
-        |   |   \---ws 
+        |   |   \---ws
         |   |           ws_home.html
-        ├─app1
-        │  ├─controllers
-        │  │  └─...
-        │  ├─views
-        │  │  ├─test1
-        │  │  │  └─v1.0
-        │  │  └─test2
+        |   |
+        +---app1
+        |   |   __init__.py
+        |   |
+        |   +---controllers
+        |   |   |   test1_controller.py
+        |   |   |   __init__.py
+        |   |   |
+        |   |   \---__pycache__
+        |   |           test1_controller.cpython-38.pyc
+        |   |           __init__.cpython-38.pyc
+        |   |
+        |   +---views
+        |   |   +---test1
+        |   |   |   \---v1.0
+        |   |   |           home.css
+        |   |   |           home.html
+        |   |   |           home1.css
+        |   |   |
+        |   |   \---test2
+        |
         +---configs
+        |       alembic.ini
         |       cache.yaml
         |       casbin-adapter.csv
         |       casbin-model.conf
         |       database.yaml
         |       general.yaml
         |       session.yaml
-        +---public
-        |       error_404.html
-        |       error_500.html
-        |       js.js
-        └─sessions
-         
+        |
+        +---data
+        |   +---alembic
+        |   |   |   env.py
+        |   |   |   README
+        |   |   |   script.py.mako
+        |   |   |
+        |   |   +---versions
+        |   |   |   |   0d0205db5b39_create_tables.py
+        |   |   |   |   0e4e15e67367_autogenerate.py
+        |   |   |   |   108dad121227__new_upgrade_operations_detected__add_.py
+        |   |   |   |   ac7ce07126b3_autogenerate.py
+        |   |   |   |   e51711eb3d84_autogenerate.py
+        |   |   |   |
+        |   |   |   \---__pycache__
+        |   |   |           0d0205db5b39_create_tables.cpython-38.pyc
+        |   |   |           0e4e15e67367_autogenerate.cpython-38.pyc
+        |   |   |           108dad121227__new_upgrade_operations_detected__add_.cpython-38.pyc
+        |   |   |           ac7ce07126b3_autogenerate.cpython-38.pyc
+        |   |   |           e51711eb3d84_autogenerate.cpython-38.pyc
+        |   |   |
+        |   |   \---__pycache__
+        |   |           env.cpython-38.pyc
+        |   |
+        |   \---db
+        |           test.db
         
         ```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.3 Summary:
+Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.4 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
 License: UNKNOWN Description: # fastapi_framework A mvc framework used FastApi
-Simple and elegant use of FastApi in MVC mode usage: ```python from
+Simple and elegant use of FastApi in MVC mode ## usage: install: ```bash pip
+install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
-import requests,openai,json from typing import Dict from fastapi_mvc_framework
-import Form application._public_auth_url = '/user/login'
-application._user_auth_url = '/user/login' @api_router(auth='public') class
-TestController(BaseController): # _auth_url = '/user/login' @api.get("/user/
-login") def login(self): """:title Login""" redirect = self.params['redirect']
-if 'redirect' in self.params else '/' return self.view() @api.get("/user/
-logout") def logout(self): return self._user_logout() @api.post("/test/
-verity_user") async def verity_user(self): form = self.params username = form
-['username'] password = form['password'] redirect = form['redirect'] if
-username and password: #do veritied if username in ['bruce','alice'] and
-password: return self._verity_successed(username,redirect) else: return
-self._verity_error() return self._verity_error() @api.get("/" ) def home
-(self,request:Request): ''' :title Home ''' c = self.session.get('home',1) c =
-c+1 # #setting cookies # self.response.set_cookie('a',c) self.cookies["a"] = c
-if c>10: del self.cookies["a"] c = 0 self.session['home'] = c text = "Hello
-World! I'm in FastapiMvcFramework" routers_map = application.routers_map
-routers = application.routes return self.view() @api.get("/xml",auth='user')
-def get_legacy_data(self): """:title XML(Protected)""" data = """<?xml
+from typing import Dict from app.services import UserService
+application._public_auth_url = '/user/login' application._user_auth_url = '/
+user/login' @api_router(auth='public') class TestController(BaseController):
+@api.get("/user/login") def login(self): """:title Login""" redirect =
+self.params['redirect'] if 'redirect' in self.params else '/' return self.view
+() @api.get("/user/logout") def logout(self): return self._user_logout()
+@api.post("/test/verity_user") async def verity_user(self): form = self.params
+username = form['username'] password = form['password'] redirect = form
+['redirect'] if username and password: #do veritied if username in
+['bruce','alice'] and password: return self._verity_successed
+(username,redirect) else: return self._verity_error() return self._verity_error
+() @api.get("/" ) def home(self,request:Request): ''' :title Home ''' c =
+self.session.get('home',1) c = c+1 self.cookies["a"] = c if c>10: del
+self.cookies["a"] c = 0 self.session['home'] = c text = "Hello World! I'm in
+FastapiMvcFramework" routers_map = application.routers_map routers =
+application.routes return self.view() @api.get("/xml",auth='user') def
+get_legacy_data(self): """:title XML(Protected)""" data = """<?xml
 version="1.0"?>   Apply shampoo here.
 You'll have to use soap here.
  """ return self.view(content=data,media_type="application/xml") @api.get("/
 chatgpt") def chatgpt(self): """ :title Chat """ return self.view() ```
 home.html: ```html
 ****** My Website ******
   {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %}
@@ -36,20 +36,33 @@
 ***** Welcome to my website *****
 This is an example of a responsive design that works well on both desktop and
 mobile devices.
 here is the `text` variable in class method:{{text}}
 {{flash}}
 
 © 2023 My Website
-``` your project directory structrue: ``` +---app | | __init__.py | | | +---
-controllers | | | test_controller.py | | | __init__.py | | | | +---views | | +-
---abc(controller name defined in app/controllers/test_controller.py) | | | \---
-2.0 | | | css.css | | | home.html | | | | | +---test | | | chatgpt.css | | |
+``` your project directory structrue like this: ``` +---app | | __init__.py | |
+| +---controllers | | | test_controller.py | | | __init__.py | | | | +---models
+| | | user_model.py | | | __init__.py | | | | +---services | | |
+user_service.py | | | __init__.py | | | | +---views | | +---abc | | | \---2.0 |
+| | css.css | | | home.html | | | | | +---test | | | chatgpt.css | | |
 chatgpt.html | | | chatgpt.js | | | home.html | | | home.js | | | login.html |
-| | | | \---ws | | ws_home.html ââapp1 â ââcontrollers â â
-ââ... â ââviews â â ââtest1 â â â ââv1.0 â â
-ââtest2 +---configs | cache.yaml | casbin-adapter.csv | casbin-model.conf |
-database.yaml | general.yaml | session.yaml +---public | error_404.html |
-error_500.html | js.js ââsessions ``` Platform: UNKNOWN Classifier:
+| | | | \---ws | | ws_home.html | | +---app1 | | __init__.py | | | +---
+controllers | | | test1_controller.py | | | __init__.py | | | | | \---
+__pycache__ | | test1_controller.cpython-38.pyc | | __init__.cpython-38.pyc | |
+| +---views | | +---test1 | | | \---v1.0 | | | home.css | | | home.html | | |
+home1.css | | | | | \---test2 | +---configs | alembic.ini | cache.yaml |
+casbin-adapter.csv | casbin-model.conf | database.yaml | general.yaml |
+session.yaml | +---data | +---alembic | | | env.py | | | README | | |
+script.py.mako | | | | | +---versions | | | | 0d0205db5b39_create_tables.py | |
+| | 0e4e15e67367_autogenerate.py | | | |
+108dad121227__new_upgrade_operations_detected__add_.py | | | |
+ac7ce07126b3_autogenerate.py | | | | e51711eb3d84_autogenerate.py | | | | | | |
+\---__pycache__ | | | 0d0205db5b39_create_tables.cpython-38.pyc | | |
+0e4e15e67367_autogenerate.cpython-38.pyc | | |
+108dad121227__new_upgrade_operations_detected__add_.cpython-38.pyc | | |
+ac7ce07126b3_autogenerate.cpython-38.pyc | | |
+e51711eb3d84_autogenerate.cpython-38.pyc | | | | | \---__pycache__ | |
+env.cpython-38.pyc | | | \---db | test.db ``` Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/SOURCES.txt` & `fastapi_mvc_framework-1.1.4/fastapi_mvc_framework.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 fastapi_mvc_framework/auth.py
 fastapi_mvc_framework/base_controller.py
 fastapi_mvc_framework/cbv.py
 fastapi_mvc_framework/config.py
 fastapi_mvc_framework/controller.py
 fastapi_mvc_framework/controller_utils.py
 fastapi_mvc_framework/core.py
+fastapi_mvc_framework/database.py
 fastapi_mvc_framework/midware.py
 fastapi_mvc_framework/midware_casbin.py
 fastapi_mvc_framework/midware_session.py
 fastapi_mvc_framework/view.py
 fastapi_mvc_framework.egg-info/PKG-INFO
 fastapi_mvc_framework.egg-info/SOURCES.txt
 fastapi_mvc_framework.egg-info/dependency_links.txt
```

### Comparing `fastapi_mvc_framework-1.1.3/setup.py` & `fastapi_mvc_framework-1.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='fastapi_mvc_framework',
-    version='1.1.3',
+    version='1.1.4',
     author='Bruce chou',
     author_email='smjkzsl@gmail.com',
     description='Simple and elegant use of FastApi in MVC mode',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     url='https://github.com/smjkzsl/fastapi_framework',
```


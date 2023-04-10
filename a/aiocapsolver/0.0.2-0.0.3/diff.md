# Comparing `tmp/aiocapsolver-0.0.2.tar.gz` & `tmp/aiocapsolver-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocapsolver-0.0.2.tar", last modified: Mon Apr 10 04:40:22 2023, max compression
+gzip compressed data, was "aiocapsolver-0.0.3.tar", last modified: Mon Apr 10 05:06:40 2023, max compression
```

## Comparing `aiocapsolver-0.0.2.tar` & `aiocapsolver-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 04:40:22.127786 aiocapsolver-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-04-10 03:23:54.000000 aiocapsolver-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1284 2023-04-10 04:40:22.126785 aiocapsolver-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-04-10 04:34:28.000000 aiocapsolver-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 04:40:22.100777 aiocapsolver-0.0.2/aiocapsolver/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:14:21.000000 aiocapsolver-0.0.2/aiocapsolver/__init__.py
--rw-rw-rw-   0        0        0     3761 2023-04-10 04:13:32.000000 aiocapsolver-0.0.2/aiocapsolver/capsolver.py
--rw-rw-rw-   0        0        0      161 2023-04-10 03:12:54.000000 aiocapsolver-0.0.2/aiocapsolver/captcha_error.py
--rw-rw-rw-   0        0        0       25 2023-04-10 03:12:54.000000 aiocapsolver-0.0.2/aiocapsolver/solution.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:40:22.123793 aiocapsolver-0.0.2/aiocapsolver.egg-info/
--rw-rw-rw-   0        0        0     1284 2023-04-10 04:40:21.000000 aiocapsolver-0.0.2/aiocapsolver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-04-10 04:40:22.000000 aiocapsolver-0.0.2/aiocapsolver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 04:40:21.000000 aiocapsolver-0.0.2/aiocapsolver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      194 2023-04-10 04:40:21.000000 aiocapsolver-0.0.2/aiocapsolver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 04:40:21.000000 aiocapsolver-0.0.2/aiocapsolver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 04:40:22.128784 aiocapsolver-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1403 2023-04-10 04:37:50.000000 aiocapsolver-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:06:40.829039 aiocapsolver-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-04-10 03:23:54.000000 aiocapsolver-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1284 2023-04-10 05:06:40.828039 aiocapsolver-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-04-10 04:34:28.000000 aiocapsolver-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 05:06:40.791030 aiocapsolver-0.0.3/aiocapsolver/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:14:21.000000 aiocapsolver-0.0.3/aiocapsolver/__init__.py
+-rw-rw-rw-   0        0        0     3896 2023-04-10 04:52:41.000000 aiocapsolver-0.0.3/aiocapsolver/capsolver.py
+-rw-rw-rw-   0        0        0      161 2023-04-10 03:12:54.000000 aiocapsolver-0.0.3/aiocapsolver/captcha_error.py
+-rw-rw-rw-   0        0        0       25 2023-04-10 03:12:54.000000 aiocapsolver-0.0.3/aiocapsolver/solution.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:06:40.825038 aiocapsolver-0.0.3/aiocapsolver.egg-info/
+-rw-rw-rw-   0        0        0     1284 2023-04-10 05:06:40.000000 aiocapsolver-0.0.3/aiocapsolver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-04-10 05:06:40.000000 aiocapsolver-0.0.3/aiocapsolver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:06:40.000000 aiocapsolver-0.0.3/aiocapsolver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      194 2023-04-10 05:06:40.000000 aiocapsolver-0.0.3/aiocapsolver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 05:06:40.000000 aiocapsolver-0.0.3/aiocapsolver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:06:40.829039 aiocapsolver-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-04-10 05:06:25.000000 aiocapsolver-0.0.3/setup.py
```

### Comparing `aiocapsolver-0.0.2/LICENSE` & `aiocapsolver-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocapsolver-0.0.2/PKG-INFO` & `aiocapsolver-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocapsolver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Async API wrapper for capsolver.com
 Home-page: UNKNOWN
 Author: Eli Chandler
 Author-email: eli.chandler@gmail.com
 License: UNKNOWN
 Keywords: python,captcha,solver,capsolver,api,wrapper
 Platform: UNKNOWN
```

### Comparing `aiocapsolver-0.0.2/README.md` & `aiocapsolver-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiocapsolver-0.0.2/aiocapsolver/capsolver.py` & `aiocapsolver-0.0.3/aiocapsolver/capsolver.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
     async def __create_session(self):
         if self.__session is aiohttp.ClientSession:
             await self.__session.close
         self.__session = aiohttp.ClientSession()
 
     async def get_balance(self) -> float:
-        data = await self.__post('getBalance')
+        data = await self.__post('getBalance', no_task=True)
         return data['balance']
 
     async def get_packages(self) -> list:
-        data = await self.__post('getBalance')
+        data = await self.__post('getBalance', no_task=True)
         return data['balance']
 
     async def solve_image_to_text(self, filepath, module='common', minimum_confidence=0.8, case=True):
         async with aiofiles.open(filepath, mode='rb') as file:
             image_data = await file.read()
             base64_data = base64.b64encode(image_data).decode('utf-8')
         return await self.__submit_task('ImageToTextTask', body=base64_data, module=module, score=minimum_confidence,
@@ -54,15 +54,15 @@
             }
         }
 
         data['task'].update(kwargs)
 
         return await self.__post('createTask', data)
 
-    async def __post(self, endpoint, data=None) -> dict:
+    async def __post(self, endpoint, data=None, no_task=False) -> dict:
         if data is None:
             data = {}
 
         data['clientKey'] = self.api_key
 
         if not self.__session:
             await self.__create_session()
@@ -73,14 +73,17 @@
 
         async with self.__session.post('https://api.capsolver.com/' + endpoint, headers=headers, json=data) as r:
             j = await r.json()
 
         if j['errorId'] == 1:
             raise (CaptchaError(j['errorCode'], j['errorDescription']))
 
+        if no_task == True:
+            return j
+
         task_id = j.get('taskId')
         status = j.get('status')
 
         if status == 'ready':
             return j.get('solution')
 
         if status == 'idle':
@@ -100,14 +103,15 @@
 
 async def main():
     api_key = os.environ.get('API_KEY')
     proxy = os.environ.get('PROXY')
     url = os.environ.get('TESTING_URL')
     sitekey = os.environ.get('TESTING_SITEKEY')
     solver = AsyncCapSolver(api_key)
+    print(await solver.get_balance())
     print(await solver.solve_cloudflare_turnstile(url, sitekey, proxy))
     await solver.close()
 
 
 if __name__ == '__main__':
     import os
     import asyncio
```

### Comparing `aiocapsolver-0.0.2/aiocapsolver.egg-info/PKG-INFO` & `aiocapsolver-0.0.3/aiocapsolver.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocapsolver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Async API wrapper for capsolver.com
 Home-page: UNKNOWN
 Author: Eli Chandler
 Author-email: eli.chandler@gmail.com
 License: UNKNOWN
 Keywords: python,captcha,solver,capsolver,api,wrapper
 Platform: UNKNOWN
```

### Comparing `aiocapsolver-0.0.2/setup.py` & `aiocapsolver-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Async API wrapper for capsolver.com'
 LONG_DESCRIPTION = 'An asynchronous API wrapper for capsolver.com, built to be reliable and versatile.'
 
 # Setting up
 setup(
     name="aiocapsolver",
     version=VERSION,
```


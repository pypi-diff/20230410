# Comparing `tmp/olist-loafer-3.0.8.tar.gz` & `tmp/olist-loafer-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olist-loafer-3.0.8.tar", max compression
+gzip compressed data, was "olist-loafer-3.0.9.tar", max compression
```

## Comparing `olist-loafer-3.0.8.tar` & `olist-loafer-3.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1083 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/LICENSE
--rw-r--r--   0        0        0     1676 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/README.md
--rw-r--r--   0        0        0        0 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/__init__.py
--rw-r--r--   0        0        0     2517 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/dispatchers.py
--rw-r--r--   0        0        0      237 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/exceptions.py
--rw-r--r--   0        0        0        0 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/ext/__init__.py
--rw-r--r--   0        0        0        0 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/ext/aws/__init__.py
--rw-r--r--   0        0        0     1920 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/ext/aws/bases.py
--rw-r--r--   0        0        0     1896 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/ext/aws/handlers.py
--rw-r--r--   0        0        0     1752 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/ext/aws/message_translators.py
--rw-r--r--   0        0        0     3301 2021-09-27 14:37:26.923980 olist-loafer-3.0.8/loafer/ext/aws/providers.py
--rw-r--r--   0        0        0     1130 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/ext/aws/routes.py
--rw-r--r--   0        0        0      329 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/ext/sentry.py
--rw-r--r--   0        0        0     2060 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/managers.py
--rw-r--r--   0        0        0      735 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/message_translators.py
--rw-r--r--   0        0        0      890 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/providers.py
--rw-r--r--   0        0        0     2938 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/routes.py
--rw-r--r--   0        0        0     2497 2021-09-25 11:54:05.667849 olist-loafer-3.0.8/loafer/runners.py
--rw-r--r--   0        0        0     1548 2021-09-25 12:45:54.182615 olist-loafer-3.0.8/loafer/utils.py
--rw-r--r--   0        0        0     1707 2021-09-27 14:37:26.923980 olist-loafer-3.0.8/pyproject.toml
--rw-r--r--   0        0        0     2478 2021-09-27 14:39:16.571384 olist-loafer-3.0.8/setup.py
--rw-r--r--   0        0        0     2845 2021-09-27 14:39:16.572251 olist-loafer-3.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/LICENSE
+-rw-r--r--   0        0        0     1676 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/README.md
+-rw-r--r--   0        0        0        0 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/__init__.py
+-rw-r--r--   0        0        0     2517 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/dispatchers.py
+-rw-r--r--   0        0        0      237 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/exceptions.py
+-rw-r--r--   0        0        0        0 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/aws/__init__.py
+-rw-r--r--   0        0        0     1920 2021-10-12 18:13:14.113715 olist-loafer-3.0.9/loafer/ext/aws/bases.py
+-rw-r--r--   0        0        0     1896 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/aws/handlers.py
+-rw-r--r--   0        0        0     1752 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/aws/message_translators.py
+-rw-r--r--   0        0        0     3356 2021-10-29 16:24:47.915708 olist-loafer-3.0.9/loafer/ext/aws/providers.py
+-rw-r--r--   0        0        0     1130 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/aws/routes.py
+-rw-r--r--   0        0        0      329 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/sentry.py
+-rw-r--r--   0        0        0     2060 2021-10-12 22:41:21.453715 olist-loafer-3.0.9/loafer/managers.py
+-rw-r--r--   0        0        0      735 2021-10-12 18:13:14.113715 olist-loafer-3.0.9/loafer/message_translators.py
+-rw-r--r--   0        0        0      890 2021-10-12 18:13:14.113715 olist-loafer-3.0.9/loafer/providers.py
+-rw-r--r--   0        0        0     2938 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/routes.py
+-rw-r--r--   0        0        0     2481 2021-10-29 17:20:45.775708 olist-loafer-3.0.9/loafer/runners.py
+-rw-r--r--   0        0        0     1548 2021-09-25 12:45:54.182615 olist-loafer-3.0.9/loafer/utils.py
+-rw-r--r--   0        0        0     1734 2021-10-29 17:20:45.785708 olist-loafer-3.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2478 2021-10-29 17:21:32.918672 olist-loafer-3.0.9/setup.py
+-rw-r--r--   0        0        0     2896 2021-10-29 17:21:32.919817 olist-loafer-3.0.9/PKG-INFO
```

### Comparing `olist-loafer-3.0.8/LICENSE` & `olist-loafer-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/README.md` & `olist-loafer-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/loafer/dispatchers.py` & `olist-loafer-3.0.9/loafer/dispatchers.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/loafer/ext/aws/bases.py` & `olist-loafer-3.0.9/loafer/ext/aws/bases.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/loafer/ext/aws/handlers.py` & `olist-loafer-3.0.9/loafer/ext/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/loafer/ext/aws/message_translators.py` & `olist-loafer-3.0.9/loafer/ext/aws/message_translators.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/loafer/ext/aws/providers.py` & `olist-loafer-3.0.9/loafer/ext/aws/providers.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from .bases import BaseSQSClient
 from loafer.exceptions import ProviderError
 from loafer.providers import AbstractProvider
 from loafer.utils import calculate_backoff_multiplier
 
 logger = logging.getLogger(__name__)
 
-VISIBILITY_TIMEOUT_LIMIT = 43200
-
 
 class SQSProvider(AbstractProvider, BaseSQSClient):
     def __init__(self, queue_name, options=None, **kwargs):
         self.queue_name = queue_name
         self._options = options or {}
         self._backoff_factor = self._options.pop("BackoffFactor", None)
         if self._backoff_factor is not None:
@@ -47,26 +45,29 @@
         if self._backoff_factor:
             backoff_multiplier = calculate_backoff_multiplier(
                 int(message["Attributes"]["ApproximateReceiveCount"]),
                 self._backoff_factor,
             )
 
             custom_visibility_timeout = round(backoff_multiplier * self._options.get("VisibilityTimeout", 30))
-            custom_visibility_timeout = min(custom_visibility_timeout, VISIBILITY_TIMEOUT_LIMIT)
             logger.info(
                 f"message not processed, receipt={receipt!r}, "
                 f"custom_visibility_timeout={custom_visibility_timeout!r}"
             )
             queue_url = await self.get_queue_url(self.queue_name)
-            async with self.get_client() as client:
-                return await client.change_message_visibility(
-                    QueueUrl=queue_url,
-                    ReceiptHandle=receipt,
-                    VisibilityTimeout=custom_visibility_timeout,
-                )
+            try:
+                async with self.get_client() as client:
+                    return await client.change_message_visibility(
+                        QueueUrl=queue_url,
+                        ReceiptHandle=receipt,
+                        VisibilityTimeout=custom_visibility_timeout,
+                    )
+            except botocore.exceptions.ClientError as exc:
+                if "InvalidParameterValue" not in str(exc):
+                    raise
 
     async def fetch_messages(self):
         logger.debug(f"fetching messages on {self.queue_name}")
         try:
             queue_url = await self.get_queue_url(self.queue_name)
             async with self.get_client() as client:
                 response = await client.receive_message(QueueUrl=queue_url, **self._options)
```

### Comparing `olist-loafer-3.0.8/loafer/ext/aws/routes.py` & `olist-loafer-3.0.9/loafer/ext/aws/routes.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/loafer/managers.py` & `olist-loafer-3.0.9/loafer/managers.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/loafer/message_translators.py` & `olist-loafer-3.0.9/loafer/message_translators.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/loafer/providers.py` & `olist-loafer-3.0.9/loafer/providers.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/loafer/routes.py` & `olist-loafer-3.0.9/loafer/routes.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/loafer/runners.py` & `olist-loafer-3.0.9/loafer/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def _cancel_all_tasks(self):
         to_cancel = asyncio.all_tasks(self.loop)
         if not to_cancel:
             return
         for task in to_cancel:
             task.cancel()
 
-        self.loop.run_until_complete(asyncio.gather(*to_cancel, loop=self.loop, return_exceptions=True))
+        self.loop.run_until_complete(asyncio.gather(*to_cancel, return_exceptions=True))
         for task in to_cancel:
             if task.cancelled():
                 continue
             if task.exception() is not None:
                 self.loop.call_exception_handler(
                     {
                         "message": "unhandled exception during asyncio.run() shutdown",
```

### Comparing `olist-loafer-3.0.8/loafer/utils.py` & `olist-loafer-3.0.9/loafer/utils.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.8/pyproject.toml` & `olist-loafer-3.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "-vv --cov=loafer --cov-report=term-missing"
 
 [tool.poetry]
 name = "olist-loafer"
-version = "3.0.8"
+version = "3.0.9"
 description = "Asynchronous message dispatcher for concurrent tasks processing"
 license = "MIT"
 authors = ["Olist <developers@olist.com>"]
 readme = "README.md"
 repository = "https://github.com/olist/olist-loafer/"
 keywords = ["asyncio", "message", "dispatcher", "tasks", "microservices"]
 classifiers = [
@@ -32,28 +32,26 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: System :: Distributed Computing",
 ]
-packages = [
-    {include = "loafer"}
-]
+packages = [{ include = "loafer" }]
 
 [tool.poetry.urls]
 "Download" = "https://github.com/olist/olist-loafer/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.10"
+python = ">=3.7,<3.11"
 aiobotocore = { version = "^1.0.0", extras = ["boto3"] }
 cached-property = "^1.3.0"
 
 [tool.poetry.dev-dependencies]
-asynctest = "*"
+asynctest = { version = "*", python = "<3.8" }
 pre-commit = "*"
 codecov = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-deadfixtures = "*"
```

### Comparing `olist-loafer-3.0.8/setup.py` & `olist-loafer-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['aiobotocore[boto3]>=1.0.0,<2.0.0', 'cached-property>=1.3.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'olist-loafer',
-    'version': '3.0.8',
+    'version': '3.0.9',
     'description': 'Asynchronous message dispatcher for concurrent tasks processing',
     'long_description': "[![PyPI latest](https://img.shields.io/pypi/v/olist-loafer.svg?maxAge=2592000)](https://pypi.python.org/pypi/loafer)\n[![Python versions](https://img.shields.io/pypi/pyversions/olist-loafer.svg?maxAge=2592000)](https://pypi.python.org/pypi/loafer)\n[![License](https://img.shields.io/pypi/l/loafer.svg?maxAge=2592000)](https://pypi.python.org/pypi/olist-loafer)\n[![CircleCI](https://circleci.com/gh/olist/olist-loafer/tree/main.svg?style=svg)](https://circleci.com/gh/olist/olist-loafer/tree/main)\n[![Olist Sponsor](https://img.shields.io/badge/sponsor-olist-53b5f6.svg?style=flat-square)](http://opensource.olist.com/)\n\n\n**olist-loafer** is an asynchronous message dispatcher for concurrent tasks processing, with the following features:\n\n* Encourages decoupling from message providers and consumers\n* Easy to extend and customize\n* Easy error handling, including integration with sentry\n* Easy to create one or multiple services\n* Generic Handlers\n* Amazon SQS integration\n\n---\n:information_source: Currently, only AWS SQS is supported\n\n---\n\n## How to use\n\nA simple message forwader, from ``source-queue`` to ``destination-queue``:\n\n```python\nfrom loafer.ext.aws.handlers import SQSHandler\nfrom loafer.ext.aws.routes import SQSRoute\nfrom loafer.managers import LoaferManager\n\nroutes = [\n    SQSRoute('source-queue', handler=SQSHandler('destination-queue')),\n]\n\nif __name__ == '__main__':\n    manager = LoaferManager(routes)\n    manager.run()\n```\n\n## How to contribute\n\nFork this repository, make changes and send us a pull request. We will review your changes and apply them. Before sending us your pull request please check if you wrote and ran tests:\n\n```bash\nmake test\n```\n",
     'author': 'Olist',
     'author_email': 'developers@olist.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/olist/olist-loafer/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.10',
+    'python_requires': '>=3.7,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `olist-loafer-3.0.8/PKG-INFO` & `olist-loafer-3.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: olist-loafer
-Version: 3.0.8
+Version: 3.0.9
 Summary: Asynchronous message dispatcher for concurrent tasks processing
 Home-page: https://github.com/olist/olist-loafer/
 License: MIT
 Keywords: asyncio,message,dispatcher,tasks,microservices
 Author: Olist
 Author-email: developers@olist.com
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: aiobotocore[boto3] (>=1.0.0,<2.0.0)
 Requires-Dist: cached-property (>=1.3.0,<2.0.0)
 Project-URL: Download, https://github.com/olist/olist-loafer/releases
```


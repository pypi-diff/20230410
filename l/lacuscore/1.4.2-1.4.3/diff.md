# Comparing `tmp/lacuscore-1.4.2.tar.gz` & `tmp/lacuscore-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.4.2.tar", max compression
+gzip compressed data, was "lacuscore-1.4.3.tar", max compression
```

## Comparing `lacuscore-1.4.2.tar` & `lacuscore-1.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.2/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.2/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.2/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.2/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    27998 2023-04-08 16:48:20.490890 lacuscore-1.4.2/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.2/lacuscore/py.typed
--rw-r--r--   0        0        0     1475 2023-04-09 10:56:54.694290 lacuscore-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 lacuscore-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.3/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.3/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.3/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.3/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    27996 2023-04-10 16:22:59.484951 lacuscore-1.4.3/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.3/lacuscore/py.typed
+-rw-r--r--   0        0        0     1470 2023-04-10 16:42:10.202694 lacuscore-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 lacuscore-1.4.3/PKG-INFO
```

### Comparing `lacuscore-1.4.2/LICENSE` & `lacuscore-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.2/README.md` & `lacuscore-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.2/lacuscore/lacus_monitoring.py` & `lacuscore-1.4.3/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.2/lacuscore/lacuscore.py` & `lacuscore-1.4.3/lacuscore/lacuscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,15 +524,14 @@
                     await capture.initialize_context()
                     playwright_result = await asyncio.wait_for(
                         capture.capture_page(
                             url, referer=to_capture.get('referer'),
                             depth=to_capture.get('depth', 0),
                             rendered_hostname_only=to_capture.get('rendered_hostname_only', True)),
                         timeout=self.max_capture_time)
-                    result = cast(CaptureResponse, playwright_result)
             except PlaywrightCaptureException as e:
                 logger.exception(f'Invalid parameters for the capture of {url} - {e}')
                 result = {'error': 'Invalid parameters for the capture of {url} - {e}'}
                 raise CaptureError
             except asyncio.CancelledError:
                 logger.warning(f'The capture of {url} has been cancelled.')
                 result = {'error': f'The capture of {url} has been cancelled.'}
@@ -542,22 +541,22 @@
                 result = {'error': f'The capture of {url} took longer than the allowed max capture time ({self.max_capture_time}s)'}
                 raise CaptureError
             except Exception as e:
                 logger.exception(f'Something went poorly {url} - {e}')
                 result = {'error': f'Something went poorly {url} - {e}'}
                 raise CaptureError
 
-            if hasattr(capture, 'should_retry') and capture.should_retry:
+            if capture.should_retry:
                 # PlaywrightCapture considers this capture elligible for a retry
                 logger.info('PlaywrightCapture considers it elligible for a retry.')
                 raise RetryCapture
         except RetryCapture:
             # Check if we already re-tried this capture
             if (current_retry := self.redis.get(f'lacus:capture_retry:{uuid}')) is None:
-                self.redis.setex(f'lacus:capture_retry:{uuid}', 300, self.max_retries)
+                self.redis.setex(f'lacus:capture_retry:{uuid}', self.max_capture_time * (self.max_retries + 1), self.max_retries)
             else:
                 self.redis.decr(f'lacus:capture_retry:{uuid}')
             if current_retry is None or int(current_retry.decode()) > 0:
                 logger.debug(f'Retrying {url}.')
                 # Just wait a little bit before retrying, expecially if it is the only capture in the queue
                 await asyncio.sleep(random.randint(5, 10))
                 retry = True
@@ -574,14 +573,15 @@
             else:
                 logger.warning(f'Unable to capture: {result["error"]}')
         except Exception as e:
             msg = f'Something unexpected happened with {url}: {e}'
             result = {'error': msg}
             logger.exception(msg)
         else:
+            result = cast(CaptureResponse, playwright_result)
             if start_time := self.redis.zscore('lacus:ongoing', uuid):
                 runtime = time.time() - start_time
                 logger.info(f'Successfully captured {url} - Runtime: {runtime}s')
                 result['runtime'] = runtime
             else:
                 logger.info(f'Successfully captured {url} - No Runtime.')
         finally:
```

### Comparing `lacuscore-1.4.2/pyproject.toml` & `lacuscore-1.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.4.2"
+version = "1.4.3"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -27,15 +27,15 @@
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.2"
 Sphinx = { version = "^6.1.3", optional = true }
-playwrightcapture = {extras = ["recaptcha"], version = "^1.19.1"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.19.3"}
 defang = "^0.5.3"
 ua-parser = "^0.16.1"
 redis = {version = "^4.5.4", extras = ["hiredis"]}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
@@ -43,9 +43,9 @@
 types-redis = {version = "^4.5.4.1"}
 mypy = "^1.2.0"
 types-requests = "^2.28.11.17"
 ipython = "^8.12.0"
 pytest = "^7.3.0"
 
 [build-system]
-requires = ["poetry_core>=1.2"]
+requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lacuscore-1.4.2/PKG-INFO` & `lacuscore-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.4.2
+Version: 1.4.3
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.19.1,<2.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.19.3,<2.0.0)
 Requires-Dist: redis[hiredis] (>=4.5.4,<5.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: ua-parser (>=0.16.1,<0.17.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
```


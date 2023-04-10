# Comparing `tmp/playwrightcapture-1.19.1.tar.gz` & `tmp/playwrightcapture-1.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.19.1.tar", max compression
+gzip compressed data, was "playwrightcapture-1.19.2.tar", max compression
```

## Comparing `playwrightcapture-1.19.1.tar` & `playwrightcapture-1.19.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.19.1/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.19.1/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.19.1/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    23599 2023-01-22 11:55:54.953807 playwrightcapture-1.19.1/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.19.1/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.19.1/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.19.1/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1739 2023-03-30 09:04:34.270138 playwrightcapture-1.19.1/pyproject.toml
--rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.19.1/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.19.2/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.19.2/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.19.2/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    24004 2023-04-10 14:58:24.358880 playwrightcapture-1.19.2/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.19.2/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.19.2/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.19.2/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1739 2023-04-10 14:59:35.323224 playwrightcapture-1.19.2/pyproject.toml
+-rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.19.2/PKG-INFO
```

### Comparing `playwrightcapture-1.19.1/LICENSE` & `playwrightcapture-1.19.2/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.1/README.md` & `playwrightcapture-1.19.2/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.1/playwrightcapture/capture.py` & `playwrightcapture-1.19.2/playwrightcapture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,10 +522,18 @@
         self.logger.debug('Capture done')
         return to_return
 
     async def __aexit__(self, exc_type: Any, exc: Any, tb: Any) -> None:
         if hasattr(self, '_temp_harfile'):
             os.unlink(self._temp_harfile.name)
 
-        await self.browser.close()
-        # This method *must* be awaited but for some reason, MyPy complains.
-        await self.playwright.stop()  # type: ignore
+        try:
+            await self.browser.close()
+        except Exception as e:
+            # We may land in a situation where the capture was forcefully closed and the browser is already closed
+            self.logger.info(f'Unable to close browser: {e}')
+        try:
+            # This method *must* be awaited but for some reason, MyPy complains.
+            await self.playwright.stop()  # type: ignore
+        except Exception as e:
+            # this should't happen, but just in case it does...
+            self.logger.info(f'Unable to stop playwright: {e}')
```

### Comparing `playwrightcapture-1.19.1/playwrightcapture/helpers.py` & `playwrightcapture-1.19.2/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.1/pyproject.toml` & `playwrightcapture-1.19.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.19.1"
+version = "1.19.2"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -19,15 +19,15 @@
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 playwright = "^1.32.1"
 dateparser = "^1.1.8"
-beautifulsoup4 = "^4.12.0"
+beautifulsoup4 = "^4.12.2"
 w3lib = "^2.1.1"
 lxml = "^4.9.2"
 requests = {version = "^2.28.2", optional = true}
 pydub = {version = "^0.25.1", optional = true}
 SpeechRecognition = {version = "^3.10.0", optional = true}
 
 [tool.poetry.extras]
```

### Comparing `playwrightcapture-1.19.1/PKG-INFO` & `playwrightcapture-1.19.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.19.1
+Version: 1.19.2
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: recaptcha
 Requires-Dist: SpeechRecognition (>=3.10.0,<4.0.0) ; extra == "recaptcha"
-Requires-Dist: beautifulsoup4 (>=4.12.0,<5.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: playwright (>=1.32.1,<2.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
 Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "recaptcha"
 Requires-Dist: w3lib (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/Lookyloo/PlaywrightCapture
```


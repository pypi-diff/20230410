# Comparing `tmp/playwrightcapture-1.19.2.tar.gz` & `tmp/playwrightcapture-1.19.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.19.2.tar", max compression
+gzip compressed data, was "playwrightcapture-1.19.3.tar", max compression
```

## Comparing `playwrightcapture-1.19.2.tar` & `playwrightcapture-1.19.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.19.2/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.19.2/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.19.2/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    24004 2023-04-10 14:58:24.358880 playwrightcapture-1.19.2/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.19.2/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.19.2/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.19.2/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1739 2023-04-10 14:59:35.323224 playwrightcapture-1.19.2/pyproject.toml
--rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.19.2/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.19.3/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.19.3/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.19.3/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    24242 2023-04-10 16:19:51.783864 playwrightcapture-1.19.3/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.19.3/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.19.3/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.19.3/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1739 2023-04-10 16:24:47.145542 playwrightcapture-1.19.3/pyproject.toml
+-rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.19.3/PKG-INFO
```

### Comparing `playwrightcapture-1.19.2/LICENSE` & `playwrightcapture-1.19.3/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.2/README.md` & `playwrightcapture-1.19.3/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.2/playwrightcapture/capture.py` & `playwrightcapture-1.19.3/playwrightcapture/capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,15 @@
                 except Error as e:
                     try:
                         error_msg = download.failure()
                         if not error_msg:
                             raise e
                         to_return['error'] = f"Error while downloading: {error_msg}"
                         self.logger.info(to_return['error'])
-                        self.retry = True
+                        self.should_retry = True
                     except Exception:
                         raise e
             else:
                 await page.bring_to_front()
 
                 # page instrumentation
                 await page.wait_for_timeout(5000)  # Wait 5 sec after document loaded
@@ -492,23 +492,25 @@
                 if depth > 0 and to_return.get('html') and to_return['html']:
                     to_return['children'] = []
                     depth -= 1
                     child_urls = get_links_from_rendered_page(page.url, to_return['html'], rendered_hostname_only)
                     self.logger.info(f'Capturing children, {len(child_urls)} URLs')
                     for url in child_urls:
                         self.logger.info(f'Capture child {url}')
-                        to_return['children'].append(await self.capture_page(url, page.url, page, depth))  # type: ignore
+                        to_return['children'].append(await self.capture_page(url=url, referer=page.url,  # type: ignore
+                                                                             page=page, depth=depth,
+                                                                             rendered_hostname_only=rendered_hostname_only))
                         try:
                             await page.go_back()
                         except PlaywrightTimeoutError as e:
                             self.logger.warning(f'Go back timed out, it is probably not a big deal: {e}')
 
         except PlaywrightTimeoutError as e:
             to_return['error'] = f"The capture took too long - {e.message}"
-            self.retry = True
+            self.should_retry = True
         except Error as e:
             to_return['error'] = e.message
             # TODO: check e.name and figure out if it is worth retrying or not.
             self.logger.critical(f'Something went poorly with {url}: {e.message}')
         finally:
             if not capturing_sub:
                 to_return['cookies'] = await self.context.cookies()
```

### Comparing `playwrightcapture-1.19.2/playwrightcapture/helpers.py` & `playwrightcapture-1.19.3/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.2/pyproject.toml` & `playwrightcapture-1.19.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.19.2"
+version = "1.19.3"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
```

### Comparing `playwrightcapture-1.19.2/PKG-INFO` & `playwrightcapture-1.19.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.19.2
+Version: 1.19.3
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```


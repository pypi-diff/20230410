# Comparing `tmp/xhs-0.1.0.tar.gz` & `tmp/xhs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.1.0.tar", last modified: Fri Apr  7 09:55:12 2023, max compression
+gzip compressed data, was "xhs-0.1.1.tar", last modified: Mon Apr 10 14:16:58 2023, max compression
```

## Comparing `xhs-0.1.0.tar` & `xhs-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 09:55:12.222416 xhs-0.1.0/
--rw-rw-rw-   0        0        0      909 2023-04-07 09:49:39.000000 xhs-0.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1086 2023-04-03 04:48:59.000000 xhs-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       85 2023-04-03 14:57:56.000000 xhs-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3014 2023-04-07 09:55:12.222416 xhs-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2023-04-06 10:28:30.000000 xhs-0.1.0/README.md
--rw-rw-rw-   0        0        0       62 2023-04-06 09:50:49.000000 xhs-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0      274 2023-04-07 09:55:12.223414 xhs-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1479 2023-04-05 13:04:46.000000 xhs-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:55:12.207497 xhs-0.1.0/tests/
--rw-rw-rw-   0        0        0      244 2023-04-05 13:14:58.000000 xhs-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2578 2023-04-06 07:52:54.000000 xhs-0.1.0/tests/test_help.py
--rw-rw-rw-   0        0        0     3108 2023-04-07 09:36:51.000000 xhs-0.1.0/tests/test_xhs.py
--rw-rw-rw-   0        0        0      102 2023-04-07 06:13:42.000000 xhs-0.1.0/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:55:12.213439 xhs-0.1.0/xhs/
--rw-rw-rw-   0        0        0      331 2023-04-06 09:42:14.000000 xhs-0.1.0/xhs/__init__.py
--rw-rw-rw-   0        0        0      465 2023-04-07 09:55:04.000000 xhs-0.1.0/xhs/__version__.py
--rw-rw-rw-   0        0        0    12557 2023-04-07 09:30:09.000000 xhs-0.1.0/xhs/core.py
--rw-rw-rw-   0        0        0       91 2023-04-06 08:24:03.000000 xhs-0.1.0/xhs/exception.py
--rw-rw-rw-   0        0        0     2070 2023-04-07 02:28:25.000000 xhs-0.1.0/xhs/help.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:55:12.221452 xhs-0.1.0/xhs.egg-info/
--rw-rw-rw-   0        0        0     3014 2023-04-07 09:55:12.000000 xhs-0.1.0/xhs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-04-07 09:55:12.000000 xhs-0.1.0/xhs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 09:55:12.000000 xhs-0.1.0/xhs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-07 09:55:12.000000 xhs-0.1.0/xhs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-04-07 09:55:12.000000 xhs-0.1.0/xhs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-07 09:55:12.000000 xhs-0.1.0/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:16:58.464274 xhs-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-10 14:16:45.000000 xhs-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-10 14:16:45.000000 xhs-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 14:16:45.000000 xhs-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-10 14:16:58.464274 xhs-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-10 14:16:45.000000 xhs-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-10 14:16:45.000000 xhs-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-10 14:16:58.464274 xhs-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-10 14:16:45.000000 xhs-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:16:58.460274 xhs-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-10 14:16:45.000000 xhs-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-10 14:16:45.000000 xhs-0.1.1/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-10 14:16:45.000000 xhs-0.1.1/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-10 14:16:45.000000 xhs-0.1.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:16:58.460274 xhs-0.1.1/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-10 14:16:45.000000 xhs-0.1.1/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-10 14:16:45.000000 xhs-0.1.1/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-04-10 14:16:45.000000 xhs-0.1.1/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 14:16:45.000000 xhs-0.1.1/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-10 14:16:45.000000 xhs-0.1.1/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:16:58.464274 xhs-0.1.1/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.1.0/LICENSE` & `xhs-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 ReaJason
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 ReaJason
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `xhs-0.1.0/PKG-INFO` & `xhs-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,94 @@
-Metadata-Version: 2.1
-Name: xhs
-Version: 0.1.0
-Summary: xiaohongshu crawl sdk.
-Home-page: https://github.com/ReaJason/xhs
-Author: ReaJason
-Author-email: reajason1225@gmail.com
-License: MIT
-Keywords: xhs crawl
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-
-<h1 align="center">
-🍰xhs
-</h1>
-
-[![](https://img.shields.io/github/license/ReaJason/17wanxiaoCheckin-Actions "协议")](https://github.com/ReaJason/17wanxiaoCheckin/blob/master/LICENSE)
-[![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
-[![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
-[![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
-
-</div>
-
-**xhs** is a crawling tool designed to extract data from [xiaohongshu website](https://www.xiaohongshu.com/explore)
-
-# Usage
-
-xhs is available on PyPI:
-
-```console
-$ python -m pip install xhs
-```
-
-basic usage:
-
-```python
-from xhs import FeedType, XhsClient
-
-cookie = "please get cookie in website"
-xhs_client = XhsClient(cookie)
-
-# get note info
-note_info = xhs_client.get_note_by_id("63db8819000000001a01ead1")
-
-# get user info
-user_info = xhs_client.get_user_info("5ff0e6410000000001008400")
-
-# get user notes
-user_notes = xhs_client.get_user_notes("63273a77000000002303cc9b")
-
-# search note
-notes = xhs_client.get_note_by_keyword("小红书")
-
-# get home recommend feed
-recommend_type = FeedType.RECOMMEND
-recommend_notes = xhs_client.get_home_feed(recommend_type)
-
-# more functions in development
-```
-
-Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
-
-use signature function:
-
-```python
-# sign get request
->>> from xhs import help
->>> help.sign("/api/sns/web/v1/user/otherinfo?target_user_id=5ff0e6410000000001008400")
-{'x-s': '1l5LsiTlZYavOYwvOid6OlU6OisCZ6dBZjvL1gsCOg13', 'x-t': '1680701208022'}
-
-# sign post request
->>> help.sign("/api/sns/web/v1/feed", {"source_note_id": "63db8819000000001a01ead1"})
-{'x-s': 'sY5LOg9WOYFKsYFWOBcis2MlsiFCsjMb0jTKZja6OjA3', 'x-t': '1680701310666'}
-
-# get search_id parameter
->>> help.get_search_id()
-'2BHU39J8HCTIW665YHFCW'
-```
+Metadata-Version: 2.1
+Name: xhs
+Version: 0.1.1
+Summary: xiaohongshu crawl sdk.
+Home-page: https://github.com/ReaJason/xhs
+Author: ReaJason
+Author-email: reajason1225@gmail.com
+License: MIT
+Keywords: xhs crawl
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+
+<h1 align="center">
+🍰xhs
+</h1>
+
+[![](https://static.pepy.tech/badge/xhs)](https://pepy.tech/project/xhs)
+[![](https://img.shields.io/github/license/ReaJason/xhs)](https://github.com/ReaJason/xhs/blob/master/LICENSE)
+[![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
+[![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
+[![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
+
+</div>
+
+**xhs** is a crawling tool designed to extract data from [xiaohongshu website](https://www.xiaohongshu.com/explore)
+
+# Usage
+
+xhs is available on PyPI:
+
+```console
+$ python -m pip install xhs
+```
+
+basic usage:
+
+```python
+from xhs import FeedType, XhsClient
+
+cookie = "please get cookie in website"
+xhs_client = XhsClient(cookie)
+
+# get note info
+note_info = xhs_client.get_note_by_id("63db8819000000001a01ead1")
+
+# get user info
+user_info = xhs_client.get_user_info("5ff0e6410000000001008400")
+
+# get user notes
+user_notes = xhs_client.get_user_notes("63273a77000000002303cc9b")
+
+# search note
+notes = xhs_client.get_note_by_keyword("小红书")
+
+# get home recommend feed
+recommend_type = FeedType.RECOMMEND
+recommend_notes = xhs_client.get_home_feed(recommend_type)
+
+# more functions in development
+```
+
+Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
+
+use signature function:
+
+```python
+# sign get request
+>>> from xhs import help
+>>> help.sign("/api/sns/web/v1/user/otherinfo?target_user_id=5ff0e6410000000001008400")
+{'x-s': '1l5LsiTlZYavOYwvOid6OlU6OisCZ6dBZjvL1gsCOg13', 'x-t': '1680701208022'}
+
+# sign post request
+>>> help.sign("/api/sns/web/v1/feed", {"source_note_id": "63db8819000000001a01ead1"})
+{'x-s': 'sY5LOg9WOYFKsYFWOBcis2MlsiFCsjMb0jTKZja6OjA3', 'x-t': '1680701310666'}
+
+# get search_id parameter
+>>> help.get_search_id()
+'2BHU39J8HCTIW665YHFCW'
+```
```

### Comparing `xhs-0.1.0/README.md` & `xhs-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,69 @@
-<div align="center">
-
-<h1 align="center">
-🍰xhs
-</h1>
-
-[![](https://img.shields.io/github/license/ReaJason/17wanxiaoCheckin-Actions "协议")](https://github.com/ReaJason/17wanxiaoCheckin/blob/master/LICENSE)
-[![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
-[![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
-[![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
-
-</div>
-
-**xhs** is a crawling tool designed to extract data from [xiaohongshu website](https://www.xiaohongshu.com/explore)
-
-# Usage
-
-xhs is available on PyPI:
-
-```console
-$ python -m pip install xhs
-```
-
-basic usage:
-
-```python
-from xhs import FeedType, XhsClient
-
-cookie = "please get cookie in website"
-xhs_client = XhsClient(cookie)
-
-# get note info
-note_info = xhs_client.get_note_by_id("63db8819000000001a01ead1")
-
-# get user info
-user_info = xhs_client.get_user_info("5ff0e6410000000001008400")
-
-# get user notes
-user_notes = xhs_client.get_user_notes("63273a77000000002303cc9b")
-
-# search note
-notes = xhs_client.get_note_by_keyword("小红书")
-
-# get home recommend feed
-recommend_type = FeedType.RECOMMEND
-recommend_notes = xhs_client.get_home_feed(recommend_type)
-
-# more functions in development
-```
-
-Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
-
-use signature function:
-
-```python
-# sign get request
->>> from xhs import help
->>> help.sign("/api/sns/web/v1/user/otherinfo?target_user_id=5ff0e6410000000001008400")
-{'x-s': '1l5LsiTlZYavOYwvOid6OlU6OisCZ6dBZjvL1gsCOg13', 'x-t': '1680701208022'}
-
-# sign post request
->>> help.sign("/api/sns/web/v1/feed", {"source_note_id": "63db8819000000001a01ead1"})
-{'x-s': 'sY5LOg9WOYFKsYFWOBcis2MlsiFCsjMb0jTKZja6OjA3', 'x-t': '1680701310666'}
-
-# get search_id parameter
->>> help.get_search_id()
-'2BHU39J8HCTIW665YHFCW'
-```
+<div align="center">
+
+<h1 align="center">
+🍰xhs
+</h1>
+
+[![](https://static.pepy.tech/badge/xhs)](https://pepy.tech/project/xhs)
+[![](https://img.shields.io/github/license/ReaJason/xhs)](https://github.com/ReaJason/xhs/blob/master/LICENSE)
+[![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
+[![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
+[![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
+
+</div>
+
+**xhs** is a crawling tool designed to extract data from [xiaohongshu website](https://www.xiaohongshu.com/explore)
+
+# Usage
+
+xhs is available on PyPI:
+
+```console
+$ python -m pip install xhs
+```
+
+basic usage:
+
+```python
+from xhs import FeedType, XhsClient
+
+cookie = "please get cookie in website"
+xhs_client = XhsClient(cookie)
+
+# get note info
+note_info = xhs_client.get_note_by_id("63db8819000000001a01ead1")
+
+# get user info
+user_info = xhs_client.get_user_info("5ff0e6410000000001008400")
+
+# get user notes
+user_notes = xhs_client.get_user_notes("63273a77000000002303cc9b")
+
+# search note
+notes = xhs_client.get_note_by_keyword("小红书")
+
+# get home recommend feed
+recommend_type = FeedType.RECOMMEND
+recommend_notes = xhs_client.get_home_feed(recommend_type)
+
+# more functions in development
+```
+
+Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
+
+use signature function:
+
+```python
+# sign get request
+>>> from xhs import help
+>>> help.sign("/api/sns/web/v1/user/otherinfo?target_user_id=5ff0e6410000000001008400")
+{'x-s': '1l5LsiTlZYavOYwvOid6OlU6OisCZ6dBZjvL1gsCOg13', 'x-t': '1680701208022'}
+
+# sign post request
+>>> help.sign("/api/sns/web/v1/feed", {"source_note_id": "63db8819000000001a01ead1"})
+{'x-s': 'sY5LOg9WOYFKsYFWOBcis2MlsiFCsjMb0jTKZja6OjA3', 'x-t': '1680701310666'}
+
+# get search_id parameter
+>>> help.get_search_id()
+'2BHU39J8HCTIW665YHFCW'
+```
```

### Comparing `xhs-0.1.0/tests/test_help.py` & `xhs-0.1.1/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.0/tests/test_xhs.py` & `xhs-0.1.1/tests/test_xhs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,114 @@
-import pytest
-
-from xhs import FeedType, XhsClient
-
-from .utils import beauty_print
-
-
-@pytest.fixture
-def xhs_client():
-    return XhsClient(
-        cookie=('webId=e3455f4405340fc431af976dbf3de167;'
-                "web_session=040069b253793fdd9ccd9bd21c364b0033a638;"))
-
-
-def test_init_with_session_id():
-    cookie = "123123"
-    xhs_client = XhsClient(cookie)
-    assert xhs_client.get_cookie() == cookie
-
-
-def test_get_note_by_id(xhs_client: XhsClient):
-    note_id = "6413cf6b00000000270115b5"
-    data = xhs_client.get_note_by_id(note_id)
-    beauty_print(data)
-    assert data["note_id"] == note_id
-
-
-def test_get_self_info(xhs_client: XhsClient):
-    data = xhs_client.get_self_info()
-    beauty_print(data)
-    assert isinstance(data, dict)
-
-
-def test_get_user_info(xhs_client: XhsClient):
-    user_id = "5ff0e6410000000001008400"
-    data = xhs_client.get_user_info(user_id)
-    basic_info = data["basic_info"]
-    beauty_print(data)
-    assert (basic_info["red_id"] == "hh06ovo"
-            or basic_info["nickname"] == "小王不爱睡")
-
-
-def test_get_home_feed(xhs_client: XhsClient):
-    recommend_type = FeedType.RECOMMEND
-    data = xhs_client.get_home_feed(recommend_type)
-    beauty_print(data)
-    assert len(data["items"]) > 0
-
-
-def test_get_note_by_keyword(xhs_client: XhsClient):
-    keyword = "小红书"
-    data = xhs_client.get_note_by_keyword(keyword)
-    beauty_print(data)
-    assert len(data["items"]) > 0
-
-
-def test_get_user_notes(xhs_client: XhsClient):
-    user_id = "63273a77000000002303cc9b"
-    data = xhs_client.get_user_notes(user_id)
-    beauty_print(data)
-    assert len(data["notes"]) > 0
-
-
-def test_get_qrcode(xhs_client: XhsClient):
-    data = xhs_client.get_qrcode()
-    beauty_print(data)
-    assert data["url"].startswith("xhsdiscover://")
-
-
-@pytest.mark.skip()
-def test_check_qrcode(xhs_client: XhsClient):
-    data = xhs_client.check_qrcode("901061680834121471", "658742")
-    assert data.get("code_status")
-
-
-@pytest.mark.skip()
-def test_comment_note(xhs_client: XhsClient):
-    data = xhs_client.comment_note("642b96640000000014027cd2", "你最好说你在说你自己")
-    beauty_print(data)
-    assert data["comment"]["id"]
-
-
-@pytest.mark.skip()
-def test_comment_user(xhs_client: XhsClient):
-    data = xhs_client.comment_user("642b96640000000014027cd2",
-                                   "642f801000000000150037f8",
-                                   "我评论你了")
-    beauty_print(data)
-    assert data["comment"]["id"]
-
-
-@pytest.mark.skip()
-def test_delete_comment(xhs_client: XhsClient):
-    data = xhs_client.delete_note_comment("642b96640000000014027cd2",
-                                          "642f801000000000150037f8")
-    beauty_print(data)
-
-
-@pytest.mark.parametrize("note_id", [
-        "6413cf6b00000000270115b5",
-        "641718a200000000130143f2"
-    ])
-@pytest.mark.skip()
-def test_save_files_from_note_id(xhs_client: XhsClient, note_id: str):
-    xhs_client.save_files_from_note_id(note_id, r"C:\Users\ReaJason\Desktop")
+import pytest
+
+from xhs import FeedType, XhsClient
+
+from .utils import beauty_print
+
+
+@pytest.fixture
+def xhs_client():
+    return XhsClient(
+        cookie=('webId=e3455f4405340fc431af976dbf3de167;'
+                "web_session=040069b253793fdd9ccd9a5f01364b856d4088"))
+
+
+def test_init_with_session_id():
+    cookie = "123123"
+    xhs_client = XhsClient(cookie)
+    assert xhs_client.get_cookie() == cookie
+
+
+def test_get_note_by_id(xhs_client: XhsClient):
+    note_id = "6413cf6b00000000270115b5"
+    data = xhs_client.get_note_by_id(note_id)
+    beauty_print(data)
+    assert data["note_id"] == note_id
+
+
+def test_get_self_info(xhs_client: XhsClient):
+    data = xhs_client.get_self_info()
+    beauty_print(data)
+    assert isinstance(data, dict)
+
+
+def test_get_user_info(xhs_client: XhsClient):
+    user_id = "5ff0e6410000000001008400"
+    data = xhs_client.get_user_info(user_id)
+    basic_info = data["basic_info"]
+    beauty_print(data)
+    assert (basic_info["red_id"] == "hh06ovo"
+            or basic_info["nickname"] == "小王不爱睡")
+
+
+def test_get_home_feed(xhs_client: XhsClient):
+    recommend_type = FeedType.RECOMMEND
+    data = xhs_client.get_home_feed(recommend_type)
+    beauty_print(data)
+    assert len(data["items"]) > 0
+
+
+def test_get_note_by_keyword(xhs_client: XhsClient):
+    keyword = "小红书"
+    data = xhs_client.get_note_by_keyword(keyword)
+    beauty_print(data)
+    assert len(data["items"]) > 0
+
+
+def test_get_user_notes(xhs_client: XhsClient):
+    user_id = "63273a77000000002303cc9b"
+    data = xhs_client.get_user_notes(user_id)
+    beauty_print(data)
+    assert len(data["notes"]) > 0
+
+
+def test_get_qrcode(xhs_client: XhsClient):
+    data = xhs_client.get_qrcode()
+    beauty_print(data)
+    assert data["url"].startswith("xhsdiscover://")
+
+
+@pytest.mark.skip()
+def test_check_qrcode(xhs_client: XhsClient):
+    data = xhs_client.check_qrcode("901061680834121471", "658742")
+    assert data.get("code_status")
+
+
+@pytest.mark.skip()
+def test_comment_note(xhs_client: XhsClient):
+    data = xhs_client.comment_note("642b96640000000014027cd2", "你最好说你在说你自己")
+    beauty_print(data)
+    assert data["comment"]["id"]
+
+
+@pytest.mark.skip()
+def test_comment_user(xhs_client: XhsClient):
+    data = xhs_client.comment_user("642b96640000000014027cd2",
+                                   "642f801000000000150037f8",
+                                   "我评论你了")
+    beauty_print(data)
+    assert data["comment"]["id"]
+
+
+@pytest.mark.skip()
+def test_delete_comment(xhs_client: XhsClient):
+    data = xhs_client.delete_note_comment("642b96640000000014027cd2",
+                                          "642f801000000000150037f8")
+    beauty_print(data)
+
+
+@pytest.mark.parametrize("note_id", [
+        "6413cf6b00000000270115b5",
+        "641718a200000000130143f2"
+    ])
+@pytest.mark.skip()
+def test_save_files_from_note_id(xhs_client: XhsClient, note_id: str):
+    xhs_client.save_files_from_note_id(note_id, r"C:\Users\ReaJason\Desktop")
+
+
+@pytest.mark.parametrize("note_id", [
+    "639a7064000000001f0098a8",
+    "635d06790000000015020497"
+])
+@pytest.mark.skip()
+def test_save_files_from_note_id_invalid_title(xhs_client: XhsClient, note_id):
+    xhs_client.save_files_from_note_id(note_id, r"C:\Users\ReaJason\Desktop")
```

### Comparing `xhs-0.1.0/xhs/core.py` & `xhs-0.1.1/xhs/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,344 +1,391 @@
-import json
-import os
-from enum import Enum
-
-import requests
-
-from xhs.exception import DataFetchError
-
-from .help import get_search_id, sign
-
-
-class FeedType(Enum):
-    # 推荐
-    RECOMMEND = "homefeed_recommend"
-    # 穿搭
-    FASION = "homefeed.fashion_v3"
-    # 美食
-    FOOD = "homefeed.food_v3"
-    # 彩妆
-    COSMETICS = "homefeed.cosmetics_v3"
-    # 影视
-    MOVIE = "homefeed.movie_and_tv_v3"
-    # 职场
-    CAREER = "homefeed.career_v3"
-    # 情感
-    EMOTION = "homefeed.love_v3"
-    # 家居
-    HOURSE = "homefeed.household_product_v3"
-    # 游戏
-    GAME = "homefeed.gaming_v3"
-    # 旅行
-    TRAVEL = "homefeed.travel_v3"
-    # 健身
-    FITNESS = "homefeed.fitness_v3"
-
-
-class NoteType(Enum):
-    NOMAL = "nomal"
-    VIDEO = "video"
-
-
-def download_file(url: str, filename: str):
-    with requests.get(url, stream=True) as r:
-        r.raise_for_status()
-        with open(filename, 'wb') as f:
-            for chunk in r.iter_content(chunk_size=8192):
-                f.write(chunk)
-
-
-def get_img_url_by_trace_id(trace_id: str):
-    return f"https://sns-img-bd.xhscdn.com/{trace_id}?imageView2/format/png"
-
-
-class XhsClient:
-    def __init__(self,
-                 cookie=None,
-                 user_agent=None,
-                 timeout=10,
-                 proxies=None):
-        """constructor
-
-        :param cookie: get it form your website, defaults to None
-        :type cookie: str, optional
-        :param user_agent: requests user agent, defaults to None
-        :type user_agent: str, optional
-        :param timeout: requests timeout, defaults to None
-        :type timeout: int, optional
-        :param proxies: requests proxies, defaults to None
-        :type proxies: dict, optional
-        """
-        self._user_agent = user_agent or ("Mozilla/5.0 "
-                                          "(Windows NT 10.0; Win64; x64) "
-                                          "AppleWebKit/537.36 "
-                                          "(KHTML, like Gecko) "
-                                          "Chrome/111.0.0.0 Safari/537.36")
-        self._cookie = cookie
-        self._proxies = proxies
-        self._session: requests.Session = requests.session()
-        self._timeout = timeout
-        self._host = "https://edith.xiaohongshu.com"
-
-    def set_cookie(self, cookie: str):
-        self._cookie = cookie
-
-    def get_cookie(self):
-        return self._cookie
-
-    def get_user_agent(self):
-        return self._user_agent
-
-    def set_user_agent(self, user_agent: str):
-        self._user_agent = user_agent
-
-    def get_proxies(self):
-        return self._proxies
-
-    def set_proxies(self, proxies: dict):
-        self._proxies = proxies
-
-    def get_timeout(self):
-        return self._timeout
-
-    def set_timeout(self, timeout):
-        self._timeout = timeout
-
-    def _pre_headers(self, url: str, data=None):
-        assert self._cookie
-        signs = sign(url, data)
-        return {
-            "User-Agent": self._user_agent,
-            "cookie": self._cookie,
-            "x-s": signs["x-s"],
-            "x-t": signs["x-t"],
-            "Content-Type": "application/json"
-        }
-
-    def request(self, method, url, **kwargs):
-        response = self._session.request(
-            method, url, timeout=self._timeout,
-            proxies=self._proxies, **kwargs)
-        data = response.json()
-        if data["success"]:
-            return data.get("data", data.get("success"))
-        else:
-            raise DataFetchError(data.get("msg", None))
-
-    def get(self, uri: str, params=None):
-        final_uri = uri
-        if isinstance(params, dict):
-            final_uri = (f"{uri}?"
-                         f"{'&'.join([f'{k}={v}'for k,v in params.items()])}")
-        headers = self._pre_headers(final_uri)
-        return self.request(method="GET", url=f"{self._host}{final_uri}",
-                            headers=headers)
-
-    def post(self, uri: str, data: dict):
-        headers = self._pre_headers(uri, data)
-        json_str = json.dumps(data, separators=(',', ':'), ensure_ascii=False)
-        return self.request(method="POST", url=f"{self._host}{uri}",
-                            data=json_str.encode("utf-8"),
-                            headers=headers)
-
-    def get_note_by_id(self, note_id: str):
-        """
-        :param note_id: note_id you want to fetch
-        :type note_id: str
-        :return: {"time":1679019883000,"user":{"nickname":"nickname","avatar":"avatar","user_id":"user_id"},"image_list":[{"url":"https://sns-img-qc.xhscdn.com/c8e505ca-4e5f-44be-fe1c-ca0205a38bad","trace_id":"1000g00826s57r6cfu0005ossb1e9gk8c65d0c80","file_id":"c8e505ca-4e5f-44be-fe1c-ca0205a38bad","height":1920,"width":1440}],"tag_list":[{"id":"5be78cdfdb601f000100d0bc","name":"jk","type":"topic"}],"desc":"裙裙","interact_info":{"followed":false,"liked":false,"liked_count":"1732","collected":false,"collected_count":"453","comment_count":"30","share_count":"41"},"at_user_list":[],"last_update_time":1679019884000,"note_id":"6413cf6b00000000270115b5","type":"normal","title":"title"}
-        :rtype: dict
-        """
-        data = {"source_note_id": note_id}
-        uri = "/api/sns/web/v1/feed"
-        res = self.post(uri, data)
-        return res["items"][0]["note_card"]
-
-    def save_files_from_note_id(self, note_id: str, dir_path: str):
-        """this function will fetch note and save file in dir_path/note_title
-
-        :param note_id: note_id that you want to fetch
-        :type note_id: str
-        :param dir_path: in fact, files will be stored in your dir_path/note_title directory
-        :type dir_path: str
-        """
-        note = self.get_note_by_id(note_id)
-        title = note["title"]
-
-        new_dir_path = os.path.join(dir_path, title)
-        if not os.path.exists(new_dir_path):
-            os.mkdir(new_dir_path)
-
-        if note["type"] == NoteType.VIDEO.value:
-            video = next(filter(lambda value: len(value), note["video"]["media"]["stream"].values()))[0]
-            video_url = video["master_url"]
-            video_filename = os.path.join(new_dir_path, f"{title}.mp4")
-            download_file(video_url, video_filename)
-        else:
-            imgs = note["image_list"]
-            for index, img in enumerate(imgs):
-                img_url = get_img_url_by_trace_id(img["trace_id"])
-                img_file_name = os.path.join(new_dir_path, f"{title}{index}.png")
-                download_file(img_url, img_file_name)
-
-    def get_self_info(self):
-        uri = "/api/sns/web/v1/user/selfinfo"
-        res = self.get(uri)
-        return res
-
-    def get_user_info(self, user_id: str):
-        """
-        :param user_id: user_id you want fetch
-        :type user_id: str
-        :return: {"basic_info":{"imageb":"imageb","nickname":"nickname","images":"images","red_id":"red_id","gender":1,"ip_location":"ip_location","desc":"desc"},"interactions":[{"count":"5","type":"follows","name":"关注"},{"type":"fans","name":"粉丝","count":"16736"},{"type":"interaction","name":"获赞与收藏","count":"293043"}],"tags":[{"icon":"icon","tagType":"info"}],"tab_public":{"collection":false},"extra_info":{"fstatus":"none"},"result":{"success":true,"code":0,"message":"success"}}
-        :rtype: dict
-        """
-        uri = "/api/sns/web/v1/user/otherinfo"
-        params = {
-            "target_user_id": user_id
-        }
-        return self.get(uri, params)
-
-    def get_home_feed(self, feed_type: FeedType):
-        uri = "/api/sns/web/v1/homefeed"
-        data = {
-            "cursor_score": "",
-            "num": 40,
-            "refresh_type": 1,
-            "note_index": 0,
-            "unread_begin_note_id": "",
-            "unread_end_note_id": "",
-            "unread_note_count": 0,
-            "category": feed_type.value
-        }
-        return self.post(uri, data)
-
-    def get_note_by_keyword(self, keyword: str):
-        uri = "/api/sns/web/v1/search/notes"
-        data = {
-            "keyword": keyword,
-            "page": 1,
-            "page_size": 20,
-            "search_id": get_search_id(),
-            "sort": "general",
-            "note_type": 0
-        }
-        return self.post(uri, data)
-
-    def get_user_notes(self, user_id: str, cursor: str = ""):
-        uri = "/api/sns/web/v1/user_posted"
-        params = {
-            "num": 30,
-            "cursor": cursor,
-            "user_id": user_id
-        }
-        return self.get(uri, params)
-
-    def comment_note(self, note_id: str, content: str):
-        """comment a note
-
-        :return: {"time":1680834576180,"toast":"评论已发布","comment":{"id":"id","note_id":"note_id","status":2,"liked":false,"show_tags":["is_author"],"ip_location":"ip_location","content":"content","at_users":[],"like_count":"0","user_info":{"image":"**","user_id":"user_id","nickname":"nickname"},"create_time":create_time}}
-        :rtype: dict
-        """
-        uri = "/api/sns/web/v1/comment/post"
-        data = {
-            "note_id": note_id,
-            "content": content,
-            "at_users": []
-        }
-        return self.post(uri, data)
-
-    def delete_note_comment(self, note_id: str, comment_id: str):
-        uri = "/api/sns/web/v1/comment/delete"
-        data = {
-            "note_id": note_id,
-            "comment_id": comment_id
-        }
-        return self.post(uri, data)
-
-    def comment_user(self, note_id: str, comment_id: str, content: str):
-        """
-        :return: {"comment":{"like_count":"0","user_info":{"user_id":user_id"user_id":"user_id","image":"image"},"show_tags":["is_author"],"ip_location":"ip_location","id":"id","content":"content","at_users":[],"create_time":1680847204059,"target_comment":{"id":"id","user_info":{"user_id":"user_id","nickname":"nickname","image":"image"}},"note_id":"note_id","status":2,"liked":false},"time":1680847204089,"toast":"你的回复已发布"}
-        :rtype: dict
-        """
-        uri = "/api/sns/web/v1/comment/post"
-        data = {
-            "note_id": note_id,
-            "content": content,
-            "target_comment_id": comment_id,
-            "at_users": []
-        }
-        return self.post(uri, data)
-
-    def follow_user(self, user_id: str):
-        uri = "/api/sns/web/v1/user/follow"
-        data = {
-            "target_user_id": user_id
-        }
-        return self.post(uri, data)
-
-    def unfollow_user(self, user_id: str):
-        uri = "/api/sns/web/v1/user/unfollow"
-        data = {
-            "target_user_id": user_id
-        }
-        return self.post(uri, data)
-
-    def collect_note(self, note_id: str):
-        uri = "/api/sns/web/v1/note/collect"
-        data = {
-            "note_id": note_id
-        }
-        return self.post(uri, data)
-
-    def uncollect_note(self, note_id: str):
-        uri = "/api/sns/web/v1/note/uncollect"
-        data = {
-            "note_ids": note_id
-        }
-        return self.post(uri, data)
-
-    def like_note(self, note_id: str):
-        uri = "/api/sns/web/v1/note/like"
-        data = {
-            "note_oid": note_id
-        }
-        return self.post(uri, data)
-
-    def like_comment(self, note_id: str, comment_id: str):
-        uri = "/api/sns/web/v1/comment/like"
-        data = {
-            "note_id": note_id,
-            "comment_id": comment_id
-        }
-        return self.post(uri, data)
-
-    def dislike_note(self, note_id: str):
-        uri = "/api/sns/web/v1/note/dislike"
-        data = {
-            "note_oid": note_id
-        }
-        return self.post(uri, data)
-
-    def dislike_comment(self, comment_id: str):
-        uri = "/api/sns/web/v1/comment/dislike"
-        data = {
-            "note_oid": comment_id
-        }
-        return self.post(uri, data)
-
-    def get_qrcode(self):
-        """create qrcode, you can trasform response url to qrcode
-
-        :return: {"qr_id":"87323168**","code":"280148","url":"xhsdiscover://**","multi_flag":0}
-        :rtype: dict
-        """
-        uri = "/api/sns/web/v1/login/qrcode/create"
-        data = {}
-        return self.post(uri, data)
-
-    def check_qrcode(self, qr_id: str, code: str):
-        uri = "/api/sns/web/v1/login/qrcode/status"
-        params = {
-            "qr_id": qr_id,
-            "code": code
-        }
-        return self.get(uri, params)
+import json
+import os
+import re
+from enum import Enum
+
+import requests
+
+from xhs.exception import DataFetchError
+
+from .help import get_search_id, sign
+
+
+class FeedType(Enum):
+    # 推荐
+    RECOMMEND = "homefeed_recommend"
+    # 穿搭
+    FASION = "homefeed.fashion_v3"
+    # 美食
+    FOOD = "homefeed.food_v3"
+    # 彩妆
+    COSMETICS = "homefeed.cosmetics_v3"
+    # 影视
+    MOVIE = "homefeed.movie_and_tv_v3"
+    # 职场
+    CAREER = "homefeed.career_v3"
+    # 情感
+    EMOTION = "homefeed.love_v3"
+    # 家居
+    HOURSE = "homefeed.household_product_v3"
+    # 游戏
+    GAME = "homefeed.gaming_v3"
+    # 旅行
+    TRAVEL = "homefeed.travel_v3"
+    # 健身
+    FITNESS = "homefeed.fitness_v3"
+
+
+class NoteType(Enum):
+    NOMAL = "nomal"
+    VIDEO = "video"
+
+
+class SearchSortType(Enum):
+    """serach sort type
+    """
+    # default
+    GENERAL = "general"
+    # most popular
+    MOST_POPULAR = "popularity_descending"
+    # Latest
+    LATEST = "time_descending"
+
+
+class SearchNoteType(Enum):
+    """search note type
+    """
+    # default
+    ALL = 0
+    # only video
+    VIDEO = 1
+    # only image
+    IMAGE = 2
+
+
+def download_file(url: str, filename: str):
+    with requests.get(url, stream=True) as r:
+        r.raise_for_status()
+        with open(filename, 'wb') as f:
+            for chunk in r.iter_content(chunk_size=8192):
+                f.write(chunk)
+
+
+def get_img_url_by_trace_id(trace_id: str):
+    return f"https://sns-img-bd.xhscdn.com/{trace_id}?imageView2/format/png"
+
+
+class XhsClient:
+    def __init__(self,
+                 cookie=None,
+                 user_agent=None,
+                 timeout=10,
+                 proxies=None):
+        """constructor
+
+        :param cookie: get it form your website, defaults to None
+        :type cookie: str, optional
+        :param user_agent: requests user agent, defaults to None
+        :type user_agent: str, optional
+        :param timeout: requests timeout, defaults to None
+        :type timeout: int, optional
+        :param proxies: requests proxies, defaults to None
+        :type proxies: dict, optional
+        """
+        self._user_agent = user_agent or ("Mozilla/5.0 "
+                                          "(Windows NT 10.0; Win64; x64) "
+                                          "AppleWebKit/537.36 "
+                                          "(KHTML, like Gecko) "
+                                          "Chrome/111.0.0.0 Safari/537.36")
+        self._cookie = cookie
+        self._proxies = proxies
+        self._session: requests.Session = requests.session()
+        self._timeout = timeout
+        self._host = "https://edith.xiaohongshu.com"
+
+    def set_cookie(self, cookie: str):
+        self._cookie = cookie
+
+    def get_cookie(self):
+        return self._cookie
+
+    def get_user_agent(self):
+        return self._user_agent
+
+    def set_user_agent(self, user_agent: str):
+        self._user_agent = user_agent
+
+    def get_proxies(self):
+        return self._proxies
+
+    def set_proxies(self, proxies: dict):
+        self._proxies = proxies
+
+    def get_timeout(self):
+        return self._timeout
+
+    def set_timeout(self, timeout):
+        self._timeout = timeout
+
+    def _pre_headers(self, url: str, data=None):
+        assert self._cookie
+        signs = sign(url, data)
+        return {
+            "User-Agent": self._user_agent,
+            "cookie": self._cookie,
+            "x-s": signs["x-s"],
+            "x-t": signs["x-t"],
+            "Content-Type": "application/json"
+        }
+
+    def request(self, method, url, **kwargs):
+        response = self._session.request(
+            method, url, timeout=self._timeout,
+            proxies=self._proxies, **kwargs)
+        data = response.json()
+        if data["success"]:
+            return data.get("data", data.get("success"))
+        else:
+            raise DataFetchError(data.get("msg", None))
+
+    def get(self, uri: str, params=None):
+        final_uri = uri
+        if isinstance(params, dict):
+            final_uri = (f"{uri}?"
+                         f"{'&'.join([f'{k}={v}'for k,v in params.items()])}")
+        headers = self._pre_headers(final_uri)
+        return self.request(method="GET", url=f"{self._host}{final_uri}",
+                            headers=headers)
+
+    def post(self, uri: str, data: dict):
+        headers = self._pre_headers(uri, data)
+        json_str = json.dumps(data, separators=(',', ':'), ensure_ascii=False)
+        return self.request(method="POST", url=f"{self._host}{uri}",
+                            data=json_str.encode("utf-8"),
+                            headers=headers)
+
+    def get_note_by_id(self, note_id: str):
+        """
+        :param note_id: note_id you want to fetch
+        :type note_id: str
+        :return: {"time":1679019883000,"user":{"nickname":"nickname","avatar":"avatar","user_id":"user_id"},"image_list":[{"url":"https://sns-img-qc.xhscdn.com/c8e505ca-4e5f-44be-fe1c-ca0205a38bad","trace_id":"1000g00826s57r6cfu0005ossb1e9gk8c65d0c80","file_id":"c8e505ca-4e5f-44be-fe1c-ca0205a38bad","height":1920,"width":1440}],"tag_list":[{"id":"5be78cdfdb601f000100d0bc","name":"jk","type":"topic"}],"desc":"裙裙","interact_info":{"followed":false,"liked":false,"liked_count":"1732","collected":false,"collected_count":"453","comment_count":"30","share_count":"41"},"at_user_list":[],"last_update_time":1679019884000,"note_id":"6413cf6b00000000270115b5","type":"normal","title":"title"}
+        :rtype: dict
+        """
+        data = {"source_note_id": note_id}
+        uri = "/api/sns/web/v1/feed"
+        res = self.post(uri, data)
+        return res["items"][0]["note_card"]
+
+    def save_files_from_note_id(self, note_id: str, dir_path: str):
+        """this function will fetch note and save file in dir_path/note_title
+
+        :param note_id: note_id that you want to fetch
+        :type note_id: str
+        :param dir_path: in fact, files will be stored in your dir_path/note_title directory
+        :type dir_path: str
+        """
+        note = self.get_note_by_id(note_id)
+        title = note["title"]
+
+        invalid_chars = '<>:"/\\|?*'
+        title = re.sub('[{}]'.format(re.escape(invalid_chars)), '_', title)
+
+        if not title:
+            title = note_id
+
+        new_dir_path = os.path.join(dir_path, title)
+        if not os.path.exists(new_dir_path):
+            os.mkdir(new_dir_path)
+
+        if note["type"] == NoteType.VIDEO.value:
+            video = next(filter(lambda value: len(value), note["video"]["media"]["stream"].values()))[0]
+            video_url = video["master_url"]
+            video_filename = os.path.join(new_dir_path, f"{title}.mp4")
+            download_file(video_url, video_filename)
+        else:
+            imgs = note["image_list"]
+            for index, img in enumerate(imgs):
+                img_url = get_img_url_by_trace_id(img["trace_id"])
+                img_file_name = os.path.join(new_dir_path, f"{title}{index}.png")
+                download_file(img_url, img_file_name)
+
+    def get_self_info(self):
+        uri = "/api/sns/web/v1/user/selfinfo"
+        res = self.get(uri)
+        return res
+
+    def get_user_info(self, user_id: str):
+        """
+        :param user_id: user_id you want fetch
+        :type user_id: str
+        :return: {"basic_info":{"imageb":"imageb","nickname":"nickname","images":"images","red_id":"red_id","gender":1,"ip_location":"ip_location","desc":"desc"},"interactions":[{"count":"5","type":"follows","name":"关注"},{"type":"fans","name":"粉丝","count":"16736"},{"type":"interaction","name":"获赞与收藏","count":"293043"}],"tags":[{"icon":"icon","tagType":"info"}],"tab_public":{"collection":false},"extra_info":{"fstatus":"none"},"result":{"success":true,"code":0,"message":"success"}}
+        :rtype: dict
+        """
+        uri = "/api/sns/web/v1/user/otherinfo"
+        params = {
+            "target_user_id": user_id
+        }
+        return self.get(uri, params)
+
+    def get_home_feed(self, feed_type: FeedType):
+        uri = "/api/sns/web/v1/homefeed"
+        data = {
+            "cursor_score": "",
+            "num": 40,
+            "refresh_type": 1,
+            "note_index": 0,
+            "unread_begin_note_id": "",
+            "unread_end_note_id": "",
+            "unread_note_count": 0,
+            "category": feed_type.value
+        }
+        return self.post(uri, data)
+
+    def get_note_by_keyword(self, keyword: str,
+                            page: int = 1, page_size: int = 20,
+                            sort: SearchSortType = SearchSortType.GENERAL,
+                            note_type: SearchNoteType = SearchNoteType.ALL):
+        """search note by keyword
+
+        :param keyword: what notes you want to search
+        :type keyword: str
+        :param page: page number, defaults to 1
+        :type page: int, optional
+        :param page_size: page size, defaults to 20
+        :type page_size: int, optional
+        :param sort: sort ordering, defaults to SearchSortType.GENERAL
+        :type sort: SearchSortType, optional
+        :param note_type: note type, defaults to SearchNoteType.ALL
+        :type note_type: SearchNoteType, optional
+        :return: {has_more: true, items: []}
+        :rtype: dict
+        """
+        uri = "/api/sns/web/v1/search/notes"
+        data = {
+            "keyword": keyword,
+            "page": page,
+            "page_size": page_size,
+            "search_id": get_search_id(),
+            "sort": sort.value,
+            "note_type": note_type.value
+        }
+        return self.post(uri, data)
+
+    def get_user_notes(self, user_id: str, cursor: str = ""):
+        uri = "/api/sns/web/v1/user_posted"
+        params = {
+            "num": 30,
+            "cursor": cursor,
+            "user_id": user_id
+        }
+        return self.get(uri, params)
+
+    def comment_note(self, note_id: str, content: str):
+        """comment a note
+
+        :return: {"time":1680834576180,"toast":"评论已发布","comment":{"id":"id","note_id":"note_id","status":2,"liked":false,"show_tags":["is_author"],"ip_location":"ip_location","content":"content","at_users":[],"like_count":"0","user_info":{"image":"**","user_id":"user_id","nickname":"nickname"},"create_time":create_time}}
+        :rtype: dict
+        """
+        uri = "/api/sns/web/v1/comment/post"
+        data = {
+            "note_id": note_id,
+            "content": content,
+            "at_users": []
+        }
+        return self.post(uri, data)
+
+    def delete_note_comment(self, note_id: str, comment_id: str):
+        uri = "/api/sns/web/v1/comment/delete"
+        data = {
+            "note_id": note_id,
+            "comment_id": comment_id
+        }
+        return self.post(uri, data)
+
+    def comment_user(self, note_id: str, comment_id: str, content: str):
+        """
+        :return: {"comment":{"like_count":"0","user_info":{"user_id":user_id"user_id":"user_id","image":"image"},"show_tags":["is_author"],"ip_location":"ip_location","id":"id","content":"content","at_users":[],"create_time":1680847204059,"target_comment":{"id":"id","user_info":{"user_id":"user_id","nickname":"nickname","image":"image"}},"note_id":"note_id","status":2,"liked":false},"time":1680847204089,"toast":"你的回复已发布"}
+        :rtype: dict
+        """
+        uri = "/api/sns/web/v1/comment/post"
+        data = {
+            "note_id": note_id,
+            "content": content,
+            "target_comment_id": comment_id,
+            "at_users": []
+        }
+        return self.post(uri, data)
+
+    def follow_user(self, user_id: str):
+        uri = "/api/sns/web/v1/user/follow"
+        data = {
+            "target_user_id": user_id
+        }
+        return self.post(uri, data)
+
+    def unfollow_user(self, user_id: str):
+        uri = "/api/sns/web/v1/user/unfollow"
+        data = {
+            "target_user_id": user_id
+        }
+        return self.post(uri, data)
+
+    def collect_note(self, note_id: str):
+        uri = "/api/sns/web/v1/note/collect"
+        data = {
+            "note_id": note_id
+        }
+        return self.post(uri, data)
+
+    def uncollect_note(self, note_id: str):
+        uri = "/api/sns/web/v1/note/uncollect"
+        data = {
+            "note_ids": note_id
+        }
+        return self.post(uri, data)
+
+    def like_note(self, note_id: str):
+        uri = "/api/sns/web/v1/note/like"
+        data = {
+            "note_oid": note_id
+        }
+        return self.post(uri, data)
+
+    def like_comment(self, note_id: str, comment_id: str):
+        uri = "/api/sns/web/v1/comment/like"
+        data = {
+            "note_id": note_id,
+            "comment_id": comment_id
+        }
+        return self.post(uri, data)
+
+    def dislike_note(self, note_id: str):
+        uri = "/api/sns/web/v1/note/dislike"
+        data = {
+            "note_oid": note_id
+        }
+        return self.post(uri, data)
+
+    def dislike_comment(self, comment_id: str):
+        uri = "/api/sns/web/v1/comment/dislike"
+        data = {
+            "note_oid": comment_id
+        }
+        return self.post(uri, data)
+
+    def get_qrcode(self):
+        """create qrcode, you can trasform response url to qrcode
+
+        :return: {"qr_id":"87323168**","code":"280148","url":"xhsdiscover://**","multi_flag":0}
+        :rtype: dict
+        """
+        uri = "/api/sns/web/v1/login/qrcode/create"
+        data = {}
+        return self.post(uri, data)
+
+    def check_qrcode(self, qr_id: str, code: str):
+        uri = "/api/sns/web/v1/login/qrcode/status"
+        params = {
+            "qr_id": qr_id,
+            "code": code
+        }
+        return self.get(uri, params)
```

### Comparing `xhs-0.1.0/xhs/help.py` & `xhs-0.1.1/xhs/help.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import hashlib
-import json
-import random
-import time
-
-
-def sign(uri, data=None, ctime=None):
-    """
-    takes in a URI (uniform resource identifier), an optional data dictionary, and an optional ctime parameter. It returns a dictionary containing two keys: "x-s" and "x-t".
-    """
-    def h(n):
-        m = ""
-        a = 0
-        d = "A4NjFqYu5wPHsO0XTdDgMa2r1ZQocVte9UJBvk6/7=yRnhISGKblCWi+LpfE8xzm3"
-        while a < 32:
-            o = ord(n[a])
-            a += 1
-            g = 0
-            if a < 32:
-                g = ord(n[a])
-            a += 1
-            h = 0
-            if a < 32:
-                h = ord(n[a])
-            a += 1
-            x = ((o & 3) << 4) | (g >> 4)
-            p = ((15 & g) << 2) | (h >> 6)
-            v = o >> 2
-            if h:
-                b = h & 63
-            else:
-                b = 64
-            if not g:
-                p = b = 64
-            m += d[v] + d[x] + d[p] + d[b]
-        return m
-
-    v = int(round(time.time() * 1000) if not ctime else ctime)
-    raw_str = f"{v}test{uri}{json.dumps(data, separators=(',', ':'), ensure_ascii=False) if isinstance(data, dict) else ''}"
-    md5_str = hashlib.md5(raw_str.encode('utf-8')).hexdigest()
-    return {
-        "x-s": h(md5_str),
-        "x-t": str(v),
-    }
-
-
-def base36encode(number, alphabet='0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ'):
-    """Converts an integer to a base36 string."""
-    if not isinstance(number, int):
-        raise TypeError('number must be an integer')
-
-    base36 = ''
-    sign = ''
-
-    if number < 0:
-        sign = '-'
-        number = -number
-
-    if 0 <= number < len(alphabet):
-        return sign + alphabet[number]
-
-    while number != 0:
-        number, i = divmod(number, len(alphabet))
-        base36 = alphabet[i] + base36
-
-    return sign + base36
-
-
-def base36decode(number):
-    return int(number, 36)
-
-
-def get_search_id():
-    e = int(time.time() * 1000) << 64
-    t = int(random.uniform(0, 2147483646))
-    return base36encode((e + t))
+import hashlib
+import json
+import random
+import time
+
+
+def sign(uri, data=None, ctime=None):
+    """
+    takes in a URI (uniform resource identifier), an optional data dictionary, and an optional ctime parameter. It returns a dictionary containing two keys: "x-s" and "x-t".
+    """
+    def h(n):
+        m = ""
+        a = 0
+        d = "A4NjFqYu5wPHsO0XTdDgMa2r1ZQocVte9UJBvk6/7=yRnhISGKblCWi+LpfE8xzm3"
+        while a < 32:
+            o = ord(n[a])
+            a += 1
+            g = 0
+            if a < 32:
+                g = ord(n[a])
+            a += 1
+            h = 0
+            if a < 32:
+                h = ord(n[a])
+            a += 1
+            x = ((o & 3) << 4) | (g >> 4)
+            p = ((15 & g) << 2) | (h >> 6)
+            v = o >> 2
+            if h:
+                b = h & 63
+            else:
+                b = 64
+            if not g:
+                p = b = 64
+            m += d[v] + d[x] + d[p] + d[b]
+        return m
+
+    v = int(round(time.time() * 1000) if not ctime else ctime)
+    raw_str = f"{v}test{uri}{json.dumps(data, separators=(',', ':'), ensure_ascii=False) if isinstance(data, dict) else ''}"
+    md5_str = hashlib.md5(raw_str.encode('utf-8')).hexdigest()
+    return {
+        "x-s": h(md5_str),
+        "x-t": str(v),
+    }
+
+
+def base36encode(number, alphabet='0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ'):
+    """Converts an integer to a base36 string."""
+    if not isinstance(number, int):
+        raise TypeError('number must be an integer')
+
+    base36 = ''
+    sign = ''
+
+    if number < 0:
+        sign = '-'
+        number = -number
+
+    if 0 <= number < len(alphabet):
+        return sign + alphabet[number]
+
+    while number != 0:
+        number, i = divmod(number, len(alphabet))
+        base36 = alphabet[i] + base36
+
+    return sign + base36
+
+
+def base36decode(number):
+    return int(number, 36)
+
+
+def get_search_id():
+    e = int(time.time() * 1000) << 64
+    t = int(random.uniform(0, 2147483646))
+    return base36encode((e + t))
```

### Comparing `xhs-0.1.0/xhs.egg-info/PKG-INFO` & `xhs-0.1.1/xhs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,94 @@
-Metadata-Version: 2.1
-Name: xhs
-Version: 0.1.0
-Summary: xiaohongshu crawl sdk.
-Home-page: https://github.com/ReaJason/xhs
-Author: ReaJason
-Author-email: reajason1225@gmail.com
-License: MIT
-Keywords: xhs crawl
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-
-<h1 align="center">
-🍰xhs
-</h1>
-
-[![](https://img.shields.io/github/license/ReaJason/17wanxiaoCheckin-Actions "协议")](https://github.com/ReaJason/17wanxiaoCheckin/blob/master/LICENSE)
-[![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
-[![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
-[![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
-
-</div>
-
-**xhs** is a crawling tool designed to extract data from [xiaohongshu website](https://www.xiaohongshu.com/explore)
-
-# Usage
-
-xhs is available on PyPI:
-
-```console
-$ python -m pip install xhs
-```
-
-basic usage:
-
-```python
-from xhs import FeedType, XhsClient
-
-cookie = "please get cookie in website"
-xhs_client = XhsClient(cookie)
-
-# get note info
-note_info = xhs_client.get_note_by_id("63db8819000000001a01ead1")
-
-# get user info
-user_info = xhs_client.get_user_info("5ff0e6410000000001008400")
-
-# get user notes
-user_notes = xhs_client.get_user_notes("63273a77000000002303cc9b")
-
-# search note
-notes = xhs_client.get_note_by_keyword("小红书")
-
-# get home recommend feed
-recommend_type = FeedType.RECOMMEND
-recommend_notes = xhs_client.get_home_feed(recommend_type)
-
-# more functions in development
-```
-
-Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
-
-use signature function:
-
-```python
-# sign get request
->>> from xhs import help
->>> help.sign("/api/sns/web/v1/user/otherinfo?target_user_id=5ff0e6410000000001008400")
-{'x-s': '1l5LsiTlZYavOYwvOid6OlU6OisCZ6dBZjvL1gsCOg13', 'x-t': '1680701208022'}
-
-# sign post request
->>> help.sign("/api/sns/web/v1/feed", {"source_note_id": "63db8819000000001a01ead1"})
-{'x-s': 'sY5LOg9WOYFKsYFWOBcis2MlsiFCsjMb0jTKZja6OjA3', 'x-t': '1680701310666'}
-
-# get search_id parameter
->>> help.get_search_id()
-'2BHU39J8HCTIW665YHFCW'
-```
+Metadata-Version: 2.1
+Name: xhs
+Version: 0.1.1
+Summary: xiaohongshu crawl sdk.
+Home-page: https://github.com/ReaJason/xhs
+Author: ReaJason
+Author-email: reajason1225@gmail.com
+License: MIT
+Keywords: xhs crawl
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+
+<h1 align="center">
+🍰xhs
+</h1>
+
+[![](https://static.pepy.tech/badge/xhs)](https://pepy.tech/project/xhs)
+[![](https://img.shields.io/github/license/ReaJason/xhs)](https://github.com/ReaJason/xhs/blob/master/LICENSE)
+[![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
+[![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
+[![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
+
+</div>
+
+**xhs** is a crawling tool designed to extract data from [xiaohongshu website](https://www.xiaohongshu.com/explore)
+
+# Usage
+
+xhs is available on PyPI:
+
+```console
+$ python -m pip install xhs
+```
+
+basic usage:
+
+```python
+from xhs import FeedType, XhsClient
+
+cookie = "please get cookie in website"
+xhs_client = XhsClient(cookie)
+
+# get note info
+note_info = xhs_client.get_note_by_id("63db8819000000001a01ead1")
+
+# get user info
+user_info = xhs_client.get_user_info("5ff0e6410000000001008400")
+
+# get user notes
+user_notes = xhs_client.get_user_notes("63273a77000000002303cc9b")
+
+# search note
+notes = xhs_client.get_note_by_keyword("小红书")
+
+# get home recommend feed
+recommend_type = FeedType.RECOMMEND
+recommend_notes = xhs_client.get_home_feed(recommend_type)
+
+# more functions in development
+```
+
+Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
+
+use signature function:
+
+```python
+# sign get request
+>>> from xhs import help
+>>> help.sign("/api/sns/web/v1/user/otherinfo?target_user_id=5ff0e6410000000001008400")
+{'x-s': '1l5LsiTlZYavOYwvOid6OlU6OisCZ6dBZjvL1gsCOg13', 'x-t': '1680701208022'}
+
+# sign post request
+>>> help.sign("/api/sns/web/v1/feed", {"source_note_id": "63db8819000000001a01ead1"})
+{'x-s': 'sY5LOg9WOYFKsYFWOBcis2MlsiFCsjMb0jTKZja6OjA3', 'x-t': '1680701310666'}
+
+# get search_id parameter
+>>> help.get_search_id()
+'2BHU39J8HCTIW665YHFCW'
+```
```


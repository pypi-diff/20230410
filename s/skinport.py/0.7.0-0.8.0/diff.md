# Comparing `tmp/skinport.py-0.7.0.tar.gz` & `tmp/skinport.py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skinport.py-0.7.0.tar", last modified: Mon Apr 10 08:25:01 2023, max compression
+gzip compressed data, was "skinport.py-0.8.0.tar", last modified: Mon Apr 10 09:50:49 2023, max compression
```

## Comparing `skinport.py-0.7.0.tar` & `skinport.py-0.8.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 08:25:01.642639 skinport.py-0.7.0/
--rw-rw-rw-   0        0        0     1089 2022-02-12 03:07:11.000000 skinport.py-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     1821 2023-04-10 08:25:01.641634 skinport.py-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      806 2022-02-20 02:32:30.000000 skinport.py-0.7.0/README.md
--rw-rw-rw-   0        0        0       82 2022-02-13 10:52:31.000000 skinport.py-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 08:25:01.643159 skinport.py-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1590 2022-12-03 10:09:01.000000 skinport.py-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:25:01.614261 skinport.py-0.7.0/skinport/
--rw-rw-rw-   0        0        0      958 2023-04-10 08:23:40.000000 skinport.py-0.7.0/skinport/__init__.py
--rw-rw-rw-   0        0        0    12086 2023-04-10 08:12:25.000000 skinport.py-0.7.0/skinport/client.py
--rw-rw-rw-   0        0        0     1599 2022-03-11 08:26:29.000000 skinport.py-0.7.0/skinport/color.py
--rw-rw-rw-   0        0        0     2298 2022-03-15 20:46:37.000000 skinport.py-0.7.0/skinport/enums.py
--rw-rw-rw-   0        0        0     4387 2022-03-11 08:02:20.000000 skinport.py-0.7.0/skinport/errors.py
--rw-rw-rw-   0        0        0     4480 2022-03-15 20:56:16.000000 skinport.py-0.7.0/skinport/http.py
--rw-rw-rw-   0        0        0     8941 2022-03-11 08:02:20.000000 skinport.py-0.7.0/skinport/item.py
--rw-rw-rw-   0        0        0     3253 2022-03-11 08:26:29.000000 skinport.py-0.7.0/skinport/iterators.py
--rw-rw-rw-   0        0        0     3359 2022-02-22 09:22:29.000000 skinport.py-0.7.0/skinport/sale.py
--rw-rw-rw-   0        0        0    17561 2022-03-11 08:38:10.000000 skinport.py-0.7.0/skinport/salefeed.py
--rw-rw-rw-   0        0        0     6812 2022-02-18 09:14:40.000000 skinport.py-0.7.0/skinport/transaction.py
--rw-rw-rw-   0        0        0      380 2022-03-15 20:56:14.000000 skinport.py-0.7.0/skinport/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:25:01.628595 skinport.py-0.7.0/skinport.py.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-10 08:25:01.000000 skinport.py-0.7.0/skinport.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      594 2023-04-10 08:25:01.000000 skinport.py-0.7.0/skinport.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 08:25:01.000000 skinport.py-0.7.0/skinport.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-10 08:25:01.000000 skinport.py-0.7.0/skinport.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 08:25:01.000000 skinport.py-0.7.0/skinport.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 08:25:01.640133 skinport.py-0.7.0/tests/
--rw-rw-rw-   0        0        0     1689 2023-04-10 08:18:52.000000 skinport.py-0.7.0/tests/test_client.py
--rw-rw-rw-   0        0        0      989 2022-03-10 18:28:07.000000 skinport.py-0.7.0/tests/test_color.py
--rw-rw-rw-   0        0        0     2833 2022-03-11 08:02:20.000000 skinport.py-0.7.0/tests/test_item.py
--rw-rw-rw-   0        0        0     5034 2022-03-11 08:02:20.000000 skinport.py-0.7.0/tests/test_sale.py
--rw-rw-rw-   0        0        0     3360 2022-03-11 08:02:20.000000 skinport.py-0.7.0/tests/test_salefeed.py
--rw-rw-rw-   0        0        0     2556 2022-03-11 08:02:20.000000 skinport.py-0.7.0/tests/test_transaction.py
--rw-rw-rw-   0        0        0      561 2022-03-15 20:56:14.000000 skinport.py-0.7.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:50:49.605711 skinport.py-0.8.0/
+-rw-rw-rw-   0        0        0     1089 2022-02-12 03:07:11.000000 skinport.py-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     1821 2023-04-10 09:50:49.604210 skinport.py-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2022-02-20 02:32:30.000000 skinport.py-0.8.0/README.md
+-rw-rw-rw-   0        0        0       82 2022-02-13 10:52:31.000000 skinport.py-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 09:50:49.605711 skinport.py-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1635 2023-04-10 09:42:35.000000 skinport.py-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:50:49.572301 skinport.py-0.8.0/skinport/
+-rw-rw-rw-   0        0        0      958 2023-04-10 09:48:24.000000 skinport.py-0.8.0/skinport/__init__.py
+-rw-rw-rw-   0        0        0    12303 2023-04-10 09:39:20.000000 skinport.py-0.8.0/skinport/client.py
+-rw-rw-rw-   0        0        0     1599 2023-04-10 09:36:05.000000 skinport.py-0.8.0/skinport/color.py
+-rw-rw-rw-   0        0        0     2298 2022-03-15 20:46:37.000000 skinport.py-0.8.0/skinport/enums.py
+-rw-rw-rw-   0        0        0     4387 2022-03-11 08:02:20.000000 skinport.py-0.8.0/skinport/errors.py
+-rw-rw-rw-   0        0        0     4480 2023-04-10 09:35:57.000000 skinport.py-0.8.0/skinport/http.py
+-rw-rw-rw-   0        0        0     8941 2022-03-11 08:02:20.000000 skinport.py-0.8.0/skinport/item.py
+-rw-rw-rw-   0        0        0     3253 2023-04-10 09:36:08.000000 skinport.py-0.8.0/skinport/iterators.py
+-rw-rw-rw-   0        0        0     3357 2023-04-10 09:34:15.000000 skinport.py-0.8.0/skinport/sale.py
+-rw-rw-rw-   0        0        0    17553 2023-04-10 09:36:12.000000 skinport.py-0.8.0/skinport/salefeed.py
+-rw-rw-rw-   0        0        0     6812 2022-02-18 09:14:40.000000 skinport.py-0.8.0/skinport/transaction.py
+-rw-rw-rw-   0        0        0      380 2022-03-15 20:56:14.000000 skinport.py-0.8.0/skinport/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:50:49.591677 skinport.py-0.8.0/skinport.py.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-10 09:50:49.000000 skinport.py-0.8.0/skinport.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-04-10 09:50:49.000000 skinport.py-0.8.0/skinport.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 09:50:49.000000 skinport.py-0.8.0/skinport.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-10 09:50:49.000000 skinport.py-0.8.0/skinport.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-10 09:50:49.000000 skinport.py-0.8.0/skinport.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 09:50:49.602689 skinport.py-0.8.0/tests/
+-rw-rw-rw-   0        0        0     1689 2023-04-10 09:37:31.000000 skinport.py-0.8.0/tests/test_client.py
+-rw-rw-rw-   0        0        0      989 2022-03-10 18:28:07.000000 skinport.py-0.8.0/tests/test_color.py
+-rw-rw-rw-   0        0        0     2833 2022-03-11 08:02:20.000000 skinport.py-0.8.0/tests/test_item.py
+-rw-rw-rw-   0        0        0     5034 2022-03-11 08:02:20.000000 skinport.py-0.8.0/tests/test_sale.py
+-rw-rw-rw-   0        0        0     3360 2022-03-11 08:02:20.000000 skinport.py-0.8.0/tests/test_salefeed.py
+-rw-rw-rw-   0        0        0     2556 2022-03-11 08:02:20.000000 skinport.py-0.8.0/tests/test_transaction.py
+-rw-rw-rw-   0        0        0      561 2023-04-10 09:34:45.000000 skinport.py-0.8.0/tests/test_utils.py
```

### Comparing `skinport.py-0.7.0/LICENSE` & `skinport.py-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/PKG-INFO` & `skinport.py-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skinport.py
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python wrapper for the Skinport API
 Home-page: https://github.com/PaxxPatriot/skinport.py
 Author: PaxxPatriot
 Author-email: skinport.py@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skinport.py-0.7.0/README.md` & `skinport.py-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/setup.py` & `skinport.py-0.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     packages=packages,
     license="MIT",
     description="A Python wrapper for the Skinport API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "aiohttp",
+        "asyncache",
+        "cachetools",
         "python-socketio[asyncio_client]",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Natural Language :: English",
```

### Comparing `skinport.py-0.7.0/skinport/__init__.py` & `skinport.py-0.8.0/skinport/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 :copyright: (c) 2022 PaxxPatriot
 :license: MIT, see LICENSE for more details.
 """
 __title__ = "skinport"
 __author__ = "PaxxPatriot"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022 PaxxPatriot"
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)
 
 import logging
 from typing import NamedTuple
 
 from . import utils
@@ -32,10 +32,10 @@
     major: int
     minor: int
     micro: int
     releaselevel: str
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=0, minor=7, micro=0, releaselevel="final", serial=0)
+version_info: VersionInfo = VersionInfo(major=0, minor=8, micro=0, releaselevel="final", serial=0)
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `skinport.py-0.7.0/skinport/client.py` & `skinport.py-0.8.0/skinport/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 SOFTWARE.
 """
 
 import asyncio
 import logging
 import signal
 from typing import Any, Coroutine, Dict, List, Union
+from asyncache import cached
+from cachetools import TTLCache
 
 import socketio
 
 from .enums import AppID, Currency, Locale
 from .errors import ParamRequired
 from .http import HTTPClient
 from .item import Item, ItemOutOfStock, ItemWithSales
@@ -200,28 +202,29 @@
                         "appid": app_id.value,
                     },
                 )
                 await self.ws.wait()
             except asyncio.TimeoutError:
                 _log.info("Connection timed out.")
                 await self.close()
-                await asyncio.sleep(5) # Sleep 5 seconds to handle connection closing
+                await asyncio.sleep(5)  # Sleep 5 seconds to handle connection closing
 
     async def close(self) -> None:
         """*coroutine*
         Closes the `aiohttp.ClientSession`.
         """
         if self._closed:
             return
 
         self._closed = True
         if self.ws.eio.http is not None:
             await self.ws.eio.http.close()
         await self.http.close()
 
+    @cached(cache=TTLCache(maxsize=128, ttl=300))
     async def get_items(
         self,
         *,
         app_id: AppID = AppID.csgo,
         currency: Currency = Currency.eur,
         tradable: bool = False,
     ) -> List[Item]:
@@ -250,14 +253,15 @@
             "app_id": app_id,
             "currency": currency.value,
             "tradable": _tradable,
         }
         data = await self.http.get_items(params=params)
         return [Item(data=item) for item in data]
 
+    @cached(cache=TTLCache(maxsize=16, ttl=3600))
     async def get_sales_history(
         self,
         app_id: int = 730,
         currency: Currency = Currency.eur,
     ) -> List[ItemWithSales]:  # sourcery skip: default-mutable-arg
         """*coroutine*
         Returns a :class:`list` of :class:`ItemWithSales`.
@@ -278,14 +282,15 @@
         params = {
             "app_id": app_id,
             "currency": currency.value,
         }
         data = await self.http.get_sales_history(params=params)
         return [ItemWithSales(data=sale) for sale in data]
 
+    @cached(cache=TTLCache(maxsize=16, ttl=3600))
     async def get_sales_out_of_stock(
         self, *, app_id: int = 730, currency: Currency = Currency.eur
     ) -> List[ItemOutOfStock]:
         """*coroutine*
         Returns a :class:`list` of :class:`ItemOutOfStock`.
 
         Parameters
```

### Comparing `skinport.py-0.7.0/skinport/color.py` & `skinport.py-0.8.0/skinport/color.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/skinport/enums.py` & `skinport.py-0.8.0/skinport/enums.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/skinport/errors.py` & `skinport.py-0.8.0/skinport/errors.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/skinport/http.py` & `skinport.py-0.8.0/skinport/http.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/skinport/item.py` & `skinport.py-0.8.0/skinport/item.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/skinport/iterators.py` & `skinport.py-0.8.0/skinport/iterators.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/skinport/sale.py` & `skinport.py-0.8.0/skinport/sale.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     @property
     def sold_at(self) -> datetime.datetime:
         """:class:`datetime.datetime`: Returns the date and time the item was sold."""
         return datetime.datetime.fromtimestamp(self._sold_at)
 
 
 class LastXDays:
-
     __slots__ = (
         "_min",
         "_max",
         "_avg",
         "_volume",
     )
```

### Comparing `skinport.py-0.7.0/skinport/salefeed.py` & `skinport.py-0.8.0/skinport/salefeed.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from .color import Color
 from .enums import AppID, Currency, SaleType
 
 __all__ = ("Tag", "SaleFeedSale", "SaleFeed", "Sticker")
 
 
 class Tag:
-
     __slots__ = (
         "_name",
         "_name_localized",
     )
 
     def __init__(self, *, data: Dict[str, Any]) -> None:
         self._name = data.get("name", "")
@@ -64,15 +63,14 @@
     @property
     def name_localized(self) -> str:
         """:class:`str`: Returns the localized name of the item."""
         return self._name_localized
 
 
 class Sticker:
-
     __slots__ = (
         "_color",
         "_img",
         "_name",
         "_name_localized",
         "_slot",
         "_sticker_id",
@@ -135,15 +133,14 @@
     @property
     def wear(self) -> Optional[float]:
         """Optional[:class:`float`]: Returns the wear of the sticker."""
         return self._wear
 
 
 class SaleFeedSale:
-
     __slots__ = (
         "_id",
         "_saleId",
         "_productId",
         "_assetId",
         "_itemId",
         "_appid",
@@ -510,15 +507,14 @@
     @property
     def own_item(self) -> bool:
         """:class:`bool`: Indicates if the item is your own."""
         return self._ownItem
 
 
 class SaleFeed:
-
     __slots__ = (
         "_event_type",
         "_sales",
     )
 
     def __init__(self, *, data: Dict[str, Any]) -> None:
         self._event_type = data.get("eventType", "")
```

### Comparing `skinport.py-0.7.0/skinport/transaction.py` & `skinport.py-0.8.0/skinport/transaction.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/skinport.py.egg-info/PKG-INFO` & `skinport.py-0.8.0/skinport.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skinport.py
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python wrapper for the Skinport API
 Home-page: https://github.com/PaxxPatriot/skinport.py
 Author: PaxxPatriot
 Author-email: skinport.py@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skinport.py-0.7.0/skinport.py.egg-info/SOURCES.txt` & `skinport.py-0.8.0/skinport.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/tests/test_client.py` & `skinport.py-0.8.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/tests/test_color.py` & `skinport.py-0.8.0/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/tests/test_item.py` & `skinport.py-0.8.0/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/tests/test_sale.py` & `skinport.py-0.8.0/tests/test_sale.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/tests/test_salefeed.py` & `skinport.py-0.8.0/tests/test_salefeed.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/tests/test_transaction.py` & `skinport.py-0.8.0/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.7.0/tests/test_utils.py` & `skinport.py-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*


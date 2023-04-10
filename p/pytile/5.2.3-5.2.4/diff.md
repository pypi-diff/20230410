# Comparing `tmp/pytile-5.2.3.tar.gz` & `tmp/pytile-5.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytile-5.2.3.tar", max compression
+gzip compressed data, was "pytile-5.2.4.tar", max compression
```

## Comparing `pytile-5.2.3.tar` & `pytile-5.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2021-07-27 03:02:30.081120 pytile-5.2.3/LICENSE
--rw-r--r--   0        0        0     5562 2021-07-27 03:02:30.081120 pytile-5.2.3/README.md
--rw-r--r--   0        0        0     1457 2021-07-27 03:02:30.081120 pytile-5.2.3/pyproject.toml
--rw-r--r--   0        0        0       72 2021-07-27 03:02:30.081120 pytile-5.2.3/pytile/__init__.py
--rw-r--r--   0        0        0     4346 2021-07-27 03:02:30.081120 pytile-5.2.3/pytile/api.py
--rw-r--r--   0        0        0      419 2021-07-27 03:02:30.081120 pytile-5.2.3/pytile/errors.py
--rw-r--r--   0        0        0        0 2021-07-27 03:02:30.081120 pytile-5.2.3/pytile/py.typed
--rw-r--r--   0        0        0     5092 2021-07-27 03:02:30.081120 pytile-5.2.3/pytile/tile.py
--rw-r--r--   0        0        0     6448 2021-07-27 03:02:37.642336 pytile-5.2.3/setup.py
--rw-r--r--   0        0        0     6476 2021-07-27 03:02:37.642715 pytile-5.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-10-18 02:28:53.036465 pytile-5.2.4/LICENSE
+-rw-r--r--   0        0        0     5562 2021-10-18 02:28:53.036465 pytile-5.2.4/README.md
+-rw-r--r--   0        0        0     1457 2021-10-18 02:28:53.040465 pytile-5.2.4/pyproject.toml
+-rw-r--r--   0        0        0       72 2021-10-18 02:28:53.040465 pytile-5.2.4/pytile/__init__.py
+-rw-r--r--   0        0        0     4533 2021-10-18 02:28:53.040465 pytile-5.2.4/pytile/api.py
+-rw-r--r--   0        0        0      419 2021-10-18 02:28:53.040465 pytile-5.2.4/pytile/errors.py
+-rw-r--r--   0        0        0        0 2021-10-18 02:28:53.040465 pytile-5.2.4/pytile/py.typed
+-rw-r--r--   0        0        0     5092 2021-10-18 02:28:53.040465 pytile-5.2.4/pytile/tile.py
+-rw-r--r--   0        0        0     6448 2021-10-18 02:29:02.286555 pytile-5.2.4/setup.py
+-rw-r--r--   0        0        0     6527 2021-10-18 02:29:02.287033 pytile-5.2.4/PKG-INFO
```

### Comparing `pytile-5.2.3/LICENSE` & `pytile-5.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytile-5.2.3/README.md` & `pytile-5.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pytile-5.2.3/pyproject.toml` & `pytile-5.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 multi_line_output = 3
 not_skip = "__init__.py"
 sections = "FUTURE,STDLIB,INBETWEENS,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 use_parentheses = true
 
 [tool.poetry]
 name = "pytile"
-version = "5.2.3"
+version = "5.2.4"
 description = "A simple Python API for Tile® Bluetooth trackers"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/pytile"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -43,8 +43,8 @@
 pylint = "^2.5.2"
 
 [tool.poetry.dev-dependencies]
 aresponses = "^2.0.0"
 pre-commit = "^2.0.1"
 pytest = "^6.0.0"
 pytest-aiohttp = "^0.3.0"
-pytest-cov = "^2.8.1"
+pytest-cov = "^3.0.0"
```

### Comparing `pytile-5.2.3/pytile/api.py` & `pytile-5.2.4/pytile/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from aiohttp.client_exceptions import ClientError
 
 from .errors import InvalidAuthError, RequestError
 from .tile import Tile
 
 _LOGGER = logging.getLogger(__name__)
 
-API_URL_SCAFFOLD: str = "https://production.tile-api.com/api/v1"
+API_URL_SCAFFOLD = "https://production.tile-api.com/api/v1"
 
-DEFAULT_APP_ID: str = "ios-tile-production"
-DEFAULT_APP_VERSION: str = "2.69.0.4123"
-DEFAULT_LOCALE: str = "en-US"
-DEFAULT_TIMEOUT: int = 10
+DEFAULT_API_VERSION = "1.0"
+DEFAULT_APP_ID = "ios-tile-production"
+DEFAULT_APP_VERSION = "2.89.1.4774"
+DEFAULT_LOCALE = "en-US"
+DEFAULT_TIMEOUT = 10
+DEFAULT_USER_AGENT = "Tile/4774 CFNetwork/1312 Darwin/21.0.0"
 
 
 class API:  # pylint: disable=too-many-instance-attributes
     """Define the API management object."""
 
     def __init__(
         self,
@@ -45,25 +47,24 @@
 
     async def _async_request(self, method: str, endpoint: str, **kwargs) -> dict:
         """Make a request against Tile."""
         if self._session_expiry and self._session_expiry <= int(time() * 1000):
             await self.async_init()
 
         kwargs.setdefault("headers", {})
-        kwargs["headers"].update(
-            {
-                "Tile_app_id": DEFAULT_APP_ID,
-                "Tile_app_version": DEFAULT_APP_VERSION,
-                "Tile_client_uuid": self.client_uuid,
-            }
-        )
+        kwargs["headers"]["User-Agent"] = DEFAULT_USER_AGENT
+        kwargs["headers"]["tile_api_version"] = DEFAULT_API_VERSION
+        kwargs["headers"]["tile_app_id"] = DEFAULT_APP_ID
+        kwargs["headers"]["tile_app_version"] = DEFAULT_APP_VERSION
+        kwargs["headers"]["tile_client_uuid"] = self.client_uuid
 
         async with self._session.request(
             method, f"{API_URL_SCAFFOLD}/{endpoint}", **kwargs
         ) as resp:
+            print(resp.cookies)
             try:
                 resp.raise_for_status()
                 data = await resp.json()
             except ClientError as err:
                 if "401" in str(err):
                     raise InvalidAuthError("Invalid credentials") from err
                 raise RequestError(
```

### Comparing `pytile-5.2.3/pytile/tile.py` & `pytile-5.2.4/pytile/tile.py`

 * *Files identical despite different names*

### Comparing `pytile-5.2.3/setup.py` & `pytile-5.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.7.4,<4.0.0', 'pylint>=2.5.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'pytile',
-    'version': '5.2.3',
+    'version': '5.2.4',
     'description': 'A simple Python API for Tile® Bluetooth trackers',
     'long_description': '# 📡 pytile: A simple Python API for Tile® Bluetooth trackers\n\n[![CI](https://github.com/bachya/pytile/workflows/CI/badge.svg)](https://github.com/bachya/pytile/actions)\n[![PyPi](https://img.shields.io/pypi/v/pytile.svg)](https://pypi.python.org/pypi/pytile)\n[![Version](https://img.shields.io/pypi/pyversions/pytile.svg)](https://pypi.python.org/pypi/pytile)\n[![License](https://img.shields.io/pypi/l/pytile.svg)](https://github.com/bachya/pytile/blob/master/LICENSE)\n[![Code Coverage](https://codecov.io/gh/bachya/pytile/branch/master/graph/badge.svg)](https://codecov.io/gh/bachya/pytile)\n[![Maintainability](https://api.codeclimate.com/v1/badges/71eb642c735e33adcdfc/maintainability)](https://codeclimate.com/github/bachya/pytile/maintainability)\n[![Say Thanks](https://img.shields.io/badge/SayThanks-!-1EAEDB.svg)](https://saythanks.io/to/bachya)\n\n`pytile` is a simple Python library for retrieving information on\n[Tile® Bluetooth trackers](https://www.thetileapp.com/en-us/) (including last\nlocation and more).\n\nThis library is built on an unpublished, unofficial Tile API; it may alter or\ncease operation at any point.\n\n- [Python Versions](#python-versions)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Contributing](#contributing)\n\n# NOTE: Version 5.0.0\n\nVersion 5.0.0 is a complete re-architecture of `pytile` – as such, the API has changed.\nPlease read the documentation carefully!\n\n# Python Versions\n\n`pytile` is currently supported on:\n\n* Python 3.6\n* Python 3.7\n* Python 3.8\n* Python 3.9\n\n# Installation\n\n```python\npip install pytile\n```\n\n# Usage\n\n## Getting an API Object\n\n`pytile` usage starts with an [`aiohttp`](https://github.com/aio-libs/aiohttp) `ClientSession` –\nnote that this ClientSession is required to properly authenticate the library:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom pytile import async_login\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        api = await async_login("<EMAIL>", "<PASSWORD>", session)\n\n\nasyncio.run(main())\n```\n\nIf for some reason you need to use a specific client UUID (to, say, ensure that the\nTile API sees you as a client it\'s seen before) or a specific locale, you can do\nso easily:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom pytile import async_login\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        api = await async_login(\n            "<EMAIL>", "<PASSWORD>", session, client_uuid="MY_UUID", locale="en-GB"\n        )\n\n\nasyncio.run(main())\n```\n\n## Getting Tiles\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom pytile import async_login\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        api = await async_login("<EMAIL>", "<PASSWORD>", session)\n\n        tiles = await api.async_get_tiles()\n\n\nasyncio.run(main())\n```\n\nThe `async_get_tiles` coroutine returns a dict with Tile UUIDs as the keys and `Tile`\nobjects as the values.\n\n### The `Tile` Object\n\nThe Tile object comes with several properties:\n\n* `accuracy`: the location accuracy of the Tile\n* `altitude`: the altitude of the Tile\n* `archetype`: the internal reference string that describes the Tile\'s "family"\n* `dead`: whether the Tile is inactive\n* `firmware_version`: the Tile\'s firmware version\n* `hardware_version`: the Tile\'s hardware version\n* `kind`: the kind of Tile (e.g., `TILE`, `PHONE`)\n* `last_timestamp`: the timestamp at which the current attributes were received\n* `latitude`: the latitude of the Tile\n* `longitude`: the latitude of the Tile\n* `lost`: whether the Tile has been marked as "lost"\n* `lost_timestamp`: the timestamp at which the Tile was last marked as "lost"\n* `name`: the name of the Tile\n* `uuid`: the Tile UUID\n* `visible`: whether the Tile is visible in the mobile app\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom pytile import async_login\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        api = await async_login("<EMAIL>", "<PASSWORD>", session)\n\n        tiles = await api.async_get_tiles()\n\n        for tile_uuid, tile in tiles.items():\n            print(f"The Tile\'s name is {tile.name}")\n            # ...\n\n\nasyncio.run(main())\n```\n\nIn addition to these properties, the `Tile` object comes with an `async_update` coroutine\nwhich requests new data from the Tile cloud API for this Tile:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom pytile import async_login\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        api = await async_login("<EMAIL>", "<PASSWORD>", session)\n\n        tiles = await api.async_get_tiles()\n\n        for tile_uuid, tile in tiles.items():\n            await tile.async_update()\n\n\nasyncio.run(main())\n```\n\n# Contributing\n\n1. [Check for open features/bugs](https://github.com/bachya/pytile/issues)\n  or [initiate a discussion on one](https://github.com/bachya/pytile/issues/new).\n2. [Fork the repository](https://github.com/bachya/pytile/fork).\n3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`\n4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`\n5. Install the dev environment: `script/setup`\n6. Code your new feature or bug fix.\n7. Write tests that cover your new functionality.\n8. Run tests and ensure 100% code coverage: `script/test`\n9. Update `README.md` with any new documentation.\n10. Add yourself to `AUTHORS.md`.\n11. Submit a pull request!\n',
     'author': 'Aaron Bach',
     'author_email': 'bachya1208@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/bachya/pytile',
```

### Comparing `pytile-5.2.3/PKG-INFO` & `pytile-5.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pytile
-Version: 5.2.3
+Version: 5.2.4
 Summary: A simple Python API for Tile® Bluetooth trackers
 Home-page: https://github.com/bachya/pytile
 License: MIT
 Author: Aaron Bach
 Author-email: bachya1208@gmail.com
 Requires-Python: >=3.6.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
```


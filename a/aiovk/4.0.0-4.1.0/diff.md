# Comparing `tmp/aiovk-4.0.0.tar.gz` & `tmp/aiovk-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiovk-4.0.0.tar", last modified: Sat Dec 19 16:35:23 2020, max compression
+gzip compressed data, was "aiovk-4.1.0.tar", last modified: Mon Apr 10 12:05:00 2023, max compression
```

## Comparing `aiovk-4.0.0.tar` & `aiovk-4.1.0.tar`

### file list

```diff
@@ -1,37 +1,44 @@
-drwxrwxr-x   0 fahreeve  (1000) fahreeve  (1000)        0 2020-12-19 16:35:23.877126 aiovk-4.0.0/
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)    11516 2020-12-19 16:35:23.877126 aiovk-4.0.0/PKG-INFO
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     8394 2020-12-19 16:34:42.000000 aiovk-4.0.0/README.rst
-drwxrwxr-x   0 fahreeve  (1000) fahreeve  (1000)        0 2020-12-19 16:35:23.873125 aiovk-4.0.0/aiovk/
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)      168 2020-12-19 16:06:20.000000 aiovk-4.0.0/aiovk/__init__.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     1809 2020-12-19 14:03:29.000000 aiovk-4.0.0/aiovk/api.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     2896 2020-12-19 13:45:19.000000 aiovk-4.0.0/aiovk/drivers.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     1401 2020-12-19 13:45:19.000000 aiovk-4.0.0/aiovk/exceptions.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     4542 2020-12-19 13:45:19.000000 aiovk-4.0.0/aiovk/longpoll.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     1322 2020-12-19 13:45:19.000000 aiovk-4.0.0/aiovk/mixins.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     2622 2019-07-02 16:02:44.000000 aiovk-4.0.0/aiovk/parser.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     4396 2020-12-19 15:59:53.000000 aiovk-4.0.0/aiovk/pools.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)    12942 2020-12-19 16:00:45.000000 aiovk-4.0.0/aiovk/sessions.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)      804 2020-12-19 13:45:19.000000 aiovk-4.0.0/aiovk/shaping.py
-drwxrwxr-x   0 fahreeve  (1000) fahreeve  (1000)        0 2020-12-19 16:35:23.873125 aiovk-4.0.0/aiovk.egg-info/
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)    11516 2020-12-19 16:35:23.000000 aiovk-4.0.0/aiovk.egg-info/PKG-INFO
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)      649 2020-12-19 16:35:23.000000 aiovk-4.0.0/aiovk.egg-info/SOURCES.txt
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)        1 2020-12-19 16:35:23.000000 aiovk-4.0.0/aiovk.egg-info/dependency_links.txt
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)       36 2020-12-19 16:35:23.000000 aiovk-4.0.0/aiovk.egg-info/requires.txt
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)       12 2020-12-19 16:35:23.000000 aiovk-4.0.0/aiovk.egg-info/top_level.txt
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)       38 2020-12-19 16:35:23.877126 aiovk-4.0.0/setup.cfg
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     1393 2020-12-19 16:15:20.000000 aiovk-4.0.0/setup.py
-drwxrwxr-x   0 fahreeve  (1000) fahreeve  (1000)        0 2020-12-19 16:35:23.873125 aiovk-4.0.0/tests/
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)        0 2019-07-02 17:22:26.000000 aiovk-4.0.0/tests/__init__.py
-drwxrwxr-x   0 fahreeve  (1000) fahreeve  (1000)        0 2020-12-19 16:35:23.877126 aiovk-4.0.0/tests/functional/
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)        0 2020-12-19 13:45:19.000000 aiovk-4.0.0/tests/functional/__init__.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     3406 2020-12-19 13:45:19.000000 aiovk-4.0.0/tests/functional/conftest.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     3671 2020-12-19 13:45:19.000000 aiovk-4.0.0/tests/functional/test_drivers.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     1490 2020-12-19 13:45:19.000000 aiovk-4.0.0/tests/functional/test_longpool.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     2141 2020-12-19 13:45:19.000000 aiovk-4.0.0/tests/functional/test_sessions.py
-drwxrwxr-x   0 fahreeve  (1000) fahreeve  (1000)        0 2020-12-19 16:35:23.877126 aiovk-4.0.0/tests/unit/
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)        0 2020-12-19 13:45:19.000000 aiovk-4.0.0/tests/unit/__init__.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     2587 2020-12-19 16:02:27.000000 aiovk-4.0.0/tests/unit/test_api.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     5333 2020-12-19 13:45:19.000000 aiovk-4.0.0/tests/unit/test_longpool.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     8445 2020-12-19 16:01:27.000000 aiovk-4.0.0/tests/unit/test_pools.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)     1018 2020-12-19 13:45:19.000000 aiovk-4.0.0/tests/unit/test_shaping.py
--rw-rw-r--   0 fahreeve  (1000) fahreeve  (1000)      526 2019-07-02 17:22:26.000000 aiovk-4.0.0/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:05:00.474878 aiovk-4.1.0/
+-rw-rw-rw-   0        0        0     1101 2023-04-10 11:34:54.000000 aiovk-4.1.0/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-04-10 12:04:46.000000 aiovk-4.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9442 2023-04-10 12:05:00.473883 aiovk-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8700 2023-04-10 11:34:54.000000 aiovk-4.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 12:05:00.451878 aiovk-4.1.0/aiovk/
+-rw-rw-rw-   0        0        0      158 2023-04-10 11:54:36.000000 aiovk-4.1.0/aiovk/__init__.py
+-rw-rw-rw-   0        0        0     1870 2023-04-10 11:34:54.000000 aiovk-4.1.0/aiovk/api.py
+-rw-rw-rw-   0        0        0     3162 2023-04-10 11:34:54.000000 aiovk-4.1.0/aiovk/drivers.py
+-rw-rw-rw-   0        0        0     1453 2023-04-10 11:34:54.000000 aiovk-4.1.0/aiovk/exceptions.py
+-rw-rw-rw-   0        0        0     4671 2023-04-10 11:34:54.000000 aiovk-4.1.0/aiovk/longpoll.py
+-rw-rw-rw-   0        0        0     1355 2023-04-10 11:34:54.000000 aiovk-4.1.0/aiovk/mixins.py
+-rw-rw-rw-   0        0        0     3133 2023-04-10 11:34:54.000000 aiovk-4.1.0/aiovk/parser.py
+-rw-rw-rw-   0        0        0     4530 2023-04-10 11:34:54.000000 aiovk-4.1.0/aiovk/pools.py
+-rw-rw-rw-   0        0        0    14005 2023-04-10 11:34:54.000000 aiovk-4.1.0/aiovk/sessions.py
+-rw-rw-rw-   0        0        0      833 2023-04-10 11:34:54.000000 aiovk-4.1.0/aiovk/shaping.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:05:00.457879 aiovk-4.1.0/aiovk.egg-info/
+-rw-rw-rw-   0        0        0     9442 2023-04-10 12:05:00.000000 aiovk-4.1.0/aiovk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2023-04-10 12:05:00.000000 aiovk-4.1.0/aiovk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 12:05:00.000000 aiovk-4.1.0/aiovk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-10 12:05:00.000000 aiovk-4.1.0/aiovk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 12:05:00.000000 aiovk-4.1.0/aiovk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       38 2023-04-10 11:34:54.000000 aiovk-4.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 12:05:00.474878 aiovk-4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1515 2023-04-10 11:55:25.000000 aiovk-4.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:05:00.459878 aiovk-4.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:05:00.463877 aiovk-4.1.0/tests/functional/
+-rw-rw-rw-   0        0        0        0 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/functional/__init__.py
+-rw-rw-rw-   0        0        0     3804 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/functional/conftest.py
+-rw-rw-rw-   0        0        0     3799 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/functional/test_drivers.py
+-rw-rw-rw-   0        0        0     1542 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/functional/test_longpool.py
+-rw-rw-rw-   0        0        0     2211 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/functional/test_sessions.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:05:00.467897 aiovk-4.1.0/tests/responses/
+-rw-rw-rw-   0        0        0      499 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/responses/auth_redirect.jinja2
+-rw-rw-rw-   0        0        0     9234 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/responses/authorize_page.jinja2
+-rw-rw-rw-   0        0        0      595 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/responses/blank.jinja2
+drwxrwxrwx   0        0        0        0 2023-04-10 12:05:00.472882 aiovk-4.1.0/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     2686 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/unit/test_api.py
+-rw-rw-rw-   0        0        0     5510 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/unit/test_longpool.py
+-rw-rw-rw-   0        0        0     8672 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/unit/test_pools.py
+-rw-rw-rw-   0        0        0     1059 2023-04-10 11:50:12.000000 aiovk-4.1.0/tests/unit/test_shaping.py
+-rw-rw-rw-   0        0        0      548 2023-04-10 11:34:54.000000 aiovk-4.1.0/tests/utils.py
```

### Comparing `aiovk-4.0.0/PKG-INFO` & `aiovk-4.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,325 +1,326 @@
-Metadata-Version: 1.2
-Name: aiovk
-Version: 4.0.0
-Summary: vk.com API python wrapper for asyncio
-Home-page: https://github.com/Fahreeve/aiovk
-Author: Fahreev Eldar
-Author-email: fahreeve@yandex.ru
-License: MIT License
-Description: vk.com API python wrapper for asyncio
-        =====================================
-        for old version of python you can use https://github.com/dimka665/vk
-        
-        Features
-        --------
-        * asynchronous
-        * support python 3.5+ versions
-        * have only one dependency - ``aiohttp 3+``
-        * support two-factor authentication
-        * support socks proxy with ``aiohttp-socks``
-        * support rate limit of requests
-        * support Long Poll connection
-        
-        TODO
-        ----
-        * need refactoring tests for ``AsyncVkExecuteRequestPool``
-        
-        Install
-        -------
-        
-        .. code-block:: bash
-        
-            pip install aiovk
-        
-        Examples
-        ========
-        Annotation
-        ----------
-        In all the examples below, I will give only the ``{code}``
-        
-        .. code-block:: python
-        
-            async def func():
-                {code}
-        
-            loop = asyncio.get_event_loop()
-            loop.run_until_complete(func())
-        
-        
-        Authorization
-        -------------
-        **TokenSession** - if you already have token or you use requests which don't require token
-        
-        .. code-block:: python
-        
-            session = TokenSession()
-            session = TokenSession(access_token='asdf123..')
-        
-        **ImplicitSession** - client authorization in js apps and standalone (desktop and mobile) apps
-        
-        .. code-block:: python
-        
-            >>> session = ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID)
-            >>> await session.authorize()
-            >>> session.access_token
-            asdfa2321afsdf12eadasf123...
-        
-        With scopes:
-        
-        .. code-block:: python
-        
-            ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify')
-            ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify,friends')
-            ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, ['notify', 'friends'])
-            ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 3)  # notify and friends
-        
-        Also you can use ``SimpleImplicitSessionMixin`` for entering confirmation code
-        or captcha key
-        
-        **AuthorizationCodeSession** - authorization for server apps or Open API
-        
-        See https://vk.com/dev/authcode_flow_user for getting the CODE
-        
-        .. code-block:: python
-        
-            >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI, CODE)
-            >>> await session.authorize()
-            >>> session.access_token
-            asdfa2321afsdf12eadasf123...
-        
-        Or:
-        
-        .. code-block:: python
-        
-            >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI)
-            >>> await session.authorize(CODE)
-            >>> session.access_token
-            asdfa2321afsdf12eadasf123...
-        
-        **Authorization using context manager** - you won't need to use session.close() after work
-        
-        .. code-block:: python
-        
-            async with aiovk.TokenSession(access_token=YOUR_VK_TOKEN) as ses:
-                api = API(ses)...
-        
-        And your session will be closed after all done or code fail(similar to simple "with" usage)
-        Works with all types of authorization
-        
-        Drivers
-        -------
-        **HttpDriver** - default driver for using ``aiohttp``
-        
-        .. code-block:: python
-        
-            >>> driver = HttpDriver()
-            >>> driver = HttpDriver(timeout=10)  # default timeout for all requests
-        
-        .. code-block:: python
-        
-            >>> driver = ProxyDriver(PROXY_ADDRESS, PORT)  # 1234 is port
-            >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, timeout=10)
-            >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, PROXY_LOGIN, PROXY_PASSWORD, timeout=10)
-        
-        How to use custom driver with session:
-        
-        .. code-block:: python
-        
-            >>> session = TokenSession(..., driver=HttpDriver())
-        
-        How to use driver with own loop:
-        
-        .. code-block:: python
-        
-            >>> loop = asyncio.get_event_loop()
-            >>> asyncio.set_event_loop(None)
-            >>> session = TokenSession(driver=HttpDriver(loop=loop))  # or ProxyDriver
-        
-        How to use driver with custom http session object:
-        
-        Solve next problem: https://stackoverflow.com/questions/29827642/asynchronous-aiohttp-requests-fails-but-synchronous-requests-succeed
-        
-        .. code-block:: python
-        
-            >>> connector = aiohttp.TCPConnector(verify_ssl=False)
-            >>> session = aiohttp.ClientSession(connector=connector)
-            >>> driver = HttpDriver(loop=loop, session=session)
-        
-        
-        **LimitRateDriverMixin** - mixin class what allow you create new drivers with speed rate limits
-        
-        .. code-block:: python
-        
-            >>> class ExampleDriver(LimitRateDriverMixin, HttpDriver):
-            ...     requests_per_period = 3
-            ...     period = 1  #seconds
-        
-        VK API
-        ------
-        First variant:
-        
-        .. code-block:: python
-        
-            >>> session = TokenSession()
-            >>> api = API(session)
-            >>> await api.users.get(user_ids=1)
-            [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
-        
-        Second variant:
-        
-        .. code-block:: python
-        
-            >>> session = TokenSession()
-            >>> api = API(session)
-            >>> await api('users.get', user_ids=1)
-            [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
-        
-        Also you can add ``timeout`` argument for each request or define it in the session
-        
-        See https://vk.com/dev/methods for detailed API guide.
-        
-        Lazy VK API
-        -----------
-        It is useful when a bot has a large message flow
-        
-        .. code-block:: python
-        
-            >>> session = TokenSession()
-            >>> api = LazyAPI(session)
-            >>> message = api.users.get(user_ids=1)
-            >>> await message()
-            [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
-        
-        Supports both variants like API object
-        
-        User Long Poll
-        --------------
-        For documentation, see: https://vk.com/dev/using_longpoll
-        
-        Use exist API object
-        
-        .. code-block:: python
-        
-            >>> api = API(session)
-            >>> lp = UserLongPoll(api, mode=2)  # default wait=25
-            >>> await lp.wait()
-            {"ts":1820350345,"updates":[...]}
-            >>> await lp.wait()
-            {"ts":1820351011,"updates":[...]}
-        
-        Use Session object
-        
-        .. code-block:: python
-        
-            >>> lp = UserLongPoll(session, mode=2)  # default wait=25
-            >>> await lp.wait()
-            {"ts":1820350345,"updates":[...]}
-            >>> await lp.get_pts()  # return pts
-            191231223
-            >>> await lp.get_pts(need_ts=True)  # return pts, ts
-            191231223, 1820350345
-        
-        You can iterate over events
-        
-        .. code-block:: python
-        
-            >>> async for event in lp.iter():
-            ...     print(event)
-            {"type":..., "object": {...}}
-        
-        Notice that ``wait`` value only for long pool connection.
-        
-        Real pause could be more ``wait`` time because of need time
-        for authorization (if needed), reconnect and etc.
-        
-        Bots Long Poll
-        --------------
-        For documentation, see: https://vk.com/dev/bots_longpoll
-        
-        Use exist API object
-        
-        .. code-block:: python
-        
-            >>> api = API(session)
-            >>> lp = BotsLongPoll(api, group_id=1)  # default wait=25
-            >>> await lp.wait()
-            {"ts":345,"updates":[...]}
-            >>> await lp.wait()
-            {"ts":346,"updates":[...]}
-        
-        Use Session object
-        
-        .. code-block:: python
-        
-            >>> lp = BotsLongPoll(session, group_id=1)  # default wait=25
-            >>> await lp.wait()
-            {"ts":78455,"updates":[...]}
-            >>> await lp.get_pts()  # return pts
-            191231223
-            >>> await lp.get_pts(need_ts=True)  # return pts, ts
-            191231223, 1820350345
-        
-        BotsLongPoll supports iterating too
-        
-        .. code-block:: python
-        
-            >>> async for event in lp.iter():
-            ...     print(event)
-            {"type":..., "object": {...}}
-        
-        Notice that ``wait`` value only for long pool connection.
-        
-        Real pause could be more ``wait`` time because of need time
-        for authorization (if needed), reconnect and etc.
-        
-        Async execute request pool
-        --------------------------
-        For documentation, see: https://vk.com/dev/execute
-        
-        .. code-block:: python
-        
-            from aiovk.pools import AsyncVkExecuteRequestPool
-        
-            async with AsyncVkExecuteRequestPool() as pool:
-                response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
-                response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
-                response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
-                response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
-        
-            >>> print(response.ok)
-            True
-            >>> print(response.result)
-            [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
-            >>> print(response2.result)
-            [{'id': 2, 'first_name': 'Александра', 'last_name': 'Владимирова'}]
-            >>> print(response3.result)
-            [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
-            >>> print(response4.ok)
-            False
-            >>> print(response4.error)
-            {'method': 'users.get', 'error_code': 113, 'error_msg': 'Invalid user id'}
-        
-        or
-        
-        .. code-block:: python
-        
-            from aiovk.pools import AsyncVkExecuteRequestPool
-        
-            pool = AsyncVkExecuteRequestPool()
-            response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
-            response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
-            response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
-            response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
-            await pool.execute()
-            ...
-        
-Keywords: vk.com api vk wrappper asyncio
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Metadata-Version: 2.1
+Name: aiovk
+Version: 4.1.0
+Summary: vk.com API python wrapper for asyncio
+Home-page: https://github.com/alexanderlarin/aiovk
+Author: Alexander Larin
+Author-email: ekzebox@gmail.com
+License: MIT License
+Keywords: vk.com api vk wrappper asyncio
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+License-File: LICENSE
+
+vk.com API python wrapper for asyncio
+=====================================
+for old version of python you can use https://github.com/dimka665/vk
+
+Features
+--------
+* asynchronous
+* support python 3.5+ versions
+* have only one dependency - ``aiohttp 3+``
+* support two-factor authentication
+* support socks proxy with ``aiohttp-socks``
+* support rate limit of requests
+* support Long Poll connection
+
+TODO
+----
+* need refactoring tests for ``AsyncVkExecuteRequestPool``
+
+Install
+-------
+
+.. code-block:: bash
+
+    pip install aiovk
+
+Examples
+========
+Annotation
+----------
+In all the examples below, I will give only the ``{code}``
+
+.. code-block:: python
+
+    async def func():
+        {code}
+
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(func())
+
+
+Authorization
+-------------
+**TokenSession** - if you already have token or you use requests which don't require token
+
+.. code-block:: python
+
+    session = TokenSession()
+    session = TokenSession(access_token='asdf123..')
+
+**ImplicitSession** - client authorization in js apps and standalone (desktop and mobile) apps
+
+.. code-block:: python
+
+    >>> session = ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID)
+    >>> await session.authorize()
+    >>> session.access_token
+    asdfa2321afsdf12eadasf123...
+
+With scopes:
+
+.. code-block:: python
+
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify')
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify,friends')
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, ['notify', 'friends'])
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 3)  # notify and friends
+
+Also you can use ``SimpleImplicitSessionMixin`` for entering confirmation code
+or captcha key
+
+**AuthorizationCodeSession** - authorization for server apps or Open API
+
+See https://vk.com/dev/authcode_flow_user for getting the CODE
+
+.. code-block:: python
+
+    >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI, CODE)
+    >>> await session.authorize()
+    >>> session.access_token
+    asdfa2321afsdf12eadasf123...
+
+Or:
+
+.. code-block:: python
+
+    >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI)
+    >>> await session.authorize(CODE)
+    >>> session.access_token
+    asdfa2321afsdf12eadasf123...
+
+**Authorization using context manager** - you won't need to use session.close() after work
+
+.. code-block:: python
+
+    async with aiovk.TokenSession(access_token=YOUR_VK_TOKEN) as ses:
+        api = API(ses)...
+
+And your session will be closed after all done or code fail(similar to simple "with" usage)
+Works with all types of authorization
+
+Drivers
+-------
+**HttpDriver** - default driver for using ``aiohttp``
+
+.. code-block:: python
+
+    >>> driver = HttpDriver()
+    >>> driver = HttpDriver(timeout=10)  # default timeout for all requests
+
+.. code-block:: python
+
+    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT)  # 1234 is port
+    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, timeout=10)
+    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, PROXY_LOGIN, PROXY_PASSWORD, timeout=10)
+
+How to use custom driver with session:
+
+.. code-block:: python
+
+    >>> session = TokenSession(..., driver=HttpDriver())
+
+How to use driver with own loop:
+
+.. code-block:: python
+
+    >>> loop = asyncio.get_event_loop()
+    >>> asyncio.set_event_loop(None)
+    >>> session = TokenSession(driver=HttpDriver(loop=loop))  # or ProxyDriver
+
+How to use driver with custom http session object:
+
+Solve next problem: https://stackoverflow.com/questions/29827642/asynchronous-aiohttp-requests-fails-but-synchronous-requests-succeed
+
+.. code-block:: python
+
+    >>> connector = aiohttp.TCPConnector(verify_ssl=False)
+    >>> session = aiohttp.ClientSession(connector=connector)
+    >>> driver = HttpDriver(loop=loop, session=session)
+
+
+**LimitRateDriverMixin** - mixin class what allow you create new drivers with speed rate limits
+
+.. code-block:: python
+
+    >>> class ExampleDriver(LimitRateDriverMixin, HttpDriver):
+    ...     requests_per_period = 3
+    ...     period = 1  #seconds
+
+VK API
+------
+First variant:
+
+.. code-block:: python
+
+    >>> session = TokenSession()
+    >>> api = API(session)
+    >>> await api.users.get(user_ids=1)
+    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
+
+Second variant:
+
+.. code-block:: python
+
+    >>> session = TokenSession()
+    >>> api = API(session)
+    >>> await api('users.get', user_ids=1)
+    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
+
+Also you can add ``timeout`` argument for each request or define it in the session
+
+See https://vk.com/dev/methods for detailed API guide.
+
+Lazy VK API
+-----------
+It is useful when a bot has a large message flow
+
+.. code-block:: python
+
+    >>> session = TokenSession()
+    >>> api = LazyAPI(session)
+    >>> message = api.users.get(user_ids=1)
+    >>> await message()
+    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
+
+Supports both variants like API object
+
+User Long Poll
+--------------
+For documentation, see: https://vk.com/dev/using_longpoll
+
+Use exist API object
+
+.. code-block:: python
+
+    >>> api = API(session)
+    >>> lp = UserLongPoll(api, mode=2)  # default wait=25
+    >>> await lp.wait()
+    {"ts":1820350345,"updates":[...]}
+    >>> await lp.wait()
+    {"ts":1820351011,"updates":[...]}
+
+Use Session object
+
+.. code-block:: python
+
+    >>> lp = UserLongPoll(session, mode=2)  # default wait=25
+    >>> await lp.wait()
+    {"ts":1820350345,"updates":[...]}
+    >>> await lp.get_pts()  # return pts
+    191231223
+    >>> await lp.get_pts(need_ts=True)  # return pts, ts
+    191231223, 1820350345
+
+You can iterate over events
+
+.. code-block:: python
+
+    >>> async for event in lp.iter():
+    ...     print(event)
+    {"type":..., "object": {...}}
+
+Notice that ``wait`` value only for long pool connection.
+
+Real pause could be more ``wait`` time because of need time
+for authorization (if needed), reconnect and etc.
+
+Bots Long Poll
+--------------
+For documentation, see: https://vk.com/dev/bots_longpoll
+
+Use exist API object
+
+.. code-block:: python
+
+    >>> api = API(session)
+    >>> lp = BotsLongPoll(api, group_id=1)  # default wait=25
+    >>> await lp.wait()
+    {"ts":345,"updates":[...]}
+    >>> await lp.wait()
+    {"ts":346,"updates":[...]}
+
+Use Session object
+
+.. code-block:: python
+
+    >>> lp = BotsLongPoll(session, group_id=1)  # default wait=25
+    >>> await lp.wait()
+    {"ts":78455,"updates":[...]}
+    >>> await lp.get_pts()  # return pts
+    191231223
+    >>> await lp.get_pts(need_ts=True)  # return pts, ts
+    191231223, 1820350345
+
+BotsLongPoll supports iterating too
+
+.. code-block:: python
+
+    >>> async for event in lp.iter():
+    ...     print(event)
+    {"type":..., "object": {...}}
+
+Notice that ``wait`` value only for long pool connection.
+
+Real pause could be more ``wait`` time because of need time
+for authorization (if needed), reconnect and etc.
+
+Async execute request pool
+--------------------------
+For documentation, see: https://vk.com/dev/execute
+
+.. code-block:: python
+
+    from aiovk.pools import AsyncVkExecuteRequestPool
+
+    async with AsyncVkExecuteRequestPool() as pool:
+        response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
+        response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
+        response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
+        response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
+
+    >>> print(response.ok)
+    True
+    >>> print(response.result)
+    [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
+    >>> print(response2.result)
+    [{'id': 2, 'first_name': 'Александра', 'last_name': 'Владимирова'}]
+    >>> print(response3.result)
+    [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
+    >>> print(response4.ok)
+    False
+    >>> print(response4.error)
+    {'method': 'users.get', 'error_code': 113, 'error_msg': 'Invalid user id'}
+
+or
+
+.. code-block:: python
+
+    from aiovk.pools import AsyncVkExecuteRequestPool
+
+    pool = AsyncVkExecuteRequestPool()
+    response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
+    response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
+    response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
+    response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
+    await pool.execute()
+    ...
```

### Comparing `aiovk-4.0.0/README.rst` & `aiovk-4.1.0/README.rst`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,306 +1,306 @@
-vk.com API python wrapper for asyncio
-=====================================
-for old version of python you can use https://github.com/dimka665/vk
-
-Features
---------
-* asynchronous
-* support python 3.5+ versions
-* have only one dependency - ``aiohttp 3+``
-* support two-factor authentication
-* support socks proxy with ``aiohttp-socks``
-* support rate limit of requests
-* support Long Poll connection
-
-TODO
-----
-* need refactoring tests for ``AsyncVkExecuteRequestPool``
-
-Install
--------
-
-.. code-block:: bash
-
-    pip install aiovk
-
-Examples
-========
-Annotation
-----------
-In all the examples below, I will give only the ``{code}``
-
-.. code-block:: python
-
-    async def func():
-        {code}
-
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(func())
-
-
-Authorization
--------------
-**TokenSession** - if you already have token or you use requests which don't require token
-
-.. code-block:: python
-
-    session = TokenSession()
-    session = TokenSession(access_token='asdf123..')
-
-**ImplicitSession** - client authorization in js apps and standalone (desktop and mobile) apps
-
-.. code-block:: python
-
-    >>> session = ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID)
-    >>> await session.authorize()
-    >>> session.access_token
-    asdfa2321afsdf12eadasf123...
-
-With scopes:
-
-.. code-block:: python
-
-    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify')
-    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify,friends')
-    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, ['notify', 'friends'])
-    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 3)  # notify and friends
-
-Also you can use ``SimpleImplicitSessionMixin`` for entering confirmation code
-or captcha key
-
-**AuthorizationCodeSession** - authorization for server apps or Open API
-
-See https://vk.com/dev/authcode_flow_user for getting the CODE
-
-.. code-block:: python
-
-    >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI, CODE)
-    >>> await session.authorize()
-    >>> session.access_token
-    asdfa2321afsdf12eadasf123...
-
-Or:
-
-.. code-block:: python
-
-    >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI)
-    >>> await session.authorize(CODE)
-    >>> session.access_token
-    asdfa2321afsdf12eadasf123...
-
-**Authorization using context manager** - you won't need to use session.close() after work
-
-.. code-block:: python
-
-    async with aiovk.TokenSession(access_token=YOUR_VK_TOKEN) as ses:
-        api = API(ses)...
-
-And your session will be closed after all done or code fail(similar to simple "with" usage)
-Works with all types of authorization
-
-Drivers
--------
-**HttpDriver** - default driver for using ``aiohttp``
-
-.. code-block:: python
-
-    >>> driver = HttpDriver()
-    >>> driver = HttpDriver(timeout=10)  # default timeout for all requests
-
-.. code-block:: python
-
-    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT)  # 1234 is port
-    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, timeout=10)
-    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, PROXY_LOGIN, PROXY_PASSWORD, timeout=10)
-
-How to use custom driver with session:
-
-.. code-block:: python
-
-    >>> session = TokenSession(..., driver=HttpDriver())
-
-How to use driver with own loop:
-
-.. code-block:: python
-
-    >>> loop = asyncio.get_event_loop()
-    >>> asyncio.set_event_loop(None)
-    >>> session = TokenSession(driver=HttpDriver(loop=loop))  # or ProxyDriver
-
-How to use driver with custom http session object:
-
-Solve next problem: https://stackoverflow.com/questions/29827642/asynchronous-aiohttp-requests-fails-but-synchronous-requests-succeed
-
-.. code-block:: python
-
-    >>> connector = aiohttp.TCPConnector(verify_ssl=False)
-    >>> session = aiohttp.ClientSession(connector=connector)
-    >>> driver = HttpDriver(loop=loop, session=session)
-
-
-**LimitRateDriverMixin** - mixin class what allow you create new drivers with speed rate limits
-
-.. code-block:: python
-
-    >>> class ExampleDriver(LimitRateDriverMixin, HttpDriver):
-    ...     requests_per_period = 3
-    ...     period = 1  #seconds
-
-VK API
-------
-First variant:
-
-.. code-block:: python
-
-    >>> session = TokenSession()
-    >>> api = API(session)
-    >>> await api.users.get(user_ids=1)
-    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
-
-Second variant:
-
-.. code-block:: python
-
-    >>> session = TokenSession()
-    >>> api = API(session)
-    >>> await api('users.get', user_ids=1)
-    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
-
-Also you can add ``timeout`` argument for each request or define it in the session
-
-See https://vk.com/dev/methods for detailed API guide.
-
-Lazy VK API
------------
-It is useful when a bot has a large message flow
-
-.. code-block:: python
-
-    >>> session = TokenSession()
-    >>> api = LazyAPI(session)
-    >>> message = api.users.get(user_ids=1)
-    >>> await message()
-    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
-
-Supports both variants like API object
-
-User Long Poll
---------------
-For documentation, see: https://vk.com/dev/using_longpoll
-
-Use exist API object
-
-.. code-block:: python
-
-    >>> api = API(session)
-    >>> lp = UserLongPoll(api, mode=2)  # default wait=25
-    >>> await lp.wait()
-    {"ts":1820350345,"updates":[...]}
-    >>> await lp.wait()
-    {"ts":1820351011,"updates":[...]}
-
-Use Session object
-
-.. code-block:: python
-
-    >>> lp = UserLongPoll(session, mode=2)  # default wait=25
-    >>> await lp.wait()
-    {"ts":1820350345,"updates":[...]}
-    >>> await lp.get_pts()  # return pts
-    191231223
-    >>> await lp.get_pts(need_ts=True)  # return pts, ts
-    191231223, 1820350345
-
-You can iterate over events
-
-.. code-block:: python
-
-    >>> async for event in lp.iter():
-    ...     print(event)
-    {"type":..., "object": {...}}
-
-Notice that ``wait`` value only for long pool connection.
-
-Real pause could be more ``wait`` time because of need time
-for authorization (if needed), reconnect and etc.
-
-Bots Long Poll
---------------
-For documentation, see: https://vk.com/dev/bots_longpoll
-
-Use exist API object
-
-.. code-block:: python
-
-    >>> api = API(session)
-    >>> lp = BotsLongPoll(api, group_id=1)  # default wait=25
-    >>> await lp.wait()
-    {"ts":345,"updates":[...]}
-    >>> await lp.wait()
-    {"ts":346,"updates":[...]}
-
-Use Session object
-
-.. code-block:: python
-
-    >>> lp = BotsLongPoll(session, group_id=1)  # default wait=25
-    >>> await lp.wait()
-    {"ts":78455,"updates":[...]}
-    >>> await lp.get_pts()  # return pts
-    191231223
-    >>> await lp.get_pts(need_ts=True)  # return pts, ts
-    191231223, 1820350345
-
-BotsLongPoll supports iterating too
-
-.. code-block:: python
-
-    >>> async for event in lp.iter():
-    ...     print(event)
-    {"type":..., "object": {...}}
-
-Notice that ``wait`` value only for long pool connection.
-
-Real pause could be more ``wait`` time because of need time
-for authorization (if needed), reconnect and etc.
-
-Async execute request pool
---------------------------
-For documentation, see: https://vk.com/dev/execute
-
-.. code-block:: python
-
-    from aiovk.pools import AsyncVkExecuteRequestPool
-
-    async with AsyncVkExecuteRequestPool() as pool:
-        response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
-        response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
-        response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
-        response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
-
-    >>> print(response.ok)
-    True
-    >>> print(response.result)
-    [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
-    >>> print(response2.result)
-    [{'id': 2, 'first_name': 'Александра', 'last_name': 'Владимирова'}]
-    >>> print(response3.result)
-    [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
-    >>> print(response4.ok)
-    False
-    >>> print(response4.error)
-    {'method': 'users.get', 'error_code': 113, 'error_msg': 'Invalid user id'}
-
-or
-
-.. code-block:: python
-
-    from aiovk.pools import AsyncVkExecuteRequestPool
-
-    pool = AsyncVkExecuteRequestPool()
-    response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
-    response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
-    response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
-    response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
-    await pool.execute()
-    ...
+vk.com API python wrapper for asyncio
+=====================================
+for old version of python you can use https://github.com/dimka665/vk
+
+Features
+--------
+* asynchronous
+* support python 3.5+ versions
+* have only one dependency - ``aiohttp 3+``
+* support two-factor authentication
+* support socks proxy with ``aiohttp-socks``
+* support rate limit of requests
+* support Long Poll connection
+
+TODO
+----
+* need refactoring tests for ``AsyncVkExecuteRequestPool``
+
+Install
+-------
+
+.. code-block:: bash
+
+    pip install aiovk
+
+Examples
+========
+Annotation
+----------
+In all the examples below, I will give only the ``{code}``
+
+.. code-block:: python
+
+    async def func():
+        {code}
+
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(func())
+
+
+Authorization
+-------------
+**TokenSession** - if you already have token or you use requests which don't require token
+
+.. code-block:: python
+
+    session = TokenSession()
+    session = TokenSession(access_token='asdf123..')
+
+**ImplicitSession** - client authorization in js apps and standalone (desktop and mobile) apps
+
+.. code-block:: python
+
+    >>> session = ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID)
+    >>> await session.authorize()
+    >>> session.access_token
+    asdfa2321afsdf12eadasf123...
+
+With scopes:
+
+.. code-block:: python
+
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify')
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify,friends')
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, ['notify', 'friends'])
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 3)  # notify and friends
+
+Also you can use ``SimpleImplicitSessionMixin`` for entering confirmation code
+or captcha key
+
+**AuthorizationCodeSession** - authorization for server apps or Open API
+
+See https://vk.com/dev/authcode_flow_user for getting the CODE
+
+.. code-block:: python
+
+    >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI, CODE)
+    >>> await session.authorize()
+    >>> session.access_token
+    asdfa2321afsdf12eadasf123...
+
+Or:
+
+.. code-block:: python
+
+    >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI)
+    >>> await session.authorize(CODE)
+    >>> session.access_token
+    asdfa2321afsdf12eadasf123...
+
+**Authorization using context manager** - you won't need to use session.close() after work
+
+.. code-block:: python
+
+    async with aiovk.TokenSession(access_token=YOUR_VK_TOKEN) as ses:
+        api = API(ses)...
+
+And your session will be closed after all done or code fail(similar to simple "with" usage)
+Works with all types of authorization
+
+Drivers
+-------
+**HttpDriver** - default driver for using ``aiohttp``
+
+.. code-block:: python
+
+    >>> driver = HttpDriver()
+    >>> driver = HttpDriver(timeout=10)  # default timeout for all requests
+
+.. code-block:: python
+
+    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT)  # 1234 is port
+    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, timeout=10)
+    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, PROXY_LOGIN, PROXY_PASSWORD, timeout=10)
+
+How to use custom driver with session:
+
+.. code-block:: python
+
+    >>> session = TokenSession(..., driver=HttpDriver())
+
+How to use driver with own loop:
+
+.. code-block:: python
+
+    >>> loop = asyncio.get_event_loop()
+    >>> asyncio.set_event_loop(None)
+    >>> session = TokenSession(driver=HttpDriver(loop=loop))  # or ProxyDriver
+
+How to use driver with custom http session object:
+
+Solve next problem: https://stackoverflow.com/questions/29827642/asynchronous-aiohttp-requests-fails-but-synchronous-requests-succeed
+
+.. code-block:: python
+
+    >>> connector = aiohttp.TCPConnector(verify_ssl=False)
+    >>> session = aiohttp.ClientSession(connector=connector)
+    >>> driver = HttpDriver(loop=loop, session=session)
+
+
+**LimitRateDriverMixin** - mixin class what allow you create new drivers with speed rate limits
+
+.. code-block:: python
+
+    >>> class ExampleDriver(LimitRateDriverMixin, HttpDriver):
+    ...     requests_per_period = 3
+    ...     period = 1  #seconds
+
+VK API
+------
+First variant:
+
+.. code-block:: python
+
+    >>> session = TokenSession()
+    >>> api = API(session)
+    >>> await api.users.get(user_ids=1)
+    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
+
+Second variant:
+
+.. code-block:: python
+
+    >>> session = TokenSession()
+    >>> api = API(session)
+    >>> await api('users.get', user_ids=1)
+    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
+
+Also you can add ``timeout`` argument for each request or define it in the session
+
+See https://vk.com/dev/methods for detailed API guide.
+
+Lazy VK API
+-----------
+It is useful when a bot has a large message flow
+
+.. code-block:: python
+
+    >>> session = TokenSession()
+    >>> api = LazyAPI(session)
+    >>> message = api.users.get(user_ids=1)
+    >>> await message()
+    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
+
+Supports both variants like API object
+
+User Long Poll
+--------------
+For documentation, see: https://vk.com/dev/using_longpoll
+
+Use exist API object
+
+.. code-block:: python
+
+    >>> api = API(session)
+    >>> lp = UserLongPoll(api, mode=2)  # default wait=25
+    >>> await lp.wait()
+    {"ts":1820350345,"updates":[...]}
+    >>> await lp.wait()
+    {"ts":1820351011,"updates":[...]}
+
+Use Session object
+
+.. code-block:: python
+
+    >>> lp = UserLongPoll(session, mode=2)  # default wait=25
+    >>> await lp.wait()
+    {"ts":1820350345,"updates":[...]}
+    >>> await lp.get_pts()  # return pts
+    191231223
+    >>> await lp.get_pts(need_ts=True)  # return pts, ts
+    191231223, 1820350345
+
+You can iterate over events
+
+.. code-block:: python
+
+    >>> async for event in lp.iter():
+    ...     print(event)
+    {"type":..., "object": {...}}
+
+Notice that ``wait`` value only for long pool connection.
+
+Real pause could be more ``wait`` time because of need time
+for authorization (if needed), reconnect and etc.
+
+Bots Long Poll
+--------------
+For documentation, see: https://vk.com/dev/bots_longpoll
+
+Use exist API object
+
+.. code-block:: python
+
+    >>> api = API(session)
+    >>> lp = BotsLongPoll(api, group_id=1)  # default wait=25
+    >>> await lp.wait()
+    {"ts":345,"updates":[...]}
+    >>> await lp.wait()
+    {"ts":346,"updates":[...]}
+
+Use Session object
+
+.. code-block:: python
+
+    >>> lp = BotsLongPoll(session, group_id=1)  # default wait=25
+    >>> await lp.wait()
+    {"ts":78455,"updates":[...]}
+    >>> await lp.get_pts()  # return pts
+    191231223
+    >>> await lp.get_pts(need_ts=True)  # return pts, ts
+    191231223, 1820350345
+
+BotsLongPoll supports iterating too
+
+.. code-block:: python
+
+    >>> async for event in lp.iter():
+    ...     print(event)
+    {"type":..., "object": {...}}
+
+Notice that ``wait`` value only for long pool connection.
+
+Real pause could be more ``wait`` time because of need time
+for authorization (if needed), reconnect and etc.
+
+Async execute request pool
+--------------------------
+For documentation, see: https://vk.com/dev/execute
+
+.. code-block:: python
+
+    from aiovk.pools import AsyncVkExecuteRequestPool
+
+    async with AsyncVkExecuteRequestPool() as pool:
+        response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
+        response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
+        response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
+        response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
+
+    >>> print(response.ok)
+    True
+    >>> print(response.result)
+    [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
+    >>> print(response2.result)
+    [{'id': 2, 'first_name': 'Александра', 'last_name': 'Владимирова'}]
+    >>> print(response3.result)
+    [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
+    >>> print(response4.ok)
+    False
+    >>> print(response4.error)
+    {'method': 'users.get', 'error_code': 113, 'error_msg': 'Invalid user id'}
+
+or
+
+.. code-block:: python
+
+    from aiovk.pools import AsyncVkExecuteRequestPool
+
+    pool = AsyncVkExecuteRequestPool()
+    response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
+    response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
+    response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
+    response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
+    await pool.execute()
+    ...
```

### Comparing `aiovk-4.0.0/aiovk/exceptions.py` & `aiovk-4.1.0/aiovk/exceptions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from urllib.parse import urlencode
-
-
-CAPTCHA_IS_NEEDED = 14
-AUTHORIZATION_FAILED = 5  # invalid access token
-
-
-class VkException(Exception):
-    pass
-
-
-class VkAuthError(VkException):
-    def __init__(self, error, description, url='', params=''):
-        self.error = error
-        self.description = description
-        self.url = "{}?{}".format(url, urlencode(params))
-
-    def __str__(self):
-        return self.description
-
-
-class VkCaptchaNeeded(VkException):
-    def __init__(self, url, sid):
-        self.url = url
-        self.sid = sid
-
-    def __str__(self):
-        return "You must enter the captcha"
-
-
-class VkTwoFactorCodeNeeded(VkException):
-    def __str__(self):
-        return "In order to confirm that you are the owner of this page " \
-               "please enter the code provided by the code generating app."
-
-
-class VkAPIError(VkException):
-    def __init__(self, error, url):
-        self.error_code = error.get('error_code')
-        self.error_msg = error.get('error_msg')
-        self.params = {param['key']: param['value'] for param in error.get('request_params', [])}
-        self.url = url
-
-
-class VkLongPollError(VkException):
-    def __init__(self, error, description, url='', params=''):
-        self.error = error
-        self.description = description
-        self.url = "{}?{}".format(url, urlencode(params))
-
-    def __str__(self):
-        return self.description
+from urllib.parse import urlencode
+
+
+CAPTCHA_IS_NEEDED = 14
+AUTHORIZATION_FAILED = 5  # invalid access token
+
+
+class VkException(Exception):
+    pass
+
+
+class VkAuthError(VkException):
+    def __init__(self, error, description, url='', params=''):
+        self.error = error
+        self.description = description
+        self.url = "{}?{}".format(url, urlencode(params))
+
+    def __str__(self):
+        return self.description
+
+
+class VkCaptchaNeeded(VkException):
+    def __init__(self, url, sid):
+        self.url = url
+        self.sid = sid
+
+    def __str__(self):
+        return "You must enter the captcha"
+
+
+class VkTwoFactorCodeNeeded(VkException):
+    def __str__(self):
+        return "In order to confirm that you are the owner of this page " \
+               "please enter the code provided by the code generating app."
+
+
+class VkAPIError(VkException):
+    def __init__(self, error, url):
+        self.error_code = error.get('error_code')
+        self.error_msg = error.get('error_msg')
+        self.params = {param['key']: param['value'] for param in error.get('request_params', [])}
+        self.url = url
+
+
+class VkLongPollError(VkException):
+    def __init__(self, error, description, url='', params=''):
+        self.error = error
+        self.description = description
+        self.url = "{}?{}".format(url, urlencode(params))
+
+    def __str__(self):
+        return self.description
```

### Comparing `aiovk-4.0.0/aiovk/longpoll.py` & `aiovk-4.1.0/aiovk/longpoll.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-import json
-from abc import ABC, abstractmethod
-from typing import Union, Optional
-
-from aiovk import API
-from aiovk.api import LazyAPI
-from aiovk.exceptions import VkLongPollError
-
-
-class BaseLongPoll(ABC):
-    """Interface for all types of Longpoll API"""
-    def __init__(self, session_or_api, mode: Optional[Union[int, list]],
-                 wait: int = 25, version: int = 2, timeout: int = None):
-        """
-        :param session_or_api: session object or data for creating a new session
-        :type session_or_api: BaseSession or API or LazyAPI
-        :param mode: additional answer options
-        :param wait: waiting period
-        :param version: protocol version
-        :param timeout: timeout for *.getLongPollServer request in current session
-        """
-        if isinstance(session_or_api, (API, LazyAPI)):
-            self.api = session_or_api
-        else:
-            self.api = API(session_or_api)
-
-        self.timeout = timeout or self.api._session.timeout
-
-        if type(mode) == list:
-            mode = sum(mode)
-
-        self.base_params = {
-            'version': version,
-            'wait': wait,
-            'act': 'a_check'
-        }
-
-        if mode is not None:
-            self.base_params['mode'] = mode
-
-        self.pts = None
-        self.ts = None
-        self.key = None
-        self.base_url = None
-
-    @abstractmethod
-    async def _get_long_poll_server(self, need_pts: bool = False) -> None:
-        """Send *.getLongPollServer request and update internal data
-
-        :param need_pts: need return the pts field
-        """
-
-    async def wait(self, need_pts=False) -> dict:
-        """Send long poll request
-
-        :param need_pts: need return the pts field
-        """
-        if not self.base_url:
-            await self._get_long_poll_server(need_pts)
-
-        params = {
-            'ts': self.ts,
-            'key': self.key,
-        }
-        params.update(self.base_params)
-        # invalid mimetype from server
-        status, response, _ = await self.api._session.driver.get_text(
-            self.base_url, params,
-            timeout=2 * self.base_params['wait']
-        )
-
-        if status == 403:
-            raise VkLongPollError(403, 'smth weth wrong', self.base_url + '/', params)
-
-        response = json.loads(response)
-        failed = response.get('failed')
-
-        if not failed:
-            self.ts = response['ts']
-            return response
-
-        if failed == 1:
-            self.ts = response['ts']
-        elif failed == 4:
-            raise VkLongPollError(
-                4,
-                'An invalid version number was passed in the version parameter',
-                self.base_url + '/',
-                params
-            )
-        else:
-            self.base_url = None
-
-        return await self.wait()
-    
-    async def iter(self):
-        while True:
-            response = await self.wait()
-            for event in response['updates']:
-                yield event
-
-    async def get_pts(self, need_ts=False):
-        if not self.base_url or not self.pts:
-            await self._get_long_poll_server(need_pts=True)
-
-        if need_ts:
-            return self.pts, self.ts
-        return self.pts
-
-
-class UserLongPoll(BaseLongPoll):
-    """Implements https://vk.com/dev/using_longpoll"""
-    # False for testing
-    use_https = True
-
-    async def _get_long_poll_server(self, need_pts=False):
-        response = await self.api('messages.getLongPollServer', need_pts=int(need_pts), timeout=self.timeout)
-        self.pts = response.get('pts')
-        self.ts = response['ts']
-        self.key = response['key']
-        # fucking differences between long poll methods in vk api!
-        self.base_url = f'http{"s" if self.use_https else ""}://{response["server"]}'
-
-
-class LongPoll(UserLongPoll):
-    """Implements https://vk.com/dev/using_longpoll
-
-    This class for backward compatibility
-    """
-
-    
-class BotsLongPoll(BaseLongPoll):
-    """Implements https://vk.com/dev/bots_longpoll"""
-    def __init__(self, session_or_api, group_id, wait=25, version=1, timeout=None):
-        super().__init__(session_or_api, None, wait, version, timeout)
-        self.group_id = group_id
-
-    async def _get_long_poll_server(self, need_pts=False):
-        response = await self.api('groups.getLongPollServer', group_id=self.group_id)
-        self.pts = response.get('pts')
-        self.ts = response['ts']
-        self.key = response['key']
-        self.base_url = '{}'.format(response['server'])  # Method already returning url with https://
+import json
+from abc import ABC, abstractmethod
+from typing import Union, Optional
+
+from . import API
+from .api import LazyAPI
+from .exceptions import VkLongPollError
+
+
+class BaseLongPoll(ABC):
+    """Interface for all types of Longpoll API"""
+    def __init__(self, session_or_api, mode: Optional[Union[int, list]],
+                 wait: int = 25, version: int = 2, timeout: int = None):
+        """
+        :param session_or_api: session object or data for creating a new session
+        :type session_or_api: BaseSession or API or LazyAPI
+        :param mode: additional answer options
+        :param wait: waiting period
+        :param version: protocol version
+        :param timeout: timeout for *.getLongPollServer request in current session
+        """
+        if isinstance(session_or_api, (API, LazyAPI)):
+            self.api = session_or_api
+        else:
+            self.api = API(session_or_api)
+
+        self.timeout = timeout or self.api._session.timeout
+
+        if type(mode) == list:
+            mode = sum(mode)
+
+        self.base_params = {
+            'version': version,
+            'wait': wait,
+            'act': 'a_check'
+        }
+
+        if mode is not None:
+            self.base_params['mode'] = mode
+
+        self.pts = None
+        self.ts = None
+        self.key = None
+        self.base_url = None
+
+    @abstractmethod
+    async def _get_long_poll_server(self, need_pts: bool = False) -> None:
+        """Send *.getLongPollServer request and update internal data
+
+        :param need_pts: need return the pts field
+        """
+
+    async def wait(self, need_pts=False) -> dict:
+        """Send long poll request
+
+        :param need_pts: need return the pts field
+        """
+        if not self.base_url:
+            await self._get_long_poll_server(need_pts)
+
+        params = {
+            'ts': self.ts,
+            'key': self.key,
+        }
+        params.update(self.base_params)
+        # invalid mimetype from server
+        status, response, _ = await self.api._session.driver.get_text(
+            self.base_url, params,
+            timeout=2 * self.base_params['wait']
+        )
+
+        if status == 403:
+            raise VkLongPollError(403, 'smth weth wrong', self.base_url + '/', params)
+
+        response = json.loads(response)
+        failed = response.get('failed')
+
+        if not failed:
+            self.ts = response['ts']
+            return response
+
+        if failed == 1:
+            self.ts = response['ts']
+        elif failed == 4:
+            raise VkLongPollError(
+                4,
+                'An invalid version number was passed in the version parameter',
+                self.base_url + '/',
+                params
+            )
+        else:
+            self.base_url = None
+
+        return await self.wait()
+    
+    async def iter(self):
+        while True:
+            response = await self.wait()
+            for event in response['updates']:
+                yield event
+
+    async def get_pts(self, need_ts=False):
+        if not self.base_url or not self.pts:
+            await self._get_long_poll_server(need_pts=True)
+
+        if need_ts:
+            return self.pts, self.ts
+        return self.pts
+
+
+class UserLongPoll(BaseLongPoll):
+    """Implements https://vk.com/dev/using_longpoll"""
+    # False for testing
+    use_https = True
+
+    async def _get_long_poll_server(self, need_pts=False):
+        response = await self.api('messages.getLongPollServer', need_pts=int(need_pts), timeout=self.timeout)
+        self.pts = response.get('pts')
+        self.ts = response['ts']
+        self.key = response['key']
+        # fucking differences between long poll methods in vk api!
+        self.base_url = f'http{"s" if self.use_https else ""}://{response["server"]}'
+
+
+class LongPoll(UserLongPoll):
+    """Implements https://vk.com/dev/using_longpoll
+
+    This class for backward compatibility
+    """
+
+    
+class BotsLongPoll(BaseLongPoll):
+    """Implements https://vk.com/dev/bots_longpoll"""
+    def __init__(self, session_or_api, group_id, wait=25, version=1, timeout=None):
+        super().__init__(session_or_api, None, wait, version, timeout)
+        self.group_id = group_id
+
+    async def _get_long_poll_server(self, need_pts=False):
+        response = await self.api('groups.getLongPollServer', group_id=self.group_id)
+        self.pts = response.get('pts')
+        self.ts = response['ts']
+        self.key = response['key']
+        self.base_url = '{}'.format(response['server'])  # Method already returning url with https://
```

### Comparing `aiovk-4.0.0/aiovk/mixins.py` & `aiovk-4.1.0/aiovk/mixins.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from aiovk.drivers import BaseDriver
-from aiovk.shaping import TaskQueue, wait_free_slot
-
-
-class LimitRateDriverMixin(BaseDriver):
-    def __init__(self, *args, requests_per_period=3, period=1, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._queue = TaskQueue(requests_per_period, period)
-
-    @wait_free_slot
-    async def post_json(self, *args, **kwargs):
-        return await super().post_json(*args, **kwargs)
-
-    @wait_free_slot
-    async def get_bin(self, *args, **kwargs):
-        return await super().get_bin(*args, **kwargs)
-
-    @wait_free_slot
-    async def get_text(self, *args, **kwargs):
-        return await super().get_text(*args, **kwargs)
-
-    @wait_free_slot
-    async def post_text(self, *args, **kwargs):
-        return await super().post_text(*args, **kwargs)
-
-    async def close(self):
-        await super().close()
-        self._queue.cancel()
-
-
-class SimpleImplicitSessionMixin:
-    """
-    Simple implementation of processing captcha and 2factor authorization
-    """
-
-    async def enter_captcha(self, url, sid):
-        bytes = await self.driver.get_bin(url, {})
-        with open('captcha.jpg', 'wb') as f:
-            f.write(bytes)
-        return input("Enter captcha: ")
-
-    async def enter_confirmation_сode(self):
-        return input('Enter confirmation сode: ')
+from .drivers import BaseDriver
+from .shaping import TaskQueue, wait_free_slot
+
+
+class LimitRateDriverMixin(BaseDriver):
+    def __init__(self, *args, requests_per_period=3, period=1, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._queue = TaskQueue(requests_per_period, period)
+
+    @wait_free_slot
+    async def post_json(self, *args, **kwargs):
+        return await super().post_json(*args, **kwargs)
+
+    @wait_free_slot
+    async def get_bin(self, *args, **kwargs):
+        return await super().get_bin(*args, **kwargs)
+
+    @wait_free_slot
+    async def get_text(self, *args, **kwargs):
+        return await super().get_text(*args, **kwargs)
+
+    @wait_free_slot
+    async def post_text(self, *args, **kwargs):
+        return await super().post_text(*args, **kwargs)
+
+    async def close(self):
+        await super().close()
+        self._queue.cancel()
+
+
+class SimpleImplicitSessionMixin:
+    """
+    Simple implementation of processing captcha and 2factor authorization
+    """
+
+    async def enter_captcha(self, url, sid):
+        bytes = await self.driver.get_bin(url, {})
+        with open('captcha.jpg', 'wb') as f:
+            f.write(bytes)
+        return input("Enter captcha: ")
+
+    async def enter_confirmation_сode(self):
+        return input('Enter confirmation сode: ')
```

### Comparing `aiovk-4.0.0/aiovk/parser.py` & `aiovk-4.1.0/aiovk/parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,100 @@
-import html.parser
-import urllib.parse
-
-
-class AuthPageParser(html.parser.HTMLParser):
-    def __init__(self):
-        super().__init__()
-        self.inputs = []
-        self.url = ''
-        self.message = ''
-        self.recording = 0
-        self.captcha_url = ''
-
-    def handle_starttag(self, tag, attrs):
-        if tag == 'input':
-            attrs = dict(attrs)
-            if attrs['type'] != 'submit':
-                self.inputs.append((attrs['name'], attrs.get('value', '')))
-        elif tag == 'form':
-            for name, value in attrs:
-                if name == 'action':
-                    self.url = value
-        elif tag == 'img':
-            attrs = dict(attrs)
-            if attrs.get('class', '') == 'captcha_img':
-                self.captcha_url = attrs['src']
-        elif tag == 'div':
-            attrs = dict(attrs)
-            if attrs.get('class', '') == 'service_msg service_msg_warning':
-                self.recording = 1
-
-    def handle_endtag(self, tag):
-        if tag == 'div':
-            self.recording = 0
-
-    def handle_data(self, data):
-        if self.recording:
-            self.message = data
-
-
-class TwoFactorCodePageParser(html.parser.HTMLParser):
-    def __init__(self):
-        super().__init__()
-        self.inputs = []
-        self.url = ''
-        self.message = ''
-        self.recording = 0
-
-    def handle_starttag(self, tag, attrs):
-        if tag == 'input':
-            attrs = dict(attrs)
-            if attrs['type'] != 'submit':
-                self.inputs.append((attrs['name'], attrs.get('value', '')))
-        elif tag == 'form':
-            for name, value in attrs:
-                if name == 'action':
-                    self.url = urllib.parse.urljoin('https://m.vk.com/', value)
-        elif tag == 'div':
-            attrs = dict(attrs)
-            if attrs.get('class', '') == 'service_msg service_msg_warning':
-                self.recording = 1
-
-    def handle_endtag(self, tag):
-        if tag == 'div':
-            self.recording = 0
-
-    def handle_data(self, data):
-        if self.recording:
-            self.message += data
-
-
-class AccessPageParser(html.parser.HTMLParser):
-    def __init__(self):
-        super().__init__()
-        self.inputs = []
-        self.url = ''
-
-    def handle_starttag(self, tag, attrs):
-        if tag == 'input':
-            attrs = dict(attrs)
-            if attrs['type'] != 'submit':
-                self.inputs.append((attrs['name'], attrs.get('value', '')))
-        elif tag == 'form':
-            for name, value in attrs:
-                if name == 'action':
-                    self.url = value
+import re
+import html.parser
+import urllib.parse
+
+
+class AuthPageParser(html.parser.HTMLParser):
+    def __init__(self):
+        super().__init__()
+        self.inputs = []
+        self.url = ''
+        self.message = ''
+        self.recording = 0
+        self.captcha_url = ''
+
+    def handle_starttag(self, tag, attrs):
+        if tag == 'input':
+            attrs = dict(attrs)
+            if attrs['type'] != 'submit':
+                self.inputs.append((attrs['name'], attrs.get('value', '')))
+        elif tag == 'form':
+            for name, value in attrs:
+                if name == 'action':
+                    self.url = value
+        elif tag == 'img':
+            attrs = dict(attrs)
+            if attrs.get('class', '') == 'captcha_img':
+                self.captcha_url = attrs['src']
+        elif tag == 'div':
+            attrs = dict(attrs)
+            if attrs.get('class', '') == 'service_msg service_msg_warning':
+                self.recording = 1
+
+    def handle_endtag(self, tag):
+        if tag == 'div':
+            self.recording = 0
+
+    def handle_data(self, data):
+        if self.recording:
+            self.message = data
+
+
+class TwoFactorCodePageParser(html.parser.HTMLParser):
+    def __init__(self):
+        super().__init__()
+        self.inputs = []
+        self.url = ''
+        self.message = ''
+        self.recording = 0
+
+    def handle_starttag(self, tag, attrs):
+        if tag == 'input':
+            attrs = dict(attrs)
+            if attrs['type'] != 'submit':
+                self.inputs.append((attrs['name'], attrs.get('value', '')))
+        elif tag == 'form':
+            for name, value in attrs:
+                if name == 'action':
+                    self.url = urllib.parse.urljoin('https://m.vk.com/', value)
+        elif tag == 'div':
+            attrs = dict(attrs)
+            if attrs.get('class', '') == 'service_msg service_msg_warning':
+                self.recording = 1
+
+    def handle_endtag(self, tag):
+        if tag == 'div':
+            self.recording = 0
+
+    def handle_data(self, data):
+        if self.recording:
+            self.message += data
+
+
+class AccessPageParser(html.parser.HTMLParser):
+    def __init__(self):
+        super().__init__()
+        self.inputs = []
+        self.url = ''
+
+    def handle_starttag(self, tag, attrs):
+        if tag == 'input':
+            attrs = dict(attrs)
+            if attrs['type'] != 'submit':
+                self.inputs.append((attrs['name'], attrs.get('value', '')))
+        elif tag == 'form':
+            for name, value in attrs:
+                if name == 'action':
+                    self.url = value
+
+
+class AuthRedirectPageParser(html.parser.HTMLParser):
+    def __init__(self):
+        super().__init__()
+        self.location = ''
+
+    def handle_starttag(self, tag, attrs):
+        if tag == 'meta':
+            attrs = dict(attrs)
+            if attrs.get('http-equiv') == 'refresh':
+                content = attrs['content']
+                self.location = re.findall(r'URL=(.*)$', content)[0]
```

### Comparing `aiovk-4.0.0/aiovk/pools.py` & `aiovk-4.1.0/aiovk/pools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-import asyncio
-import json
-from collections import defaultdict
-from dataclasses import dataclass
-from typing import List, Dict, Optional
-
-from aiovk import TokenSession, API
-from aiovk.exceptions import VkAuthError
-
-
-class AsyncResult:
-    def __init__(self):
-        self._result = None
-        self.ready = False
-        self.error = None
-
-    @property
-    def result(self):
-        return self._result
-
-    @result.setter
-    def result(self, val):
-        self._result = val
-        self.ready = True
-
-    @property
-    def ok(self):
-        return self.ready and not self.error
-
-
-@dataclass
-class VkCall:
-    method: str
-    method_args: dict
-    result: AsyncResult
-
-    def get_execute_representation(self) -> str:
-        return f"API.{self.method}({json.dumps(self.method_args, ensure_ascii=False)})"
-
-
-class AsyncVkExecuteRequestPool:
-    """
-    Allows concatenation of api calls using one token into groups and execute each group of hits in
-    one request using `execute` method
-    """
-
-    def __init__(self, call_number_per_request=25, token_session_class=TokenSession):
-        self.token_session_class = token_session_class
-        self.call_number_per_request = call_number_per_request
-        self.pool: Dict[str, List[VkCall]] = defaultdict(list)
-        self.sessions = []
-
-    async def __aenter__(self):
-        return self
-
-    async def __aexit__(self, *args, **kwargs):
-        await self.execute()
-
-    async def execute(self):
-        try:
-            await self._execute()
-            await asyncio.gather(*[session.close() for session in self.sessions])
-        finally:
-            self.pool.clear()
-            self.sessions.clear()
-
-    async def _execute(self):
-        """
-        Groups hits and executes them using the execute method, after execution the pool is cleared
-        """
-        executed_pools = []
-        for token, calls in self.pool.items():
-            session = self.token_session_class(token)
-            self.sessions.append(session)
-            api = API(session)
-
-            for methods_pool in chunks(calls, self.call_number_per_request):
-                executed_pools.append(VkExecuteMethodsPool(methods_pool).execute(api))
-        await asyncio.gather(*executed_pools)
-
-    def add_call(self, method, token, method_args=None) -> AsyncResult:
-        """
-        Adds an any api method call to the execute pool
-
-        :param method: api vk method name
-        :param token: session token
-        :param method_args: params
-        :return: object that will contain the result after the pool is closed
-        """
-        if method_args is None:
-            method_args = {}
-
-        result = None
-        # searching already added calls with equal token, method and values
-        for call in self.pool[token]:
-            if call.method == method and call.method_args == method_args:
-                result = call.result
-                break
-        if result:
-            return result
-        result = AsyncResult()
-        self.pool[token].append(VkCall(method=method, method_args=method_args, result=result))
-        return result
-
-
-class VkExecuteMethodsPool:
-    def __init__(self, pool: Optional[VkCall] = None):
-        if not pool:
-            pool = []
-        self.pool: List[VkCall] = pool
-
-    async def execute(self, api: API):
-        """
-        Executes calls to the pool using the execute method and stores the results for each call
-
-        :param api: API object to make the request
-        """
-        methods = [call.get_execute_representation() for call in self.pool]
-        code = f"return [{','.join(methods)}];"
-        try:
-            response = await api.execute(code=code, raw_response=True)
-        except VkAuthError as e:
-            for call in self.pool:
-                call.result.error = {
-                    'method': call.method,
-                    'error_code': 5,
-                    'error_msg': e.description
-                }
-            return
-        errors = response.pop('execute_errors', [])[::-1]
-        response = response['response']
-
-        for call, result in zip(self.pool, response):
-            if result is False:
-                call.result.error = errors.pop()
-            else:
-                call.result.result = result
-
-
-def chunks(lst, n):
-    """Yield successive n-sized chunks from lst."""
-    for i in range(0, len(lst), n):
-        yield lst[i: i + n]
+import asyncio
+import json
+from collections import defaultdict
+from dataclasses import dataclass
+from typing import List, Dict, Optional
+
+from . import TokenSession, API
+from .exceptions import VkAuthError
+
+
+class AsyncResult:
+    def __init__(self):
+        self._result = None
+        self.ready = False
+        self.error = None
+
+    @property
+    def result(self):
+        return self._result
+
+    @result.setter
+    def result(self, val):
+        self._result = val
+        self.ready = True
+
+    @property
+    def ok(self):
+        return self.ready and not self.error
+
+
+@dataclass
+class VkCall:
+    method: str
+    method_args: dict
+    result: AsyncResult
+
+    def get_execute_representation(self) -> str:
+        return f"API.{self.method}({json.dumps(self.method_args, ensure_ascii=False)})"
+
+
+class AsyncVkExecuteRequestPool:
+    """
+    Allows concatenation of api calls using one token into groups and execute each group of hits in
+    one request using `execute` method
+    """
+
+    def __init__(self, call_number_per_request=25, token_session_class=TokenSession):
+        self.token_session_class = token_session_class
+        self.call_number_per_request = call_number_per_request
+        self.pool: Dict[str, List[VkCall]] = defaultdict(list)
+        self.sessions = []
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, *args, **kwargs):
+        await self.execute()
+
+    async def execute(self):
+        try:
+            await self._execute()
+            await asyncio.gather(*[session.close() for session in self.sessions])
+        finally:
+            self.pool.clear()
+            self.sessions.clear()
+
+    async def _execute(self):
+        """
+        Groups hits and executes them using the execute method, after execution the pool is cleared
+        """
+        executed_pools = []
+        for token, calls in self.pool.items():
+            session = self.token_session_class(token)
+            self.sessions.append(session)
+            api = API(session)
+
+            for methods_pool in chunks(calls, self.call_number_per_request):
+                executed_pools.append(VkExecuteMethodsPool(methods_pool).execute(api))
+        await asyncio.gather(*executed_pools)
+
+    def add_call(self, method, token, method_args=None) -> AsyncResult:
+        """
+        Adds an any api method call to the execute pool
+
+        :param method: api vk method name
+        :param token: session token
+        :param method_args: params
+        :return: object that will contain the result after the pool is closed
+        """
+        if method_args is None:
+            method_args = {}
+
+        result = None
+        # searching already added calls with equal token, method and values
+        for call in self.pool[token]:
+            if call.method == method and call.method_args == method_args:
+                result = call.result
+                break
+        if result:
+            return result
+        result = AsyncResult()
+        self.pool[token].append(VkCall(method=method, method_args=method_args, result=result))
+        return result
+
+
+class VkExecuteMethodsPool:
+    def __init__(self, pool: Optional[VkCall] = None):
+        if not pool:
+            pool = []
+        self.pool: List[VkCall] = pool
+
+    async def execute(self, api: API):
+        """
+        Executes calls to the pool using the execute method and stores the results for each call
+
+        :param api: API object to make the request
+        """
+        methods = [call.get_execute_representation() for call in self.pool]
+        code = f"return [{','.join(methods)}];"
+        try:
+            response = await api.execute(code=code, raw_response=True)
+        except VkAuthError as e:
+            for call in self.pool:
+                call.result.error = {
+                    'method': call.method,
+                    'error_code': 5,
+                    'error_msg': e.description
+                }
+            return
+        errors = response.pop('execute_errors', [])[::-1]
+        response = response['response']
+
+        for call, result in zip(self.pool, response):
+            if result is False:
+                call.result.error = errors.pop()
+            else:
+                call.result.result = result
+
+
+def chunks(lst, n):
+    """Yield successive n-sized chunks from lst."""
+    for i in range(0, len(lst), n):
+        yield lst[i: i + n]
```

### Comparing `aiovk-4.0.0/aiovk/sessions.py` & `aiovk-4.1.0/aiovk/sessions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,326 +1,346 @@
-import json
-from abc import ABC, abstractmethod
-from typing import Tuple
-from urllib.parse import parse_qsl
-
-from yarl import URL
-
-from aiovk.drivers import HttpDriver
-from aiovk.exceptions import AUTHORIZATION_FAILED, CAPTCHA_IS_NEEDED, VkAPIError, VkAuthError, VkCaptchaNeeded, \
-    VkTwoFactorCodeNeeded
-from aiovk.parser import AccessPageParser, AuthPageParser, TwoFactorCodePageParser
-
-
-class BaseSession(ABC):
-    """Interface for all types of sessions"""
-
-    @abstractmethod
-    async def __aenter__(self):
-        """Make avaliable usage of "async with" context manager"""
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        """Closes session after usage of context manager with Session"""
-        await self.close()
-
-    async def close(self) -> None:
-        """Perform the actions associated with the completion of the current session"""
-
-    @abstractmethod
-    async def send_api_request(self, method_name: str, params: dict = None, timeout: int = None,
-                               raw_response: bool = False) -> dict:
-        """Method that use API instance for sending request to vk server
-
-        :param method_name: any value from the left column of the methods table from `https://vk.com/dev/methods`
-        :param params: dict of params that available for current method.
-                       For example see `Parameters` block from: `https://vk.com/dev/account.getInfo`
-        :param timeout: timeout for response from the server
-        :param raw_response: return full response
-        :return: dict that contain data from `Result` block. Example see here: `https://vk.com/dev/account.getInfo`
-        """
-
-
-class TokenSession(BaseSession):
-    """Implements simple session that uses existed token for work"""
-
-    API_VERSION = '5.74'
-    REQUEST_URL = 'https://api.vk.com/method/'
-
-    def __init__(self, access_token: str = None, timeout: int = 10, driver=None):
-        """
-        :param access_token: see `User Token` block from `https://vk.com/dev/access_token`
-        :param timeout: default time out for any request in current session
-        :param driver: TODO add description
-        """
-        self.timeout = timeout
-        self.access_token = access_token
-        self.driver = HttpDriver(timeout) if driver is None else driver
-
-    async def __aenter__(self) -> BaseSession:
-        """Make available usage of `async with` context manager"""
-        return self
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        return await self.close()
-
-    async def send_api_request(self, method_name: str, params: dict = None, timeout: int = None,
-                               raw_response: bool = False) -> dict:
-        # Prepare request
-        if not timeout:
-            timeout = self.timeout
-        if not params:
-            params = {}
-        if self.access_token:
-            params['access_token'] = self.access_token
-        if 'v' not in params:
-            params['v'] = self.API_VERSION
-
-        # Send request
-        _, response = await self.driver.post_json(self.REQUEST_URL + method_name, params, timeout)
-
-        # Process response
-        # Checking the section with errors
-        error = response.get('error')
-        if error:
-            err_code = error.get('error_code')
-            if err_code == CAPTCHA_IS_NEEDED:
-                # Collect information about Captcha
-                captcha_sid = error.get('captcha_sid')
-                captcha_url = error.get('captcha_img')
-                params['captcha_key'] = await self.enter_captcha(captcha_url, captcha_sid)
-                params['captcha_sid'] = captcha_sid
-                # Send request again
-                # Provide one attempt to repeat the request
-                return await self.send_api_request(method_name, params, timeout, raw_response)
-            elif err_code == AUTHORIZATION_FAILED:
-                await self.authorize()
-                # Send request again
-                # Provide one attempt to repeat the request
-                return await self.send_api_request(method_name, params, timeout, raw_response)
-            else:
-                # Other errors is not related with security
-                raise VkAPIError(error, self.REQUEST_URL + method_name)
-        if raw_response:
-            return response
-        # Return only useful data
-        return response['response']
-
-    async def authorize(self) -> None:
-        """Getting a new token from server"""
-        # For `TokenSession` we have not credentials for getting new token
-        raise VkAuthError('invalid_token', 'User authorization failed')
-
-    async def enter_captcha(self, url: str, sid: str) -> str:
-        """
-        Override this method for processing captcha.
-
-        :param url: link to captcha image
-        :param sid: captcha id. I do not know why pass here but may be useful
-        :return captcha value
-        """
-        raise VkCaptchaNeeded(url, sid)
-
-    async def close(self):
-        return await self.driver.close()
-
-
-class ImplicitSession(TokenSession):
-    """
-    For client authorization in js apps and standalone (desktop and mobile) apps
-    See more in https://new.vk.com/dev/implicit_flow_user
-    """
-    AUTH_URL = 'https://oauth.vk.com/authorize'
-
-    def __init__(self, login: str, password: str, app_id: int, scope: str or int or list = None,
-                 timeout: int = 10, num_of_attempts: int = 5, driver=None):
-        """
-        :param login: user login
-        :param password: user password
-        :param app_id: application id. More details in `Application registration` block in `https://vk.com/dev/first_guide`
-        :param scope: access rights. See `Access rights` block in `https://vk.com/dev/first_guide`
-        :param timeout: default time out for any request in current session
-        :param num_of_attempts: number of authorization attempts
-        :param driver: TODO add description
-        """
-        super().__init__(access_token=None, timeout=timeout, driver=driver)
-        self.login = login
-        self.password = password
-        self.app_id = app_id
-        self.num_of_attempts = num_of_attempts
-        if isinstance(scope, (str, int, type(None))):
-            self.scope = scope
-        elif isinstance(scope, list):
-            self.scope = ",".join(scope)
-
-    async def authorize(self) -> None:
-        """Getting a new token from server"""
-        url, html = await self._get_auth_page()
-        for step in range(self.num_of_attempts):
-            if url.path == '/authorize':
-                if '__q_hash' in url.query:
-                    # Give rights for app
-                    url, html = await self._process_access_form(html)
-                else:
-                    # Invalid login or password  and 'email' in q.query
-                    url, html = await self._process_auth_form(html)
-            if url.path == '/login' and url.query.get('act', '') == 'authcheck':
-                # Entering 2auth code
-                url, html = await self._process_2auth_form(html)
-            if url.path == '/login' and url.query.get('act', '') == 'authcheck_code':
-                # Need captcha
-                url, html = await self._process_auth_form(html)
-            if url.path == '/authorize' and '__q_hash' in url.query:
-                # Give rights for app
-                url, html = await self._process_access_form(html)
-            if url.path == '/blank.html':
-                # Success
-                parsed_fragments = dict(parse_qsl(url.fragment))
-                self.access_token = parsed_fragments['access_token']
-                return
-        raise VkAuthError('Something went wrong', 'Exceeded the number of attempts to log in')
-
-    async def _get_auth_page(self) -> Tuple[str, str]:
-        """
-        Get authorization mobile page without js
-        :return: redirect_url, html page
-        """
-        # Prepare request
-        params = {
-            'client_id': self.app_id,
-            'redirect_uri': 'https://oauth.vk.com/blank.html',
-            'display': 'mobile',
-            'response_type': 'token',
-            'v': self.API_VERSION
-        }
-        if self.scope:
-            params['scope'] = self.scope
-
-        # Send request
-        status, response, redirect_url = await self.driver.get_text(self.AUTH_URL, params)
-
-        # Process response
-        if status != 200:
-            error_dict = json.loads(response)
-            raise VkAuthError(error_dict['error'], error_dict['error_description'], self.AUTH_URL, params)
-        return redirect_url, response
-
-    async def _process_auth_form(self, html: str) -> (str, str):
-        """
-        Parsing data from authorization page and filling the form and submitting the form
-
-        :param html: html page
-        :return: url and  html from redirected page
-        """
-        # Parse page
-        p = AuthPageParser()
-        p.feed(html)
-        p.close()
-
-        # Get data from hidden inputs
-        form_data = dict(p.inputs)
-        form_url = p.url
-        form_data['email'] = self.login
-        form_data['pass'] = self.password
-        if p.message:
-            # Show form errors
-            raise VkAuthError('invalid_data', p.message, form_url, form_data)
-        elif p.captcha_url:
-            form_data['captcha_key'] = await self.enter_captcha(
-                "https://m.vk.com{}".format(p.captcha_url),
-                form_data['captcha_sid']
-            )
-            form_url = "https://m.vk.com{}".format(form_url)
-
-        # Send request
-        _, html, redirect_url = await self.driver.post_text(form_url, form_data)
-        return redirect_url, html
-
-    async def _process_2auth_form(self, html: str) -> (str, str):
-        """
-        Parsing two-factor authorization page and filling the code
-
-        :param html: html page
-        :return: url and  html from redirected page
-        """
-        # Parse page
-        p = TwoFactorCodePageParser()
-        p.feed(html)
-        p.close()
-
-        # Prepare request data
-        form_url = p.url
-        form_data = dict(p.inputs)
-        form_data['remember'] = 0
-        if p.message:
-            raise VkAuthError('invalid_data', p.message, form_url, form_data)
-        form_data['code'] = await self.enter_confirmation_code()
-
-        # Send request
-        _, html, redirect_url = await self.driver.post_text(form_url, form_data)
-        return redirect_url, html
-
-    async def _process_access_form(self, html: str) -> (str, str):
-        """
-        Parsing page with access rights
-
-        :param html: html page
-        :return: url and  html from redirected page
-        """
-        # Parse page
-        p = AccessPageParser()
-        p.feed(html)
-        p.close()
-
-        form_url = p.url
-        form_data = dict(p.inputs)
-
-        # Send request
-        _, html, redirect_url = await self.driver.post_text(form_url, form_data)
-        return redirect_url, html
-
-    async def enter_confirmation_code(self) -> str:
-        """
-        Override this method for processing confirmation 2uth code.
-        :return confirmation code
-        """
-        raise VkTwoFactorCodeNeeded()
-
-
-class AuthorizationCodeSession(TokenSession):
-    """
-    For client authorization in js apps and standalone (desktop and mobile) apps
-    See more in https://new.vk.com/dev/implicit_flow_user
-    """
-    CODE_URL = 'https://oauth.vk.com/access_token'
-
-    def __init__(self, app_id: int, app_secret: str, redirect_uri: str, code: str, timeout: int = 10, driver=None):
-        """
-        :param app_id: application id. More details in `Application registration` block in `https://vk.com/dev/first_guide`
-        :param app_secret: application secure key. See https://vk.com/editapp?id={app_id}&section=options
-        :param redirect_uri: Authorized redirect URI.
-        :param code: See `https://vk.com/dev/authcode_flow_user`
-        :param timeout:default time out for any request in current session
-        :param driver: TODO add description
-        """
-        super().__init__(access_token=None, timeout=timeout, driver=driver)
-        self.code = code
-        self.app_id = app_id
-        self.app_secret = app_secret
-        self.redirect_uri = redirect_uri
-
-    async def authorize(self, code: str = None) -> None:
-        """Getting a new token from server"""
-        code = await self.get_code(code)
-        params = {
-            'client_id': self.app_id,
-            'client_secret': self.app_secret,
-            'redirect_uri': self.redirect_uri,
-            'code': code
-        }
-        _, response = await self.driver.post_json(self.CODE_URL, params, self.timeout)
-        if 'error' in response:
-            raise VkAuthError(response['error'], response['error_description'], self.CODE_URL, params)
-        self.access_token = response['access_token']
-
-    async def get_code(self, code: str = None) -> str:
-        """Get temporary code from external sources"""
-        return code or self.code
+import json
+from abc import ABC, abstractmethod
+from typing import Tuple
+from urllib.parse import parse_qsl
+
+import aiohttp.hdrs
+
+from .drivers import HttpDriver
+from .exceptions import AUTHORIZATION_FAILED, CAPTCHA_IS_NEEDED, VkAPIError, VkAuthError, VkCaptchaNeeded, \
+    VkTwoFactorCodeNeeded
+from .parser import AccessPageParser, AuthPageParser, TwoFactorCodePageParser, AuthRedirectPageParser
+
+
+class BaseSession(ABC):
+    """Interface for all types of sessions"""
+
+    @abstractmethod
+    async def __aenter__(self):
+        """Make avaliable usage of "async with" context manager"""
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        """Closes session after usage of context manager with Session"""
+        await self.close()
+
+    async def close(self) -> None:
+        """Perform the actions associated with the completion of the current session"""
+
+    @abstractmethod
+    async def send_api_request(self, method_name: str, params: dict = None, timeout: int = None,
+                               raw_response: bool = False) -> dict:
+        """Method that use API instance for sending request to vk server
+
+        :param method_name: any value from the left column of the methods table from `https://vk.com/dev/methods`
+        :param params: dict of params that available for current method.
+                       For example see `Parameters` block from: `https://vk.com/dev/account.getInfo`
+        :param timeout: timeout for response from the server
+        :param raw_response: return full response
+        :return: dict that contain data from `Result` block. Example see here: `https://vk.com/dev/account.getInfo`
+        """
+
+
+class TokenSession(BaseSession):
+    """Implements simple session that uses existed token for work"""
+
+    API_VERSION = '5.81'
+    REQUEST_URL = 'https://api.vk.com/method/'
+
+    def __init__(self, access_token: str = None, timeout: int = 10, driver=None):
+        """
+        :param access_token: see `User Token` block from `https://vk.com/dev/access_token`
+        :param timeout: default time out for any request in current session
+        :param driver: TODO add description
+        """
+        self.timeout = timeout
+        self.access_token = access_token
+        self.driver = HttpDriver(timeout) if driver is None else driver
+
+    async def __aenter__(self) -> BaseSession:
+        """Make available usage of `async with` context manager"""
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        return await self.close()
+
+    async def send_api_request(self, method_name: str, params: dict = None, timeout: int = None,
+                               raw_response: bool = False) -> dict:
+        # Prepare request
+        if not timeout:
+            timeout = self.timeout
+        if not params:
+            params = {}
+        if self.access_token:
+            params['access_token'] = self.access_token
+        if 'v' not in params:
+            params['v'] = self.API_VERSION
+
+        # Send request
+        _, response = await self.driver.post_json(self.REQUEST_URL + method_name, params, timeout=timeout)
+
+        # Process response
+        # Checking the section with errors
+        error = response.get('error')
+        if error:
+            err_code = error.get('error_code')
+            if err_code == CAPTCHA_IS_NEEDED:
+                # Collect information about Captcha
+                captcha_sid = error.get('captcha_sid')
+                captcha_url = error.get('captcha_img')
+                params['captcha_key'] = await self.enter_captcha(captcha_url, captcha_sid)
+                params['captcha_sid'] = captcha_sid
+                # Send request again
+                # Provide one attempt to repeat the request
+                return await self.send_api_request(method_name, params, timeout, raw_response)
+            elif err_code == AUTHORIZATION_FAILED:
+                await self.authorize()
+                # Send request again
+                # Provide one attempt to repeat the request
+                return await self.send_api_request(method_name, params, timeout, raw_response)
+            else:
+                # Other errors is not related with security
+                raise VkAPIError(error, self.REQUEST_URL + method_name)
+        if raw_response:
+            return response
+        # Return only useful data
+        return response['response']
+
+    async def authorize(self) -> None:
+        """Getting a new token from server"""
+        # For `TokenSession` we have not credentials for getting new token
+        raise VkAuthError('invalid_token', 'User authorization failed')
+
+    async def enter_captcha(self, url: str, sid: str) -> str:
+        """
+        Override this method for processing captcha.
+
+        :param url: link to captcha image
+        :param sid: captcha id. I do not know why pass here but may be useful
+        :return captcha value
+        """
+        raise VkCaptchaNeeded(url, sid)
+
+    async def close(self):
+        return await self.driver.close()
+
+
+class ImplicitSession(TokenSession):
+    """
+    For client authorization in js apps and standalone (desktop and mobile) apps
+    See more in https://new.vk.com/dev/implicit_flow_user
+    """
+    AUTH_URL = 'https://oauth.vk.com/authorize'
+
+    def __init__(self, login: str, password: str, app_id: int, scope: str or int or list = None,
+                 timeout: int = 10, num_of_attempts: int = 5, driver=None):
+        """
+        :param login: user login
+        :param password: user password
+        :param app_id: application id. More details in `Application registration` block in `https://vk.com/dev/first_guide`
+        :param scope: access rights. See `Access rights` block in `https://vk.com/dev/first_guide`
+        :param timeout: default time out for any request in current session
+        :param num_of_attempts: number of authorization attempts
+        :param driver: TODO add description
+        """
+        super().__init__(access_token=None, timeout=timeout, driver=driver)
+        self.login = login
+        self.password = password
+        self.app_id = app_id
+        self.num_of_attempts = num_of_attempts
+        if isinstance(scope, (str, int, type(None))):
+            self.scope = scope
+        elif isinstance(scope, list):
+            self.scope = ",".join(scope)
+
+    async def authorize(self) -> None:
+        """Getting a new token from server"""
+        url, html = await self._get_auth_page()
+        for step in range(self.num_of_attempts):
+            if url.path == '/authorize':
+                if '__q_hash' in url.query:
+                    # Give rights for app
+                    url, html = await self._process_access_form(html)
+                else:
+                    # Invalid login or password  and 'email' in q.query
+                    url, html = await self._process_auth_form(html)
+            if url.path == '/login' and url.query.get('act', '') == 'authcheck':
+                # Entering 2auth code
+                url, html = await self._process_2auth_form(html)
+            if url.path == '/login' and url.query.get('act', '') == 'authcheck_code':
+                # Need captcha
+                url, html = await self._process_auth_form(html)
+            if url.path == '/authorize' and '__q_hash' in url.query:
+                # Give rights for app
+                url, html = await self._process_access_form(html)
+            if url.path == '/auth_redirect':
+                # Process client-side auth redirect
+                url, html = await self._process_auth_redirect_page(html)
+            if url.path == '/blank.html':
+                # Success
+                parsed_fragments = dict(parse_qsl(url.fragment))
+                self.access_token = parsed_fragments['access_token']
+                return
+        raise VkAuthError('Something went wrong', 'Exceeded the number of attempts to log in')
+
+    async def _get_auth_page(self) -> Tuple[str, str]:
+        """
+        Get authorization mobile page without js
+        :return: redirect_url, html page
+        """
+        # Prepare request
+        params = {
+            'client_id': self.app_id,
+            'redirect_uri': 'https://oauth.vk.com/blank.html',
+            'display': 'mobile',
+            'response_type': 'token',
+            'v': self.API_VERSION
+        }
+        if self.scope:
+            params['scope'] = self.scope
+
+        # Send request
+        status, response, redirect_url = await self.driver.get_text(self.AUTH_URL, params)
+
+        # Process response
+        if status != 200:
+            error_dict = json.loads(response)
+            raise VkAuthError(error_dict['error'], error_dict['error_description'], self.AUTH_URL, params)
+        return redirect_url, response
+
+    async def _process_auth_form(self, html: str) -> (str, str):
+        """
+        Parsing data from authorization page and filling the form and submitting the form
+
+        :param html: html page
+        :return: url and  html from redirected page
+        """
+        # Parse page
+        p = AuthPageParser()
+        p.feed(html)
+        p.close()
+
+        # Get data from hidden inputs
+        form_data = dict(p.inputs)
+        form_url = p.url
+        form_data['email'] = self.login
+        form_data['pass'] = self.password
+        if p.message:
+            # Show form errors
+            raise VkAuthError('invalid_data', p.message, form_url, form_data)
+        elif p.captcha_url:
+            form_data['captcha_key'] = await self.enter_captcha(
+                "https://m.vk.com{}".format(p.captcha_url),
+                form_data['captcha_sid']
+            )
+            form_url = "https://m.vk.com{}".format(form_url)
+
+        # Send request
+        _, html, redirect_url = await self.driver.post_text(
+            form_url, form_data, headers={aiohttp.hdrs.REFERER: 'https://oauth.vk.com/'})
+        return redirect_url, html
+
+    async def _process_2auth_form(self, html: str) -> (str, str):
+        """
+        Parsing two-factor authorization page and filling the code
+
+        :param html: html page
+        :return: url and  html from redirected page
+        """
+        # Parse page
+        p = TwoFactorCodePageParser()
+        p.feed(html)
+        p.close()
+
+        # Prepare request data
+        form_url = p.url
+        form_data = dict(p.inputs)
+        form_data['remember'] = 0
+        if p.message:
+            raise VkAuthError('invalid_data', p.message, form_url, form_data)
+        form_data['code'] = await self.enter_confirmation_code()
+
+        # Send request
+        _, html, redirect_url = await self.driver.post_text(form_url, form_data)
+        return redirect_url, html
+
+    async def _process_access_form(self, html: str) -> (str, str):
+        """
+        Parsing page with access rights
+
+        :param html: html page
+        :return: url and  html from redirected page
+        """
+        # Parse page
+        p = AccessPageParser()
+        p.feed(html)
+        p.close()
+
+        form_url = p.url
+        form_data = dict(p.inputs)
+
+        # Send request
+        _, html, redirect_url = await self.driver.post_text(form_url, form_data)
+        return redirect_url, html
+
+    async def enter_confirmation_code(self) -> str:
+        """
+        Override this method for processing confirmation 2uth code.
+        :return confirmation code
+        """
+        raise VkTwoFactorCodeNeeded()
+
+    async def _process_auth_redirect_page(self, html: str) -> (str, str):
+        """
+        Parse client auth redirect page
+
+        :param html: html page
+        :return: url and  html from redirected page
+        """
+        # Parse page
+        p = AuthRedirectPageParser()
+        p.feed(html)
+        p.close()
+
+        # Send request
+        _, html, redirect_url = await self.driver.get_text(p.location, {})
+        return redirect_url, html
+
+
+class AuthorizationCodeSession(TokenSession):
+    """
+    For client authorization in js apps and standalone (desktop and mobile) apps
+    See more in https://new.vk.com/dev/implicit_flow_user
+    """
+    CODE_URL = 'https://oauth.vk.com/access_token'
+
+    def __init__(self, app_id: int, app_secret: str, redirect_uri: str, code: str, timeout: int = 10, driver=None):
+        """
+        :param app_id: application id. More details in `Application registration` block in `https://vk.com/dev/first_guide`
+        :param app_secret: application secure key. See https://vk.com/editapp?id={app_id}&section=options
+        :param redirect_uri: Authorized redirect URI.
+        :param code: See `https://vk.com/dev/authcode_flow_user`
+        :param timeout:default time out for any request in current session
+        :param driver: TODO add description
+        """
+        super().__init__(access_token=None, timeout=timeout, driver=driver)
+        self.code = code
+        self.app_id = app_id
+        self.app_secret = app_secret
+        self.redirect_uri = redirect_uri
+
+    async def authorize(self, code: str = None) -> None:
+        """Getting a new token from server"""
+        code = await self.get_code(code)
+        params = {
+            'client_id': self.app_id,
+            'client_secret': self.app_secret,
+            'redirect_uri': self.redirect_uri,
+            'code': code
+        }
+        _, response = await self.driver.post_json(self.CODE_URL, params, timeout=self.timeout)
+        if 'error' in response:
+            raise VkAuthError(response['error'], response['error_description'], self.CODE_URL, params)
+        self.access_token = response['access_token']
+
+    async def get_code(self, code: str = None) -> str:
+        """Get temporary code from external sources"""
+        return code or self.code
```

### Comparing `aiovk-4.0.0/aiovk/shaping.py` & `aiovk-4.1.0/aiovk/shaping.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import asyncio
-
-
-class TaskQueue(asyncio.Queue):
-    def __init__(self, max_size, period, *args, **kwargs):
-        super().__init__(max_size, *args, **kwargs)
-        self.period = period
-
-    def _init(self, maxsize):
-        super()._init(maxsize)
-        for i in range(maxsize):
-            self._queue.append(1)
-        self.task = asyncio.ensure_future(self.dispatcher(maxsize))
-
-    async def dispatcher(self, maxsize):
-        while True:
-            await asyncio.sleep(self.period)
-            for i in range(maxsize - self.qsize()):
-                self.put_nowait(1)
-
-    def cancel(self):
-        self.task.cancel()
-
-
-def wait_free_slot(func):
-    async def wrapper(self, *args, **kwargs):
-        await self._queue.get()
-        return await func(self, *args, **kwargs)
-    return wrapper
+import asyncio
+
+
+class TaskQueue(asyncio.Queue):
+    def __init__(self, max_size, period, *args, **kwargs):
+        super().__init__(max_size, *args, **kwargs)
+        self.period = period
+
+    def _init(self, maxsize):
+        super()._init(maxsize)
+        for i in range(maxsize):
+            self._queue.append(1)
+        self.task = asyncio.ensure_future(self.dispatcher(maxsize))
+
+    async def dispatcher(self, maxsize):
+        while True:
+            await asyncio.sleep(self.period)
+            for i in range(maxsize - self.qsize()):
+                self.put_nowait(1)
+
+    def cancel(self):
+        self.task.cancel()
+
+
+def wait_free_slot(func):
+    async def wrapper(self, *args, **kwargs):
+        await self._queue.get()
+        return await func(self, *args, **kwargs)
+    return wrapper
```

### Comparing `aiovk-4.0.0/aiovk.egg-info/PKG-INFO` & `aiovk-4.1.0/aiovk.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,325 +1,326 @@
-Metadata-Version: 1.2
-Name: aiovk
-Version: 4.0.0
-Summary: vk.com API python wrapper for asyncio
-Home-page: https://github.com/Fahreeve/aiovk
-Author: Fahreev Eldar
-Author-email: fahreeve@yandex.ru
-License: MIT License
-Description: vk.com API python wrapper for asyncio
-        =====================================
-        for old version of python you can use https://github.com/dimka665/vk
-        
-        Features
-        --------
-        * asynchronous
-        * support python 3.5+ versions
-        * have only one dependency - ``aiohttp 3+``
-        * support two-factor authentication
-        * support socks proxy with ``aiohttp-socks``
-        * support rate limit of requests
-        * support Long Poll connection
-        
-        TODO
-        ----
-        * need refactoring tests for ``AsyncVkExecuteRequestPool``
-        
-        Install
-        -------
-        
-        .. code-block:: bash
-        
-            pip install aiovk
-        
-        Examples
-        ========
-        Annotation
-        ----------
-        In all the examples below, I will give only the ``{code}``
-        
-        .. code-block:: python
-        
-            async def func():
-                {code}
-        
-            loop = asyncio.get_event_loop()
-            loop.run_until_complete(func())
-        
-        
-        Authorization
-        -------------
-        **TokenSession** - if you already have token or you use requests which don't require token
-        
-        .. code-block:: python
-        
-            session = TokenSession()
-            session = TokenSession(access_token='asdf123..')
-        
-        **ImplicitSession** - client authorization in js apps and standalone (desktop and mobile) apps
-        
-        .. code-block:: python
-        
-            >>> session = ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID)
-            >>> await session.authorize()
-            >>> session.access_token
-            asdfa2321afsdf12eadasf123...
-        
-        With scopes:
-        
-        .. code-block:: python
-        
-            ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify')
-            ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify,friends')
-            ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, ['notify', 'friends'])
-            ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 3)  # notify and friends
-        
-        Also you can use ``SimpleImplicitSessionMixin`` for entering confirmation code
-        or captcha key
-        
-        **AuthorizationCodeSession** - authorization for server apps or Open API
-        
-        See https://vk.com/dev/authcode_flow_user for getting the CODE
-        
-        .. code-block:: python
-        
-            >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI, CODE)
-            >>> await session.authorize()
-            >>> session.access_token
-            asdfa2321afsdf12eadasf123...
-        
-        Or:
-        
-        .. code-block:: python
-        
-            >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI)
-            >>> await session.authorize(CODE)
-            >>> session.access_token
-            asdfa2321afsdf12eadasf123...
-        
-        **Authorization using context manager** - you won't need to use session.close() after work
-        
-        .. code-block:: python
-        
-            async with aiovk.TokenSession(access_token=YOUR_VK_TOKEN) as ses:
-                api = API(ses)...
-        
-        And your session will be closed after all done or code fail(similar to simple "with" usage)
-        Works with all types of authorization
-        
-        Drivers
-        -------
-        **HttpDriver** - default driver for using ``aiohttp``
-        
-        .. code-block:: python
-        
-            >>> driver = HttpDriver()
-            >>> driver = HttpDriver(timeout=10)  # default timeout for all requests
-        
-        .. code-block:: python
-        
-            >>> driver = ProxyDriver(PROXY_ADDRESS, PORT)  # 1234 is port
-            >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, timeout=10)
-            >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, PROXY_LOGIN, PROXY_PASSWORD, timeout=10)
-        
-        How to use custom driver with session:
-        
-        .. code-block:: python
-        
-            >>> session = TokenSession(..., driver=HttpDriver())
-        
-        How to use driver with own loop:
-        
-        .. code-block:: python
-        
-            >>> loop = asyncio.get_event_loop()
-            >>> asyncio.set_event_loop(None)
-            >>> session = TokenSession(driver=HttpDriver(loop=loop))  # or ProxyDriver
-        
-        How to use driver with custom http session object:
-        
-        Solve next problem: https://stackoverflow.com/questions/29827642/asynchronous-aiohttp-requests-fails-but-synchronous-requests-succeed
-        
-        .. code-block:: python
-        
-            >>> connector = aiohttp.TCPConnector(verify_ssl=False)
-            >>> session = aiohttp.ClientSession(connector=connector)
-            >>> driver = HttpDriver(loop=loop, session=session)
-        
-        
-        **LimitRateDriverMixin** - mixin class what allow you create new drivers with speed rate limits
-        
-        .. code-block:: python
-        
-            >>> class ExampleDriver(LimitRateDriverMixin, HttpDriver):
-            ...     requests_per_period = 3
-            ...     period = 1  #seconds
-        
-        VK API
-        ------
-        First variant:
-        
-        .. code-block:: python
-        
-            >>> session = TokenSession()
-            >>> api = API(session)
-            >>> await api.users.get(user_ids=1)
-            [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
-        
-        Second variant:
-        
-        .. code-block:: python
-        
-            >>> session = TokenSession()
-            >>> api = API(session)
-            >>> await api('users.get', user_ids=1)
-            [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
-        
-        Also you can add ``timeout`` argument for each request or define it in the session
-        
-        See https://vk.com/dev/methods for detailed API guide.
-        
-        Lazy VK API
-        -----------
-        It is useful when a bot has a large message flow
-        
-        .. code-block:: python
-        
-            >>> session = TokenSession()
-            >>> api = LazyAPI(session)
-            >>> message = api.users.get(user_ids=1)
-            >>> await message()
-            [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
-        
-        Supports both variants like API object
-        
-        User Long Poll
-        --------------
-        For documentation, see: https://vk.com/dev/using_longpoll
-        
-        Use exist API object
-        
-        .. code-block:: python
-        
-            >>> api = API(session)
-            >>> lp = UserLongPoll(api, mode=2)  # default wait=25
-            >>> await lp.wait()
-            {"ts":1820350345,"updates":[...]}
-            >>> await lp.wait()
-            {"ts":1820351011,"updates":[...]}
-        
-        Use Session object
-        
-        .. code-block:: python
-        
-            >>> lp = UserLongPoll(session, mode=2)  # default wait=25
-            >>> await lp.wait()
-            {"ts":1820350345,"updates":[...]}
-            >>> await lp.get_pts()  # return pts
-            191231223
-            >>> await lp.get_pts(need_ts=True)  # return pts, ts
-            191231223, 1820350345
-        
-        You can iterate over events
-        
-        .. code-block:: python
-        
-            >>> async for event in lp.iter():
-            ...     print(event)
-            {"type":..., "object": {...}}
-        
-        Notice that ``wait`` value only for long pool connection.
-        
-        Real pause could be more ``wait`` time because of need time
-        for authorization (if needed), reconnect and etc.
-        
-        Bots Long Poll
-        --------------
-        For documentation, see: https://vk.com/dev/bots_longpoll
-        
-        Use exist API object
-        
-        .. code-block:: python
-        
-            >>> api = API(session)
-            >>> lp = BotsLongPoll(api, group_id=1)  # default wait=25
-            >>> await lp.wait()
-            {"ts":345,"updates":[...]}
-            >>> await lp.wait()
-            {"ts":346,"updates":[...]}
-        
-        Use Session object
-        
-        .. code-block:: python
-        
-            >>> lp = BotsLongPoll(session, group_id=1)  # default wait=25
-            >>> await lp.wait()
-            {"ts":78455,"updates":[...]}
-            >>> await lp.get_pts()  # return pts
-            191231223
-            >>> await lp.get_pts(need_ts=True)  # return pts, ts
-            191231223, 1820350345
-        
-        BotsLongPoll supports iterating too
-        
-        .. code-block:: python
-        
-            >>> async for event in lp.iter():
-            ...     print(event)
-            {"type":..., "object": {...}}
-        
-        Notice that ``wait`` value only for long pool connection.
-        
-        Real pause could be more ``wait`` time because of need time
-        for authorization (if needed), reconnect and etc.
-        
-        Async execute request pool
-        --------------------------
-        For documentation, see: https://vk.com/dev/execute
-        
-        .. code-block:: python
-        
-            from aiovk.pools import AsyncVkExecuteRequestPool
-        
-            async with AsyncVkExecuteRequestPool() as pool:
-                response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
-                response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
-                response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
-                response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
-        
-            >>> print(response.ok)
-            True
-            >>> print(response.result)
-            [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
-            >>> print(response2.result)
-            [{'id': 2, 'first_name': 'Александра', 'last_name': 'Владимирова'}]
-            >>> print(response3.result)
-            [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
-            >>> print(response4.ok)
-            False
-            >>> print(response4.error)
-            {'method': 'users.get', 'error_code': 113, 'error_msg': 'Invalid user id'}
-        
-        or
-        
-        .. code-block:: python
-        
-            from aiovk.pools import AsyncVkExecuteRequestPool
-        
-            pool = AsyncVkExecuteRequestPool()
-            response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
-            response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
-            response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
-            response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
-            await pool.execute()
-            ...
-        
-Keywords: vk.com api vk wrappper asyncio
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Metadata-Version: 2.1
+Name: aiovk
+Version: 4.1.0
+Summary: vk.com API python wrapper for asyncio
+Home-page: https://github.com/alexanderlarin/aiovk
+Author: Alexander Larin
+Author-email: ekzebox@gmail.com
+License: MIT License
+Keywords: vk.com api vk wrappper asyncio
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+License-File: LICENSE
+
+vk.com API python wrapper for asyncio
+=====================================
+for old version of python you can use https://github.com/dimka665/vk
+
+Features
+--------
+* asynchronous
+* support python 3.5+ versions
+* have only one dependency - ``aiohttp 3+``
+* support two-factor authentication
+* support socks proxy with ``aiohttp-socks``
+* support rate limit of requests
+* support Long Poll connection
+
+TODO
+----
+* need refactoring tests for ``AsyncVkExecuteRequestPool``
+
+Install
+-------
+
+.. code-block:: bash
+
+    pip install aiovk
+
+Examples
+========
+Annotation
+----------
+In all the examples below, I will give only the ``{code}``
+
+.. code-block:: python
+
+    async def func():
+        {code}
+
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(func())
+
+
+Authorization
+-------------
+**TokenSession** - if you already have token or you use requests which don't require token
+
+.. code-block:: python
+
+    session = TokenSession()
+    session = TokenSession(access_token='asdf123..')
+
+**ImplicitSession** - client authorization in js apps and standalone (desktop and mobile) apps
+
+.. code-block:: python
+
+    >>> session = ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID)
+    >>> await session.authorize()
+    >>> session.access_token
+    asdfa2321afsdf12eadasf123...
+
+With scopes:
+
+.. code-block:: python
+
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify')
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 'notify,friends')
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, ['notify', 'friends'])
+    ImplicitSession(USER_LOGIN, USER_PASSWORD, APP_ID, 3)  # notify and friends
+
+Also you can use ``SimpleImplicitSessionMixin`` for entering confirmation code
+or captcha key
+
+**AuthorizationCodeSession** - authorization for server apps or Open API
+
+See https://vk.com/dev/authcode_flow_user for getting the CODE
+
+.. code-block:: python
+
+    >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI, CODE)
+    >>> await session.authorize()
+    >>> session.access_token
+    asdfa2321afsdf12eadasf123...
+
+Or:
+
+.. code-block:: python
+
+    >>> session = AuthorizationCodeSession(APP_ID, APP_SECRET, REDIRECT_URI)
+    >>> await session.authorize(CODE)
+    >>> session.access_token
+    asdfa2321afsdf12eadasf123...
+
+**Authorization using context manager** - you won't need to use session.close() after work
+
+.. code-block:: python
+
+    async with aiovk.TokenSession(access_token=YOUR_VK_TOKEN) as ses:
+        api = API(ses)...
+
+And your session will be closed after all done or code fail(similar to simple "with" usage)
+Works with all types of authorization
+
+Drivers
+-------
+**HttpDriver** - default driver for using ``aiohttp``
+
+.. code-block:: python
+
+    >>> driver = HttpDriver()
+    >>> driver = HttpDriver(timeout=10)  # default timeout for all requests
+
+.. code-block:: python
+
+    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT)  # 1234 is port
+    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, timeout=10)
+    >>> driver = ProxyDriver(PROXY_ADDRESS, PORT, PROXY_LOGIN, PROXY_PASSWORD, timeout=10)
+
+How to use custom driver with session:
+
+.. code-block:: python
+
+    >>> session = TokenSession(..., driver=HttpDriver())
+
+How to use driver with own loop:
+
+.. code-block:: python
+
+    >>> loop = asyncio.get_event_loop()
+    >>> asyncio.set_event_loop(None)
+    >>> session = TokenSession(driver=HttpDriver(loop=loop))  # or ProxyDriver
+
+How to use driver with custom http session object:
+
+Solve next problem: https://stackoverflow.com/questions/29827642/asynchronous-aiohttp-requests-fails-but-synchronous-requests-succeed
+
+.. code-block:: python
+
+    >>> connector = aiohttp.TCPConnector(verify_ssl=False)
+    >>> session = aiohttp.ClientSession(connector=connector)
+    >>> driver = HttpDriver(loop=loop, session=session)
+
+
+**LimitRateDriverMixin** - mixin class what allow you create new drivers with speed rate limits
+
+.. code-block:: python
+
+    >>> class ExampleDriver(LimitRateDriverMixin, HttpDriver):
+    ...     requests_per_period = 3
+    ...     period = 1  #seconds
+
+VK API
+------
+First variant:
+
+.. code-block:: python
+
+    >>> session = TokenSession()
+    >>> api = API(session)
+    >>> await api.users.get(user_ids=1)
+    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
+
+Second variant:
+
+.. code-block:: python
+
+    >>> session = TokenSession()
+    >>> api = API(session)
+    >>> await api('users.get', user_ids=1)
+    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
+
+Also you can add ``timeout`` argument for each request or define it in the session
+
+See https://vk.com/dev/methods for detailed API guide.
+
+Lazy VK API
+-----------
+It is useful when a bot has a large message flow
+
+.. code-block:: python
+
+    >>> session = TokenSession()
+    >>> api = LazyAPI(session)
+    >>> message = api.users.get(user_ids=1)
+    >>> await message()
+    [{'first_name': 'Pavel', 'last_name': 'Durov', 'id': 1}]
+
+Supports both variants like API object
+
+User Long Poll
+--------------
+For documentation, see: https://vk.com/dev/using_longpoll
+
+Use exist API object
+
+.. code-block:: python
+
+    >>> api = API(session)
+    >>> lp = UserLongPoll(api, mode=2)  # default wait=25
+    >>> await lp.wait()
+    {"ts":1820350345,"updates":[...]}
+    >>> await lp.wait()
+    {"ts":1820351011,"updates":[...]}
+
+Use Session object
+
+.. code-block:: python
+
+    >>> lp = UserLongPoll(session, mode=2)  # default wait=25
+    >>> await lp.wait()
+    {"ts":1820350345,"updates":[...]}
+    >>> await lp.get_pts()  # return pts
+    191231223
+    >>> await lp.get_pts(need_ts=True)  # return pts, ts
+    191231223, 1820350345
+
+You can iterate over events
+
+.. code-block:: python
+
+    >>> async for event in lp.iter():
+    ...     print(event)
+    {"type":..., "object": {...}}
+
+Notice that ``wait`` value only for long pool connection.
+
+Real pause could be more ``wait`` time because of need time
+for authorization (if needed), reconnect and etc.
+
+Bots Long Poll
+--------------
+For documentation, see: https://vk.com/dev/bots_longpoll
+
+Use exist API object
+
+.. code-block:: python
+
+    >>> api = API(session)
+    >>> lp = BotsLongPoll(api, group_id=1)  # default wait=25
+    >>> await lp.wait()
+    {"ts":345,"updates":[...]}
+    >>> await lp.wait()
+    {"ts":346,"updates":[...]}
+
+Use Session object
+
+.. code-block:: python
+
+    >>> lp = BotsLongPoll(session, group_id=1)  # default wait=25
+    >>> await lp.wait()
+    {"ts":78455,"updates":[...]}
+    >>> await lp.get_pts()  # return pts
+    191231223
+    >>> await lp.get_pts(need_ts=True)  # return pts, ts
+    191231223, 1820350345
+
+BotsLongPoll supports iterating too
+
+.. code-block:: python
+
+    >>> async for event in lp.iter():
+    ...     print(event)
+    {"type":..., "object": {...}}
+
+Notice that ``wait`` value only for long pool connection.
+
+Real pause could be more ``wait`` time because of need time
+for authorization (if needed), reconnect and etc.
+
+Async execute request pool
+--------------------------
+For documentation, see: https://vk.com/dev/execute
+
+.. code-block:: python
+
+    from aiovk.pools import AsyncVkExecuteRequestPool
+
+    async with AsyncVkExecuteRequestPool() as pool:
+        response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
+        response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
+        response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
+        response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
+
+    >>> print(response.ok)
+    True
+    >>> print(response.result)
+    [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
+    >>> print(response2.result)
+    [{'id': 2, 'first_name': 'Александра', 'last_name': 'Владимирова'}]
+    >>> print(response3.result)
+    [{'id': 1, 'first_name': 'Павел', 'last_name': 'Дуров'}]
+    >>> print(response4.ok)
+    False
+    >>> print(response4.error)
+    {'method': 'users.get', 'error_code': 113, 'error_msg': 'Invalid user id'}
+
+or
+
+.. code-block:: python
+
+    from aiovk.pools import AsyncVkExecuteRequestPool
+
+    pool = AsyncVkExecuteRequestPool()
+    response = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 1})
+    response2 = pool.add_call('users.get', 'YOUR_TOKEN', {'user_ids': 2})
+    response3 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': 1})
+    response4 = pool.add_call('users.get', 'ANOTHER_TOKEN', {'user_ids': -1})
+    await pool.execute()
+    ...
```

### Comparing `aiovk-4.0.0/tests/unit/test_api.py` & `aiovk-4.1.0/tests/unit/test_api.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import pytest
-
-from aiovk import API
-from aiovk.api import Request, LazyRequest, LazyAPI
-from aiovk.sessions import BaseSession
-
-pytestmark = pytest.mark.asyncio
-
-
-class TestSession(BaseSession):
-    async def __aenter__(self):
-        pass
-
-    async def send_api_request(self, method_name, params=None, timeout=None, raw_response=None):
-        out = {
-            'method_name': method_name,
-            'params': params,
-            'timeout': timeout,
-        }
-        return out
-
-
-@pytest.mark.parametrize(
-    'request_method', [
-        'test',
-        'test.test',
-])
-@pytest.mark.parametrize(
-    'request_params, timeout', [
-        ({}, None),
-        ({'arg': 1}, None),
-        ({'timeout': 1}, 1),
-        ({'arg': 1, 'timeout': 1}, 1),
-])
-@pytest.mark.parametrize(
-    'request_class, is_lazy', [
-        (Request, False),
-        (LazyRequest, True),
-])
-@pytest.mark.parametrize(
-    'api', [
-        API(TestSession()),
-        LazyAPI(TestSession()),
-    ]
-)
-async def test_request(api, request_class, request_method, request_params, timeout, is_lazy):
-    request = request_class(api, request_method)
-    if is_lazy:
-        lazy_obj = request(**request_params)
-        response = await lazy_obj()
-    else:
-        response = await request(**request_params)
-
-    params = request_params.copy()
-    params.pop('timeout', None)
-    expected = {
-        'params': params,
-        'timeout': timeout,
-        'method_name': request_method
-    }
-    assert response == expected
-
-
-@pytest.mark.parametrize(
-    'request_params, timeout', [
-        ({}, None),
-        ({'arg': 1}, None),
-        ({'timeout': 1}, 1),
-        ({'arg': 1, 'timeout': 1}, 1),
-])
-@pytest.mark.parametrize(
-    'method, method_name', [
-        (lambda x, **kwargs: x.test(**kwargs), 'test'),
-        (lambda x, **kwargs: x.test1.test2(**kwargs), 'test1.test2'),
-        (lambda x, **kwargs: x('test', **kwargs), 'test'),
-        (lambda x, **kwargs: x('test1.test2', **kwargs), 'test1.test2'),
-    ]
-)
-@pytest.mark.parametrize(
-    'api, is_lazy', [
-        (LazyAPI(TestSession()), True),
-        (API(TestSession()), False),
-    ]
-)
-async def test_api(api, method, request_params, timeout, method_name, is_lazy):
-    if is_lazy:
-        lazy_obj = method(api, **request_params)
-        response = await lazy_obj()
-    else:
-        response = await method(api, **request_params)
-
-    params = request_params.copy()
-    params.pop('timeout', None)
-    expected = {
-        'params': params,
-        'timeout': timeout,
-        'method_name': method_name
-    }
-    assert response == expected
+import pytest
+
+from aiovk import API
+from aiovk.api import Request, LazyRequest, LazyAPI
+from aiovk.sessions import BaseSession
+
+pytestmark = pytest.mark.asyncio
+
+
+class TestSession(BaseSession):
+    async def __aenter__(self):
+        pass
+
+    async def send_api_request(self, method_name, params=None, timeout=None, raw_response=None):
+        out = {
+            'method_name': method_name,
+            'params': params,
+            'timeout': timeout,
+        }
+        return out
+
+
+@pytest.mark.parametrize(
+    'request_method', [
+        'test',
+        'test.test',
+])
+@pytest.mark.parametrize(
+    'request_params, timeout', [
+        ({}, None),
+        ({'arg': 1}, None),
+        ({'timeout': 1}, 1),
+        ({'arg': 1, 'timeout': 1}, 1),
+])
+@pytest.mark.parametrize(
+    'request_class, is_lazy', [
+        (Request, False),
+        (LazyRequest, True),
+])
+@pytest.mark.parametrize(
+    'api', [
+        API(TestSession()),
+        LazyAPI(TestSession()),
+    ]
+)
+async def test_request(api, request_class, request_method, request_params, timeout, is_lazy):
+    request = request_class(api, request_method)
+    if is_lazy:
+        lazy_obj = request(**request_params)
+        response = await lazy_obj()
+    else:
+        response = await request(**request_params)
+
+    params = request_params.copy()
+    params.pop('timeout', None)
+    expected = {
+        'params': params,
+        'timeout': timeout,
+        'method_name': request_method
+    }
+    assert response == expected
+
+
+@pytest.mark.parametrize(
+    'request_params, timeout', [
+        ({}, None),
+        ({'arg': 1}, None),
+        ({'timeout': 1}, 1),
+        ({'arg': 1, 'timeout': 1}, 1),
+])
+@pytest.mark.parametrize(
+    'method, method_name', [
+        (lambda x, **kwargs: x.test(**kwargs), 'test'),
+        (lambda x, **kwargs: x.test1.test2(**kwargs), 'test1.test2'),
+        (lambda x, **kwargs: x('test', **kwargs), 'test'),
+        (lambda x, **kwargs: x('test1.test2', **kwargs), 'test1.test2'),
+    ]
+)
+@pytest.mark.parametrize(
+    'api, is_lazy', [
+        (LazyAPI(TestSession()), True),
+        (API(TestSession()), False),
+    ]
+)
+async def test_api(api, method, request_params, timeout, method_name, is_lazy):
+    if is_lazy:
+        lazy_obj = method(api, **request_params)
+        response = await lazy_obj()
+    else:
+        response = await method(api, **request_params)
+
+    params = request_params.copy()
+    params.pop('timeout', None)
+    expected = {
+        'params': params,
+        'timeout': timeout,
+        'method_name': method_name
+    }
+    assert response == expected
```

### Comparing `aiovk-4.0.0/tests/unit/test_longpool.py` & `aiovk-4.1.0/tests/unit/test_longpool.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-import json
-
-import pytest
-
-from aiovk import LongPoll, API
-from aiovk.drivers import BaseDriver
-from aiovk.exceptions import VkLongPollError
-from aiovk.longpoll import BotsLongPoll
-from aiovk.sessions import BaseSession
-
-pytestmark = pytest.mark.asyncio
-
-
-class Driver(BaseDriver):
-    counter = 0
-    message = None
-    original_event = {"type": "group_join", "object": {"user_id": 1, "join_type": "approved"}, "group_id": 1}
-    expected_version = None
-    expected_ts = None
-    expected_mode = None
-
-    async def get_text(self, url, params, timeout=None):
-        message = json.dumps(self.messages[self.counter])
-        self.counter += 1
-        if self.expected_mode is not None:
-            assert params['mode'] == self.expected_mode
-
-        if self.expected_version is not None:
-            assert params['version'] == self.expected_version
-
-        if self.expected_ts is not None:
-            assert params['ts'] == self.expected_ts
-
-        return 200, message, url
-
-
-class Session(BaseSession):
-    async def __aenter__(self):
-        pass
-
-    timeout = 10
-    TS = 1
-    PTS = 2
-    KEY = 'key'
-    SERVER = 'superhost'
-
-    def __init__(self):
-        self.driver = Driver()
-
-    async def send_api_request(self, *args, **kwargs) -> dict:
-        return {"key": self.KEY, "server": self.SERVER, "ts": self.TS, "pts": self.PTS}
-
-
-@pytest.mark.parametrize(
-    'session',
-    [
-        Session(),
-        API(Session())
-    ]
-)
-async def test_longpoll_get_pts(session):
-    lp = LongPoll(session, mode=0)
-    pts = await lp.get_pts()
-    assert pts == Session.PTS
-
-
-@pytest.mark.parametrize(
-    'session',
-    [
-        Session(),
-        API(Session())
-    ]
-)
-async def test_longpoll_get_cached_pts(session):
-    lp = LongPoll(session, mode=0)
-    await lp.get_pts()
-    pts = await lp.get_pts()
-    assert pts == Session.PTS
-
-
-@pytest.mark.parametrize(
-    'session',
-    [
-        Session(),
-        API(Session())
-    ]
-)
-async def test_longpoll_get_pts_need_ts(session):
-    lp = LongPoll(session, mode=0)
-    result = await lp.get_pts(need_ts=True)
-    assert len(result) == 2
-    assert result[0] == Session.PTS
-    assert result[1] == Session.TS
-
-
-@pytest.mark.parametrize(
-    'messages, exception, ts',
-    [
-        ([{'ts': 23}], None, 23),
-        ([{'failed': 1, 'ts': 42}, {'ts': 45, 'updates': [Driver.original_event]}], None, 45),
-        ([{'failed': 2}, {'ts': 63, 'updates': [Driver.original_event]}], None, 63),
-        ([{'failed': 3}, {'ts': 56, 'updates': [Driver.original_event]}], None, 56),
-        ([{'failed': 4}, {'ts': 11, 'updates': [Driver.original_event]}], VkLongPollError, None),
-    ]
-)
-@pytest.mark.parametrize(
-    'longpoll',
-    [
-        lambda session: LongPoll(session, mode=0),
-        lambda session: LongPoll(session, mode=1),
-        lambda session: LongPoll(session, mode=1, version=1),
-        lambda session: BotsLongPoll(session, group_id=1),
-        lambda session: BotsLongPoll(session, group_id=1, version=3),
-    ]
-)
-async def test_longpoll_wait(longpoll, messages, exception, ts):
-    session = Session()
-    session.driver.messages = messages
-    session = API(session)
-    lp = longpoll(session)
-    session._session.driver.expected_mode = lp.base_params.get('mode')
-    session._session.driver.expected_version = lp.base_params.get('version')
-
-
-    if exception is None:
-        response = await lp.wait()
-        assert response == messages[-1]
-        _, real_ts = await lp.get_pts(need_ts=True)
-        assert real_ts == ts
-    else:
-        with pytest.raises(exception):
-            await lp.wait()
-
-
-@pytest.mark.parametrize(
-    'messages, exception, ts',
-    [
-        ([{'failed': 1, 'ts': 42}, {'ts': 45, 'updates': [Driver.original_event]}], None, 45),
-        ([{'failed': 2}, {'ts': 63, 'updates': [Driver.original_event]}], None, 63),
-        ([{'failed': 3}, {'ts': 56, 'updates': [Driver.original_event]}], None, 56),
-        ([{'failed': 4}, {'ts': 11, 'updates': [Driver.original_event]}], VkLongPollError, None),
-        ([{'failed': 3}, {'ts': 56, 'updates': [Driver.original_event]},
-                         {'ts': 58, 'updates': [Driver.original_event]}], None, 58),
-    ]
-)
-@pytest.mark.parametrize(
-    'longpoll',
-    [
-        lambda session: LongPoll(session, mode=0),
-        lambda session: LongPoll(session, mode=1),
-        lambda session: LongPoll(session, mode=1, version=1),
-        lambda session: BotsLongPoll(session, group_id=1),
-        lambda session: BotsLongPoll(session, group_id=1, version=3),
-    ]
-)
-async def test_longpoll_iter(longpoll, messages, exception, ts):
-    session = Session()
-    session.driver.messages = messages
-    session = API(session)
-    lp = longpoll(session)
-    session._session.driver.expected_mode = lp.base_params.get('mode')
-    session._session.driver.expected_version = lp.base_params.get('version')
-
-    if exception is None:
-        num_of_iterations = len([m for m in messages if 'updates' in m])
-        i = 0
-        async for event in lp.iter():
-            assert event == messages[-1]['updates'][0]
-            i += 1
-            if i >= num_of_iterations:
-                break
-        _, real_ts = await lp.get_pts(need_ts=True)
-        assert real_ts == ts
-    else:
-        with pytest.raises(exception):
-            async for _ in lp.iter():
-                pass
+import json
+
+import pytest
+
+from aiovk import LongPoll, API
+from aiovk.drivers import BaseDriver
+from aiovk.exceptions import VkLongPollError
+from aiovk.longpoll import BotsLongPoll
+from aiovk.sessions import BaseSession
+
+pytestmark = pytest.mark.asyncio
+
+
+class Driver(BaseDriver):
+    counter = 0
+    message = None
+    original_event = {"type": "group_join", "object": {"user_id": 1, "join_type": "approved"}, "group_id": 1}
+    expected_version = None
+    expected_ts = None
+    expected_mode = None
+
+    async def get_text(self, url, params, timeout=None):
+        message = json.dumps(self.messages[self.counter])
+        self.counter += 1
+        if self.expected_mode is not None:
+            assert params['mode'] == self.expected_mode
+
+        if self.expected_version is not None:
+            assert params['version'] == self.expected_version
+
+        if self.expected_ts is not None:
+            assert params['ts'] == self.expected_ts
+
+        return 200, message, url
+
+
+class Session(BaseSession):
+    async def __aenter__(self):
+        pass
+
+    timeout = 10
+    TS = 1
+    PTS = 2
+    KEY = 'key'
+    SERVER = 'superhost'
+
+    def __init__(self):
+        self.driver = Driver()
+
+    async def send_api_request(self, *args, **kwargs) -> dict:
+        return {"key": self.KEY, "server": self.SERVER, "ts": self.TS, "pts": self.PTS}
+
+
+@pytest.mark.parametrize(
+    'session',
+    [
+        Session(),
+        API(Session())
+    ]
+)
+async def test_longpoll_get_pts(session):
+    lp = LongPoll(session, mode=0)
+    pts = await lp.get_pts()
+    assert pts == Session.PTS
+
+
+@pytest.mark.parametrize(
+    'session',
+    [
+        Session(),
+        API(Session())
+    ]
+)
+async def test_longpoll_get_cached_pts(session):
+    lp = LongPoll(session, mode=0)
+    await lp.get_pts()
+    pts = await lp.get_pts()
+    assert pts == Session.PTS
+
+
+@pytest.mark.parametrize(
+    'session',
+    [
+        Session(),
+        API(Session())
+    ]
+)
+async def test_longpoll_get_pts_need_ts(session):
+    lp = LongPoll(session, mode=0)
+    result = await lp.get_pts(need_ts=True)
+    assert len(result) == 2
+    assert result[0] == Session.PTS
+    assert result[1] == Session.TS
+
+
+@pytest.mark.parametrize(
+    'messages, exception, ts',
+    [
+        ([{'ts': 23}], None, 23),
+        ([{'failed': 1, 'ts': 42}, {'ts': 45, 'updates': [Driver.original_event]}], None, 45),
+        ([{'failed': 2}, {'ts': 63, 'updates': [Driver.original_event]}], None, 63),
+        ([{'failed': 3}, {'ts': 56, 'updates': [Driver.original_event]}], None, 56),
+        ([{'failed': 4}, {'ts': 11, 'updates': [Driver.original_event]}], VkLongPollError, None),
+    ]
+)
+@pytest.mark.parametrize(
+    'longpoll',
+    [
+        lambda session: LongPoll(session, mode=0),
+        lambda session: LongPoll(session, mode=1),
+        lambda session: LongPoll(session, mode=1, version=1),
+        lambda session: BotsLongPoll(session, group_id=1),
+        lambda session: BotsLongPoll(session, group_id=1, version=3),
+    ]
+)
+async def test_longpoll_wait(longpoll, messages, exception, ts):
+    session = Session()
+    session.driver.messages = messages
+    session = API(session)
+    lp = longpoll(session)
+    session._session.driver.expected_mode = lp.base_params.get('mode')
+    session._session.driver.expected_version = lp.base_params.get('version')
+
+
+    if exception is None:
+        response = await lp.wait()
+        assert response == messages[-1]
+        _, real_ts = await lp.get_pts(need_ts=True)
+        assert real_ts == ts
+    else:
+        with pytest.raises(exception):
+            await lp.wait()
+
+
+@pytest.mark.parametrize(
+    'messages, exception, ts',
+    [
+        ([{'failed': 1, 'ts': 42}, {'ts': 45, 'updates': [Driver.original_event]}], None, 45),
+        ([{'failed': 2}, {'ts': 63, 'updates': [Driver.original_event]}], None, 63),
+        ([{'failed': 3}, {'ts': 56, 'updates': [Driver.original_event]}], None, 56),
+        ([{'failed': 4}, {'ts': 11, 'updates': [Driver.original_event]}], VkLongPollError, None),
+        ([{'failed': 3}, {'ts': 56, 'updates': [Driver.original_event]},
+                         {'ts': 58, 'updates': [Driver.original_event]}], None, 58),
+    ]
+)
+@pytest.mark.parametrize(
+    'longpoll',
+    [
+        lambda session: LongPoll(session, mode=0),
+        lambda session: LongPoll(session, mode=1),
+        lambda session: LongPoll(session, mode=1, version=1),
+        lambda session: BotsLongPoll(session, group_id=1),
+        lambda session: BotsLongPoll(session, group_id=1, version=3),
+    ]
+)
+async def test_longpoll_iter(longpoll, messages, exception, ts):
+    session = Session()
+    session.driver.messages = messages
+    session = API(session)
+    lp = longpoll(session)
+    session._session.driver.expected_mode = lp.base_params.get('mode')
+    session._session.driver.expected_version = lp.base_params.get('version')
+
+    if exception is None:
+        num_of_iterations = len([m for m in messages if 'updates' in m])
+        i = 0
+        async for event in lp.iter():
+            assert event == messages[-1]['updates'][0]
+            i += 1
+            if i >= num_of_iterations:
+                break
+        _, real_ts = await lp.get_pts(need_ts=True)
+        assert real_ts == ts
+    else:
+        with pytest.raises(exception):
+            async for _ in lp.iter():
+                pass
```

### Comparing `aiovk-4.0.0/tests/unit/test_pools.py` & `aiovk-4.1.0/tests/unit/test_pools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,194 +1,196 @@
-import os
-from unittest import IsolatedAsyncioTestCase
-
-# from dotenv import load_dotenv
-
-from aiovk.pools import AsyncResult, AsyncVkExecuteRequestPool
-
-# load_dotenv(
-#     os.path.join(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))), ".env")
-# )
-token1 = os.getenv('TEST_TOKEN_1')
-token2 = os.getenv('TEST_TOKEN_2')
-
-
-# TODO need refactoring
-class ExecutePoolTestCase(IsolatedAsyncioTestCase):
-    async def test_one_call_per_request(self):
-        async with AsyncVkExecuteRequestPool() as pool:
-            result = pool.add_call('users.get', token1, {'user_ids': 1})
-            self.assertIsInstance(result, AsyncResult)
-        self.assertIsNotNone(result.result)
-        self.assertEqual(1, result.result[0]['id'])
-
-        async with AsyncVkExecuteRequestPool() as pool:
-            result = pool.add_call('users.get', token1, {'user_ids': 1})
-            self.assertIsInstance(result, AsyncResult)
-            result2 = pool.add_call('users.get', token2, {'user_ids': 2})
-            self.assertIsInstance(result2, AsyncResult)
-
-        self.assertTrue(result.ok)
-        self.assertIsNotNone(result.result)
-        self.assertEqual(1, result.result[0]['id'])
-        self.assertTrue(result2.ok)
-        self.assertIsNotNone(result2.result)
-        self.assertEqual(2, result2.result[0]['id'])
-
-    async def test_less_or_equal_than_25_calls_per_token(self):
-        users = []
-        async with AsyncVkExecuteRequestPool() as pool:
-            for i in range(1, 2):
-                result = pool.add_call('users.get', token1, {'user_ids': i})
-                users.append(result)
-                self.assertIsInstance(result, AsyncResult)
-
-        for i, result in enumerate(users, start=1):
-            self.assertTrue(result.ok)
-            self.assertIsNotNone(result.result)
-            self.assertEqual(i, result.result[0]['id'])
-
-        users = []
-        async with AsyncVkExecuteRequestPool() as pool:
-            for i in range(1, 25):
-                result = pool.add_call('users.get', token1, {'user_ids': i})
-                users.append(result)
-                self.assertIsInstance(result, AsyncResult)
-
-        for i, result in enumerate(users, start=1):
-            self.assertTrue(result.ok)
-            self.assertIsNotNone(result.result)
-            self.assertEqual(i, result.result[0]['id'])
-
-        users = []
-        async with AsyncVkExecuteRequestPool() as pool:
-            for i in range(1, 26):
-                result = pool.add_call('users.get', token1, {'user_ids': i})
-                users.append(result)
-                self.assertIsInstance(result, AsyncResult)
-
-            for i in range(26, 51):
-                result = pool.add_call('users.get', token2, {'user_ids': i})
-                users.append(result)
-                self.assertIsInstance(result, AsyncResult)
-
-        for i, result in enumerate(users, start=1):
-            self.assertTrue(result.ok)
-            self.assertIsNotNone(result.result)
-            self.assertEqual(i, result.result[0]['id'])
-
-    async def test_greater_than_25_calls_per_token(self):
-        users = []
-        async with AsyncVkExecuteRequestPool() as pool:
-            for i in range(1, 26):
-                result = pool.add_call('users.get', token1, {'user_ids': i})
-                users.append(result)
-                self.assertIsInstance(result, AsyncResult)
-
-        for i, result in enumerate(users, start=1):
-            self.assertTrue(result.ok)
-            self.assertIsNotNone(result.result)
-            self.assertEqual(i, result.result[0]['id'])
-
-        users = []
-        async with AsyncVkExecuteRequestPool() as pool:
-            for i in range(1, 50):
-                result = pool.add_call('users.get', token1, {'user_ids': i})
-                users.append(result)
-                self.assertIsInstance(result, AsyncResult)
-
-        for i, result in enumerate(users, start=1):
-            self.assertTrue(result.ok)
-            self.assertIsNotNone(result.result)
-            self.assertEqual(i, result.result[0]['id'])
-
-        users = []
-        async with AsyncVkExecuteRequestPool() as pool:
-            for i in range(1, 51):
-                result = pool.add_call('users.get', token1, {'user_ids': i})
-                users.append(result)
-                self.assertIsInstance(result, AsyncResult)
-
-            for i in range(51, 99):
-                result = pool.add_call('users.get', token2, {'user_ids': i})
-                users.append(result)
-                self.assertIsInstance(result, AsyncResult)
-
-        for i, result in enumerate(users, start=1):
-            self.assertTrue(result.ok)
-            self.assertIsNotNone(result.result)
-            self.assertEqual(i, result.result[0]['id'])
-
-    async def test_error_requests(self):
-        async with AsyncVkExecuteRequestPool() as pool:
-            error_result = pool.add_call('users.get', token1, {'user_ids': -1})
-            self.assertIsInstance(error_result, AsyncResult)
-
-        self.assertFalse(error_result.ok)
-        self.assertIsNone(error_result.result)
-        self.assertIsNotNone(error_result.error)
-        self.assertDictEqual({
-            'method': 'users.get', 'error_code': 113, 'error_msg': 'Invalid user id'
-        }, error_result.error)
-
-        async with AsyncVkExecuteRequestPool() as pool:
-            error_result = pool.add_call('users.get', token1, {'user_ids': -1})
-            success_result = pool.add_call('users.get', token2, {'user_ids': 1})
-
-        self.assertFalse(error_result.ok)
-        self.assertIsNone(error_result.result)
-        self.assertIsNotNone(error_result.error)
-        self.assertDictEqual({
-            'method': 'users.get', 'error_code': 113, 'error_msg': 'Invalid user id'
-        }, error_result.error)
-
-        self.assertTrue(success_result.ok)
-        self.assertIsNotNone(success_result.result)
-        self.assertEqual(1, success_result.result[0]['id'])
-
-    async def test_request_without_values(self):
-        async with AsyncVkExecuteRequestPool() as pool:
-            result = pool.add_call('users.get', token1)
-        self.assertTrue(result.ok)
-        self.assertIsNotNone(result.result)
-
-    async def test_false_cast_response(self):
-        async with AsyncVkExecuteRequestPool() as pool:
-            result = pool.add_call("groups.isMember", token1, {"user_id": 1, "group_id": 1})
-        self.assertTrue(result.ok)
-        self.assertIsNotNone(result.result)
-        self.assertEqual(0, result.result)
-
-    async def test_equal_requests(self):
-        """Тестирование того, что одинаковые запросы для одного токена будут выполняться только один раз"""
-        async with AsyncVkExecuteRequestPool() as pool:
-            result = pool.add_call("groups.isMember", token1, {"user_id": 1, "group_id": 1})
-            result2 = pool.add_call("groups.isMember", token1, {"user_id": 1, "group_id": 1})
-            result3 = pool.add_call("groups.isMember", token1, {"user_id": 1, "group_id": 1})
-            self.assertEqual(1, len(pool.pool[token1]))
-        self.assertIs(result, result2)
-        self.assertIs(result, result3)
-
-    async def test_invalid_token(self):
-        async with AsyncVkExecuteRequestPool() as pool:
-            result = pool.add_call("groups.isMember", 'invalid_token', {"user_id": 1, "group_id": 1})
-        self.assertEqual(5, result.error["error_code"])
-        self.assertEqual("groups.isMember", result.error["method"])
-
-    async def test_invalid_call(self):
-        async with AsyncVkExecuteRequestPool() as pool:
-            result = pool.add_call("groups.isMember", token1, {"user_id": -1, "group_id": 1})
-        self.assertEqual(100, result.error['error_code'])
-
-    async def test_invalid_token_type(self):
-        """Вызов метода, который доступен только с токеном пользователя, с токеном группы"""
-        async with AsyncVkExecuteRequestPool() as pool:
-            result = pool.add_call("likes.isLiked", token1, {
-                "user_id": 1,
-                "owner_id": -1,
-                "type": "post",
-                "item_id": 396449,
-            })
-        self.assertIsNone(result.result)
-        self.assertIsNotNone(result.error)
-        self.assertEqual(27, result.error['error_code'])
-        self.assertEqual('likes.isLiked', result.error['method'])
+import os
+import unittest
+from unittest import IsolatedAsyncioTestCase
+
+# from dotenv import load_dotenv
+
+from aiovk.pools import AsyncResult, AsyncVkExecuteRequestPool
+
+# load_dotenv(
+#     os.path.join(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))), ".env")
+# )
+token1 = os.getenv('TEST_TOKEN_1')
+token2 = os.getenv('TEST_TOKEN_2')
+
+
+# TODO need refactoring
+@unittest.skip
+class ExecutePoolTestCase(IsolatedAsyncioTestCase):
+    async def test_one_call_per_request(self):
+        async with AsyncVkExecuteRequestPool() as pool:
+            result = pool.add_call('users.get', token1, {'user_ids': 1})
+            self.assertIsInstance(result, AsyncResult)
+        self.assertIsNotNone(result.result)
+        self.assertEqual(1, result.result[0]['id'])
+
+        async with AsyncVkExecuteRequestPool() as pool:
+            result = pool.add_call('users.get', token1, {'user_ids': 1})
+            self.assertIsInstance(result, AsyncResult)
+            result2 = pool.add_call('users.get', token2, {'user_ids': 2})
+            self.assertIsInstance(result2, AsyncResult)
+
+        self.assertTrue(result.ok)
+        self.assertIsNotNone(result.result)
+        self.assertEqual(1, result.result[0]['id'])
+        self.assertTrue(result2.ok)
+        self.assertIsNotNone(result2.result)
+        self.assertEqual(2, result2.result[0]['id'])
+
+    async def test_less_or_equal_than_25_calls_per_token(self):
+        users = []
+        async with AsyncVkExecuteRequestPool() as pool:
+            for i in range(1, 2):
+                result = pool.add_call('users.get', token1, {'user_ids': i})
+                users.append(result)
+                self.assertIsInstance(result, AsyncResult)
+
+        for i, result in enumerate(users, start=1):
+            self.assertTrue(result.ok)
+            self.assertIsNotNone(result.result)
+            self.assertEqual(i, result.result[0]['id'])
+
+        users = []
+        async with AsyncVkExecuteRequestPool() as pool:
+            for i in range(1, 25):
+                result = pool.add_call('users.get', token1, {'user_ids': i})
+                users.append(result)
+                self.assertIsInstance(result, AsyncResult)
+
+        for i, result in enumerate(users, start=1):
+            self.assertTrue(result.ok)
+            self.assertIsNotNone(result.result)
+            self.assertEqual(i, result.result[0]['id'])
+
+        users = []
+        async with AsyncVkExecuteRequestPool() as pool:
+            for i in range(1, 26):
+                result = pool.add_call('users.get', token1, {'user_ids': i})
+                users.append(result)
+                self.assertIsInstance(result, AsyncResult)
+
+            for i in range(26, 51):
+                result = pool.add_call('users.get', token2, {'user_ids': i})
+                users.append(result)
+                self.assertIsInstance(result, AsyncResult)
+
+        for i, result in enumerate(users, start=1):
+            self.assertTrue(result.ok)
+            self.assertIsNotNone(result.result)
+            self.assertEqual(i, result.result[0]['id'])
+
+    async def test_greater_than_25_calls_per_token(self):
+        users = []
+        async with AsyncVkExecuteRequestPool() as pool:
+            for i in range(1, 26):
+                result = pool.add_call('users.get', token1, {'user_ids': i})
+                users.append(result)
+                self.assertIsInstance(result, AsyncResult)
+
+        for i, result in enumerate(users, start=1):
+            self.assertTrue(result.ok)
+            self.assertIsNotNone(result.result)
+            self.assertEqual(i, result.result[0]['id'])
+
+        users = []
+        async with AsyncVkExecuteRequestPool() as pool:
+            for i in range(1, 50):
+                result = pool.add_call('users.get', token1, {'user_ids': i})
+                users.append(result)
+                self.assertIsInstance(result, AsyncResult)
+
+        for i, result in enumerate(users, start=1):
+            self.assertTrue(result.ok)
+            self.assertIsNotNone(result.result)
+            self.assertEqual(i, result.result[0]['id'])
+
+        users = []
+        async with AsyncVkExecuteRequestPool() as pool:
+            for i in range(1, 51):
+                result = pool.add_call('users.get', token1, {'user_ids': i})
+                users.append(result)
+                self.assertIsInstance(result, AsyncResult)
+
+            for i in range(51, 99):
+                result = pool.add_call('users.get', token2, {'user_ids': i})
+                users.append(result)
+                self.assertIsInstance(result, AsyncResult)
+
+        for i, result in enumerate(users, start=1):
+            self.assertTrue(result.ok)
+            self.assertIsNotNone(result.result)
+            self.assertEqual(i, result.result[0]['id'])
+
+    async def test_error_requests(self):
+        async with AsyncVkExecuteRequestPool() as pool:
+            error_result = pool.add_call('users.get', token1, {'user_ids': -1})
+            self.assertIsInstance(error_result, AsyncResult)
+
+        self.assertFalse(error_result.ok)
+        self.assertIsNone(error_result.result)
+        self.assertIsNotNone(error_result.error)
+        self.assertDictEqual({
+            'method': 'users.get', 'error_code': 113, 'error_msg': 'Invalid user id'
+        }, error_result.error)
+
+        async with AsyncVkExecuteRequestPool() as pool:
+            error_result = pool.add_call('users.get', token1, {'user_ids': -1})
+            success_result = pool.add_call('users.get', token2, {'user_ids': 1})
+
+        self.assertFalse(error_result.ok)
+        self.assertIsNone(error_result.result)
+        self.assertIsNotNone(error_result.error)
+        self.assertDictEqual({
+            'method': 'users.get', 'error_code': 113, 'error_msg': 'Invalid user id'
+        }, error_result.error)
+
+        self.assertTrue(success_result.ok)
+        self.assertIsNotNone(success_result.result)
+        self.assertEqual(1, success_result.result[0]['id'])
+
+    async def test_request_without_values(self):
+        async with AsyncVkExecuteRequestPool() as pool:
+            result = pool.add_call('users.get', token1)
+        self.assertTrue(result.ok)
+        self.assertIsNotNone(result.result)
+
+    async def test_false_cast_response(self):
+        async with AsyncVkExecuteRequestPool() as pool:
+            result = pool.add_call("groups.isMember", token1, {"user_id": 1, "group_id": 1})
+        self.assertTrue(result.ok)
+        self.assertIsNotNone(result.result)
+        self.assertEqual(0, result.result)
+
+    async def test_equal_requests(self):
+        """Тестирование того, что одинаковые запросы для одного токена будут выполняться только один раз"""
+        async with AsyncVkExecuteRequestPool() as pool:
+            result = pool.add_call("groups.isMember", token1, {"user_id": 1, "group_id": 1})
+            result2 = pool.add_call("groups.isMember", token1, {"user_id": 1, "group_id": 1})
+            result3 = pool.add_call("groups.isMember", token1, {"user_id": 1, "group_id": 1})
+            self.assertEqual(1, len(pool.pool[token1]))
+        self.assertIs(result, result2)
+        self.assertIs(result, result3)
+
+    async def test_invalid_token(self):
+        async with AsyncVkExecuteRequestPool() as pool:
+            result = pool.add_call("groups.isMember", 'invalid_token', {"user_id": 1, "group_id": 1})
+        self.assertEqual(5, result.error["error_code"])
+        self.assertEqual("groups.isMember", result.error["method"])
+
+    async def test_invalid_call(self):
+        async with AsyncVkExecuteRequestPool() as pool:
+            result = pool.add_call("groups.isMember", token1, {"user_id": -1, "group_id": 1})
+        self.assertEqual(100, result.error['error_code'])
+
+    async def test_invalid_token_type(self):
+        """Вызов метода, который доступен только с токеном пользователя, с токеном группы"""
+        async with AsyncVkExecuteRequestPool() as pool:
+            result = pool.add_call("likes.isLiked", token1, {
+                "user_id": 1,
+                "owner_id": -1,
+                "type": "post",
+                "item_id": 396449,
+            })
+        self.assertIsNone(result.result)
+        self.assertIsNotNone(result.error)
+        self.assertEqual(27, result.error['error_code'])
+        self.assertEqual('likes.isLiked', result.error['method'])
```

### Comparing `aiovk-4.0.0/tests/utils.py` & `aiovk-4.1.0/tests/utils.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import os
-from unittest import TestCase
-
-from aiohttp.test_utils import setup_test_loop, teardown_test_loop
-
-TEST_DIR = os.path.dirname(os.path.abspath(__file__))
-
-
-class AioTestCase(TestCase):
-    def setUp(self):
-        self.loop = setup_test_loop()
-        self.loop.run_until_complete(self.setUpAsync())
-
-    async def setUpAsync(self):
-        pass
-
-    def tearDown(self):
-        self.loop.run_until_complete(self.tearDownAsync())
-        teardown_test_loop(self.loop)
-
-    async def tearDownAsync(self):
-        pass
+import os
+from unittest import TestCase
+
+from aiohttp.test_utils import setup_test_loop, teardown_test_loop
+
+TEST_DIR = os.path.dirname(os.path.abspath(__file__))
+
+
+class AioTestCase(TestCase):
+    def setUp(self):
+        self.loop = setup_test_loop()
+        self.loop.run_until_complete(self.setUpAsync())
+
+    async def setUpAsync(self):
+        pass
+
+    def tearDown(self):
+        self.loop.run_until_complete(self.tearDownAsync())
+        teardown_test_loop(self.loop)
+
+    async def tearDownAsync(self):
+        pass
```


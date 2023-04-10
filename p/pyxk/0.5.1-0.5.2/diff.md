# Comparing `tmp/pyxk-0.5.1.tar.gz` & `tmp/pyxk-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.5.1.tar", last modified: Sun Apr  9 12:40:04 2023, max compression
+gzip compressed data, was "pyxk-0.5.2.tar", last modified: Mon Apr 10 03:09:59 2023, max compression
```

## Comparing `pyxk-0.5.1.tar` & `pyxk-0.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.368316 pyxk-0.5.1/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.1/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-09 12:40:04.368316 pyxk-0.5.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.1/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.358316 pyxk-0.5.1/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)      701 2023-04-09 12:39:02.000000 pyxk-0.5.1/pyxk/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    11004 2023-04-09 12:38:52.000000 pyxk-0.5.1/pyxk/aclient.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.358316 pyxk-0.5.1/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       79 2023-02-24 04:10:40.000000 pyxk-0.5.1/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3639 2023-04-06 15:25:24.000000 pyxk-0.5.1/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4701 2023-04-06 15:27:39.000000 pyxk-0.5.1/pyxk/aes/cryptor.py
--rw-rw----   0 root         (0) everybody  (9997)      954 2023-03-15 06:04:12.000000 pyxk-0.5.1/pyxk/lazy_loader.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.358316 pyxk-0.5.1/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       82 2023-03-16 14:08:36.000000 pyxk-0.5.1/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     8292 2023-03-16 12:13:38.000000 pyxk-0.5.1/pyxk/m3u8/_download.py
--rw-rw----   0 root         (0) everybody  (9997)     3199 2023-03-16 16:35:49.000000 pyxk-0.5.1/pyxk/m3u8/_entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)     7791 2023-03-16 16:35:32.000000 pyxk-0.5.1/pyxk/m3u8/_m3u8.py
--rw-rw----   0 root         (0) everybody  (9997)     4504 2023-03-17 04:00:18.000000 pyxk-0.5.1/pyxk/m3u8/_parser.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.368316 pyxk-0.5.1/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      235 2023-04-06 15:53:39.000000 pyxk-0.5.1/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     5598 2023-04-06 16:07:00.000000 pyxk-0.5.1/pyxk/requests/_entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)     7514 2023-03-31 10:17:41.000000 pyxk-0.5.1/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)    21859 2023-04-06 15:20:21.000000 pyxk-0.5.1/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    12202 2023-04-06 16:00:37.000000 pyxk-0.5.1/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.358316 pyxk-0.5.1/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      539 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       91 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-09 12:40:04.368316 pyxk-0.5.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      916 2023-04-09 12:40:00.000000 pyxk-0.5.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.2/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-10 03:09:59.266989 pyxk-0.5.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)      726 2023-04-10 02:29:14.000000 pyxk-0.5.2/pyxk/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    15453 2023-04-10 03:02:22.000000 pyxk-0.5.2/pyxk/aclient.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       79 2023-02-24 04:10:40.000000 pyxk-0.5.2/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3639 2023-04-06 15:25:24.000000 pyxk-0.5.2/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4701 2023-04-06 15:27:39.000000 pyxk-0.5.2/pyxk/aes/cryptor.py
+-rw-rw----   0 root         (0) everybody  (9997)      954 2023-04-09 12:40:57.000000 pyxk-0.5.2/pyxk/lazy_loader.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       82 2023-03-16 14:08:36.000000 pyxk-0.5.2/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     8292 2023-03-16 12:13:38.000000 pyxk-0.5.2/pyxk/m3u8/_download.py
+-rw-rw----   0 root         (0) everybody  (9997)     3199 2023-03-16 16:35:49.000000 pyxk-0.5.2/pyxk/m3u8/_entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     7791 2023-03-16 16:35:32.000000 pyxk-0.5.2/pyxk/m3u8/_m3u8.py
+-rw-rw----   0 root         (0) everybody  (9997)     4504 2023-03-17 04:00:18.000000 pyxk-0.5.2/pyxk/m3u8/_parser.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      235 2023-04-06 15:53:39.000000 pyxk-0.5.2/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5598 2023-04-06 16:07:00.000000 pyxk-0.5.2/pyxk/requests/_entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     7514 2023-03-31 10:17:41.000000 pyxk-0.5.2/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)    21859 2023-04-06 15:20:21.000000 pyxk-0.5.2/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    12202 2023-04-09 12:40:57.000000 pyxk-0.5.2/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      539 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       91 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-10 03:09:59.266989 pyxk-0.5.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      917 2023-04-10 03:09:51.000000 pyxk-0.5.2/setup.py
```

### Comparing `pyxk-0.5.1/LICENSE` & `pyxk-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/__init__.py` & `pyxk-0.5.2/pyxk/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,11 +29,12 @@
     request,
     wget,
     Session,
 )
 from pyxk.lazy_loader import LazyLoader
 from pyxk.aclient import (
     AsyncSession,
+    NovelSpiderTemplate,
     default_live,
     default_progress_columns,
     default_download_progress_columns
 )
```

### Comparing `pyxk-0.5.1/pyxk/aclient.py` & `pyxk-0.5.2/pyxk/aclient.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import re
+import sys
 import types
 import typing
 import asyncio
+from itertools import zip_longest
 from multidict import CIMultiDict
-from asyncio import AbstractEventLoop
+from asyncio import AbstractEventLoop as EventLoop
 
 from yarl import URL
 from lxml import etree
 from aiohttp import (
     ClientTimeout,
     TCPConnector,
     ClientSession as Session
 )
 import aiohttp.client_exceptions
 import rich.live as rich_live
+import rich.console as rich_console
 import rich.progress as rich_progress
 from aiohttp.client_reqrep import ClientResponse as Response
 
 from pyxk.utils import get_user_agent
 from pyxk.lazy_loader import LazyLoader
 
 rich_box = LazyLoader("rich_box", globals(), "rich.box")
 rich_panel = LazyLoader("rich_panel", globals(), "rich.panel")
 rich_table = LazyLoader("rich_table", globals(), "rich.table")
-rich_console = LazyLoader("rich_console", globals(), "rich.console")
 
 
 
 class AsyncSession:
 
     limit: int = 16
     timeout: typing.Union[int, float, dict] = {
@@ -40,18 +42,18 @@
     start_urls: list = []
     user_agent: str = get_user_agent("android")
     aiohttp_kwargs: dict = {}
 
     def __init__(
         self,
         *,
-        loop: AbstractEventLoop=None,
+        loop: EventLoop=None,
         session: Session=None
     ):
-        self._loop: AbstractEventLoop = loop
+        self._loop: EventLoop = loop
         self._session: Session = session
 
     async def start(self):
         """运行开始之前调用"""
 
     async def stop(self):
         """运行完成之后调用"""
@@ -60,31 +62,31 @@
     def run(cls, **kwargs) -> typing.Union[object, list]:
         """类方法: 协程入口 run, 应该从这里开始
 
         Return: ClientSession, [..., ...]
         返回值: 当前类的实例化, 协程运行结果列表
         """
         # Event loop
-        if not isinstance(kwargs.get("loop", None), AbstractEventLoop):
+        if not isinstance(kwargs.get("loop", None), EventLoop):
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
             kwargs["loop"] = loop
         # Instance
-        self: ClientSession = cls(**kwargs)
+        self = cls(**kwargs)
         result: list = self._loop.run_until_complete(self.async_start())
         # close event loop
-        if isinstance(self._loop, AbstractEventLoop):
+        if isinstance(self._loop, EventLoop):
             self._loop.close()
         return self, result
 
     async def async_start(self):
         try:
             # event loop
             if (
-                not isinstance(self._loop, AbstractEventLoop)
+                not isinstance(self._loop, EventLoop)
                 or self._loop.is_closed() is True
             ):
                 self._loop = asyncio.get_event_loop()
                 asyncio.set_event_loop(self._loop)
             # create aiohttp.ClientSession
             if not (
                 isinstance(self._session, Session)
@@ -106,15 +108,15 @@
             await self._session.close()
 
     async def create_client_session(self):
         "创建 aiohttp.ClientSession"
         return Session(loop=self._loop, headers=self.merge_headers(), **self.merge_aiohttp_kwargs())
 
     @property
-    def loop(self) -> AbstractEventLoop:
+    def loop(self) -> EventLoop:
         return self._loop
 
     def merge_headers(self) -> CIMultiDict:
         """aiohttp.ClientSession Headers"""
         user_agent = self.user_agent if isinstance(self.user_agent, str) else get_user_agent("android")
         headers = CIMultiDict(self.headers or {})
         headers.setdefault("User-Agent", user_agent)
@@ -152,22 +154,23 @@
 
         :params: url
         :params: callback: 回调函数
         :params: method: 请求方法
         :params: cb_kwargs: 回调函数关键词参数
         :params: **kwargs: 异步请求参数
         """
+        cb_kwargs = cb_kwargs if isinstance(cb_kwargs, dict) else {}
         while True:
             try:
                 async with self._session.request(method=method, url=url, **kwargs) as response:
                     response = add_response_method(response)
                     if callable(callback):
-                        result = await callback(response=response, **cb_kwargs or {})
+                        result = await callback(response=response, **cb_kwargs)
                         return result
-                    return
+                    return response
             # 请求超时 重试
             except asyncio.exceptions.TimeoutError:
                 await asyncio.sleep(1)
             # 连接错误 重试
             except (
                 aiohttp.client_exceptions.ClientOSError,
                 aiohttp.client_exceptions.ClientPayloadError,
@@ -179,43 +182,47 @@
                 await asyncio.sleep(2)
 
     async def gather_urls(
         self,
         *urls,
         callback: callable=None,
         method: str="GET",
-        cb_kwargs: dict=None,
+        cb_kwargs_list: typing.List[dict]=None,
         return_exceptions: bool=False,
         **kwargs
     ):
         """异步Request gather方法 异步发送大量url
 
-        :params: urls: url列表
+        :params: *urls: url列表
         :params: callback: 回调函数
         :params: method: 请求方法
-        :params: cb_kwargs: 回调函数关键词参数
+        :params: cb_kwargs_list: 回调函数关键词参数 列表
         :params: return_exceptions: 异常传递 若为真,异常将不抛出 传递值返回结果中
         :params: **kwargs: 异步请求参数
         """
+        if isinstance(cb_kwargs_list, dict):
+            cb_kwargs_list = [cb_kwargs_list]
+        elif not isinstance(cb_kwargs_list, list):
+            cb_kwargs_list = []
         tasks = [
             self.request(
                 url=url,
                 callback=callback,
                 method=method,
-                cb_kwargs=cb_kwargs,
+                cb_kwargs=dict(cb_kwargs),
                 **kwargs
             )
-            for url in urls
+            for url, cb_kwargs in zip_longest(urls, cb_kwargs_list, fillvalue={})
         ]
         return await asyncio.gather(*tasks, return_exceptions=return_exceptions)
 
     async def start_request(self):
         """异步请求入口方法"""
         if not self.start_urls:
-            raise NotImplementedError(f"{self.__class__.__name__}.start_urls is empty")
+            raise NotImplementedError(f"{self.__class__.__name__}.start_urls is empty(Must be a 'list')")
         tasks = [
             self.request(url, callback=self.parse)
             for url in self.start_urls
         ]
         result = await asyncio.gather(*tasks)
         return result
 
@@ -223,19 +230,22 @@
         """默认解析方法
 
         :params: response: 异步请求响应
         :参数传递可以使用 cb_kwargs
         """
         raise NotImplementedError(f"'{self.__class__.__name__}.parse' not implemented")
 
+    async def sleep(self, delay: typing.Union[int, float]=0, result: any=None):
+        return await asyncio.sleep(delay, result=result)
+
 
 def add_response_method(response: Response) -> Response:
     # 为 Response 添加 xpath解析方法
-    async def _xpath(self, _xpath, **kwargs):
-        _htmlparse = etree.HTML(await self.text())
+    async def _xpath(self, _xpath, *, encoding=None, errors="strict", **kwargs):
+        _htmlparse = etree.HTML(await self.text(encoding=encoding, errors=errors))
         class XpathList(list):
             def get(self, default=None):
                 if not self:
                     return default
                 return self[0]
         return XpathList(_htmlparse.xpath(_xpath, **kwargs))
 
@@ -333,7 +343,109 @@
     live = rich_live.Live(
         live,
         transient=transient,
         console=console,
         refresh_per_second=refresh_per_second
     )
     return live, progress, progress_task
+
+
+class NovelSpiderTemplate(AsyncSession):
+    """小说爬虫模板文件
+
+    :params: keyword: 爬虫搜索值
+    """
+
+    name: str = None
+    store: str = None
+    start_urls: str = None
+    user_agent: str = get_user_agent("windows")
+
+    def __init__(self, *, keyword: str=None, **kwargs):
+        super().__init__(**kwargs)
+        self._console = rich_console.Console()
+        self._keyword = keyword
+        self.book, self.author = None, None
+
+    async def start_request(self):
+        """异步请求入口方法"""
+        if not self.start_urls:
+            raise NotImplementedError(f"{self.__class__.__name__}.start_urls is empty(Must be a 'str')")
+        if not self.name:
+            raise NotImplementedError(f"{self.__class__.__name__}.name is empty(Must be a 'str')")
+        if not self.store:
+            raise NotImplementedError(f"{self.__class__.__name__}.store is empty(Must be a 'str')")
+        self._console.print(f"[magenta b]{self.name}[/] < {self.start_urls} >\n", justify="center")
+        return await self.request(self.start_urls, self.parse)
+
+    @property
+    def keyword(self) -> str:
+        """搜索 keyword"""
+        while not(self._keyword and isinstance(self._keyword, str)):
+            self._keyword = self._console.input("[yellow b]搜索书名或作者[/][Exit]: ").strip()
+            if self._keyword.lower() in ("e", "exit"):
+                self._console.print("[red]Exit[/]")
+                sys.exit()
+        return self._keyword
+
+    def default_print_search_result(self, *col_names: typing.Tuple[str], books_info: typing.Dict[str, dict]):
+        """使用 rich.table 打印搜索结果
+
+        :params: *colv_names: table表头 - 表头每列名称
+        :params: books_info: table内容
+        """
+        table = rich_table.Table(
+            caption=f"[dim]< {self._keyword} > Total: {len(books_info)}[/]",
+            caption_justify="right",
+            box=rich_box.ASCII_DOUBLE_HEAD
+        )
+        # table 添加列
+        table.add_column("", no_wrap=False, style="cyan", justify="center")
+        for item in col_names:
+            table.add_column(str(item), justify="center")
+        # table 添加行
+        for index, book in books_info.items():
+            table.add_row(str(index), *[book.get(item, "") for item in col_names])
+        self._console.print(table)
+
+    def default_print_novel_detail(self, *args: typing.Tuple[str]):
+        """使用 rich.panel 打印小说详情页
+
+        :params: *args: 每行内容
+        """
+        renderable = rich_table.Table(show_header=False, box=rich_box.SIMPLE_HEAD)
+        renderable.add_column(justify="left", overflow="fold",)
+        for item in args:
+            renderable.add_row(item)
+        panel = rich_panel.Panel(renderable, border_style="bright_blue")
+        self._console.print(panel)
+
+    def select_form_items(
+        self,
+        *items: typing.Tuple[str],
+        description: str=None,
+        exception: typing.List[str]=None,
+        arbitrary: bool=False
+    ):
+        """选择器
+
+        :params: *items: input选择范围
+        :params: description: 说明，介绍
+        :params: exception: 额外的选择范围, 当input输入在其中是返回
+        :params: arbitrary: 任意值返回
+
+        注意: 输入 'e' 或者 'exit' 将使用 sys.exit() 关闭程序
+        """
+        # 需要额外处理的参数
+        exception = [str(e).lower() for e in exception or []]
+        exception = set(exception)
+        items = [str(item) for item in items]
+        items.extend(exception)
+        description = description or "[yellow b]请选择: [/]"
+        while True:
+            select = self._console.input(description).strip()
+            if select.lower() in ("e", "exit"):
+                self._console.print("[red]Exit[/]")
+                sys.exit()
+            if select in items or arbitrary:
+                break
+        return select
```

### Comparing `pyxk-0.5.1/pyxk/aes/_fmtdata.py` & `pyxk-0.5.2/pyxk/aes/_fmtdata.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/aes/cryptor.py` & `pyxk-0.5.2/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/lazy_loader.py` & `pyxk-0.5.2/pyxk/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/m3u8/_download.py` & `pyxk-0.5.2/pyxk/m3u8/_download.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/m3u8/_entry_point.py` & `pyxk-0.5.2/pyxk/m3u8/_entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/m3u8/_m3u8.py` & `pyxk-0.5.2/pyxk/m3u8/_m3u8.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/m3u8/_parser.py` & `pyxk-0.5.2/pyxk/m3u8/_parser.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/requests/_entry_point.py` & `pyxk-0.5.2/pyxk/requests/_entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/requests/api.py` & `pyxk-0.5.2/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/requests/sessions.py` & `pyxk-0.5.2/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk/utils.py` & `pyxk-0.5.2/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/pyxk.egg-info/SOURCES.txt` & `pyxk-0.5.2/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.1/setup.py` & `pyxk-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyxk",
-    version="0.5.1",
+    version="0.5.2",
     author="xiek",
     install_requires=[
         "requests",
         "pycryptodome",
         "rich",
         "m3u8",
         "aiohttp",
@@ -31,8 +31,8 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
-)
+)
```


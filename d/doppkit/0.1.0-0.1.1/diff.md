# Comparing `tmp/doppkit-0.1.0.tar.gz` & `tmp/doppkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-0.1.0.tar", last modified: Tue Mar 21 17:45:51 2023, max compression
+gzip compressed data, was "doppkit-0.1.1.tar", last modified: Mon Apr 10 17:56:28 2023, max compression
```

## Comparing `doppkit-0.1.0.tar` & `doppkit-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:51.147263 doppkit-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-21 17:45:32.000000 doppkit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-03-21 17:45:51.147263 doppkit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-21 17:45:32.000000 doppkit-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-21 17:45:32.000000 doppkit-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 17:45:51.147263 doppkit-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:51.143263 doppkit-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:51.143263 doppkit-0.1.0/src/doppkit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-21 17:45:32.000000 doppkit-0.1.0/src/doppkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-21 17:45:32.000000 doppkit-0.1.0/src/doppkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-21 17:45:32.000000 doppkit-0.1.0/src/doppkit/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-03-21 17:45:32.000000 doppkit-0.1.0/src/doppkit/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-03-21 17:45:32.000000 doppkit-0.1.0/src/doppkit/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-21 17:45:32.000000 doppkit-0.1.0/src/doppkit/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-03-21 17:45:32.000000 doppkit-0.1.0/src/doppkit/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:51.143263 doppkit-0.1.0/src/doppkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-03-21 17:45:51.000000 doppkit-0.1.0/src/doppkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-21 17:45:51.000000 doppkit-0.1.0/src/doppkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 17:45:51.000000 doppkit-0.1.0/src/doppkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-21 17:45:51.000000 doppkit-0.1.0/src/doppkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 17:45:50.000000 doppkit-0.1.0/src/doppkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-21 17:45:51.000000 doppkit-0.1.0/src/doppkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-21 17:45:51.000000 doppkit-0.1.0/src/doppkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:56:28.982736 doppkit-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 17:56:14.000000 doppkit-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 17:56:28.982736 doppkit-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 17:56:14.000000 doppkit-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-10 17:56:14.000000 doppkit-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:56:28.982736 doppkit-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:56:28.978736 doppkit-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:56:28.978736 doppkit-0.1.1/src/doppkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:56:28.982736 doppkit-0.1.1/src/doppkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/top_level.txt
```

### Comparing `doppkit-0.1.0/LICENSE` & `doppkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.0/PKG-INFO` & `doppkit-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-0.1.0/pyproject.toml` & `doppkit-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.0/src/doppkit/app.py` & `doppkit-0.1.1/src/doppkit/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+import asyncio
 import click
 import logging
 import pathlib
 
 from .sync import sync as syncFunction
 from .list import listAOIs as listAOIsFunction
 from .list import listExports as listExportsFunction
 
 
-class Application(object):
+class Application:
     def __init__(self, token=None, url=None, log_level=logging.ERROR, threads=20):
         self.token = token
         self.url = url
         self.log_level = log_level
         self.threads = threads
         self.progress = False
         self.logging = logging
+        self.limit = asyncio.Semaphore(threads)
+
 
 @click.group()
 @click.option(
     "--token",
     envvar="GRID_ACCESS_TOKEN",
     help="GRiD access token. Use GRID_ACCESS_TOKEN environment variable to globally override",
     type=str,
```

### Comparing `doppkit-0.1.0/src/doppkit/cache.py` & `doppkit-0.1.1/src/doppkit/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,58 +84,76 @@
             "[progress.percentage]{task.percentage:>3.0f}%",
             text_column,
             bar_column,
             DownloadColumn(),
             TransferSpeedColumn(),
             transient=True,
         ) as progress:
+
             files = await asyncio.gather(
-                *[cache_url(args, url, headers, client, progress) for url in urls],
+                *[asyncio.create_task(
+                    cache_url(
+                        args,
+                        url,
+                        headers,
+                        client,
+                        progress,
+                    )
+                ) for url in urls],
                 return_exceptions=True,
             )
     return files
 
 
 async def cache_url(args, url, headers, client, progress):
-    request = client.build_request("GET", url, headers=headers, timeout=None)
-    response = await client.send(request, stream=True)
-    filename = None  # placeholder
-    total = max(0, int(response.headers.get("Content-length", 0)))
-
-    while response.next_request is not None:
-        extracted_filename = Content._extract_filename(response.headers)
-        filename = extracted_filename if extracted_filename is not None else filename
-        request = response.next_request
-        await response.aclose()
+    limit = args.limit
+    async with limit:
+        request = client.build_request("GET", url, headers=headers, timeout=None)
         response = await client.send(request, stream=True)
-        total = max(total, int(response.headers.get("Content-length", 0)))
 
-    c = Content(response.headers, filename=filename, args=args)
-    if args.progress:
-        name = c.target.name if isinstance(c.target, pathlib.Path) else "bytesIO"
-        download_task = progress.add_task(f"{name}", total=total)
-    chunk_count = 0
-
-    if isinstance(c.target, BytesIO):
-        # do in-memory stuff
-        async for chunk in response.aiter_bytes():
-            _ = c.target.write(chunk)
-            chunk_count += 1
-
-            if args.progress:
-                progress.update(download_task, completed=response.num_bytes_downloaded)
-        c.target.flush()
-        c.target.seek(0)
-
-    else:
-        # we are writing to disk asyncronously
-        async with aiofiles.open(c.target, "wb+") as f:
+
+        filename = None  # placeholder
+        total = max(0, int(response.headers.get("Content-length", 0)))
+
+        while response.next_request is not None:
+            extracted_filename = Content._extract_filename(response.headers)
+            filename = extracted_filename if extracted_filename is not None else filename
+            request = response.next_request
+            await response.aclose()
+            response = await client.send(request, stream=True)
+            total = max(total, int(response.headers.get("Content-length", 0)))
+
+        c = Content(response.headers, filename=filename, args=args)
+        if args.progress:
+            name = c.target.name if isinstance(c.target, pathlib.Path) else "bytesIO"
+            download_task = progress.add_task(f"{name}", total=total)
+        chunk_count = 0
+
+        if isinstance(c.target, BytesIO):
+            # do in-memory stuff
             async for chunk in response.aiter_bytes():
-                await f.write(chunk)
+                _ = c.target.write(chunk)
                 chunk_count += 1
 
                 if args.progress:
-                    progress.update(
-                        download_task, completed=response.num_bytes_downloaded
-                    )
-    await response.aclose()
+                    progress.update(download_task, completed=response.num_bytes_downloaded)
+            c.target.flush()
+            c.target.seek(0)
+
+        else:
+            # we are writing to disk asyncronously
+            async with aiofiles.open(c.target, "wb+") as f:
+                async for chunk in response.aiter_bytes():
+                    await f.write(chunk)
+                    chunk_count += 1
+
+                    if args.progress:
+                        progress.update(
+                            download_task, completed=response.num_bytes_downloaded
+                        )
+        if args.progress:
+            # we can hide the task now that it's finished
+            progress.update(download_task, visible=False)
+        await response.aclose()
+        if limit.locked():
+            await asyncio.sleep(0.5)
     return c
```

### Comparing `doppkit-0.1.0/src/doppkit/grid.py` & `doppkit-0.1.1/src/doppkit/grid.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.0/src/doppkit/list.py` & `doppkit-0.1.1/src/doppkit/list.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.0/src/doppkit/sync.py` & `doppkit-0.1.1/src/doppkit/sync.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.0/src/doppkit.egg-info/PKG-INFO` & `doppkit-0.1.1/src/doppkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```


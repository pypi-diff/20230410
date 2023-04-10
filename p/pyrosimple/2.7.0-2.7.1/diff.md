# Comparing `tmp/pyrosimple-2.7.0.tar.gz` & `tmp/pyrosimple-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosimple-2.7.0.tar", max compression
+gzip compressed data, was "pyrosimple-2.7.1.tar", max compression
```

## Comparing `pyrosimple-2.7.0.tar` & `pyrosimple-2.7.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     2131 2022-12-15 22:23:39.854116 pyrosimple-2.7.0/README.md
--rw-r--r--   0        0        0     3333 2023-02-11 21:43:55.610494 pyrosimple-2.7.0/pyproject.toml
--rw-r--r--   0        0        0      538 2022-12-19 17:11:38.923701 pyrosimple-2.7.0/src/pyrosimple/__init__.py
--rw-r--r--   0        0        0     8747 2023-02-09 18:43:16.912640 pyrosimple-2.7.0/src/pyrosimple/config.py
--rw-r--r--   0        0        0    10194 2022-12-29 00:29:13.781861 pyrosimple-2.7.0/src/pyrosimple/data/full-example.rc
--rw-r--r--   0        0        0     1273 2022-12-19 17:11:38.923701 pyrosimple-2.7.0/src/pyrosimple/error.py
--rw-r--r--   0        0        0        0 2022-12-19 17:11:41.443698 pyrosimple-2.7.0/src/pyrosimple/io/__init__.py
--rw-r--r--   0        0        0     8564 2023-01-14 04:07:35.778617 pyrosimple-2.7.0/src/pyrosimple/io/scgi.py
--rw-r--r--   0        0        0        0 2022-12-19 17:11:41.443698 pyrosimple-2.7.0/src/pyrosimple/job/__init__.py
--rw-r--r--   0        0        0     2963 2022-12-19 17:11:41.443698 pyrosimple-2.7.0/src/pyrosimple/job/action.py
--rw-r--r--   0        0        0     2977 2022-12-29 19:15:58.212292 pyrosimple-2.7.0/src/pyrosimple/job/base.py
--rw-r--r--   0        0        0     9469 2023-02-04 20:21:51.797829 pyrosimple-2.7.0/src/pyrosimple/job/metrics.py
--rw-r--r--   0        0        0     1691 2023-02-04 21:14:43.625074 pyrosimple-2.7.0/src/pyrosimple/job/move_path.py
--rw-r--r--   0        0        0     1743 2022-12-19 17:11:41.443698 pyrosimple-2.7.0/src/pyrosimple/job/move_torrent.py
--rw-r--r--   0        0        0     4197 2023-01-22 17:54:55.278327 pyrosimple-2.7.0/src/pyrosimple/job/queue.py
--rw-r--r--   0        0        0     9954 2022-12-30 00:02:14.668573 pyrosimple-2.7.0/src/pyrosimple/job/watch.py
--rw-r--r--   0        0        0        0 2022-12-19 17:11:41.443698 pyrosimple-2.7.0/src/pyrosimple/job/web.py
--rw-r--r--   0        0        0        0 2022-12-18 17:48:03.812685 pyrosimple-2.7.0/src/pyrosimple/py.typed
--rw-r--r--   0        0        0      112 2023-01-15 15:15:41.811874 pyrosimple-2.7.0/src/pyrosimple/scripts/__init__.py
--rw-r--r--   0        0        0     8026 2023-01-20 16:41:42.211717 pyrosimple-2.7.0/src/pyrosimple/scripts/base.py
--rw-r--r--   0        0        0    17685 2023-01-20 14:31:25.993111 pyrosimple-2.7.0/src/pyrosimple/scripts/chtor.py
--rw-r--r--   0        0        0     6605 2023-02-04 20:14:33.176453 pyrosimple-2.7.0/src/pyrosimple/scripts/lstor.py
--rw-r--r--   0        0        0     9754 2023-01-20 16:43:56.561457 pyrosimple-2.7.0/src/pyrosimple/scripts/mktor.py
--rw-r--r--   0        0        0    11595 2023-02-08 21:58:09.039159 pyrosimple-2.7.0/src/pyrosimple/scripts/pyroadmin.py
--rw-r--r--   0        0        0     9598 2023-02-09 21:38:39.940787 pyrosimple-2.7.0/src/pyrosimple/scripts/pyrotorque.py
--rw-r--r--   0        0        0    35333 2023-02-07 02:15:02.309145 pyrosimple-2.7.0/src/pyrosimple/scripts/rtcontrol.py
--rw-r--r--   0        0        0    10294 2023-02-05 16:02:43.027002 pyrosimple-2.7.0/src/pyrosimple/scripts/rtxmlrpc.py
--rw-r--r--   0        0        0      117 2022-12-19 17:11:41.447031 pyrosimple-2.7.0/src/pyrosimple/torrent/__init__.py
--rw-r--r--   0        0        0    29476 2023-01-29 21:08:43.079947 pyrosimple-2.7.0/src/pyrosimple/torrent/engine.py
--rw-r--r--   0        0        0    37192 2023-02-04 21:31:37.058381 pyrosimple-2.7.0/src/pyrosimple/torrent/rtorrent.py
--rw-r--r--   0        0        0      118 2022-12-19 17:11:41.447031 pyrosimple-2.7.0/src/pyrosimple/ui/__init__.py
--rw-r--r--   0        0        0     2903 2022-12-19 17:12:53.930262 pyrosimple-2.7.0/src/pyrosimple/ui/categories.py
--rw-r--r--   0        0        0      122 2022-12-19 17:11:41.447031 pyrosimple-2.7.0/src/pyrosimple/util/__init__.py
--rw-r--r--   0        0        0     2106 2022-12-29 14:05:43.470686 pyrosimple-2.7.0/src/pyrosimple/util/cache.py
--rw-r--r--   0        0        0     7891 2023-02-08 18:31:37.923717 pyrosimple-2.7.0/src/pyrosimple/util/fmt.py
--rw-r--r--   0        0        0      459 2022-12-19 17:11:41.447031 pyrosimple-2.7.0/src/pyrosimple/util/logutil.py
--rw-r--r--   0        0        0    29886 2023-02-08 21:50:48.130463 pyrosimple-2.7.0/src/pyrosimple/util/matching.py
--rw-r--r--   0        0        0    26410 2023-02-04 21:31:37.195048 pyrosimple-2.7.0/src/pyrosimple/util/metafile.py
--rw-r--r--   0        0        0     1999 2022-12-19 17:11:41.447031 pyrosimple-2.7.0/src/pyrosimple/util/pymagic.py
--rwxr-xr-x   0        0        0     9220 2023-01-13 20:57:44.004459 pyrosimple-2.7.0/src/pyrosimple/util/rpc.py
--rw-r--r--   0        0        0     8584 2022-12-19 17:11:41.447031 pyrosimple-2.7.0/src/pyrosimple/util/traits.py
--rw-r--r--   0        0        0     2187 2023-01-10 16:31:49.350547 pyrosimple-2.7.0/src/pyrosimple/util/ui.py
--rw-r--r--   0        0        0     4172 1970-01-01 00:00:00.000000 pyrosimple-2.7.0/setup.py
--rw-r--r--   0        0        0     4287 1970-01-01 00:00:00.000000 pyrosimple-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2131 2023-03-04 03:16:06.914134 pyrosimple-2.7.1/README.md
+-rw-r--r--   0        0        0     3349 2023-04-10 02:50:11.296848 pyrosimple-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0      538 2022-12-19 17:11:38.923701 pyrosimple-2.7.1/src/pyrosimple/__init__.py
+-rw-r--r--   0        0        0     8752 2023-03-04 03:16:46.423995 pyrosimple-2.7.1/src/pyrosimple/config.py
+-rw-r--r--   0        0        0       67 2023-02-28 18:23:01.538870 pyrosimple-2.7.1/src/pyrosimple/data/__init__.py
+-rw-r--r--   0        0        0    10194 2023-02-28 18:06:46.631474 pyrosimple-2.7.1/src/pyrosimple/data/full-example.rc
+-rw-r--r--   0        0        0     1273 2022-12-19 17:11:38.923701 pyrosimple-2.7.1/src/pyrosimple/error.py
+-rw-r--r--   0        0        0        0 2022-12-19 17:11:41.443698 pyrosimple-2.7.1/src/pyrosimple/io/__init__.py
+-rw-r--r--   0        0        0     8616 2023-04-02 15:39:14.262135 pyrosimple-2.7.1/src/pyrosimple/io/scgi.py
+-rw-r--r--   0        0        0        0 2022-12-19 17:11:41.443698 pyrosimple-2.7.1/src/pyrosimple/job/__init__.py
+-rw-r--r--   0        0        0     2963 2022-12-19 17:11:41.443698 pyrosimple-2.7.1/src/pyrosimple/job/action.py
+-rw-r--r--   0        0        0     2977 2022-12-29 19:15:58.212292 pyrosimple-2.7.1/src/pyrosimple/job/base.py
+-rw-r--r--   0        0        0     9444 2023-02-18 20:32:42.360835 pyrosimple-2.7.1/src/pyrosimple/job/metrics.py
+-rw-r--r--   0        0        0     1691 2023-02-04 21:14:43.625074 pyrosimple-2.7.1/src/pyrosimple/job/move_path.py
+-rw-r--r--   0        0        0     1743 2022-12-19 17:11:41.443698 pyrosimple-2.7.1/src/pyrosimple/job/move_torrent.py
+-rw-r--r--   0        0        0     4197 2023-01-22 17:54:55.278327 pyrosimple-2.7.1/src/pyrosimple/job/queue.py
+-rw-r--r--   0        0        0     9954 2023-03-28 00:31:31.950154 pyrosimple-2.7.1/src/pyrosimple/job/watch.py
+-rw-r--r--   0        0        0        0 2022-12-18 17:48:03.812685 pyrosimple-2.7.1/src/pyrosimple/py.typed
+-rw-r--r--   0        0        0      112 2023-01-15 15:15:41.811874 pyrosimple-2.7.1/src/pyrosimple/scripts/__init__.py
+-rw-r--r--   0        0        0     8190 2023-04-08 13:35:58.048768 pyrosimple-2.7.1/src/pyrosimple/scripts/base.py
+-rw-r--r--   0        0        0    17593 2023-04-08 13:23:16.125477 pyrosimple-2.7.1/src/pyrosimple/scripts/chtor.py
+-rw-r--r--   0        0        0     6590 2023-03-25 15:45:13.757347 pyrosimple-2.7.1/src/pyrosimple/scripts/lstor.py
+-rw-r--r--   0        0        0     9723 2023-03-27 23:30:07.160434 pyrosimple-2.7.1/src/pyrosimple/scripts/mktor.py
+-rw-r--r--   0        0        0    13634 2023-03-27 23:36:36.156689 pyrosimple-2.7.1/src/pyrosimple/scripts/pyroadmin.py
+-rw-r--r--   0        0        0     9555 2023-03-18 01:42:48.673745 pyrosimple-2.7.1/src/pyrosimple/scripts/pyrotorque.py
+-rw-r--r--   0        0        0    35338 2023-03-04 03:16:46.760660 pyrosimple-2.7.1/src/pyrosimple/scripts/rtcontrol.py
+-rw-r--r--   0        0        0    10294 2023-03-30 18:14:33.472926 pyrosimple-2.7.1/src/pyrosimple/scripts/rtxmlrpc.py
+-rw-r--r--   0        0        0      117 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/torrent/__init__.py
+-rw-r--r--   0        0        0    29545 2023-03-28 02:07:56.670430 pyrosimple-2.7.1/src/pyrosimple/torrent/engine.py
+-rw-r--r--   0        0        0    37489 2023-03-28 02:04:30.984695 pyrosimple-2.7.1/src/pyrosimple/torrent/rtorrent.py
+-rw-r--r--   0        0        0      118 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/ui/__init__.py
+-rw-r--r--   0        0        0     2903 2022-12-19 17:12:53.930262 pyrosimple-2.7.1/src/pyrosimple/ui/categories.py
+-rw-r--r--   0        0        0      122 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/util/__init__.py
+-rw-r--r--   0        0        0     2106 2022-12-29 14:05:43.470686 pyrosimple-2.7.1/src/pyrosimple/util/cache.py
+-rw-r--r--   0        0        0     7891 2023-02-08 18:31:37.923717 pyrosimple-2.7.1/src/pyrosimple/util/fmt.py
+-rw-r--r--   0        0        0      459 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/util/logutil.py
+-rw-r--r--   0        0        0    31824 2023-04-03 02:55:17.578411 pyrosimple-2.7.1/src/pyrosimple/util/matching.py
+-rw-r--r--   0        0        0    26411 2023-03-25 15:41:05.564729 pyrosimple-2.7.1/src/pyrosimple/util/metafile.py
+-rw-r--r--   0        0        0     1999 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/util/pymagic.py
+-rwxr-xr-x   0        0        0     9554 2023-04-02 15:37:53.245666 pyrosimple-2.7.1/src/pyrosimple/util/rpc.py
+-rw-r--r--   0        0        0     8584 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/util/traits.py
+-rw-r--r--   0        0        0     2187 2023-01-10 16:31:49.350547 pyrosimple-2.7.1/src/pyrosimple/util/ui.py
+-rw-r--r--   0        0        0     4166 1970-01-01 00:00:00.000000 pyrosimple-2.7.1/setup.py
+-rw-r--r--   0        0        0     4287 1970-01-01 00:00:00.000000 pyrosimple-2.7.1/PKG-INFO
```

### Comparing `pyrosimple-2.7.0/README.md` & `pyrosimple-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/pyproject.toml` & `pyrosimple-2.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyrosimple"
-version = "2.7.0"
+version = "2.7.1"
 description = "A stripped-down version of the pyrocore tools for working with rTorrent"
 authors = ["kannibalox <kannibalox@gmail.com>"]
 repository = "https://github.com/kannibalox/pyrosimple"
 documentation = "https://kannibalox.github.io/pyrosimple/"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 classifiers = [
@@ -29,15 +29,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<4"
 "bencode.py" = "^4.0.0"
 APScheduler = {version = "^3.9.0", optional = true}
 Jinja2 = "^3.1.0"
-python-daemon = "^2.3.0"
+python-daemon = "^3.0.1"
 importlib-resources = { version = "^5.4.0", python = "<3.9" }
 parsimonious = "^0.10.0"
 prometheus-client = "^0.16.0"
 prompt-toolkit = "^3.0.30"
 requests = "^2.28.1"
 shtab = "^1.5.5"
 inotify = {version = "^0.2.10", optional = true}
@@ -62,14 +62,15 @@
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.0.5"
 pylint = "^2.15.7"
 pytest = "^7.0.1"
 typing-extensions = "^4.1.1"
 black = "^23.1.0"
 isort = "^5.10.1"
+mypy = "^1.1.1"
 
 [tool.poetry.group.docs]
 optional = true
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.3.0"
 mkdocs-material = "^9.0.4"
 mkdocs-include-markdown-plugin = "^3.8.1"
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/__init__.py` & `pyrosimple-2.7.1/src/pyrosimple/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/config.py` & `pyrosimple-2.7.1/src/pyrosimple/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,16 @@
     except IndexError:
         return parts.netloc
 
 
 def load_custom_py():
     """Load custom python configuration.
 
-    This only gets called when CLI tools are called to prevent some weird code injection"""
+    This only gets called when CLI tools are called to prevent some weird code injection
+    """
     log = logging.getLogger(__name__)
     if not settings.CONFIG_PY:
         log.debug("Custom code loading is disabled")
     if settings.CONFIG_PY_LOADED:
         log.debug("Custom code has already been loaded")
     config_file = Path(settings.CONFIG_PY).expanduser()
     if config_file.exists():
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/data/full-example.rc` & `pyrosimple-2.7.1/src/pyrosimple/data/full-example.rc`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/error.py` & `pyrosimple-2.7.1/src/pyrosimple/error.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/io/scgi.py` & `pyrosimple-2.7.1/src/pyrosimple/io/scgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Handles RPC methods over various transports"""
 import io
 import logging
 import socket
 import subprocess
 import sys
 
-from typing import Dict, List, Tuple, Type
+from typing import Dict, List, Optional, Tuple, Type
 from urllib import parse as urlparse
 from urllib.error import URLError
 from xmlrpc import client as xmlrpclib
 
 from prometheus_client import Counter, Summary
 
 
@@ -112,15 +112,15 @@
         self.verbose = verbose
         target = urlparse.urlparse(self.url)
         with response_time_summary.time():
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
                 host, port = target.netloc.split(":")
                 sock.connect((host, int(port)))
                 sock.sendall(_encode_payload(request_body, self._headers))
-                with sock.makefile("rb") as handle:
+                with sock.makefile(mode="rb") as handle:
                     response = _parse_response(handle.read())[0]
         response_size_counter.inc(len(response))
         return self.parse_response(io.BytesIO(response))
 
 
 class UnixTransport(RTorrentTransport):
     """Transport via UNIX domain socket."""
@@ -129,16 +129,16 @@
         request_counter.inc()
         request_size_counter.inc(len(request_body))
         self.verbose = verbose
         target = urlparse.urlparse(self.url).path
         with response_time_summary.time():
             with socket.socket(socket.AF_UNIX, socket.SOCK_STREAM) as sock:
                 sock.connect(target)
-                sock.sendall(_encode_payload(request_body))
-                with sock.makefile("b") as handle:
+                sock.sendall(_encode_payload(request_body, self._headers))
+                with sock.makefile(mode="rb") as handle:
                     response = _parse_response(handle.read())[0]
         response_size_counter.inc(len(response))
         return self.parse_response(io.BytesIO(response))
 
 
 TRANSPORTS = {
     "scgi": TCPTransport,
@@ -184,15 +184,17 @@
 def _encode_headers(headers: List[Tuple[str, str]]) -> bytes:
     "Make SCGI header bytes from list of tuples."
     return b"".join(
         [b"%s\0%s\0" % (k.encode("ascii"), v.encode("ascii")) for k, v in headers]
     )
 
 
-def _encode_payload(data: bytes, headers: List[Tuple[str, str]] = None) -> bytes:
+def _encode_payload(
+    data: bytes, headers: Optional[List[Tuple[str, str]]] = None
+) -> bytes:
     "Wrap data in an SCGI request."
     prolog: bytes = b"CONTENT_LENGTH\0%d\0SCGI\x001\0" % len(data)
     if headers:
         prolog += _encode_headers(headers)
 
     return _encode_netstring(prolog) + data
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/job/action.py` & `pyrosimple-2.7.1/src/pyrosimple/job/action.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/job/base.py` & `pyrosimple-2.7.1/src/pyrosimple/job/base.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/job/metrics.py` & `pyrosimple-2.7.1/src/pyrosimple/job/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,15 @@
 
         TmpServer.address_family, addr = exposition._get_best_family(addr, port)
         app = exposition.make_wsgi_app(REGISTRY)
         # Hold onto the server class so that we can shut it down during cleanup
         self.httpd = exposition.make_server(
             addr, port, app, TmpServer, handler_class=exposition._SilentHandler
         )
-        t = Thread(target=self.httpd.serve_forever)
-        t.daemon = True
-        t.start()
+        Thread(target=self.httpd.serve_forever, daemon=True).start()
 
     def init_item(self) -> None:
         """Initialize item metrics"""
         for s in self.item_stats:
             self.add_metric(
                 s,
                 Gauge,
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/job/move_path.py` & `pyrosimple-2.7.1/src/pyrosimple/job/move_path.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/job/move_torrent.py` & `pyrosimple-2.7.1/src/pyrosimple/job/move_torrent.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/job/queue.py` & `pyrosimple-2.7.1/src/pyrosimple/job/queue.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/job/watch.py` & `pyrosimple-2.7.1/src/pyrosimple/job/watch.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -220,18 +220,14 @@
                     continue
                 metapath = Path(path, filename)
                 self.load_metafile(metapath)
             except Exception as exc:  # pylint: disable=broad-except
                 self.log.error("Could not load metafile from event %s: %s", event, exc)
 
 
-if __name__ == "__main__":
-    main()
-
-
 def main():
     """Show available templating values for a file"""
     # pylint: disable=import-outside-toplevel
     import logging
     import pprint
     import sys
 
@@ -246,7 +242,11 @@
     job = TreeWatch({"path": "/tmp", "start_immediately": False})
     logging.getLogger().setLevel(logging.INFO)
     job.log.info("Building template variables for '%s'", path)
     job.log.info(
         "Available variables: %s",
         pprint.pformat(job.build_metafile_variables(path, None)),
     )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/scripts/base.py` & `pyrosimple-2.7.1/src/pyrosimple/scripts/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 import os
 import signal
 import sys
 import textwrap
 import time
 import traceback
 
-from argparse import ArgumentParser, RawDescriptionHelpFormatter
+from argparse import ArgumentParser, Namespace, RawDescriptionHelpFormatter
 from typing import List, Optional
 
 import shtab
 
 from pyrosimple import error
 from pyrosimple.util import pymagic
 
 
 class ScriptBase:
     """Base class for command line interfaces."""
 
     # additonal stuff appended after the command handler's docstring
     ADDITIONAL_HELP: List[str] = []
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize CLI."""
         self.startup = time.time()
         # self.LOG exists only for backwards compatibility
         self.LOG = self.log = pymagic.get_class_logger(self)
 
-        self.args = None
-        self.options = None
+        self.args: Optional[List] = None
+        self.options = Namespace()
         self.return_code = 0
         self.engine = None
         self.intermixed_args = False
 
         logging.basicConfig(level=logging.WARNING)
         # For python 3.7 compatibility
         try:
@@ -51,14 +51,17 @@
         except ImportError:
             version = "unknown"
         implementation = sys.implementation.name
         if implementation == "cpython":
             implementation = "Python"
         version_info = f"{version} on {implementation} {sys.version.split()[0]}"
 
+        if getattr(self, "__doc__", None) is None:
+            self.__doc__ = ""
+
         self.parser = ArgumentParser(
             formatter_class=RawDescriptionHelpFormatter,
             description="%(prog)s "
             + version_info
             + "\n\n"
             + textwrap.dedent(self.__doc__.rstrip()).lstrip("\n")
             + "\n".join(self.ADDITIONAL_HELP)
@@ -137,15 +140,15 @@
         # Template method to add options of derived class
         self.add_options()
 
         if self.intermixed_args:
             self.options = self.parser.parse_intermixed_args(self.args)
         else:
             self.options = self.parser.parse_args(self.args)
-        self.args: Optional[List] = getattr(self.options, "args", None)
+        self.args = getattr(self.options, "args", None)
 
         if self.options.log_level:
             logging.getLogger("pyrosimple").setLevel(self.options.log_level)
 
         self.log.debug(
             "Options: %s",
             ", ".join("%s=%r" % i for i in sorted(vars(self.options).items())),
@@ -157,17 +160,18 @@
             self.log.fatal("%s (%s)", msg, exc)
             if logging.getLogger().isEnabledFor(logging.DEBUG):
                 return  # let the caller re-raise it
         else:
             self.log.fatal(msg)
         sys.exit(error.EX_SOFTWARE)
 
-    def run(self, args=None):
+    def run(self, args: Optional[List[str]] = None):
         """The main program skeleton."""
-        self.args = args
+        if args is not None:
+            self.args = args
         try:
             try:
                 # Preparation steps
                 self.get_options()
 
                 # Template method with the tool's main loop
                 self.mainloop()
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/scripts/chtor.py` & `pyrosimple-2.7.1/src/pyrosimple/scripts/chtor.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,30 +391,29 @@
                 # Set specific keys?
                 torrent.assign_fields(self.options.set)
                 replace_fields(torrent, self.options.regex)
 
                 # Write new metafile, if changed
 
                 if self.options.output_directory:
-                    filename = os.path.join(
+                    filename = Path(
                         self.options.output_directory, os.path.basename(filename)
                     )
                     self.log.info("Will write %r...", filename)
 
                     if not self.options.dry_run:
-                        with open(filename, "wb") as fh:
-                            fh.write(bencode.bencode(torrent))
+                        torrent.save(filename)
                         if "libtorrent_resume" in torrent:
                             # Also write clean version
                             filename = filename.replace(
                                 ".torrent", "-no-resume.torrent"
                             )
                             del torrent["libtorrent_resume"]
                             self.log.info("Writing '%s'...", filename)
-                            bencode.bwrite(torrent, filename)
+                            torrent.save(filename)
                 else:
                     current_torrent = metafile.Metafile.from_file(filename)
                     diff = diff_metafiles(current_torrent, torrent, filename)
                     if self.options.diff:
                         sys.stdout.writelines(diff)
                     if not diff:
                         self.log.info("No change to file %r", filename)
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/scripts/lstor.py` & `pyrosimple-2.7.1/src/pyrosimple/scripts/lstor.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,31 +93,30 @@
                     from pyrosimple.util.ui import HashProgressBar
 
                     with HashProgressBar() as pb:
                         if (
                             logging.getLogger().isEnabledFor(logging.WARNING)
                             and sys.stdout.isatty()
                         ):
-                            c = pb()
-                            progress_callback = c.progress_callback
+                            progress_callback = pb().progress_callback
                         else:
                             progress_callback = None
 
                         piece_logger = PieceLogger(torrent, self.log)
 
                         data_correct = torrent.hash_check(
                             Path(self.options.check_data),
                             progress_callback=progress_callback,
                             piece_callback=piece_logger.check_piece,
                         )
                     if not data_correct:
                         self.log.error(
-                            "File %s does match data from %s",
+                            "File %s does not match data in %s",
                             filename,
-                            self.options.check_data,
+                            Path(self.options.check_data).absolute(),
                         )
                         sys.exit(EX_DATAERR)
 
                 if self.options.raw:
                     from pyrosimple.util.fmt import (  # pylint: disable=import-outside-toplevel
                         BencodeJSONEncoder,
                     )
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/scripts/mktor.py` & `pyrosimple-2.7.1/src/pyrosimple/scripts/mktor.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
             "--hashed",
             "--fast-resume",
             help="create second metafile containing libtorrent fast-resume information",
         )
 
     # TODO: Optionally pass torrent directly to rTorrent (--load / --start)
     # TODO: Optionally limit disk I/O bandwidth used (incl. a config default!)
-    # TODO: Set "encoding" correctly
     # TODO: Support multi-tracker extension ("announce-list" field)
     # TODO: DHT "nodes" field?! [[str IP, int port], ...]
     # TODO: Web-seeding http://www.getright.com/seedtorrent.html
     #       field 'url-list': ['http://...'] on top-level
 
     def make_magnet_meta(self, magnet_url):
         """Create a magnet-url torrent."""
@@ -212,15 +211,15 @@
                     c.total = totalsize
                     c.items_completed = totalhashed
                     c.progress_bar.invalidate()
 
                 progress = pb_tracker
             else:
                 progress = None
-            # Create and metafile with the first announce as a placeholder
+            # Create a metafile with the first announce as a placeholder
             torrent = metafile.Metafile.from_path(
                 datapath,
                 self.args[1],
                 progress=progress,
                 root_name=self.options.root_name,
                 private=self.options.private,
                 created_by="PyroSimple",
@@ -234,21 +233,21 @@
             )
         torrent["created by"] = "PyroSimple"
         if self.options.comment:
             torrent["comment"] = self.options.comment
         if not self.options.no_date:
             torrent["creation date"] = int(time.time())
 
-        # If only one announce, just save to file
         for alias, announce in tracker_urls.items():
             torrent["announce"] = announce
             torrent["info"]["source"] = alias
             torrent["info"]["x_cross_seed"] = hashlib.md5(announce.encode()).hexdigest()
             torrent.assign_fields(self.options.set)
             if len(self.args) == 2:
+                # If only one announce, just save to file
                 save_metapath = metapath
             else:
                 save_metapath = Path(f"{alias}_{metapath}")
             self.log.info("Writing metafile %s...", save_metapath)
             torrent.save(save_metapath)
 
             # Create second metafile with fast-resume?
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/scripts/pyroadmin.py` & `pyrosimple-2.7.1/src/pyrosimple/scripts/pyroadmin.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import tomli_w
 
 import pyrosimple
 
 from pyrosimple import config
 from pyrosimple.scripts.base import ScriptBase
-from pyrosimple.util import matching
+from pyrosimple.util import matching, rpc
 
 
 class AdminTool(ScriptBase):
     """Support for administrative tasks."""
 
     # TODO: config create, dump, set, get
     # TODO: backup session/config
@@ -57,23 +57,24 @@
             help="Print changes instead of applying them",
             action="store_true",
         )
 
     def dump_rc(self):
         """Print a representative .rtorrent.rc as gleaned from a running instance.
 
-        This is neat but somewhat brittle, and behaves differently between XMLRPC and JSON-RPC."""
+        This is neat but somewhat brittle, and behaves differently between XMLRPC and JSON-RPC.
+        """
 
         proxy = pyrosimple.connect().open()
         methods = proxy.system.listMethods()
         # XXX This is a heuristic and might break in newer rTorrent versions!
         builtins = set(methods[: methods.index("view.sort_new") + 1])
         methods = set(methods)
         plain_re = re.compile(r"^[a-zA-Z0-9_.]+$")
-        RC_CONTINUATION_THRESHOLD = 50
+        rc_continuation_threshold = 50
 
         def is_method(name):
             "Helper"
             prefixes = (
                 "d.",
                 "f.",
                 "p.",
@@ -110,20 +111,19 @@
                             and text[1] == 0
                         ):
                             text = text[:1]
                 text = wrap_fmt % ", ".join(
                     [rc_quoted(x, in_brace=(wrap_fmt[0] == "{")) for x in text]
                 )
                 return text.replace("))))", ")) ))")
-            elif isinstance(text, int):
+            if isinstance(text, int):
                 return "(value, {:d})".format(text)
-            elif plain_re.match(text) or is_method(text):
+            if plain_re.match(text) or is_method(text):
                 return text
-            else:
-                return '"{}"'.format(text.replace("\\", "\\\\").replace('"', '\\"'))
+            return '"{}"'.format(text.replace("\\", "\\\\").replace('"', '\\"'))
 
         group = None
         for name in sorted(methods):
             try:
                 value = proxy.method.get("", name)
                 const = bool(proxy.method.const("", name))
             except xmlrpclib.Fault as exc:
@@ -142,15 +142,15 @@
                 value = [rc_quoted(x) for x in value]
                 wrap_fmt = "((%s))" if value and is_method(value[0]) else "{%s}"
                 definition = wrap_fmt % ", ".join(value)
             elif objtype is dict:
                 print("method.insert = {}, multi|rlookup|static".format(name))
                 for key, val in sorted(value.items()):
                     val = rc_quoted(val)
-                    if len(val) > RC_CONTINUATION_THRESHOLD:
+                    if len(val) > rc_continuation_threshold:
                         val = "\\\n    " + val
                     print('method.set_key = {}, "{}", {}'.format(name, key, val))
             elif objtype is str:
                 definition = rc_quoted(value)
             elif objtype is int:
                 definition = "{:d}".format(value)
             else:
@@ -163,15 +163,15 @@
                 if name in builtins:
                     print("{}.set = {}".format(name, definition))
                 else:
                     rctype = {str: "string", int: "value"}.get(objtype, "simple")
                     if const:
                         rctype += "|const"
                         const = None
-                    if len(definition) > RC_CONTINUATION_THRESHOLD:
+                    if len(definition) > rc_continuation_threshold:
                         definition = "\\\n    " + definition
                     definition = definition.replace(" ;     ", " ;\\\n     ").replace(
                         ",    ", ",\\\n    "
                     )
                     print("method.insert = {}, {}, {}".format(name, rctype, definition))
             if const:
                 print("method.const.enable = {}".format(name))
@@ -187,15 +187,15 @@
             )
         config.settings["FAST_QUERY"] = 0
         engine = pyrosimple.connect()
         engine.open()
         for i in engine.view("main", matching.create_matcher("loaded=0 metafile=/.+/")):
             try:
                 mtime = int(Path(i.metafile).stat().st_mtime)
-                if self.args.dry_run:
+                if self.options.dry_run:
                     dt = datetime.fromtimestamp(mtime)
                     self.log.info(
                         "Would set %s tm_loaded to %s from metafile %s",
                         i.hash,
                         dt,
                         i.metafile,
                     )
@@ -203,30 +203,30 @@
                     i.rpc_call("d.custom.set", ["tm_loaded", str(mtime)])
                     i.flush()
             except Exception as e:
                 self.log.error("Could not set tm_loaded for %s: %s", i.hash, e)
         for i in engine.view("main", matching.create_matcher("loaded=0 path=/.+/")):
             try:
                 mtime = int(Path(i.path).stat().st_mtime)
-                if self.args.dry_run:
+                if self.options.dry_run:
                     dt = datetime.fromtimestamp(mtime)
                     self.log.info(
                         "Would set %s tm_loaded to %s from path %s", i.hash, dt, i.path
                     )
                 else:
                     i.rpc_call("d.custom.set", ["tm_loaded", str(mtime)])
                     i.flush()
             except Exception as e:
                 self.log.error("Could not set tm_loaded for %s: %s", i.hash, e)
         for i in engine.view(
             "main", matching.create_matcher("completed=0 is_complete=yes path=/.+/")
         ):
             try:
                 mtime = int(Path(i.path).stat().st_mtime)
-                if self.args.dry_run:
+                if self.options.dry_run:
                     dt = datetime.fromtimestamp(mtime)
                     self.log.info(
                         "Would set %s tm_completed to %s from path %s",
                         i.hash,
                         dt,
                         i.path,
                     )
@@ -234,50 +234,56 @@
                     i.rpc_call("d.custom.set", ["tm_completed", str(mtime)])
                     i.flush()
             except Exception as e:
                 self.log.error("Could not set tm_loaded for %s: %s", i.hash, e)
 
     def create_config(self):
         """Create a configuration file"""
-        config_path = Path("~/.config/pyrosimple/config.toml").expanduser()
+        config_path = Path(config.settings.CONFIG)
         if config_path.exists():
             self.log.info(
                 "Pyrosimple config path %s already exists, not overwriting", config_path
             )
         else:
             self.log.info("Creating pyrosimple config file '%s'", config_path)
+            config_path.parent.mkdir(parents=True, exist_ok=True)
             with config_path.open("wb") as fh:
                 tomli_w.dump(pyrosimple.config.settings.to_dict(), fh)
 
     def create_rtorrent_rc(self):
         """Create a rtorrent.rc file"""
         rtorrent_rc_path = Path(pyrosimple.config.settings.RTORRENT_RC).expanduser()
         if rtorrent_rc_path.exists():
             self.log.info(
                 "rtorrent.rc path %s already exists, not overwriting", rtorrent_rc_path
             )
         else:
             self.log.info("Creating rtorrent.rc at '%s'", rtorrent_rc_path)
             home = str(Path("~").expanduser())
+            rtorrent_rc_path.parent.mkdir(parents=True, exist_ok=True)
             with rtorrent_rc_path.open("w", encoding="utf-8") as fh:
                 fh.write(
                     importlib.resources.open_text("pyrosimple.data", "full-example.rc")
                     .read()
                     .replace("/home/USERNAME", home)
                 )
 
     def config(self):
         """Handle the config subcommand"""
-        if self.args.dump_rc:
+        if self.options.dump_rc:
             self.dump_rc()
-        if self.args.create_config:
+        if self.options.create_config:
             self.create_config()
-        if self.args.create_rtorrent_rc:
+        if self.options.create_rtorrent_rc:
             self.create_rtorrent_rc()
-        if self.args.check:
+        if self.options.check:
+            if self.options.url:
+                config.settings["SCGI_URL"] = config.lookup_connection_alias(
+                    self.options.url
+                )
             try:
                 config.autoload_scgi_url()
             except Exception:
                 self.log.error("Error loading SCGI URL:")
                 raise
             self.log.debug("Loaded SCGI URL successfully")
             try:
@@ -285,21 +291,64 @@
             except ConnectionRefusedError:
                 self.log.error(
                     "SCGI URL '%s' found, but rTorrent may not be running!",
                     config.autoload_scgi_url(),
                 )
                 raise
             self.log.info("Connected to rTorrent successfully")
+            self.config_check_timestamps()
+
+    def config_check_timestamps(self):
+        """Confirm usual methods for timestamps exist"""
+        proxy = pyrosimple.connect().open()
+        event_field_map = {
+            "event.download.resumed": "started",
+            "event.download.finished": "completed",
+            "event.download.inserted_new": "loaded",
+        }
+        print_timestamp_help = False
+        for event, field in event_field_map.items():
+            if "!time_stamp" not in proxy.method.get("", event):
+                self.log.warning(
+                    "Method '!time_stamp' not found in '%s', field '%s' may not function correctly",
+                    event,
+                    field,
+                )
+                print_timestamp_help = True
+        try:
+            proxy.method.get("", "pyro.last_xfer.min_rate")
+        except rpc.RpcError as exc:
+            if exc.faultCode in [-32602, -503]:
+                self.log.warning(
+                    "Method 'pyro.last_xfer.min_rate' not found, field 'last_xfer' may not function correctly"
+                )
+                print_timestamp_help = True
+            else:
+                raise
+        try:
+            proxy.method.get("", "d.timestamp.last_active")
+        except rpc.RpcError as exc:
+            if exc.faultCode in [-32602, -503]:
+                self.log.warning(
+                    "Method 'd.timestamp.last_active' not found, field 'last_active' may not function correctly"
+                )
+                print_timestamp_help = True
+            else:
+                raise
+
+        if print_timestamp_help:
+            self.log.warning(
+                "To configure timestamp fields, see https://kannibalox.github.io/pyrosimple/rtorrent-config/#timestamps"
+            )
 
     def mainloop(self):
-        self.args = self.parser.parse_args()
-        if self.args.func is None:
+        if self.options.func is None:
             self.parser.print_help()
             return
-        self.args.func()
+        self.options.func()
 
 
 def run():  # pragma: no cover
     """The entry point."""
     AdminTool().run()
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/scripts/pyrotorque.py` & `pyrosimple-2.7.1/src/pyrosimple/scripts/pyrotorque.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,14 @@
                 self.sched.add_job(
                     self.classes[name].run,
                     name=name,
                     id=name,
                     trigger="cron",
                     **params["schedule"],
                 )
-                print(self.jobs[name])
 
     def unload_jobs(self):
         """Allows jobs classes to clean up any global resources if the
         cleanup() method exists.
 
         This should be called only once the jobs have finished
         running, so that a successive run doesn't re-create the
@@ -142,15 +141,15 @@
                 self.validate_config()
                 self.sched.pause()
                 self.sched.remove_all_jobs()
                 self.unload_jobs()
                 self.sched.resume()
                 self.add_jobs()
                 self.running_config = dict(config.settings.TORQUE)
-        except (Exception) as exc:  # pylint: disable=broad-except
+        except Exception as exc:  # pylint: disable=broad-except
             self.log.error("Error while reloading config: %s", exc)
         else:
             self.sched.resume()
 
     def run_forever(self):
         """Run configured jobs until termination request."""
         self.running_config = dict(config.settings.TORQUE)
@@ -169,15 +168,15 @@
                 self.log.info("System exit (RC=%r)", self.return_code)
                 break
 
     def mainloop(self):
         """The main loop."""
         try:
             self.validate_config()
-        except (error.ConfigurationError) as exc:
+        except error.ConfigurationError as exc:
             self.fatal(exc)
 
         # Defaults for process control paths
         if not self.options.pid_file:
             self.options.pid_file = TimeoutPIDLockFile(
                 Path(self.RUNTIME_DIR, "pyrotorque.pid").expanduser()
             )
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/scripts/rtcontrol.py` & `pyrosimple-2.7.1/src/pyrosimple/scripts/rtcontrol.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,16 @@
         return result
 
 
 class RtorrentAction(argparse.Action):
     """This class is used by the argparse action parameter for adding rtcontrol actions to a master list in the namespace.
 
     There is a rather unfortunate name collision between argparse's actions and rtcontrol's actions.
-    'const' is used as the method name to call, with the arguments being pulled from the value"""
+    'const' is used as the method name to call, with the arguments being pulled from the value
+    """
 
     def __init__(self, option_strings, dest, nargs=None, **kwargs):
         """Build the action, default to 1 narg since that's the most common"""
         if nargs is None:
             nargs = 1
         if "const" not in kwargs:
             kwargs["const"] = option_strings[0].lstrip("-").replace("-", "_")
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/scripts/rtxmlrpc.py` & `pyrosimple-2.7.1/src/pyrosimple/scripts/rtxmlrpc.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/torrent/engine.py` & `pyrosimple-2.7.1/src/pyrosimple/torrent/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import time
 import warnings
 
 from typing import Callable, Dict, Optional, Set, cast
 
 from pyrosimple import config, error
 from pyrosimple.util import fmt, matching, metafile, rpc, traits
+from pyrosimple.util.cache import ExpiringCache
 
 
 logger = logging.getLogger(__name__)
 
 
 def untyped(val):
     """A type specifier for fields that does nothing."""
@@ -269,15 +270,15 @@
         name,
         doc,
         accessor=None,
         matcher=None,
         formatter=None,
         requires=None,
         prefilter_field=None,
-        setter: Callable = None,
+        setter: Optional[Callable] = None,
     ):
         super().__init__(
             valtype, name, doc, accessor, matcher, formatter, requires, prefilter_field
         )
         self._setter = setter
 
     def __set__(self, obj, val, cls=None):
@@ -895,15 +896,15 @@
             "p_": generate_sub_multicall("p"),
             "t_": generate_sub_multicall("t"),
         }.items():
             cls.add_field_generator(prefix, generator)
 
     def __init__(self):
         """Initialize object."""
-        self._fields = {}
+        self._fields = ExpiringCache()
 
     def __hash__(self):
         """Make item hashable for Python."""
         return self.hash
 
     def __eq__(self, other):
         """Compare items based on their infohash."""
@@ -951,15 +952,15 @@
     def _fetch_items(self):
         """Fetch to attribute."""
         if self._items is None:
             self._items = list(self.engine.items(self))
 
         return self._items
 
-    def _check_hash_view(self) -> Optional[str]:
+    def check_hash_view(self) -> Optional[str]:
         """Return infohash if view name refers to a single item, else None."""
         infohash = None
         if self.viewname.startswith("#"):
             infohash = self.viewname[1:]
         elif len(self.viewname) == 40:
             try:
                 int(self.viewname, 16)
@@ -967,15 +968,15 @@
                 pass
             else:
                 infohash = str(self.viewname)
         return infohash
 
     def size(self) -> int:
         """Total unfiltered size of view."""
-        if self._check_hash_view():
+        if self.check_hash_view():
             return 1
         return int(self.engine.open().view.size(rpc.NOHASH, self.viewname))
 
     def items(self):
         """Get list of download items."""
         if self.matcher:
             for item in self._fetch_items():
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/torrent/rtorrent.py` & `pyrosimple-2.7.1/src/pyrosimple/torrent/rtorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,14 +415,16 @@
         if self._engine.has_method("d.custom.keys"):
             custom_fields = {}
             for key in proxy.d.custom.keys(self.hash):
                 custom_fields[key] = proxy.d.custom(self.hash, key)
             return custom_fields
         proxy.d.save_full_session(self.hash)
         info_file = Path(proxy.session.path(), f"{self.hash}.torrent.rtorrent")
+        if info_file.exists():
+            return dict(bencode.decode(info_file.read_bytes())["custom"])
         return dict(
             bencode.decode(proxy.execute.capture(rpc.NOHASH, "cat", info_file))[
                 "custom"
             ]
         )
 
     def move(self, dest: os.PathLike, move_func: Optional[Callable] = None):
@@ -515,36 +517,38 @@
 
         remote_proxy.d.start(self.hash)
         if not copy:
             proxy.d.erase(self.hash)
             self._fields.clear()
         return True
 
-    def delete(self):
+    def delete(self) -> None:
         """Remove torrent from client."""
         self.stop()
         tied_file = self.rpc_call("d.tied_to_file")
         if tied_file:
             self._make_it_so("removing metafile of", ["d.delete_tied"])
         self._make_it_so("erasing", ["d.erase"])
 
     # TODO: def set_files_priority(self, pattern, prio)
     # Set priority of selected files
     # NOTE: need to call d.update_priorities after f.priority.set!
 
-    def purge(self):
+    def purge(self) -> None:
         """Delete PARTIAL data files and remove torrent from client."""
 
         def partial_file(item):
             "Filter out partial files"
             return item.completed_chunks < item.size_chunks
 
         self.cull(file_filter=partial_file, attrs=["completed_chunks", "size_chunks"])
 
-    def cull(self, file_filter: Optional[Callable] = None, attrs: List[str] = None):
+    def cull(
+        self, file_filter: Optional[Callable] = None, attrs: Optional[List[str]] = None
+    ):
         """Delete ALL data files and remove torrent from client.
 
         @param file_filter: Optional callable for selecting a subset of all files.
             The callable gets a file item as described for RtorrentItem._get_files
             and must return True for items eligible for deletion.
         @param attrs: Optional list of additional attributes to fetch (for
             file_filter to use).
@@ -578,15 +582,15 @@
                 if e.errno != errno.ENOTEMPTY:
                     raise
 
         # Delete item from engine
         if not dry_run:
             self.delete()
 
-    def flush(self):
+    def flush(self) -> None:
         """Write volatile data to disk."""
         self._make_it_so("saving session data of", ["d.save_resume"])
 
 
 class RtorrentEngine:
     """The rTorrent backend proxy."""
 
@@ -623,52 +627,49 @@
         "d.is_open",
         "d.message",
         "d.ratio",
         "d.up.rate",
         "d.up.total",
     }
 
-    def __init__(self, url=None, auto_open=False):
+    def __init__(self, url: Optional[str] = None, auto_open: bool = False):
         """Initialize proxy."""
         self.logger = pymagic.get_class_logger(self)
         self.engine_id = "N/A"  # ID of the instance we're connecting to
         self.engine_software = "rTorrent"  # Name and version of software
         self.startup = time.time()
-        self.rpc = None
-        self.properties = {}
+        self.properties: Dict[str, str] = {}
         self.known_throttle_names = {"", "NULL"}
         self.url: str
         if url is None:
             config.autoload_scgi_url()
             self.url = config.settings.SCGI_URL
         else:
             self.url = url
+        if not self.url:
+            raise error.UserError(
+                "You need to configure a RPC connection, read"
+                " https://kannibalox.github.io/pyrosimple/configuration/#top-level-section"
+            )
+        self.rpc = rpc.RTorrentProxy(self.url)
         if auto_open:
             self.open()
 
     def view(self, viewname="default", matcher=None):
         """Get list of download items."""
         return engine.TorrentView(self, viewname, matcher)
 
     def __repr__(self):
         """Return a representation of internal state."""
+        name = self.__class__.__name__
         if self.rpc:
             # Connected state
-            return "{} connected to {} [{}, up {}] via {!r}".format(
-                self.__class__.__name__,
-                self.engine_id,
-                self.engine_software,
-                fmt.human_duration(self.uptime, 0, 2, True).strip(),
-                self.url,
-            )
+            return f"{name} connected to {self.engine_id} [{self.engine_software}] via {self.url!r}"
         # Unconnected state
-        return "{} connectable via {!r}".format(
-            self.__class__.__name__,
-            self.url,
-        )
+        return f"{self.__class__.__name__} connectable via {self.url!r}"
 
     @property
     def uptime(self):
         """rTorrent's uptime."""
         return time.time() - self.startup
 
     def _resolve_viewname(self, viewname: str) -> str:
@@ -688,47 +689,41 @@
         for method, params in methods.items():
             call.append({"methodName": method, "params": params})
         for index, r in enumerate(self.rpc.system.multicall(call)):
             results[list(methods.keys())[index]] = r[0]
         return results
 
     @lru_cache(maxsize=32)
-    def has_method(self, method_name: str):
+    def has_method(self, method_name: str) -> bool:
         """Cached check to see if method exists"""
         if method_name in self.rpc.system.listMethods():
             return True
         return False
 
-    def open(self):
+    def open(self) -> rpc.RTorrentProxy:
         """Open connection."""
-        # Only connect once
-        if self.rpc is not None:
+        # Avoid scraping properties twice
+        if self.properties:
             return self.rpc
 
         # Reading abilities are on the downfall, so...
-        if not self.url:
-            raise error.UserError(
-                "You need to configure a RPC connection, read"
-                " https://kannibalox.github.io/pyrosimple/configuration/#top-level-section"
-            )
 
         # Connect and get instance ID (also ensures we're connectable)
-        self.rpc = rpc.RTorrentProxy(self.url)
         self.properties = self.system_multicall(
             {
                 "system.client_version": [],
                 "system.library_version": [],
                 "system.time_usec": [],
                 "session.name": [],
                 "directory.default": [],
                 "session.path": [],
             }
         )
         self.engine_id = self.properties["session.name"]
-        time_usec = self.properties["system.time_usec"]
+        time_usec = float(self.properties["system.time_usec"])
 
         # Make sure xmlrpc-c works as expected
         if time_usec < 2**32:
             self.logger.warning(
                 "Unsupported xmlrpc-c version (64 bit integer support missing,"
                 " %r returned instead)",
                 type(time_usec),
@@ -793,26 +788,30 @@
         items = []
         multi_args: List
         try:
             # Prepare multi-call arguments
             args = sorted(prefetch)
 
             # Check if view is in the format of a single hash
-            infohash = view._check_hash_view()
+            infohash = view.check_hash_view()
             if infohash:
                 multi_call = self.open().system.multicall
                 multi_args = [
                     {
                         "methodName": field.rsplit("=", 1)[0],
                         "params": [infohash]
                         + (field.rsplit("=", 1)[1].split(",") if "=" in field else []),
                     }
                     for field in args
                 ]
-                raw_items = [[i[0] for i in multi_call(multi_args)]]
+                multi_resp = multi_call(multi_args)
+                if any("faultCode" in r for r in multi_resp):
+                    uniq_errors = {str(r) for r in multi_resp if "faultCode" in r}
+                    raise rpc.RpcError(f"Errors in system.multicall: {uniq_errors}")
+                raw_items = [[i[0] for i in multi_resp]]
             # Otherwise prepare a multicall as expected
             else:
                 multi_call = self.open().d.multicall2
                 multi_args = ["", view.viewname] + [
                     field if "=" in field else field + "=" for field in args
                 ]
                 if view.matcher and int(config.settings.get("FAST_QUERY")) > 0:
@@ -929,15 +928,15 @@
     variables.update(namespace)
     # Expand template
     return template.render(**variables)
 
 
 def format_item_str(
     template_str: str, item: Union[Dict, str, RtorrentItem], defaults=None
-):
+) -> str:
     """Simple helper function to format a string with an item"""
     template = env.from_string(template_str)
     return format_item(template, item, defaults)
 
 
 def format_item(
     template: jinja2.Template,
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/ui/categories.py` & `pyrosimple-2.7.1/src/pyrosimple/ui/categories.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/util/cache.py` & `pyrosimple-2.7.1/src/pyrosimple/util/cache.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/util/fmt.py` & `pyrosimple-2.7.1/src/pyrosimple/util/fmt.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/util/matching.py` & `pyrosimple-2.7.1/src/pyrosimple/util/matching.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     "gt": FilterOperator("gt", ">"),
     "lt": FilterOperator("lt", "<"),
     "ge": FilterOperator("ge", ">="),
     "le": FilterOperator("le", "<="),
 }
 
 
-def truth(val, context="statement") -> bool:
+def truth(val: Any, context="statement") -> bool:
     """Convert truth value in "val" to a boolean."""
     # Try coercing it to an int then a bool
     try:
         return bool(0 + val)
     except TypeError:
         pass
 
@@ -77,14 +77,28 @@
         return False
 
     raise FilterError(
         f"Bad boolean value {val!r} in {context!r} (expected one of '{TRUE}', or '{FALSE}')"
     )
 
 
+TIMEDELTA_UNITS = {
+    "y": lambda d: d * 365 * 86400,
+    "M": lambda d: d * 30 * 86400,
+    "w": lambda d: d * 7 * 86400,
+    "d": lambda d: d * 86400,
+    "h": lambda d: d * 3600,
+    "m": lambda d: d * 60,
+    "s": lambda d: d,
+}
+TIMEDELTA_RE = re.compile(
+    "^" + "".join(r"(?:(?P<{0}>\d+)[{0}{0}])?".format(i) for i in "yMwdhms") + "$"
+)
+
+
 def unquote_pre_filter(
     pre_filter: str, regex_: re.Pattern = re.compile(r"[\\]+")
 ) -> str:
     """Unquote a pre-filter condition."""
     if pre_filter.startswith('"') and pre_filter.endswith('"'):
         # Unquote outer level
         pre_filter = pre_filter[1:-1]
@@ -281,22 +295,22 @@
 class PatternFilter(FieldFilter):
     """Pattern filter, either a glob or a /regex/ pattern."""
 
     CLEAN_PRE_VAL_RE = re.compile(r"(?:\[.*?\])|(?:\(.*?\))|(?:{.*?})|(?:\\)")
     SPLIT_PRE_VAL_RE = re.compile(r"[^a-zA-Z0-9/_]+")
     SPLIT_PRE_GLOB_RE = re.compile(r"[?*]+")
 
-    def validate(self):
+    def validate(self) -> None:
         """Validate filter condition (template method)."""
 
         super().validate()
         self._value: str = self._value
         self._template = None
         self._flags = 0
-        self._matcher: Callable[Any, Any]
+        self._matcher: Callable[[str, Any], bool]
         if (
             self._value == '""'
         ):  # Replace an empty string with a simple truthiness check
             self._matcher = lambda val, _: val == ""
         elif self._value.startswith("/") and (
             self._value.endswith("/") or self._value.endswith("/i")
         ):
@@ -307,25 +321,27 @@
                 self._matcher = lambda val, __: bool(val)
             else:
                 value = self._value
                 if self._value.endswith("/i"):
                     self._flags = re.IGNORECASE
                     value = self._value.rstrip("i")
                 regex = re.compile(value[1:-1], self._flags)
-                self._matcher = lambda val, _: regex.search(val)
+                self._matcher = lambda val, _: bool(regex.search(val))
         elif self._value.startswith("{{") or self._value.endswith("}}"):
+            self._template = self._value
 
-            def _template_globber(val, item):
+            def _template_globber(val, item) -> bool:
                 """Helper method to allow templating a glob."""
-                pattern = torrent.rtorrent.format_item(
-                    torrent.rtorrent.env.from_string(self._template), item
-                )
-                return fnmatch.fnmatchcase(val, pattern)
+                if self._template is not None:
+                    pattern = torrent.rtorrent.format_item(
+                        torrent.rtorrent.env.from_string(self._template), item
+                    )
+                    return fnmatch.fnmatchcase(val, pattern)
+                return False
 
-            self._template = self._value
             self._matcher = _template_globber
         else:
             # Pick out a glob that can be simplified
             if self._value == "*":
                 self._matcher = lambda _, __: True
             else:
                 self._matcher = lambda val, _: fnmatch.fnmatchcase(val, self._value)
@@ -359,15 +375,15 @@
         if needle:
             # Skip trying to filter on non-ASCII characters
             try:
                 needle.encode("ascii")
             except UnicodeEncodeError:
                 return ""
             needle = needle.replace('"', r"\\\"")
-            return r'"string.contains_i=${},\"{}\""'.format(pf, needle)
+            return rf'"string.contains_i=${pf},\"{needle}\""'
 
         return ""
 
     def eq(self, item):
         """Return True if filter matches item."""
         val = getattr(item, self._name) or ""
         result = self._matcher(val, item)
@@ -400,17 +416,16 @@
         """Return rTorrent condition to speed up data transfer."""
         pf = prefilter_field_lookup(self._name)
         if pf is not None:
             if self._exact and not self._value:
                 return f'"equal={pf},cat="'
             if not self._value:
                 return f'"not=${pf}"'
-            return r'"string.contains_i=${},\"{}\""'.format(
-                pf, self._value.replace('"', r"\\\"")
-            )
+            needle = self._value.replace('"', r"\\\"")
+            return rf'"string.contains_i=${pf},\"{needle}\""'
         return ""
 
     def validate(self):
         """Validate filter condition (template method)."""
         super().validate()
         self._value = self._value.lower()
 
@@ -466,15 +481,15 @@
     def match(self, item) -> bool:
         """Return True if filter matches item."""
         val = getattr(item, self._name) or 0
         if self.not_null and self._value and not val:
             return False
         # Grab the function from the native operator module
         op = getattr(operator, self._op.name)
-        return bool(op(float(val), self._value))
+        return bool(op(float(val), float(self._value)))
 
 
 def prefilter_field_lookup(name: str) -> Optional[str]:
     """Return the prefield field for a given name (if available)"""
     field = torrent.engine.field_lookup(name)
     if field is None:
         return None
@@ -493,15 +508,15 @@
 
         rTorrent doesn't actually have floats, so we need to do a
         little translation for the prefiltering
         """
         pf = prefilter_field_lookup(self._name)
         if pf is None:
             return ""
-        val = self._value * self.FIELD_SCALE.get(self._name, 1)
+        val = int(self._value) * self.FIELD_SCALE.get(self._name, 1)
         lookup_table = {
             "eq": ("equal", int(val)),
             "ge": ("greater", math.floor(val - 1)),
             "gt": ("greater", math.floor(val)),
             "le": ("less", math.ceil(val + 1)),
             "lt": ("less", math.ceil(val)),
         }
@@ -534,158 +549,205 @@
     }
     TIMEDELTA_RE = re.compile(
         "^" + "".join(r"(?:(?P<{0}>\d+)[{0}{0}])?".format(i) for i in "yMwdhms") + "$"
     )
 
     # pylint: disable=super-init-not-called
     def __init__(self, name: str, op: FilterOperator, value: str):
-        self.children = []
-        self._name = name
-        self.not_null = False
-        self._condition = value
-        self._op: FilterOperator = op
-        self._duration = False
-        self._flipped = False
+        # During validate(), one of these two must be set to something
+        # non-None
+        self._timestamp_offset = None
+        self._timestamp = None
+        super().__init__(name, op, value)
 
     def pre_filter(self) -> str:
         """Return rTorrent condition to speed up data transfer."""
         # A "0" might indicate just that, or possibly an empty
         # custom value.
         if self._value == 0:
             return ""
         pf = prefilter_field_lookup(self._name)
-        if pf is not None:
-            if not self._duration:
-                return ""
-            # Adding a day of fuzz to avoid any possible timezone problems
-            if self._op.name == "gt":
-                timestamp = float(self._value) + 86400
-                cmp_ = "greater"
-            elif self._op.name == "lt":
-                timestamp = float(self._value) - 86400
-                cmp_ = "less"
-            elif self._op.name == "eq":
-                timestamp = 0
-                cmp_ = "equal"
-            else:
-                return ""
-            timestamp = float(self._value) + (
-                -86400
-                if self._op.name == "gt"
-                else 86400
-                if self._op.name == "lt"
-                else 0
-            )
+        # Add a day of wiggle room to avoid any possible timezone problems
+        time_fuzz = 60 * 60 * 24
+        timestamp = 0
+        cmp_ = ""
+        if pf is None:
+            return ""
+        if self._op.name in ["gt", "ge"]:
+            timestamp = int(float(self._value)) - time_fuzz
+            cmp_ = "greater"
+        elif self._op.name in ["lt", "le"]:
+            timestamp = int(float(self._value)) + time_fuzz
+            cmp_ = "less"
 
+        if timestamp and cmp_:
             return '"{}=value=${},value={}"'.format(cmp_, pf, int(timestamp))
         return ""
 
+    def validate(self):
+        # 0 is a special case
+        delta = self._parse_delta()
+        if delta is not None:
+            self._timestamp_offset = delta
+            # Invert the operators to be more intuitive, i.e. <3d
+            # should match for values of less than 3 days *ago*.
+            self._invert_operator()
+            return
+        self._timestamp = self._parse_absolute_timestamp()
+        if self._timestamp is None:
+            raise ValueError(f"Could not parse timestamp {self._condition!r}")
+
     @property
-    def _value(self):
-        timestamp = now = time.time()
+    def _value(self) -> str:
+        if self._timestamp_offset is not None:
+            return str(time.time() - self._timestamp_offset)
+        if self._timestamp is not None:
+            return str(self._timestamp)
+        raise ValueError(f"Unset time value from condition {self._condition!r}")
+
+    @_value.setter
+    def _value(self, _: str) -> None:
+        """Discard attempts to set the value, primarily because the
+        grandparent FieldFilter tries to do it in __init__()"""
+        return None
+
+    def _invert_operator(self):
+        if self._op.name == "gt":
+            self._op = Operators["le"]
+        elif self._op.name == "ge":
+            self._op = Operators["lt"]
+        elif self._op.name == "lt":
+            self._op = Operators["ge"]
+        elif self._op.name == "le":
+            self._op = Operators["gt"]
+
+    def _parse_delta(self) -> Optional[int]:
+        match = self.TIMEDELTA_RE.match(self._condition)
+        if not match:
+            return None
+        delta_val = 0
+        for unit, val in match.groupdict().items():
+            if val:
+                delta_val = self.TIMEDELTA_UNITS[unit](int(val, 10))
+        return delta_val
 
+    def _parse_absolute_timestamp(self) -> Optional[int]:
         if str(self._condition).isdigit():
             # Literal UNIX timestamp
             try:
-                timestamp = float(self._condition)
+                return int(self._condition)
             except (ValueError, TypeError) as exc:
                 raise FilterError(
-                    f"Bad timestamp value {self._condition!r} in {self._condition!r}"
+                    f"Bad UNIX timestamp value {self._condition!r}"
                 ) from exc
+        # Assume it's an absolute date
+        if "/" in self._condition:
+            # U.S.
+            dtfmt = "%m/%d/%Y"
+        elif "." in self._condition:
+            # European
+            dtfmt = "%d.%m.%Y"
         else:
-            # Something human readable
-            delta = self.TIMEDELTA_RE.match(self._condition)
-            if delta:
-                # Time delta
-                for unit, val in delta.groupdict().items():
-                    if val:
-                        delta_val = self.TIMEDELTA_UNITS[unit](int(val, 10))
-
-                if self._duration:
-                    timestamp = delta_val
-                else:
-                    # Invert the value for more intuitive matching (in
-                    # line with original code too) e.g. 'completed<1d'
-                    # should return things completed less than one day
-                    # *ago*. It needs to be guarded like this since
-                    # the property will be called multiple times
-                    # during the course of a run.
-                    if not self._flipped:
-                        if self._op.name == "gt":
-                            self._op = Operators["le"]
-                        elif self._op.name == "ge":
-                            self._op = Operators["lt"]
-                        elif self._op.name == "lt":
-                            self._op = Operators["ge"]
-                        elif self._op.name == "le":
-                            self._op = Operators["gt"]
-                        self._flipped = True
-                    timestamp = now - delta_val
-            else:
-                # Assume it's an absolute date
-                if "/" in self._condition:
-                    # U.S.
-                    dtfmt = "%m/%d/%Y"
-                elif "." in self._condition:
-                    # European
-                    dtfmt = "%d.%m.%Y"
-                else:
-                    # Fall back to ISO
-                    dtfmt = "%Y-%m-%d"
-
-                val = str(self._condition).upper().replace(" ", "T")
-                if "T" in val:
-                    # Time also given
-                    dtfmt += "T%H:%M:%S"[: 3 + 3 * val.count(":")]
-
-                try:
-                    timestamp = time.mktime(tuple(time.strptime(val, dtfmt)))
-                except (ValueError) as exc:
-                    raise FilterError(
-                        f"Bad timestamp value {self._condition!r} in {self._condition!r} ({exc})"
-                    ) from exc
-
-                if self._duration:
-                    timestamp -= now
-        return timestamp
+            # Fall back to ISO
+            dtfmt = "%Y-%m-%d"
 
-    def validate(self):
-        """Validate filter condition (template method)."""
-        self._value  # pylint: disable=pointless-statement
+        val = str(self._condition).upper().replace(" ", "T")
+        if "T" in val:
+            # Time also given
+            dtfmt += "T%H:%M:%S"[: 3 + 3 * val.count(":")]
+
+        try:
+            timestamp = time.mktime(time.strptime(val, dtfmt))
+        except ValueError as exc:
+            raise FilterError(
+                f"Could not parse timestamp {self._condition!r} with format {dtfmt!r}"
+            ) from exc
+        return int(timestamp)
 
 
 class TimeFilterNotNull(TimeFilter):
     """Filter UNIX timestamp values, ignore unset values unless compared to 0."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.not_null = True
-        self._duration = False
 
 
 class DurationFilter(TimeFilter):
     """Filter durations in seconds."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.not_null = True
-        self._duration = True
+
+    @property
+    def _value(self):
+        if self._condition == "0":
+            return 0
+        if self._timestamp_offset is not None:
+            return self._timestamp_offset
+        if self._timestamp is not None:
+            return time.time() - self._timestamp
+        raise ValueError(f"Unset time value from condition {self._condition!r}")
+
+    @_value.setter
+    def _value(self, _):
+        """Discard attempts to set the value, primarily because the
+        grandparent FieldFilter tries to do it in __init__()"""
+        return None
+
+    def validate(self):
+        # 0 is a special case
+        if self._condition == "0":
+            return
+        delta = self._parse_delta()
+        if delta is not None:
+            self._timestamp_offset = delta
+            return
+        self._timestamp = self._parse_absolute_timestamp()
+        if self._timestamp is None:
+            raise ValueError(f"Could not parse timestamp {self._condition!r}")
 
     def match(self, item) -> bool:
         """Return True if filter matches item."""
         if getattr(item, self._name) is None:
             # Never match "N/A" items, except when "-0" was specified
             return not bool(self._value)
         return super().match(item)
 
+    def pre_filter(self) -> str:
+        """Return rTorrent condition to speed up data transfer."""
+        # A "0" might indicate just that, or possibly an empty
+        # custom value.
+        if self._value == 0:
+            return ""
+        pf = prefilter_field_lookup(self._name)
+        time_fuzz = (
+            60 * 60 * 24
+        )  # Add a day of wiggle room to avoid any possible timezone problems
+        timestamp = 0
+        cmp_ = ""
+        if pf is None:
+            return ""
+        if self._op.name in ["gt", "ge"]:
+            timestamp = self._value + time_fuzz
+            cmp_ = "greater"
+        elif self._op.name in ["lt", "le"]:
+            timestamp = self._value - time_fuzz
+            cmp_ = "less"
+
+        if timestamp and cmp_:
+            return '"{}=value=${},value={}"'.format(cmp_, pf, int(timestamp))
+        return ""
+
 
 class ByteSizeFilter(NumericFilterBase):
     """Filter size and bandwidth values."""
 
-    UNITS = {"b": 1, "k": 1024, "m": 1024**2, "g": 1024**3}
+    UNITS = {"b": 1, "k": 1024, "m": 1024**2, "g": 1024**3, "t": 1024**4}
 
     def pre_filter(self) -> str:
         """Return rTorrent condition to speed up data transfer."""
         comparers = {
             "gt": "greater",
             "lt": "less",
             "eq": "equal",
@@ -828,18 +890,20 @@
             children = [visited_children[0]] + visited_children[1]
         else:
             children = visited_children
         pared = self.__pare_children(children, AndNode)
         return pared
 
     def visit_cond(self, node, visited_children):
-        if len(visited_children) == 1 and isinstance(
-            visited_children[0], (str, re.Pattern)
-        ):
-            return create_filter("name", Operators["eq"], visited_children[0])
+        if len(visited_children) == 1:
+            child = visited_children[0]
+            if isinstance(child, str):
+                return create_filter("name", Operators["eq"], child)
+            if isinstance(child, re.Pattern):
+                return create_filter("name", Operators["eq"], child.pattern)
         return self.generic_visit(node, visited_children)
 
     def visit_query(self, node, visited_children):
         return self.__pare_children(visited_children, AndNode)
 
     # Unfortunate but necessary boilerplate methods
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/util/metafile.py` & `pyrosimple-2.7.1/src/pyrosimple/util/metafile.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     ["info", "pieces"],
     ["info", "private"],
     ["info", "files"],
     ["info", "files", "length"],
     ["info", "files", "path"],
 ]
 
+
 # PieceLogger and PieceFailer are both utility classes for passing
 # into Metafile.make_info()'s piece_callback.
 class PieceLogger:
     """Holds some state to display useful error messages
     if pieces fail to hash check"""
 
     def __init__(self, meta: Dict, logger=None):
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/util/pymagic.py` & `pyrosimple-2.7.1/src/pyrosimple/util/pymagic.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/util/rpc.py` & `pyrosimple-2.7.1/src/pyrosimple/util/rpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,17 +129,20 @@
             methodname,
             encoding=self.__encoding,
             allow_none=self.__allow_none,
         ).encode(self.__encoding, "xmlcharrefreplace")
         if self.__verbose:
             logger.info("req: %s", request)
 
-        response = self.__transport.request(
-            self.__host, self.__handler, request, verbose=self.__verbose
-        )
+        try:
+            response = self.__transport.request(
+                self.__host, self.__handler, request, verbose=self.__verbose
+            )
+        except xmlrpclib.Fault as exc:
+            raise RpcError(exc.faultString, exc.faultCode) from exc
 
         if len(response) == 1:
             return response[0]
         return response
 
     def __batch_request_json(self, calls: List) -> List:
         """Handle JSON-RPC multicalls in place of XMLRPC's built-in
@@ -166,14 +169,17 @@
                 verbose=self.__verbose,
             ),
         )
 
         def sort_key(i: Dict) -> int:
             return int(i["id"])
 
+        if any("error" in r for r in response):
+            uniq_errors = {str(r["error"]) for r in response if "error" in r}
+            raise RpcError(f"Errors in JSON-RPC batch call: {uniq_errors}")
         result = [[r["result"]] for r in sorted(response, key=sort_key)]
         return result
 
     def __request_json(self, methodname, params):
         if not params:
             params = [""]
```

### Comparing `pyrosimple-2.7.0/src/pyrosimple/util/traits.py` & `pyrosimple-2.7.1/src/pyrosimple/util/traits.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/src/pyrosimple/util/ui.py` & `pyrosimple-2.7.1/src/pyrosimple/util/ui.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.0/setup.py` & `pyrosimple-2.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
 ['pyrosimple',
+ 'pyrosimple.data',
  'pyrosimple.io',
  'pyrosimple.job',
  'pyrosimple.scripts',
  'pyrosimple.torrent',
  'pyrosimple.ui',
  'pyrosimple.util']
 
 package_data = \
-{'': ['*'], 'pyrosimple': ['data/*']}
+{'': ['*']}
 
 modules = \
 ['py']
 install_requires = \
 ['Jinja2>=3.1.0,<4.0.0',
  'bencode.py>=4.0.0,<5.0.0',
  'parsimonious>=0.10.0,<0.11.0',
  'prometheus-client>=0.16.0,<0.17.0',
  'prompt-toolkit>=3.0.30,<4.0.0',
  'python-box>=7.0.0,<8.0.0',
- 'python-daemon>=2.3.0,<3.0.0',
+ 'python-daemon>=3.0.1,<4.0.0',
  'requests>=2.28.1,<3.0.0',
  'shtab>=1.5.5,<2.0.0',
  'tomli-w>=1.0.0,<2.0.0']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0'],
  ':python_version < "3.9"': ['importlib-resources>=5.4.0,<6.0.0'],
@@ -42,15 +43,15 @@
                      'pyroadmin = pyrosimple.scripts.pyroadmin:run',
                      'pyrotorque = pyrosimple.scripts.pyrotorque:run',
                      'rtcontrol = pyrosimple.scripts.rtcontrol:run',
                      'rtxmlrpc = pyrosimple.scripts.rtxmlrpc:run']}
 
 setup_kwargs = {
     'name': 'pyrosimple',
-    'version': '2.7.0',
+    'version': '2.7.1',
     'description': 'A stripped-down version of the pyrocore tools for working with rTorrent',
     'long_description': "# pyrosimple\n\n[![GitHub Workflow Status](http://img.shields.io/github/actions/workflow/status/kannibalox/pyrosimple/pylint.yml?branch=main)](https://github.com/kannibalox/pyrosimple/actions/workflows/pylint.yml)\n[![PyPI](https://img.shields.io/pypi/v/pyrosimple)](https://pypi.org/project/pyrosimple/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyrosimple)\n\nA overhauled Python 3 fork of the [pyrocore\ntools](https://github.com/pyroscope/pyrocore), for working with the\n[rTorrent client](https://github.com/rakshasa/rtorrent).\n\n## Installation\n\n```bash\npip install pyrosimple\n# pip install 'pyrosimple[torque]' # Optional dependencies for using pyrotorque\n```\n\nSee the [documentation for usage](https://kannibalox.github.io/pyrosimple/).\nIf you've used rtcontrol/rtxmlrpc before, you should feel right at home.\n\n## What's the point of this?\n\nThe pyrocore tools are great, but being stuck on python 2, along with\nthe complicated install procedure made integrating both the tools and\nthe code into other processes very painful.\n\n## Differences from pyrocore\n\nThe following lists are not exhaustive, and don't cover many of the\ninternal improvements and refactoring.\n\n- Only supports python 3 and rTorrent 0.9.6+ (this includes\n  rTorrent-PS and rTorrent-PS-CH)\n  - pypy is supported, but not as well tested\n- Simpler poetry-based build system, with a single package to install\n- Performance improvements (faster templating and only fetching\n  required fields)\n\n### New features\n\n- Multi-instance support for rtcontrol/rtxmlrpc\n- Replaced Tempita with Jinja2\n- Support for JSON-RPC (only implemented by\n  https://github.com/jesec/rtorrent)\n- Actions to move torrent between paths, or torrents between hosts\n\nSee https://kannibalox.github.io/pyrosimple/migrate/ for how to\nmigrate scripts to the new features.\n\n## Legacy branch\n\nIf you just want to use the pyrocore tools on python 3 without all the\nnew features, you can use the `release-1.X` branch (1.3 is the latest\nrelease at time of writing).  These releases will only receive bug\nfixes or changes to maintain compatibility with the original pyrocore\ntools.\n",
     'author': 'kannibalox',
     'author_email': 'kannibalox@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kannibalox/pyrosimple',
```

### Comparing `pyrosimple-2.7.0/PKG-INFO` & `pyrosimple-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosimple
-Version: 2.7.0
+Version: 2.7.1
 Summary: A stripped-down version of the pyrocore tools for working with rTorrent
 Home-page: https://github.com/kannibalox/pyrosimple
 License: GPL-3.0-or-later
 Author: kannibalox
 Author-email: kannibalox@gmail.com
 Requires-Python: >=3.7.2,<4
 Classifier: Development Status :: 4 - Beta
@@ -32,15 +32,15 @@
 Requires-Dist: bencode.py (>=4.0.0,<5.0.0)
 Requires-Dist: importlib-resources (>=5.4.0,<6.0.0) ; python_version < "3.9"
 Requires-Dist: inotify (>=0.2.10,<0.3.0) ; extra == "torque"
 Requires-Dist: parsimonious (>=0.10.0,<0.11.0)
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Requires-Dist: prompt-toolkit (>=3.0.30,<4.0.0)
 Requires-Dist: python-box (>=7.0.0,<8.0.0)
-Requires-Dist: python-daemon (>=2.3.0,<3.0.0)
+Requires-Dist: python-daemon (>=3.0.1,<4.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: shtab (>=1.5.5,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://kannibalox.github.io/pyrosimple/
 Project-URL: Repository, https://github.com/kannibalox/pyrosimple
 Description-Content-Type: text/markdown
```


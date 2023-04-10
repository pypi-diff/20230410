# Comparing `tmp/sonos-websocket-0.0.1.tar.gz` & `tmp/sonos-websocket-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonos-websocket-0.0.1.tar", last modified: Sun Apr  9 03:39:44 2023, max compression
+gzip compressed data, was "sonos-websocket-0.0.3.tar", last modified: Mon Apr 10 02:59:36 2023, max compression
```

## Comparing `sonos-websocket-0.0.1.tar` & `sonos-websocket-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jasonl     (501) staff       (20)        0 2023-04-09 03:39:44.276904 sonos-websocket-0.0.1/
--rw-r--r--   0 jasonl     (501) staff       (20)     1578 2023-04-09 03:39:44.276763 sonos-websocket-0.0.1/PKG-INFO
--rw-r--r--   0 jasonl     (501) staff       (20)      762 2023-04-09 03:32:04.000000 sonos-websocket-0.0.1/README.md
--rw-r--r--   0 jasonl     (501) staff       (20)     1551 2023-04-09 03:02:26.000000 sonos-websocket-0.0.1/pyproject.toml
--rw-r--r--   0 jasonl     (501) staff       (20)        8 2023-04-08 23:44:54.000000 sonos-websocket-0.0.1/requirements.txt
--rw-r--r--   0 jasonl     (501) staff       (20)       38 2023-04-09 03:39:44.276945 sonos-websocket-0.0.1/setup.cfg
-drwxr-xr-x   0 jasonl     (501) staff       (20)        0 2023-04-09 03:39:44.270150 sonos-websocket-0.0.1/sonos_websocket/
--rw-r--r--   0 jasonl     (501) staff       (20)      127 2023-04-09 00:39:51.000000 sonos-websocket-0.0.1/sonos_websocket/__init__.py
--rw-r--r--   0 jasonl     (501) staff       (20)      997 2023-04-09 01:35:51.000000 sonos-websocket-0.0.1/sonos_websocket/__main__.py
--rw-r--r--   0 jasonl     (501) staff       (20)       90 2023-04-08 17:22:25.000000 sonos-websocket-0.0.1/sonos_websocket/const.py
--rw-r--r--   0 jasonl     (501) staff       (20)      447 2023-04-09 03:02:09.000000 sonos-websocket-0.0.1/sonos_websocket/exception.py
--rw-r--r--   0 jasonl     (501) staff       (20)     5060 2023-04-09 03:03:45.000000 sonos-websocket-0.0.1/sonos_websocket/websocket.py
-drwxr-xr-x   0 jasonl     (501) staff       (20)        0 2023-04-09 03:39:44.276492 sonos-websocket-0.0.1/sonos_websocket.egg-info/
--rw-r--r--   0 jasonl     (501) staff       (20)     1578 2023-04-09 03:39:44.000000 sonos-websocket-0.0.1/sonos_websocket.egg-info/PKG-INFO
--rw-r--r--   0 jasonl     (501) staff       (20)      374 2023-04-09 03:39:44.000000 sonos-websocket-0.0.1/sonos_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 jasonl     (501) staff       (20)        1 2023-04-09 03:39:44.000000 sonos-websocket-0.0.1/sonos_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 jasonl     (501) staff       (20)        8 2023-04-09 03:39:44.000000 sonos-websocket-0.0.1/sonos_websocket.egg-info/requires.txt
--rw-r--r--   0 jasonl     (501) staff       (20)       16 2023-04-09 03:39:44.000000 sonos-websocket-0.0.1/sonos_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:59:36.489954 sonos-websocket-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-10 02:59:36.489954 sonos-websocket-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:59:36.489954 sonos-websocket-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:59:36.489954 sonos-websocket-0.0.3/sonos_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/sonos_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/sonos_websocket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/sonos_websocket/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/sonos_websocket/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/sonos_websocket/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:59:36.489954 sonos-websocket-0.0.3/sonos_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-10 02:59:36.000000 sonos-websocket-0.0.3/sonos_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 02:59:36.000000 sonos-websocket-0.0.3/sonos_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:59:36.000000 sonos-websocket-0.0.3/sonos_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 02:59:36.000000 sonos-websocket-0.0.3/sonos_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 02:59:36.000000 sonos-websocket-0.0.3/sonos_websocket.egg-info/top_level.txt
```

### Comparing `sonos-websocket-0.0.1/PKG-INFO` & `sonos-websocket-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonos-websocket
-Version: 0.0.1
+Version: 0.0.3
 Summary: An asynchronous Python library to communicate with Sonos devices over websockets.
 Author-email: Jason Lawrence <jjlawren@users.noreply.github.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jjlawren/sonos-websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -26,8 +26,8 @@
 The below shows how to run `sonos-websocket` as a script:
 ```
 python -m sonos_websocket \
     --ip_addr 192.168.1.88 \
     --uri https://freetestdata.com/wp-content/uploads/2021/09/Free_Test_Data_100KB_MP3.mp3 \
     --volume 15
 ```
-Basic use of how to integrate the package can be found [here](sonos_websocket/__main__.py).
+Basic use of how to integrate the package can be found [here](https://github.com/jjlawren/sonos-websocket/blob/main/sonos_websocket/__main__.py).
```

### Comparing `sonos-websocket-0.0.1/README.md` & `sonos-websocket-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 The below shows how to run `sonos-websocket` as a script:
 ```
 python -m sonos_websocket \
     --ip_addr 192.168.1.88 \
     --uri https://freetestdata.com/wp-content/uploads/2021/09/Free_Test_Data_100KB_MP3.mp3 \
     --volume 15
 ```
-Basic use of how to integrate the package can be found [here](sonos_websocket/__main__.py).
+Basic use of how to integrate the package can be found [here](https://github.com/jjlawren/sonos-websocket/blob/main/sonos_websocket/__main__.py).
```

### Comparing `sonos-websocket-0.0.1/pyproject.toml` & `sonos-websocket-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.0.1/sonos_websocket/__main__.py` & `sonos-websocket-0.0.3/sonos_websocket/__main__.py`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.0.1/sonos_websocket/websocket.py` & `sonos-websocket-0.0.3/sonos_websocket/websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,17 +72,18 @@
     ) -> list[dict[str, Any]]:
         """Send commands over the websocket and handle their responses."""
         if not self.ws or self.ws.closed:
             await self.connect()
             assert self.ws
 
         payload = [command, options or {}]
+        _LOGGER.debug("Sending command: %s", payload)
         await self.ws.send_json(payload)
         response = await self.ws.receive_json()
-        _LOGGER.debug("%s response: %s", command["command"], response)
+        _LOGGER.debug("Response: %s", response)
         return response
 
     async def play_clip(
         self, uri: str, volume: int | None = None
     ) -> list[dict[str, Any]]:
         """Play an audio clip."""
         command = {
@@ -102,15 +103,15 @@
     async def get_household_id(self) -> str:
         """Get the household ID of this device.
 
         Note: This is an invalid command but returns the household ID anyway.
         """
         if self._household_id:
             return self._household_id
-        response, _ = await self.send_command({"command": "getHouseholdId"})
+        response, _ = await self.send_command({})
         if household_id := response.get("householdId"):
             self._household_id = household_id
             return household_id
         raise SonosWebsocketError("Could not determine household ID")
 
     async def get_groups(self) -> list[dict[str, Any]]:
         """Return the current group and player configuration."""
```

### Comparing `sonos-websocket-0.0.1/sonos_websocket.egg-info/PKG-INFO` & `sonos-websocket-0.0.3/sonos_websocket.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonos-websocket
-Version: 0.0.1
+Version: 0.0.3
 Summary: An asynchronous Python library to communicate with Sonos devices over websockets.
 Author-email: Jason Lawrence <jjlawren@users.noreply.github.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jjlawren/sonos-websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -26,8 +26,8 @@
 The below shows how to run `sonos-websocket` as a script:
 ```
 python -m sonos_websocket \
     --ip_addr 192.168.1.88 \
     --uri https://freetestdata.com/wp-content/uploads/2021/09/Free_Test_Data_100KB_MP3.mp3 \
     --volume 15
 ```
-Basic use of how to integrate the package can be found [here](sonos_websocket/__main__.py).
+Basic use of how to integrate the package can be found [here](https://github.com/jjlawren/sonos-websocket/blob/main/sonos_websocket/__main__.py).
```


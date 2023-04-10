# Comparing `tmp/aiotruenas-client-0.8.0.tar.gz` & `tmp/aiotruenas-client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotruenas-client-0.8.0.tar", last modified: Fri Jul  2 23:24:07 2021, max compression
+gzip compressed data, was "aiotruenas-client-0.9.0.tar", last modified: Fri Dec 31 20:16:33 2021, max compression
```

## Comparing `aiotruenas-client-0.8.0.tar` & `aiotruenas-client-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-02 23:24:07.759395 aiotruenas-client-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3236 2021-07-02 23:24:07.759395 aiotruenas-client-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2503 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-02 23:24:07.755394 aiotruenas-client-0.8.0/aiotruenas_client/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3085 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/disk.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/jail.py
--rw-r--r--   0 runner    (1001) docker     (121)     1981 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/job.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/virtualmachine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-02 23:24:07.759395 aiotruenas-client-0.8.0/aiotruenas_client/websockets/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4703 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/websockets/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4899 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/websockets/disk.py
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/websockets/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/websockets/jail.py
--rw-r--r--   0 runner    (1001) docker     (121)     3988 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/websockets/job.py
--rw-r--r--   0 runner    (1001) docker     (121)     8075 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/websockets/machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     4208 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/websockets/pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     7196 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/websockets/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     5180 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/aiotruenas_client/websockets/virtualmachine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-02 23:24:07.755394 aiotruenas-client-0.8.0/aiotruenas_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3236 2021-07-02 23:24:07.000000 aiotruenas-client-0.8.0/aiotruenas_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      881 2021-07-02 23:24:07.000000 aiotruenas-client-0.8.0/aiotruenas_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-02 23:24:07.000000 aiotruenas-client-0.8.0/aiotruenas_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-07-02 23:24:07.000000 aiotruenas-client-0.8.0/aiotruenas_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-07-02 23:24:07.000000 aiotruenas-client-0.8.0/aiotruenas_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-07-02 23:24:07.759395 aiotruenas-client-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-07-02 23:24:03.000000 aiotruenas-client-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 20:16:33.693563 aiotruenas-client-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3337 2021-12-31 20:16:33.693563 aiotruenas-client-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2503 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 20:16:33.693563 aiotruenas-client-0.9.0/aiotruenas_client/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3085 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1513 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/disk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/jail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1981 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1325 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/machine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2077 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1756 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/virtualmachine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 20:16:33.693563 aiotruenas-client-0.9.0/aiotruenas_client/websockets/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4703 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/websockets/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4899 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/websockets/disk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2609 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/websockets/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4484 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/websockets/jail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3988 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/websockets/job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8851 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/websockets/machine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4208 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/websockets/pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7196 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/websockets/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5180 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/aiotruenas_client/websockets/virtualmachine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 20:16:33.693563 aiotruenas-client-0.9.0/aiotruenas_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3337 2021-12-31 20:16:33.000000 aiotruenas-client-0.9.0/aiotruenas_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2021-12-31 20:16:33.000000 aiotruenas-client-0.9.0/aiotruenas_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-31 20:16:33.000000 aiotruenas-client-0.9.0/aiotruenas_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-12-31 20:16:33.000000 aiotruenas-client-0.9.0/aiotruenas_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-31 20:16:33.000000 aiotruenas-client-0.9.0/aiotruenas_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2021-12-31 20:16:33.697563 aiotruenas-client-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2021-12-31 20:16:29.000000 aiotruenas-client-0.9.0/setup.py
```

### Comparing `aiotruenas-client-0.8.0/LICENSE` & `aiotruenas-client-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/PKG-INFO` & `aiotruenas-client-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: aiotruenas-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python client library for the TrueNAS API
 Home-page: UNKNOWN
 Author: Shawn Wilsher
 Author-email: me@shawnwilsher.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/sdwilsh/aiotruenas-client/issues
 Project-URL: Release Notes, https://github.com/sdwilsh/aiotruenas-client/releases/
 Project-URL: Source, https://github.com/sdwilsh/aiotruenas-client
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <4,>3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Lint](https://github.com/sdwilsh/aiotruenas-client/workflows/Lint/badge.svg)
 ![Build](https://github.com/sdwilsh/aiotruenas-client/workflows/Build/badge.svg)
```

### Comparing `aiotruenas-client-0.8.0/README.md` & `aiotruenas-client-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/dataset.py` & `aiotruenas-client-0.9.0/aiotruenas_client/dataset.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/disk.py` & `aiotruenas-client-0.9.0/aiotruenas_client/disk.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/jail.py` & `aiotruenas-client-0.9.0/aiotruenas_client/jail.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/job.py` & `aiotruenas-client-0.9.0/aiotruenas_client/job.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/machine.py` & `aiotruenas-client-0.9.0/aiotruenas_client/machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     async def get_datasets(self) -> List[Dataset]:
         """Get the datasets on the remote machine."""
 
     @abstractmethod
     async def get_disks(self, include_temperature: bool) -> List[Disk]:
         """Get the disks on the remote machine."""
 
+    @abstractmethod
     async def get_jails(self) -> List[Jail]:
         """Get the jails on the remote machine."""
 
     @abstractmethod
     async def get_job(self, id: TJobId) -> Job:
         """Get the specified Job from the remote machine."""
```

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/pool.py` & `aiotruenas-client-0.9.0/aiotruenas_client/pool.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/virtualmachine.py` & `aiotruenas-client-0.9.0/aiotruenas_client/virtualmachine.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/websockets/dataset.py` & `aiotruenas-client-0.9.0/aiotruenas_client/websockets/dataset.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/websockets/disk.py` & `aiotruenas-client-0.9.0/aiotruenas_client/websockets/disk.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/websockets/interfaces.py` & `aiotruenas-client-0.9.0/aiotruenas_client/websockets/interfaces.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/websockets/jail.py` & `aiotruenas-client-0.9.0/aiotruenas_client/websockets/jail.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/websockets/job.py` & `aiotruenas-client-0.9.0/aiotruenas_client/websockets/job.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/websockets/machine.py` & `aiotruenas-client-0.9.0/aiotruenas_client/websockets/machine.py`

 * *Files 11% similar despite different names*

```diff
@@ -86,32 +86,47 @@
             auth_protocol = truenas_api_key_auth_protocol_factory(api_key)
         elif username and password:
             auth_protocol = truenas_password_auth_protocol_factory(username, password)
         else:
             raise AssertionError
 
         await self._connect(auth_protocol, host, secure)
+        assert self._client is not None
+        ip_address = self._client.remote_address[0]
+        port = self._client.remote_address[1]
+        logger.debug("Connected to %s on port %d.", ip_address, port)
 
     async def close(self) -> None:
         """Closes the conenction to the server."""
         assert self._client is not None
         for subscriber in self._subscribers:
             try:
                 await subscriber.unsubscribe()
             except Exception as exc:
                 logger.exception(
                     "Caught exception while closing connection.",
                     exc_info=exc,
                 )
+        ip_address = self._client.remote_address[0]
+        port = self._client.remote_address[1]
         await self._client.close()
+        logger.debug("Connection closed to %s on port %d", ip_address, port)
         self._client = None
 
     @property
     def closed(self) -> bool:
         """Indicates if the connection to the server is closed or not."""
+        if (not self._client is None) and self._client.closed:
+            # Log some additional information to help debug why a connection might be unexpectedly closed.
+            logger.debug(
+                "%s closed with code %d (%s)",
+                self._client.side,
+                self._client.close_code,
+                self._client.close_reason or "[no reason]",
+            )
         return self._client is None or self._client.closed
 
     async def get_datasets(self) -> List[CachingDataset]:
         """Returns a list of datasets on the host."""
         return await self._dataset_fetcher.get_datasets()
 
     @property
```

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/websockets/pool.py` & `aiotruenas-client-0.9.0/aiotruenas_client/websockets/pool.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/websockets/protocol.py` & `aiotruenas-client-0.9.0/aiotruenas_client/websockets/protocol.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client/websockets/virtualmachine.py` & `aiotruenas-client-0.9.0/aiotruenas_client/websockets/virtualmachine.py`

 * *Files identical despite different names*

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client.egg-info/PKG-INFO` & `aiotruenas-client-0.9.0/aiotruenas_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: aiotruenas-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python client library for the TrueNAS API
 Home-page: UNKNOWN
 Author: Shawn Wilsher
 Author-email: me@shawnwilsher.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/sdwilsh/aiotruenas-client/issues
 Project-URL: Release Notes, https://github.com/sdwilsh/aiotruenas-client/releases/
 Project-URL: Source, https://github.com/sdwilsh/aiotruenas-client
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <4,>3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Lint](https://github.com/sdwilsh/aiotruenas-client/workflows/Lint/badge.svg)
 ![Build](https://github.com/sdwilsh/aiotruenas-client/workflows/Build/badge.svg)
```

### Comparing `aiotruenas-client-0.8.0/aiotruenas_client.egg-info/SOURCES.txt` & `aiotruenas-client-0.9.0/aiotruenas_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


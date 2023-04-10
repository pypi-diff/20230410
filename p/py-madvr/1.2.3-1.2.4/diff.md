# Comparing `tmp/py_madvr-1.2.3.tar.gz` & `tmp/py_madvr-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.2.3.tar", last modified: Wed Mar 15 23:52:53 2023, max compression
+gzip compressed data, was "py_madvr-1.2.4.tar", last modified: Mon Apr 10 02:33:16 2023, max compression
```

## Comparing `py_madvr-1.2.3.tar` & `py_madvr-1.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:52:53.258067 py_madvr-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-15 23:52:43.000000 py_madvr-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-15 23:52:53.258067 py_madvr-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-15 23:52:43.000000 py_madvr-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:52:53.258067 py_madvr-1.2.3/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-15 23:52:43.000000 py_madvr-1.2.3/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-03-15 23:52:43.000000 py_madvr-1.2.3/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-15 23:52:43.000000 py_madvr-1.2.3/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21785 2023-03-15 23:52:43.000000 py_madvr-1.2.3/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:52:53.258067 py_madvr-1.2.3/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-15 23:52:53.000000 py_madvr-1.2.3/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-15 23:52:53.000000 py_madvr-1.2.3/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 23:52:53.000000 py_madvr-1.2.3/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-15 23:52:53.000000 py_madvr-1.2.3/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 23:52:53.258067 py_madvr-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-15 23:52:43.000000 py_madvr-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:52:53.258067 py_madvr-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 23:52:43.000000 py_madvr-1.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-15 23:52:43.000000 py_madvr-1.2.3/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:33:16.946104 py_madvr-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-10 02:33:03.000000 py_madvr-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 02:33:16.946104 py_madvr-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-10 02:33:03.000000 py_madvr-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:33:16.946104 py_madvr-1.2.4/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-10 02:33:03.000000 py_madvr-1.2.4/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-10 02:33:03.000000 py_madvr-1.2.4/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-10 02:33:03.000000 py_madvr-1.2.4/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19693 2023-04-10 02:33:03.000000 py_madvr-1.2.4/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:33:16.946104 py_madvr-1.2.4/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 02:33:16.000000 py_madvr-1.2.4/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-10 02:33:16.000000 py_madvr-1.2.4/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:33:16.000000 py_madvr-1.2.4/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 02:33:16.000000 py_madvr-1.2.4/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:33:16.946104 py_madvr-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-10 02:33:03.000000 py_madvr-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:33:16.946104 py_madvr-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:33:03.000000 py_madvr-1.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-10 02:33:03.000000 py_madvr-1.2.4/tests/testMadVR.py
```

### Comparing `py_madvr-1.2.3/LICENSE` & `py_madvr-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.2.3/PKG-INFO` & `py_madvr-1.2.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.2.3
+Version: 1.2.4
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.2.3/madvr/commands.py` & `py_madvr-1.2.4/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.2.3/madvr/madvr.py` & `py_madvr-1.2.4/madvr/madvr.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     def close_connection(self) -> None:
         """close the connection"""
         try:
             self.client.close()
         except AttributeError:
             # means its already closed
             pass
-        
+
         try:
             self.notification_client.close()
         except AttributeError:
             # means its already closed
             pass
 
         self.client = None
@@ -193,23 +193,19 @@
                 )
                 time.sleep(2)
                 continue
 
             # includes conn refused
             # backoff to not spam HA
             except socket.timeout:
-                self.logger.warning(
-                    "Connecting timeout, retrying in %s seconds", 2
-                )
+                self.logger.warning("Connecting timeout, retrying in %s seconds", 2)
                 time.sleep(2)
                 continue
             except OSError as err:
-                self.logger.warning(
-                    "Connecting failed, retrying in %s seconds", 2
-                )
+                self.logger.warning("Connecting failed, retrying in %s seconds", 2)
                 self.logger.debug(err)
                 time.sleep(2)
                 continue
 
     def _send_heartbeat(self) -> None:
         """
         Send a heartbeat to keep connection open
@@ -248,60 +244,63 @@
 
             self.logger.debug("Handshakes complete")
 
             return
 
         raise HeartBeatError("Sending heartbeat fatal error")
 
-    def _construct_command(self, raw_command: Union[str, list]) -> tuple[bytes, bool, str]:
+    def _construct_command(self, raw_command: Union[str, list]) -> tuple[bytes, str]:
         """
         Transform commands into their byte values from the string value
 
         Raises NotImplementedError
 
         Return:
             bytes: the value to send in bytes
-            bool: if its informational
             str: the 'msg' field in the Enum used to filter notifications
         """
         self.logger.debug("raw_command: %s", raw_command)
+        self.logger.debug("raw_command length: %s", len(raw_command))
         skip_val = False
         # HA seems to always send commands as a list even if you set them as a str
 
         # This lets you use single cmds or something with val like KEYPRESS
         # If len is 1, then try to split, otherwise its just one word
         if len(raw_command) == 1:
             try:
                 # ['key_press, menu']
                 command, raw_value = raw_command[0].split(",")
                 # remove space
                 value = raw_value.strip()
                 self.logger.debug("using command %s and value %s", command, value)
             # if valuerror it means theres just one command like PowerOff, so use that directly
-            except ValueError:
+            except ValueError as err:
+                self.logger.debug(err)
+                self.logger.debug("Using raw_command directly")
                 command = raw_command
                 skip_val = True
         # if there are more than two values, this is incorrect, error
         elif len(raw_command) > 2:
-            self.logger.error("More than two command values provided. Envy does not have more than 2 command values e.g KeyPress MENU")
+            self.logger.error(
+                "More than two command values provided. Envy does not have more than 2 command values e.g KeyPress MENU"
+            )
             raise NotImplementedError(f"Too many values provided {raw_command}")
         else:
             # else a command was provided as a proper list ['keypress', 'menu']
             # raw command will be a list of 2
             command, value = raw_command
 
-
         self.logger.debug("using command %s", command)
 
         # Check if command is implemented
         if not hasattr(Commands, command):
             raise NotImplementedError(f"Command not implemented: {command}")
 
         # construct the command with nested Enums
-        command_name, val, is_info = Commands[command].value
+        command_name, val, _ = Commands[command].value
 
         # if there is a value to process
         if not skip_val:
             try:
                 command_base: bytes = command_name + b" " + val[value.lstrip(" ")].value
                 # Construct command based on required values
                 cmd: bytes = command_base + Footer.footer.value
@@ -310,15 +309,15 @@
                     "Incorrect parameter given for command"
                 ) from exc
         else:
             cmd: bytes = command_name + Footer.footer.value
 
         self.logger.debug("constructed command: %s", cmd)
 
-        return cmd, is_info.value, val
+        return cmd, val
 
     def _read_until_ok(self, client: socket.socket) -> bool:
         """
         Read the buffer until we get ok or timeout because a timeout means no more to read
         """
         counter = 0
         # exit loop if exceed maximum checks for ok or retries
@@ -338,26 +337,27 @@
             except (socket.timeout, socket.error):
                 self.logger.debug("Timeout reading ack with counter: %s", counter)
                 return False
 
     def send_command(self, command: Union[str, list]) -> str:
         """
         send a given command same as the official madvr ones
+        To keep this simple, just send the command without reading response
 
         command: str - command to send like KeyPress, MENU
         Raises RetryExceededError
         """
 
         # Verify the command is supported
         try:
-            cmd, is_info, enum_type = self._construct_command(command)
+            cmd, enum_type = self._construct_command(command)
         except NotImplementedError:
             return f"Command not found: {command}"
 
-        self.logger.debug("using values: %s %s %s", cmd, is_info, enum_type)
+        self.logger.debug("using values: %s %s", cmd, enum_type)
 
         # reconnect if client is not init or its off
         if self.client is None or self.is_on is False:
             # Don't reconnect if poweroff or standby because HA will complain
             if "PowerOff" in command or "Standby" in command:
                 return ""
             self.logger.debug("Connection lost - restarting connection")
@@ -366,64 +366,43 @@
         # simple retry logic
         retry_count = 0
 
         while retry_count < 5:
             # Send the command
             try:
                 self.client.send(cmd)
-
-                if not self._read_until_ok(self.client):
-                    self.logger.debug("OK not found when reading response, retrying")
-                    retry_count += 1
-                    continue
+                # if not self._read_until_ok(self.client):
+                #     self.logger.debug("OK not found when reading response, retrying")
+                #     retry_count += 1
+                #     continue
 
             except socket.timeout:
                 self.logger.debug("OK receipt timed out, retrying")
                 retry_count += 1
                 continue
 
             # should catch connection is closed
             except OSError:
                 self.logger.warning("connection failed when reading OK, retrying")
                 retry_count += 1
                 continue
 
-            # If its an info, get the rest of the info
-            try:
-                if is_info:
-                    # read response
-                    res = self.client.recv(self.read_limit)
-                    self.logger.debug("Response from info: %s", res)
-
-                    # TODO one day: whatever is not part of our command, write that to attr
-                    # e.g if we ask signal, and get notification for aspect, detect it and write that
-                    # so polling isn't required
-
-                    # process the output
-                    return self._process_info(res, enum_type["msg"].value)
-
-                return ""
-
-            except socket.timeout:
-                self.logger.debug("Ack receipt timed out, retrying")
-                retry_count += 1
-                continue
+            return ""
 
         # if we got here something went wrong
         self.close_connection()
         self._reconnect()
 
         return ""
 
-    def read_notifications(self, wait_forever: bool) -> None:
+    def start_read_notifications(self, wait_forever: bool) -> None:
         """
         Listen for notifications. Meant to run as a background task
         wait_forever: bool -> if true, it will block forever. False useful for testing
         """
-        # TODO: should this be a second integration?
         # Is there a way for HA to always poll in background?z
 
         # Receive data in a loop
         i = 0
         while wait_forever or i < 5:
             try:
                 self.notification_client.sendall(self.HEARTBEAT)
@@ -443,39 +422,19 @@
                 self.notification_client.sendall(self.HEARTBEAT)
                 continue
             except socket.error:
                 self.logger.debug("Connection error")
                 self.notification_client.sendall(self.HEARTBEAT)
                 continue
 
-    def poll_status(self) -> None:
-        """
-        Poll the status for attributes and write them to state
-        """
-        try:
-            # send heartbeat so it doesnt close our connection
-            self._send_heartbeat()
-            # Get incoming signal info
-            for cmd in [
-                "GetIncomingSignalInfo",
-                "GetAspectRatio",
-                "GetTemperatures",
-                "GetOutgoingSignalInfo",
-            ]:
-                res = self.send_command(cmd)
-                self.logger.debug("poll_status resp: %s", res)
-                self._process_notifications(res)
-        except (socket.timeout, socket.error, HeartBeatError) as err:
-            self.logger.error("Error getting update: %s", err)
-
     def _process_notifications(self, input_data: Union[bytes, str]) -> None:
         """
         Process arbitrary stream of notifications and set them as instance attr
         """
-
+        # This code constructs a dict for all values processed
         self.logger.debug("Processing data for %s", input_data)
         try:
             if isinstance(input_data, bytes):
                 # This pattern will be able to extract from the byte encoded stream
                 pattern = r"([A-Z][^\r\n]*)\r\n"
                 groups = re.findall(pattern, input_data.decode())
                 # split the groups, the first element is the key, remove the key from the values
@@ -551,32 +510,14 @@
             self.is_on = False
 
             return res
 
         except RetryExceededError:
             return "Retries Exceeded"
 
-    def _process_info(self, input_data: bytes, filter_str: str) -> str:
-        """
-        Process info given input and a filter str to only return the thing we want
-        e.g for IncomingSignalInfo
-        b"Ok\r\nIncomingSignalInfo 3840x2160 23.976p 2D 422
-        10bit HDR10 2020 TV 16:9\r\nAspect Ratio ETC ETC\r\n"
-        turns into -> IncomingSignalInfo 3840x2160 23.976p 2D 422 10bit HDR10 2020 TV 16:9
-
-        This is used by _process_notifications to turn it into a dict, add to instance attr
-        """
-
-        lines = input_data.decode().split("\r\n")
-        for line in lines:
-            if filter_str in line:
-                return line
-
-        return ""
-
     def print_commands(self) -> str:
         """
         Print out all supported commands
         """
         print_commands = sorted(
             [
                 command.name
```

### Comparing `py_madvr-1.2.3/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.2.4/py_madvr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.2.3
+Version: 1.2.4
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.2.3/setup.py` & `py_madvr-1.2.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.2.3",
+    version="1.2.4",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.2.3/tests/testMadVR.py` & `py_madvr-1.2.4/tests/testMadVR.py`

 * *Files identical despite different names*


# Comparing `tmp/robotframework-mainframe3270-3.1.tar.gz` & `tmp/robotframework-mainframe3270-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-mainframe3270-3.1.tar", last modified: Wed Mar 15 15:55:15 2023, max compression
+gzip compressed data, was "robotframework-mainframe3270-3.2.tar", last modified: Sat Apr  1 12:37:43 2023, max compression
```

## Comparing `robotframework-mainframe3270-3.1.tar` & `robotframework-mainframe3270-3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 15:55:15.268312 robotframework-mainframe3270-3.1/
--rw-rw-rw-   0        0        0     1086 2022-06-21 10:15:16.000000 robotframework-mainframe3270-3.1/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-03-15 15:55:15.224746 robotframework-mainframe3270-3.1/Mainframe3270/
--rw-rw-rw-   0        0        0     4946 2023-02-16 21:25:05.000000 robotframework-mainframe3270-3.1/Mainframe3270/__init__.py
--rw-rw-rw-   0        0        0    16074 2023-03-15 15:17:04.000000 robotframework-mainframe3270-3.1/Mainframe3270/py3270.py
--rw-rw-rw-   0        0        0       17 2023-03-15 15:48:44.000000 robotframework-mainframe3270-3.1/Mainframe3270/version.py
--rw-rw-rw-   0        0        0    32828 2023-03-15 15:17:04.000000 robotframework-mainframe3270-3.1/Mainframe3270/x3270.py
--rw-rw-rw-   0        0        0     8603 2023-03-15 15:55:15.267282 robotframework-mainframe3270-3.1/PKG-INFO
--rw-rw-rw-   0        0        0     7658 2023-03-15 15:44:45.000000 robotframework-mainframe3270-3.1/README.md
--rw-rw-rw-   0        0        0     2100 2022-06-21 10:15:16.000000 robotframework-mainframe3270-3.1/THIRD-PARTY-NOTICES.txt
-drwxrwxrwx   0        0        0        0 2023-03-15 15:55:15.264255 robotframework-mainframe3270-3.1/robotframework_mainframe3270.egg-info/
--rw-rw-rw-   0        0        0     8603 2023-03-15 15:55:15.000000 robotframework-mainframe3270-3.1/robotframework_mainframe3270.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-03-15 15:55:15.000000 robotframework-mainframe3270-3.1/robotframework_mainframe3270.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 15:55:15.000000 robotframework-mainframe3270-3.1/robotframework_mainframe3270.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-15 15:55:15.000000 robotframework-mainframe3270-3.1/robotframework_mainframe3270.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-15 15:55:15.000000 robotframework-mainframe3270-3.1/robotframework_mainframe3270.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 15:55:15.269304 robotframework-mainframe3270-3.1/setup.cfg
--rw-rw-rw-   0        0        0     1643 2023-02-16 21:25:05.000000 robotframework-mainframe3270-3.1/setup.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-01 12:37:43.653147 robotframework-mainframe3270-3.2/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1065 2023-02-12 18:46:10.000000 robotframework-mainframe3270-3.2/LICENSE.md
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-01 12:37:43.645147 robotframework-mainframe3270-3.2/Mainframe3270/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4830 2023-04-01 12:22:17.000000 robotframework-mainframe3270-3.2/Mainframe3270/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    15590 2023-03-17 04:57:06.000000 robotframework-mainframe3270-3.2/Mainframe3270/py3270.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)       16 2023-04-01 12:26:46.000000 robotframework-mainframe3270-3.2/Mainframe3270/version.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    35623 2023-04-01 12:22:17.000000 robotframework-mainframe3270-3.2/Mainframe3270/x3270.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7343 2023-04-01 12:37:43.653147 robotframework-mainframe3270-3.2/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6443 2023-04-01 12:22:17.000000 robotframework-mainframe3270-3.2/README.md
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2063 2023-03-16 03:55:46.000000 robotframework-mainframe3270-3.2/THIRD-PARTY-NOTICES.txt
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-01 12:37:43.649147 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7343 2023-04-01 12:37:43.000000 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)      410 2023-04-01 12:37:43.000000 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/SOURCES.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-04-01 12:37:43.000000 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/dependency_links.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       44 2023-04-01 12:37:43.000000 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/requires.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       14 2023-04-01 12:37:43.000000 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/top_level.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-04-01 12:37:43.653147 robotframework-mainframe3270-3.2/setup.cfg
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1597 2023-03-16 03:55:46.000000 robotframework-mainframe3270-3.2/setup.py
```

### Comparing `robotframework-mainframe3270-3.1/LICENSE.md` & `robotframework-mainframe3270-3.2/LICENSE.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 altranpt
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
+Copyright (c) 2018 altranpt
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

### Comparing `robotframework-mainframe3270-3.1/Mainframe3270/__init__.py` & `robotframework-mainframe3270-3.2/Mainframe3270/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-from datetime import timedelta
-from typing import Any
-
-from robot.api import logger
-from robot.api.deco import keyword
-from robot.libraries.BuiltIn import BuiltIn
-from robotlibcore import DynamicCore
-
-from .version import VERSION
-from .x3270 import x3270
-
-
-class Mainframe3270(DynamicCore):
-    r"""
-    Mainframe3270 is a library for Robot Framework based on the [https://pypi.org/project/py3270/|py3270 project],
-    a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
-
-    = Installation  =
-
-    For use this library you need to install the [http://x3270.bgp.nu/download.html|x3270 project]
-    and put the directory on your PATH. On Windows, you need to download wc3270 and put
-    the "C:\Program Files\wc3270" in PATH of the Environment Variables.
-
-    = Example =
-
-    | *** Settings ***
-    | Library           Mainframe3270
-    |
-    | *** Test Cases ***
-    | Example
-    |     Open Connection    Hostname    LUname
-    |     Change Wait Time    0.4 seconds
-    |     Change Wait Time After Write    0.4 seconds
-    |     Set Screenshot Folder    C:\\Temp\\IMG
-    |     ${value}    Read    3    10    17
-    |     Page Should Contain String    ENTER APPLICATION
-    |     Wait Field Detected
-    |     Write Bare    applicationname
-    |     Send Enter
-    |     Take Screenshot
-    |     Close Connection
-    """
-
-    ROBOT_LIBRARY_SCOPE = "TEST SUITE"
-    ROBOT_LIBRARY_VERSION = VERSION
-
-    def __init__(
-        self,
-        visible: bool = True,
-        timeout: timedelta = timedelta(seconds=30),
-        wait_time: timedelta = timedelta(milliseconds=500),
-        wait_time_after_write: timedelta = timedelta(seconds=0),
-        img_folder: str = ".",
-        run_on_failure_keyword: str = "Take Screenshot",
-    ) -> None:
-        """
-        By default the emulator visibility is set to visible=True.
-        In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
-        You can change this by setting visible=False.
-        Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
-        This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
-
-        Timeout, waits and screenshot folder are set on library import as shown above.
-        However, they can be changed during runtime. To modify the ``wait_time``, see `Change Wait Time`,
-        to modify the ``img_folder``, see `Set Screenshot Folder`,
-        and to modify the ``timeout``, see the `Change Timeout` keyword. Timeouts support all available
-        Robot Framework [https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format|time formats].
-
-        By default, Mainframe3270 will take a screenshot on failure.
-        You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option.
-        If you pass ``None`` to this argument, no keyword will be run.
-        To change the ``run_on_failure_keyword`` during runtime, see `Register Run On Failure Keyword`.
-        """
-        self._running_on_failure_keyword = False
-        self.register_run_on_failure_keyword(run_on_failure_keyword)
-        libraries = [
-            x3270(visible, timeout, wait_time, wait_time_after_write, img_folder)
-        ]
-        DynamicCore.__init__(self, libraries)
-
-    @keyword
-    def register_run_on_failure_keyword(self, keyword: str) -> None:
-        """
-        This keyword lets you change the keyword that runs on failure during test execution.
-        The default is `Take Screenshot`, which is set on library import.
-
-        You can set ``None`` to this keyword, if you do not want to run any keyword on failure.
-
-        Example:
-            | Register Run On Failure Keyword | None | # no keyword is run on failure |
-            | Register Run On Failure Keyword | Custom Keyword | # Custom Keyword is run on failure |
-        """
-        if keyword.lower() == "none":
-            self.run_on_failure_keyword = None
-        else:
-            self.run_on_failure_keyword = keyword
-
-    def run_keyword(self, name: str, args: list, kwargs: dict) -> Any:
-        try:
-            return DynamicCore.run_keyword(self, name, args, kwargs)
-        except Exception:
-            self.run_on_failure()
-            raise
-
-    def run_on_failure(self) -> None:
-        if self._running_on_failure_keyword or not self.run_on_failure_keyword:
-            return
-        try:
-            self._running_on_failure_keyword = True
-            BuiltIn().run_keyword(self.run_on_failure_keyword)
-        except Exception as error:
-            logger.warn(
-                f"Keyword '{self.run_on_failure_keyword}' could not be run on failure: {error}"
-            )
-        finally:
-            self._running_on_failure_keyword = False
+from datetime import timedelta
+from typing import Any
+
+from robot.api import logger
+from robot.api.deco import keyword
+from robot.libraries.BuiltIn import BuiltIn
+from robotlibcore import DynamicCore
+
+from .version import VERSION
+from .x3270 import X3270
+
+
+class Mainframe3270(DynamicCore):
+    r"""
+    Mainframe3270 is a library for Robot Framework based on the [https://pypi.org/project/py3270/|py3270 project],
+    a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
+
+    = Installation  =
+
+    For use this library you need to install the [http://x3270.bgp.nu/download.html|x3270 project]
+    and put the directory on your PATH. On Windows, you need to download wc3270 and put
+    the "C:\Program Files\wc3270" in PATH of the Environment Variables.
+
+    = Example =
+
+    | *** Settings ***
+    | Library           Mainframe3270
+    |
+    | *** Test Cases ***
+    | Example
+    |     Open Connection    Hostname    LUname
+    |     Change Wait Time    0.4 seconds
+    |     Change Wait Time After Write    0.4 seconds
+    |     Set Screenshot Folder    C:\\Temp\\IMG
+    |     ${value}    Read    3    10    17
+    |     Page Should Contain String    ENTER APPLICATION
+    |     Wait Field Detected
+    |     Write Bare    applicationname
+    |     Send Enter
+    |     Take Screenshot
+    |     Close Connection
+    """
+
+    ROBOT_LIBRARY_SCOPE = "TEST SUITE"
+    ROBOT_LIBRARY_VERSION = VERSION
+
+    def __init__(
+        self,
+        visible: bool = True,
+        timeout: timedelta = timedelta(seconds=30),
+        wait_time: timedelta = timedelta(milliseconds=500),
+        wait_time_after_write: timedelta = timedelta(seconds=0),
+        img_folder: str = ".",
+        run_on_failure_keyword: str = "Take Screenshot",
+    ) -> None:
+        """
+        By default the emulator visibility is set to visible=True.
+        In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
+        You can change this by setting visible=False.
+        Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
+        This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
+
+        Timeout, waits and screenshot folder are set on library import as shown above.
+        However, they can be changed during runtime. To modify the ``wait_time``, see `Change Wait Time`,
+        to modify the ``img_folder``, see `Set Screenshot Folder`,
+        and to modify the ``timeout``, see the `Change Timeout` keyword. Timeouts support all available
+        Robot Framework [https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format|time formats].
+
+        By default, Mainframe3270 will take a screenshot on failure.
+        You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option.
+        If you pass ``None`` to this argument, no keyword will be run.
+        To change the ``run_on_failure_keyword`` during runtime, see `Register Run On Failure Keyword`.
+        """
+        self._running_on_failure_keyword = False
+        self.register_run_on_failure_keyword(run_on_failure_keyword)
+        libraries = [
+            X3270(visible, timeout, wait_time, wait_time_after_write, img_folder)
+        ]
+        DynamicCore.__init__(self, libraries)
+
+    @keyword
+    def register_run_on_failure_keyword(self, keyword: str) -> None:
+        """
+        This keyword lets you change the keyword that runs on failure during test execution.
+        The default is `Take Screenshot`, which is set on library import.
+
+        You can set ``None`` to this keyword, if you do not want to run any keyword on failure.
+
+        Example:
+            | Register Run On Failure Keyword | None | # no keyword is run on failure |
+            | Register Run On Failure Keyword | Custom Keyword | # Custom Keyword is run on failure |
+        """
+        if keyword.lower() == "none":
+            self.run_on_failure_keyword = None
+        else:
+            self.run_on_failure_keyword = keyword
+
+    def run_keyword(self, name: str, args: list, kwargs: dict) -> Any:
+        try:
+            return DynamicCore.run_keyword(self, name, args, kwargs)
+        except Exception:
+            self.run_on_failure()
+            raise
+
+    def run_on_failure(self) -> None:
+        if self._running_on_failure_keyword or not self.run_on_failure_keyword:
+            return
+        try:
+            self._running_on_failure_keyword = True
+            BuiltIn().run_keyword(self.run_on_failure_keyword)
+        except Exception as error:
+            logger.warn(
+                f"Keyword '{self.run_on_failure_keyword}' could not be run on failure: {error}"
+            )
+        finally:
+            self._running_on_failure_keyword = False
```

### Comparing `robotframework-mainframe3270-3.1/Mainframe3270/x3270.py` & `robotframework-mainframe3270-3.2/Mainframe3270/x3270.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,775 +1,850 @@
-import os
-import re
-import socket
-import time
-from datetime import timedelta
-from typing import Any, List, Optional, Union
-
-from robot.api import logger
-from robot.api.deco import keyword
-from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
-from robot.utils import Matcher, secs_to_timestr, timestr_to_secs
-
-from .py3270 import Emulator
-
-
-class x3270(object):
-    def __init__(
-        self,
-        visible: bool,
-        timeout: timedelta,
-        wait_time: timedelta,
-        wait_time_after_write: timedelta,
-        img_folder: str,
-    ) -> None:
-        self.visible = visible
-        self.timeout = self._convert_timeout(timeout)
-        self.wait = self._convert_timeout(wait_time)
-        self.wait_write = self._convert_timeout(wait_time_after_write)
-        self.imgfolder = img_folder
-        self.mf: Emulator = None  # type: ignore
-        # Try Catch to run in Pycharm, and make a documentation in libdoc with no error
-        try:
-            self.output_folder = BuiltIn().get_variable_value("${OUTPUT DIR}")
-        except RobotNotRunningError:
-            self.output_folder = os.getcwd()
-
-    def _convert_timeout(self, time):
-        if isinstance(time, timedelta):
-            return time.total_seconds()
-        return timestr_to_secs(time, round_to=None)
-
-    @keyword("Change Timeout")
-    def change_timeout(self, seconds: timedelta) -> None:
-        """
-        Change the timeout for connection in seconds.
-
-        Example:
-            | Change Timeout | 3 seconds |
-        """
-        self.timeout = self._convert_timeout(seconds)
-
-    @keyword("Open Connection")
-    def open_connection(
-        self,
-        host: str,
-        LU: Optional[str] = None,
-        port: int = 23,
-        extra_args: Optional[Union[List[str], os.PathLike]] = None,
-    ):
-        """Create a connection to an IBM3270 mainframe with the default port 23.
-        To establish a connection, only the hostname is required. Optional parameters include logical unit name (LU) and port.
-
-        Additional configuration data can be provided through the `extra_args` parameter.
-        `extra_args` accepts either a list or a path to a file containing [https://x3270.miraheze.org/wiki/Category:Command-line_options|x3270 command line options].
-
-        Entries in the argfile can be on one line or multiple lines. Lines starting with "#" are considered comments.
-
-        | # example_argfile_oneline.txt
-        | -accepthostname myhost.com
-
-        | # example_argfile_multiline.txt
-        | -accepthostname myhost.com
-        | # this is a comment
-        | -charset french
-        | -port 992
-
-        Please ensure that the arguments provided are available for your specific x3270 application and version.
-        Refer to the [https://x3270.miraheze.org/wiki/Wc3270/Command-line_options|wc3270 command line options] for a subset of available options.
-
-        Note: If you specify the port with the `-port` command-line option in `extra_args` (or use the -xrm resource command for it),
-        it will take precedence over the `port` argument provided in the `Open Connection` keyword.
-
-        Example:
-            | Open Connection | Hostname |
-            | Open Connection | Hostname | LU=LUname |
-            | Open Connection | Hostname | port=992 |
-            | @{extra_args}   | Create List | -accepthostname | myhost.com | -cafile | ${CURDIR}/cafile.crt |
-            | Append To List  | ${extra_args} | -port | 992 |
-            | Open Connection | Hostname | extra_args=${extra_args} |
-            | Open Connection | Hostname | extra_args=${CURDIR}/argfile.txt |
-        """
-        if self.mf:
-            self.close_connection()
-        extra_args = self._process_args(extra_args)
-        self.mf = Emulator(self.visible, self.timeout, extra_args)
-        host_string = f"{LU}@{host}" if LU else host
-        if self._port_in_extra_args(extra_args):
-            if port != 23:
-                logger.warn(
-                    "The connection port has been specified both in the `port` argument and in `extra_args`. "
-                    "The port specified in `extra_args` will take precedence over the `port` argument. "
-                    "To avoid this warning, you can either remove the port command-line option from `extra_args`, "
-                    "or leave the `port` argument at its default value of 23."
-                )
-            self.mf.connect(host_string)
-        else:
-            self.mf.connect(f"{host_string}:{port}")
-
-    def _process_args(self, args) -> list:
-        processed_args = []
-        if not args:
-            return []
-        elif isinstance(args, list):
-            processed_args = args
-        elif isinstance(args, os.PathLike) or isinstance(args, str):
-            with open(args) as file:
-                for line in file:
-                    if line.lstrip().startswith("#"):
-                        continue
-                    for arg in line.replace("\n", "").rstrip().split(" "):
-                        processed_args.append(arg)
-        return processed_args
-
-    def _port_in_extra_args(self, args) -> bool:
-        if not args:
-            return False
-        for arg in args:
-            if arg == "-port" or ".port" in arg:
-                return True
-        return False
-
-    @keyword("Close Connection")
-    def close_connection(self) -> None:
-        """Disconnect from the host."""
-        try:
-            self.mf.terminate()
-        except socket.error:
-            pass
-        self.mf = None  # type: ignore
-
-    @keyword("Change Wait Time")
-    def change_wait_time(self, wait_time: timedelta) -> None:
-        """To give time for the mainframe screen to be "drawn" and receive the next commands, a "wait time" has been
-        created, which by default is set to 0.5 seconds. This is a sleep applied AFTER the following keywords:
-
-        - `Execute Command`
-        - `Send Enter`
-        - `Send PF`
-        - `Write`
-        - `Write in position`
-
-        If you want to change this value, just use this keyword passing the time in seconds.
-
-        Example:
-            | Change Wait Time | 0.5              |
-            | Change Wait Time | 200 milliseconds |
-            | Change Wait Time | 0:00:01.500      |
-        """
-        self.wait = self._convert_timeout(wait_time)
-
-    @keyword("Change Wait Time After Write")
-    def change_wait_time_after_write(self, wait_time_after_write: timedelta) -> None:
-        """To give the user time to see what is happening inside the mainframe, a "wait time after write" has
-        been created, which by default is set to 0 seconds. This is a sleep applied AFTER sending a string in these
-        keywords:
-
-        - `Write`
-        - `Write Bare`
-        - `Write in position`
-        - `Write Bare in position`
-
-        If you want to change this value, just use this keyword passing the time in seconds.
-
-        Note: This keyword is useful for debug purpose
-
-        Example:
-            | Change Wait Time After Write | 1             |
-            | Change Wait Time After Write | 0.5 seconds   |
-            | Change Wait Time After Write | 0:00:02       |
-        """
-        self.wait_write = self._convert_timeout(wait_time_after_write)
-
-    @keyword("Read")
-    def read(self, ypos: int, xpos: int, length: int) -> str:
-        """Get a string of ``length`` at screen co-ordinates ``ypos`` / ``xpos``.
-
-        Co-ordinates are 1 based, as listed in the status area of the terminal.
-
-        Example for read a string in the position y=8 / x=10 of a length 15:
-            | ${value} | Read | 8 | 10 | 15 |
-        """
-        self._check_limits(ypos, xpos)
-        # Checks if the user has passed a length that will be larger than the x limit of the screen.
-        if (xpos + length) > (80 + 1):
-            raise Exception(
-                "You have exceeded the x-axis limit of the mainframe screen"
-            )
-        string = self.mf.string_get(ypos, xpos, length)
-        return string
-
-    @keyword("Read All Screen")
-    def read_all_screen(self) -> str:
-        """Read the current screen and returns all content in one string.
-
-        This is useful if your automation scripts should take different routes depending
-        on a message shown on the screen.
-
-        Example:
-            | ${screen} | Read All Screen              |
-            | IF   | 'certain text' in '''${screen}''' |
-            |      | Do Something                      |
-            | ELSE |                                   |
-            |      | Do Something Else                 |
-            | END  |                                   |
-        """
-        return self._read_all_screen()
-
-    @keyword("Execute Command")
-    def execute_command(self, cmd: str) -> None:
-        """Execute a [http://x3270.bgp.nu/wc3270-man.html#Actions|x3270 command].
-
-        Example:
-            | Execute Command | Enter |
-            | Execute Command | Home |
-            | Execute Command | Tab |
-            | Execute Command | PF(1) |
-        """
-        self.mf.exec_command(cmd.encode("utf-8"))
-        time.sleep(self.wait)
-
-    @keyword("Set Screenshot Folder")
-    def set_screenshot_folder(self, path: str) -> None:
-        r"""Set a folder to keep the html files generated by the `Take Screenshot` keyword.
-
-        Note that the folder needs to exist before running your automation scripts. Else the images
-        will be stored in the ``${OUTPUT DIR}`` set by robotframework.
-
-        Example:
-            | Set Screenshot Folder | C:\\Temp\\Images |
-        """
-        if os.path.exists(os.path.normpath(os.path.join(self.output_folder, path))):
-            self.imgfolder = path
-        else:
-            logger.error('Given screenshots path "%s" does not exist' % path)
-            logger.warn('Screenshots will be saved in "%s"' % self.imgfolder)
-
-    @keyword("Take Screenshot")
-    def take_screenshot(
-        self, height: int = 410, width: int = 670, filename_prefix: str = "screenshot"
-    ) -> str:
-        """Generate a screenshot of the IBM 3270 Mainframe in a html format. The
-        default folder is the log folder of RobotFramework, if you want change see the `Set Screenshot Folder`.
-
-        The Screenshot is printed in a iframe log, with the values of height=410 and width=670, you
-        can change these values by passing them to the keyword.
-
-        The file name prefix can be set, the default is "screenshot".
-
-        The full file path is returned.
-
-        Example:
-            | ${filepath} | Take Screenshot |
-            | ${filepath} | Take Screenshot | height=500 | width=700 |
-            | Take Screenshot | height=500 | width=700 |
-            | Take Screenshot | filename_prefix=MyScreenshot |
-        """
-        extension = "html"
-        filename_sufix = round(time.time() * 1000)
-        filepath = os.path.join(
-            self.imgfolder, "%s_%s.%s" % (filename_prefix, filename_sufix, extension)
-        )
-        self.mf.save_screen(os.path.join(self.output_folder, filepath))
-        logger.write(
-            '<iframe src="%s" height="%s" width="%s"></iframe>'
-            % (filepath.replace("\\", "/"), height, width),
-            level="INFO",
-            html=True,
-        )
-        return filepath
-
-    @keyword("Wait Field Detected")
-    def wait_field_detected(self) -> None:
-        """Wait until the screen is ready, the cursor has been positioned
-        on a modifiable field, and the keyboard is unlocked.
-
-        Sometimes the server will "unlock" the keyboard but the screen
-        will not yet be ready.  In that case, an attempt to read or write to the
-        screen will result in a 'E' keyboard status because we tried to read from
-        a screen that is not ready yet.
-
-        Using this method tells the client to wait until a field is
-        detected and the cursor has been positioned on it.
-        """
-        self.mf.wait_for_field()
-
-    @keyword("Delete Char")
-    def delete_char(
-        self, ypos: Optional[int] = None, xpos: Optional[int] = None
-    ) -> None:
-        """Delete the character under the cursor. If you want to delete a character that is in
-        another position, simply pass the coordinates ``ypos`` / ``xpos``.
-
-        Co-ordinates are 1 based, as listed in the status area of the
-        terminal.
-
-        Example:
-            | Delete Char |
-            | Delete Char | ypos=9 | xpos=25 |
-        """
-        if ypos is not None and xpos is not None:
-            self.mf.move_to(ypos, xpos)
-        self.mf.exec_command(b"Delete")
-
-    @keyword("Delete Field")
-    def delete_field(
-        self, ypos: Optional[int] = None, xpos: Optional[int] = None
-    ) -> None:
-        """Delete the entire content of a field at the current cursor location and positions
-        the cursor at beginning of field. If you want to delete a field that is in
-        another position, simply pass the coordinates ``ypos`` / ``xpos`` of any part in the field.
-
-        Co-ordinates are 1 based, as listed in the status area of the
-        terminal.
-
-        Example:
-            | Delete Field |
-            | Delete Field | ypos=12 | xpos=6 |
-        """
-        if ypos is not None and xpos is not None:
-            self.mf.move_to(ypos, xpos)
-        self.mf.delete_field()
-
-    @keyword("Send Enter")
-    def send_enter(self) -> None:
-        """Send an Enter to the screen."""
-        self.mf.send_enter()
-        time.sleep(self.wait)
-
-    @keyword("Move Next Field")
-    def move_next_field(self) -> None:
-        """Move the cursor to the next input field. Equivalent to pressing the Tab key."""
-        self.mf.exec_command(b"Tab")
-
-    @keyword("Move Previous Field")
-    def move_previous_field(self) -> None:
-        """Move the cursor to the previous input field. Equivalent to pressing the Shift+Tab keys."""
-        self.mf.exec_command(b"BackTab")
-
-    @keyword("Send PF")
-    def send_PF(self, PF: str) -> None:
-        """Send a Program Function to the screen.
-
-        Example:
-               | Send PF | 3 |
-        """
-        self.mf.exec_command(("PF({0})").format(PF).encode("utf-8"))
-        time.sleep(self.wait)
-
-    @keyword("Write")
-    def write(self, txt: str) -> None:
-        """Send a string *and Enter* to the screen at the current cursor location.
-
-        Example:
-            | Write | something |
-        """
-        self._write(txt, enter=1)
-
-    @keyword("Write Bare")
-    def write_bare(self, txt: str) -> None:
-        """Send only the string to the screen at the current cursor location.
-
-        Example:
-            | Write Bare | something |
-        """
-        self._write(txt)
-
-    @keyword("Write In Position")
-    def write_in_position(self, txt: str, ypos: int, xpos: int) -> None:
-        """Send a string *and Enter* to the screen at screen co-ordinates ``ypos`` / ``xpos``.
-
-        Co-ordinates are 1 based, as listed in the status area of the
-        terminal.
-
-        Example:
-            | Write in Position | something | 9 | 11 |
-        """
-        self._write(txt, ypos, xpos, enter=1)
-
-    @keyword("Write Bare In Position")
-    def write_bare_in_position(self, txt: str, ypos: int, xpos: int):
-        """Send only the string to the screen at screen co-ordinates ``ypos`` / ``xpos``.
-
-        Co-ordinates are 1 based, as listed in the status area of the
-        terminal.
-
-        Example:
-            | Write Bare in Position | something | 9 | 11 |
-        """
-        self._write(txt, ypos, xpos)
-
-    def _write(
-        self,
-        txt: Any,
-        ypos: Optional[int] = None,
-        xpos: Optional[int] = None,
-        enter: int = 0,
-    ) -> None:
-        txt = txt.encode("unicode_escape")
-        if ypos is not None and xpos is not None:
-            self._check_limits(ypos, xpos)
-            self.mf.send_string(txt, ypos, xpos)
-        else:
-            self.mf.send_string(txt)
-        time.sleep(self.wait_write)
-        for i in range(enter):
-            self.mf.send_enter()
-            time.sleep(self.wait)
-
-    @keyword("Wait Until String")
-    def wait_until_string(
-        self, txt: str, timeout: timedelta = timedelta(seconds=5)
-    ) -> str:
-        """Wait until a string exists on the mainframe screen to perform the next step. If the string does not appear in
-        5 seconds, the keyword will raise an exception. You can define a different timeout.
-
-        Example:
-            | Wait Until String | something |
-            | Wait Until String | something | 10 |
-            | Wait Until String | something | 15 s |
-            | Wait Until String | something | 0:00:15 |
-        """
-        timeout = self._convert_timeout(timeout)
-        max_time = time.time() + timeout  # type: ignore
-        while time.time() < max_time:
-            result = self._search_string(str(txt))
-            if result:
-                return txt
-        raise Exception(f'String "{txt}" not found in {secs_to_timestr(timeout)}')
-
-    def _search_string(self, string: str, ignore_case: bool = False) -> bool:
-        """Search if a string exists on the mainframe screen and return True or False."""
-
-        def __read_screen(string: str, ignore_case: bool) -> bool:
-            for ypos in range(24):
-                line = self.mf.string_get(ypos + 1, 1, 80)
-                if ignore_case:
-                    line = line.lower()
-                if string in line:
-                    return True
-            return False
-
-        status = __read_screen(string, ignore_case)
-        return status
-
-    @keyword("Page Should Contain String")
-    def page_should_contain_string(
-        self, txt: str, ignore_case: bool = False, error_message: Optional[str] = None
-    ) -> None:
-        """Assert that a given string exists on the mainframe screen.
-
-        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
-
-        You can change the exception message by setting a custom string to error_message.
-
-        Example:
-            | Page Should Contain String | something |
-            | Page Should Contain String | someTHING | ignore_case=True                |
-            | Page Should Contain String | something | error_message=New error message |
-        """
-        message = f'The string "{txt}" was not found'
-        if error_message:
-            message = error_message
-        if ignore_case:
-            txt = txt.lower()
-        result = self._search_string(txt, ignore_case)
-        if not result:
-            raise Exception(message)
-        logger.info(f'The string "{txt}" was found')
-
-    @keyword("Page Should Not Contain String")
-    def page_should_not_contain_string(
-        self, txt: str, ignore_case: bool = False, error_message: Optional[str] = None
-    ) -> None:
-        """Assert that a given string does NOT exists on the mainframe screen.
-
-        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
-
-        You can change the exception message by setting a custom string to error_message.
-
-        Example:
-            | Page Should Not Contain String | something |
-            | Page Should Not Contain String | someTHING | ignore_case=True |
-            | Page Should Not Contain String | something | error_message=New error message |
-        """
-        message = f'The string "{txt}" was found'
-        if error_message:
-            message = error_message
-        if ignore_case:
-            txt = txt.lower()
-        result = self._search_string(txt, ignore_case)
-        if result:
-            raise Exception(message)
-
-    @keyword("Page Should Contain Any String")
-    def page_should_contain_any_string(
-        self,
-        list_string: List[str],
-        ignore_case: bool = False,
-        error_message: Optional[str] = None,
-    ) -> None:
-        """Assert that one of the strings in a given list exists on the mainframe screen.
-
-        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
-
-        You can change the exception message by setting a custom string to error_message.
-
-        Example:
-            | Page Should Contain Any String | ${list_of_string} |
-            | Page Should Contain Any String | ${list_of_string} | ignore_case=True |
-            | Page Should Contain Any String | ${list_of_string} | error_message=New error message |
-        """
-        message = f'The strings "{list_string}" were not found'
-        if error_message:
-            message = error_message
-        if ignore_case:
-            list_string = [item.lower() for item in list_string]
-        for string in list_string:
-            result = self._search_string(string, ignore_case)
-            if result:
-                break
-        if not result:
-            raise Exception(message)
-
-    @keyword("Page Should Not Contain Any String")
-    def page_should_not_contain_any_string(
-        self,
-        list_string: List[str],
-        ignore_case: bool = False,
-        error_message: Optional[str] = None,
-    ) -> None:
-        """Assert that none of the strings in a given list exists on the mainframe screen. If one or more of the
-        string are found, the keyword will raise a exception.
-
-        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
-
-        You can change the exception message by setting a custom string to error_message.
-
-        Example:
-            | Page Should Not Contain Any Strings | ${list_of_string} |
-            | Page Should Not Contain Any Strings | ${list_of_string} | ignore_case=True |
-            | Page Should Not Contain Any Strings | ${list_of_string} | error_message=New error message |
-        """
-        self._compare_all_list_with_screen_text(
-            list_string, ignore_case, error_message, should_match=False
-        )
-
-    @keyword("Page Should Contain All Strings")
-    def page_should_contain_all_strings(
-        self,
-        list_string: List[str],
-        ignore_case: bool = False,
-        error_message: Optional[str] = None,
-    ) -> None:
-        """Assert that all of the strings in a given list exist on the mainframe screen.
-
-        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
-
-        You can change the exception message by setting a custom string to error_message.
-
-        Example:
-            | Page Should Contain All Strings | ${list_of_string} |
-            | Page Should Contain All Strings | ${list_of_string} | ignore_case=True |
-            | Page Should Contain All Strings | ${list_of_string} | error_message=New error message |
-        """
-        self._compare_all_list_with_screen_text(
-            list_string, ignore_case, error_message, should_match=True
-        )
-
-    @keyword("Page Should Not Contain All Strings")
-    def page_should_not_contain_all_strings(
-        self,
-        list_string: List[str],
-        ignore_case: bool = False,
-        error_message: Optional[str] = None,
-    ) -> None:
-        """Fails if one of the strings in a given list exists on the mainframe screen. If one of the string
-        are found, the keyword will raise a exception.
-
-        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
-
-        You can change the exception message by setting a custom string to error_message.
-
-        Example:
-            | Page Should Not Contain All Strings | ${list_of_string} |
-            | Page Should Not Contain All Strings | ${list_of_string} | ignore_case=True |
-            | Page Should Not Contain All Strings | ${list_of_string} | error_message=New error message |
-        """
-        message = error_message
-        if ignore_case:
-            list_string = [item.lower() for item in list_string]
-        for string in list_string:
-            result = self._search_string(string, ignore_case)
-            if result:
-                if message is None:
-                    message = f'The string "{string}" was found'
-                raise Exception(message)
-
-    @keyword("Page Should Contain String X Times")
-    def page_should_contain_string_x_times(
-        self,
-        txt: str,
-        number: int,
-        ignore_case: bool = False,
-        error_message: Optional[str] = None,
-    ) -> None:
-        """Asserts that the entered string appears the desired number of times on the mainframe screen.
-
-        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
-
-        You can change the exception message by setting a custom string to error_message.
-
-        Example:
-               | Page Should Contain String X Times | something | 3 |
-               | Page Should Contain String X Times | someTHING | 3 | ignore_case=True |
-               | Page Should Contain String X Times | something | 3 | error_message=New error message |
-        """
-        message = error_message
-        number = number
-        all_screen = self._read_all_screen()
-        if ignore_case:
-            txt = txt.lower()
-            all_screen = all_screen.lower()
-        number_of_times = all_screen.count(txt)
-        if number_of_times != number:
-            if message is None:
-                message = f'The string "{txt}" was not found "{number}" times, it appears "{number_of_times}" times'
-            raise Exception(message)
-        logger.info(f'The string "{txt}" was found "{number}" times')
-
-    @keyword("Page Should Match Regex")
-    def page_should_match_regex(self, regex_pattern: str) -> None:
-        r"""Fails if string does not match pattern as a regular expression. Regular expression check is
-        implemented using the Python [https://docs.python.org/2/library/re.html|re module]. Python's
-        regular expression syntax is derived from Perl, and it is thus also very similar to the syntax used,
-        for example, in Java, Ruby and .NET.
-
-        Backslash is an escape character in the test data, and possible backslashes in the pattern must
-        thus be escaped with another backslash (e.g. \\d\\w+).
-        """
-        page_text = self._read_all_screen()
-        if not re.findall(regex_pattern, page_text, re.MULTILINE):
-            raise Exception(f'No matches found for "{regex_pattern}" pattern')
-
-    @keyword("Page Should Not Match Regex")
-    def page_should_not_match_regex(self, regex_pattern: str) -> None:
-        r"""Fails if string does match pattern as a regular expression. Regular expression check is
-        implemented using the Python [https://docs.python.org/2/library/re.html|re module]. Python's
-        regular expression syntax is derived from Perl, and it is thus also very similar to the syntax used,
-        for example, in Java, Ruby and .NET.
-
-        Backslash is an escape character in the test data, and possible backslashes in the pattern must
-        thus be escaped with another backslash (e.g. \\d\\w+).
-        """
-        page_text = self._read_all_screen()
-        if re.findall(regex_pattern, page_text, re.MULTILINE):
-            raise Exception(f'There are matches found for "{regex_pattern}" pattern')
-
-    @keyword("Page Should Contain Match")
-    def page_should_contain_match(
-        self, txt: str, ignore_case: bool = False, error_message: Optional[str] = None
-    ) -> None:
-        """Assert that the text displayed on the mainframe screen matches the given pattern.
-
-        Pattern matching is similar to matching files in a shell, and it is always case sensitive.
-        In the pattern, * matches anything and ? matches any single character.
-
-        Note that for this keyword the entire screen is considered a string. So if you want to search
-        for the string "something" and it is somewhere other than at the beginning or end of the screen, it
-        should be reported as follows: **something**
-
-        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
-
-        You can change the exception message by setting a custom string to error_message.
-
-        Example:
-            | Page Should Contain Match | **something** |
-            | Page Should Contain Match | **so???hing** |
-            | Page Should Contain Match | **someTHING** | ignore_case=True |
-            | Page Should Contain Match | **something** | error_message=New error message |
-        """
-        message = error_message
-        all_screen = self._read_all_screen()
-        if ignore_case:
-            txt = txt.lower()
-            all_screen = all_screen.lower()
-        matcher = Matcher(txt, caseless=False, spaceless=False)
-        result = matcher.match(all_screen)
-        if not result:
-            if message is None:
-                message = f'No matches found for "{txt}" pattern'
-            raise Exception(message)
-
-    @keyword("Page Should Not Contain Match")
-    def page_should_not_contain_match(
-        self, txt: str, ignore_case: bool = False, error_message: Optional[str] = None
-    ) -> None:
-        """Assert that the text displayed on the mainframe screen does NOT match the given pattern.
-
-        Pattern matching is similar to matching files in a shell, and it is always case sensitive.
-        In the pattern, * matches anything and ? matches any single character.
-
-        Note that for this keyword the entire screen is considered a string. So if you want to search
-        for the string "something" and it is somewhere other than at the beginning or end of the screen, it
-        should be reported as follows: **something**
-
-        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
-
-        You can change the exception message by setting a custom string to error_message.
-
-        Example:
-            | Page Should Not Contain Match | **something** |
-            | Page Should Not Contain Match | **so???hing** |
-            | Page Should Not Contain Match | **someTHING** | ignore_case=True |
-            | Page Should Not Contain Match | **something** | error_message=New error message |
-        """
-        message = error_message
-        all_screen = self._read_all_screen()
-        if ignore_case:
-            txt = txt.lower()
-            all_screen = all_screen.lower()
-        matcher = Matcher(txt, caseless=False, spaceless=False)
-        result = matcher.match(all_screen)
-        if result:
-            if message is None:
-                message = f'There are matches found for "{txt}" pattern'
-            raise Exception(message)
-
-    def _read_all_screen(self) -> str:
-        """Read all the mainframe screen and return in a single string."""
-        full_text = ""
-        for ypos in range(24):
-            full_text += self.mf.string_get(ypos + 1, 1, 80)
-        return full_text
-
-    def _compare_all_list_with_screen_text(
-        self,
-        list_string: List[str],
-        ignore_case: bool,
-        message: Optional[str],
-        should_match: bool,
-    ) -> None:
-        if ignore_case:
-            list_string = [item.lower() for item in list_string]
-        for string in list_string:
-            result = self._search_string(string, ignore_case)
-            if not should_match and result:
-                if message is None:
-                    message = f'The string "{string}" was found'
-                raise Exception(message)
-            elif should_match and not result:
-                if message is None:
-                    message = f'The string "{string}" was not found'
-                raise Exception(message)
-
-    @staticmethod
-    def _check_limits(ypos: int, xpos: int):
-        """Checks if the user has passed some coordinate y / x greater than that existing in the mainframe"""
-        if ypos > 24:
-            raise Exception(
-                "You have exceeded the y-axis limit of the mainframe screen"
-            )
-        if xpos > 80:
-            raise Exception(
-                "You have exceeded the x-axis limit of the mainframe screen"
-            )
+import os
+import re
+import shlex
+import socket
+import time
+from datetime import timedelta
+from os import name as os_name
+from typing import Any, List, Optional, Union
+
+from robot.api import logger
+from robot.api.deco import keyword
+from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
+from robot.utils import Matcher, secs_to_timestr, timestr_to_secs
+
+from .py3270 import Emulator
+
+
+class X3270(object):
+    def __init__(
+        self,
+        visible: bool,
+        timeout: timedelta,
+        wait_time: timedelta,
+        wait_time_after_write: timedelta,
+        img_folder: str,
+    ) -> None:
+        self.visible = visible
+        self.timeout = self._convert_timeout(timeout)
+        self.wait = self._convert_timeout(wait_time)
+        self.wait_write = self._convert_timeout(wait_time_after_write)
+        self.imgfolder = img_folder
+        self.mf: Emulator = None  # type: ignore
+        # Try Catch to run in Pycharm, and make a documentation in libdoc with no error
+        try:
+            self.output_folder = BuiltIn().get_variable_value("${OUTPUT DIR}")
+        except RobotNotRunningError:
+            self.output_folder = os.getcwd()
+
+    def _convert_timeout(self, time):
+        if isinstance(time, timedelta):
+            return time.total_seconds()
+        return timestr_to_secs(time, round_to=None)
+
+    @keyword("Change Timeout")
+    def change_timeout(self, seconds: timedelta) -> None:
+        """
+        Change the timeout for connection in seconds.
+
+        Example:
+            | Change Timeout | 3 seconds |
+        """
+        self.timeout = self._convert_timeout(seconds)
+
+    @keyword("Open Connection")
+    def open_connection(
+        self,
+        host: str,
+        LU: Optional[str] = None,
+        port: int = 23,
+        extra_args: Optional[Union[List[str], os.PathLike]] = None,
+    ):
+        """Create a connection to an IBM3270 mainframe with the default port 23.
+        To establish a connection, only the hostname is required. Optional parameters include logical unit name (LU) and port.
+
+        Additional configuration data can be provided through the `extra_args` parameter.
+        `extra_args` accepts either a list or a path to a file containing [https://x3270.miraheze.org/wiki/Category:Command-line_options|x3270 command line options].
+
+        Entries in the argfile can be on one line or multiple lines. Lines starting with "#" are considered comments.
+        Arguments containing whitespace must be enclosed in single or double quotes.
+
+        | # example_argfile_oneline.txt
+        | -accepthostname myhost.com
+
+        | # example_argfile_multiline.txt
+        | -xrm "wc3270.acceptHostname: myhost.com"
+        | # this is a comment
+        | -charset french
+        | -port 992
+
+        Please ensure that the arguments provided are available for your specific x3270 application and version.
+        Refer to the [https://x3270.miraheze.org/wiki/Wc3270/Command-line_options|wc3270 command line options] for a subset of available options.
+
+        Note: If you specify the port with the `-port` command-line option in `extra_args` (or use the -xrm resource command for it),
+        it will take precedence over the `port` argument provided in the `Open Connection` keyword.
+
+        Example:
+            | Open Connection | Hostname |
+            | Open Connection | Hostname | LU=LUname |
+            | Open Connection | Hostname | port=992 |
+            | @{extra_args}   | Create List | -accepthostname | myhost.com | -cafile | ${CURDIR}/cafile.crt |
+            | Append To List  | ${extra_args} | -port | 992 |
+            | Open Connection | Hostname | extra_args=${extra_args} |
+            | Open Connection | Hostname | extra_args=${CURDIR}/argfile.txt |
+        """
+        if self.mf:
+            self.close_connection()
+        extra_args = self._process_args(extra_args)
+        self.mf = Emulator(self.visible, self.timeout, extra_args)
+        host_string = f"{LU}@{host}" if LU else host
+        if self._port_in_extra_args(extra_args):
+            if port != 23:
+                logger.warn(
+                    "The connection port has been specified both in the `port` argument and in `extra_args`. "
+                    "The port specified in `extra_args` will take precedence over the `port` argument. "
+                    "To avoid this warning, you can either remove the port command-line option from `extra_args`, "
+                    "or leave the `port` argument at its default value of 23."
+                )
+            self.mf.connect(host_string)
+        else:
+            self.mf.connect(f"{host_string}:{port}")
+
+    def _process_args(self, args) -> list:
+        processed_args = []
+        if not args:
+            return []
+        elif isinstance(args, list):
+            processed_args = args
+        elif isinstance(args, os.PathLike) or isinstance(args, str):
+            with open(args) as file:
+                for line in file:
+                    if line.lstrip().startswith("#"):
+                        continue
+                    for arg in shlex.split(line):
+                        processed_args.append(arg)
+        return processed_args
+
+    def _port_in_extra_args(self, args) -> bool:
+        if not args:
+            return False
+        for arg in args:
+            if arg == "-port" or ".port" in arg:
+                return True
+        return False
+
+    @keyword("Open Connection From Session File")
+    def open_connection_from_session_file(self, session_file: os.PathLike):
+        """Create a connection to an IBM3270 mainframe using a [https://x3270.miraheze.org/wiki/Session_file|session file].
+
+        The session file contains [https://x3270.miraheze.org/wiki/Category:Resources|resources (settings)] for a specific host session.
+        The only mandatory setting required to establish the connection is the [https://x3270.miraheze.org/wiki/Hostname_resource|hostname resource].
+
+        This keyword is an alternative to `Open Connection`. Please note that the Robot-Framework-Mainframe-3270-Library
+        currently only supports model "2". Specifying any other model will result in a failure.
+
+        For more information on session file syntax and detailed examples, please consult the [https://x3270.miraheze.org/wiki/Session_file|x3270 wiki].
+
+        Example:
+        | Open Connection From Session File | ${CURDIR}/session.wc3270 |
+
+        where the content of `session.wc3270` is:
+        | wc3270.hostname: myhost.com:23
+        | wc3270.model: 2
+        """
+        if self.mf:
+            self.close_connection()
+        self._check_session_file_extension(session_file)
+        self._check_contains_hostname(session_file)
+        self._check_model(session_file)
+        if os_name == "nt" and self.visible:
+            self.mf = Emulator(self.visible, self.timeout)
+            self.mf.connect(str(session_file))
+        else:
+            self.mf = Emulator(self.visible, self.timeout, [str(session_file)])
+
+    def _check_session_file_extension(self, session_file):
+        file_extension = str(session_file).rsplit(".")[-1]
+        expected_extensions = {
+            ("nt", True): "wc3270",
+            ("nt", False): "ws3270",
+            ("posix", True): "x3270",
+            ("posix", False): "s3270",
+        }
+        expected_extension = expected_extensions.get((os_name, self.visible))
+        if file_extension != expected_extension:
+            raise ValueError(
+                f"Based on the emulator that you are using, "
+                f'the session file extension has to be ".{expected_extension}", '
+                f'but it was ".{file_extension}"'
+            )
+
+    def _check_contains_hostname(self, session_file):
+        with open(session_file) as file:
+            if "hostname:" not in file.read():
+                raise ValueError(
+                    "Your session file needs to specify the hostname resource "
+                    "to set up the connection. "
+                    "An example for wc3270 looks like this: \n"
+                    "wc3270.hostname: myhost.com\n"
+                )
+
+    def _check_model(self, session_file):
+        with open(session_file) as file:
+            pattern = re.compile(r"[wcxs3270.*]+model:\s*([327892345E-]+)")
+            match = pattern.findall(file.read())
+            if not match:
+                return
+            elif match[-1] == "2":
+                return
+            else:
+                raise ValueError(
+                    f'Robot-Framework-Mainframe-3270-Library currently only supports model "2", '
+                    f'the model you specified in your session file was "{match[-1]}". '
+                    f'Please change it to "2", using either the session wizard if you are on Windows, '
+                    f'or by editing the model resource like this "*model: 2"'
+                )
+
+    @keyword("Close Connection")
+    def close_connection(self) -> None:
+        """Disconnect from the host."""
+        try:
+            self.mf.terminate()
+        except socket.error:
+            pass
+        self.mf = None  # type: ignore
+
+    @keyword("Change Wait Time")
+    def change_wait_time(self, wait_time: timedelta) -> None:
+        """To give time for the mainframe screen to be "drawn" and receive the next commands, a "wait time" has been
+        created, which by default is set to 0.5 seconds. This is a sleep applied AFTER the following keywords:
+
+        - `Execute Command`
+        - `Send Enter`
+        - `Send PF`
+        - `Write`
+        - `Write in position`
+
+        If you want to change this value, just use this keyword passing the time in seconds.
+
+        Example:
+            | Change Wait Time | 0.5              |
+            | Change Wait Time | 200 milliseconds |
+            | Change Wait Time | 0:00:01.500      |
+        """
+        self.wait = self._convert_timeout(wait_time)
+
+    @keyword("Change Wait Time After Write")
+    def change_wait_time_after_write(self, wait_time_after_write: timedelta) -> None:
+        """To give the user time to see what is happening inside the mainframe, a "wait time after write" has
+        been created, which by default is set to 0 seconds. This is a sleep applied AFTER sending a string in these
+        keywords:
+
+        - `Write`
+        - `Write Bare`
+        - `Write in position`
+        - `Write Bare in position`
+
+        If you want to change this value, just use this keyword passing the time in seconds.
+
+        Note: This keyword is useful for debug purpose
+
+        Example:
+            | Change Wait Time After Write | 1             |
+            | Change Wait Time After Write | 0.5 seconds   |
+            | Change Wait Time After Write | 0:00:02       |
+        """
+        self.wait_write = self._convert_timeout(wait_time_after_write)
+
+    @keyword("Read")
+    def read(self, ypos: int, xpos: int, length: int) -> str:
+        """Get a string of ``length`` at screen co-ordinates ``ypos`` / ``xpos``.
+
+        Co-ordinates are 1 based, as listed in the status area of the terminal.
+
+        Example for read a string in the position y=8 / x=10 of a length 15:
+            | ${value} | Read | 8 | 10 | 15 |
+        """
+        self._check_limits(ypos, xpos)
+        # Checks if the user has passed a length that will be larger than the x limit of the screen.
+        if (xpos + length) > (80 + 1):
+            raise Exception(
+                "You have exceeded the x-axis limit of the mainframe screen"
+            )
+        string = self.mf.string_get(ypos, xpos, length)
+        return string
+
+    @keyword("Read All Screen")
+    def read_all_screen(self) -> str:
+        """Read the current screen and returns all content in one string.
+
+        This is useful if your automation scripts should take different routes depending
+        on a message shown on the screen.
+
+        Example:
+            | ${screen} | Read All Screen              |
+            | IF   | 'certain text' in '''${screen}''' |
+            |      | Do Something                      |
+            | ELSE |                                   |
+            |      | Do Something Else                 |
+            | END  |                                   |
+        """
+        return self._read_all_screen()
+
+    @keyword("Execute Command")
+    def execute_command(self, cmd: str) -> None:
+        """Execute a [http://x3270.bgp.nu/wc3270-man.html#Actions|x3270 command].
+
+        Example:
+            | Execute Command | Enter |
+            | Execute Command | Home |
+            | Execute Command | Tab |
+            | Execute Command | PF(1) |
+        """
+        self.mf.exec_command(cmd.encode("utf-8"))
+        time.sleep(self.wait)
+
+    @keyword("Set Screenshot Folder")
+    def set_screenshot_folder(self, path: str) -> None:
+        r"""Set a folder to keep the html files generated by the `Take Screenshot` keyword.
+
+        Note that the folder needs to exist before running your automation scripts. Else the images
+        will be stored in the ``${OUTPUT DIR}`` set by robotframework.
+
+        Example:
+            | Set Screenshot Folder | C:\\Temp\\Images |
+        """
+        if os.path.exists(os.path.normpath(os.path.join(self.output_folder, path))):
+            self.imgfolder = path
+        else:
+            logger.error('Given screenshots path "%s" does not exist' % path)
+            logger.warn('Screenshots will be saved in "%s"' % self.imgfolder)
+
+    @keyword("Take Screenshot")
+    def take_screenshot(
+        self, height: int = 410, width: int = 670, filename_prefix: str = "screenshot"
+    ) -> str:
+        """Generate a screenshot of the IBM 3270 Mainframe in a html format. The
+        default folder is the log folder of RobotFramework, if you want change see the `Set Screenshot Folder`.
+
+        The Screenshot is printed in a iframe log, with the values of height=410 and width=670, you
+        can change these values by passing them to the keyword.
+
+        The file name prefix can be set, the default is "screenshot".
+
+        The full file path is returned.
+
+        Example:
+            | ${filepath} | Take Screenshot |
+            | ${filepath} | Take Screenshot | height=500 | width=700 |
+            | Take Screenshot | height=500 | width=700 |
+            | Take Screenshot | filename_prefix=MyScreenshot |
+        """
+        extension = "html"
+        filename_sufix = round(time.time() * 1000)
+        filepath = os.path.join(
+            self.imgfolder, "%s_%s.%s" % (filename_prefix, filename_sufix, extension)
+        )
+        self.mf.save_screen(os.path.join(self.output_folder, filepath))
+        logger.write(
+            '<iframe src="%s" height="%s" width="%s"></iframe>'
+            % (filepath.replace("\\", "/"), height, width),
+            level="INFO",
+            html=True,
+        )
+        return filepath
+
+    @keyword("Wait Field Detected")
+    def wait_field_detected(self) -> None:
+        """Wait until the screen is ready, the cursor has been positioned
+        on a modifiable field, and the keyboard is unlocked.
+
+        Sometimes the server will "unlock" the keyboard but the screen
+        will not yet be ready.  In that case, an attempt to read or write to the
+        screen will result in a 'E' keyboard status because we tried to read from
+        a screen that is not ready yet.
+
+        Using this method tells the client to wait until a field is
+        detected and the cursor has been positioned on it.
+        """
+        self.mf.wait_for_field()
+
+    @keyword("Delete Char")
+    def delete_char(
+        self, ypos: Optional[int] = None, xpos: Optional[int] = None
+    ) -> None:
+        """Delete the character under the cursor. If you want to delete a character that is in
+        another position, simply pass the coordinates ``ypos`` / ``xpos``.
+
+        Co-ordinates are 1 based, as listed in the status area of the
+        terminal.
+
+        Example:
+            | Delete Char |
+            | Delete Char | ypos=9 | xpos=25 |
+        """
+        if ypos is not None and xpos is not None:
+            self.mf.move_to(ypos, xpos)
+        self.mf.exec_command(b"Delete")
+
+    @keyword("Delete Field")
+    def delete_field(
+        self, ypos: Optional[int] = None, xpos: Optional[int] = None
+    ) -> None:
+        """Delete the entire content of a field at the current cursor location and positions
+        the cursor at beginning of field. If you want to delete a field that is in
+        another position, simply pass the coordinates ``ypos`` / ``xpos`` of any part in the field.
+
+        Co-ordinates are 1 based, as listed in the status area of the
+        terminal.
+
+        Example:
+            | Delete Field |
+            | Delete Field | ypos=12 | xpos=6 |
+        """
+        if ypos is not None and xpos is not None:
+            self.mf.move_to(ypos, xpos)
+        self.mf.delete_field()
+
+    @keyword("Send Enter")
+    def send_enter(self) -> None:
+        """Send an Enter to the screen."""
+        self.mf.send_enter()
+        time.sleep(self.wait)
+
+    @keyword("Move Next Field")
+    def move_next_field(self) -> None:
+        """Move the cursor to the next input field. Equivalent to pressing the Tab key."""
+        self.mf.exec_command(b"Tab")
+
+    @keyword("Move Previous Field")
+    def move_previous_field(self) -> None:
+        """Move the cursor to the previous input field. Equivalent to pressing the Shift+Tab keys."""
+        self.mf.exec_command(b"BackTab")
+
+    @keyword("Send PF")
+    def send_PF(self, PF: str) -> None:
+        """Send a Program Function to the screen.
+
+        Example:
+               | Send PF | 3 |
+        """
+        self.mf.exec_command(("PF({0})").format(PF).encode("utf-8"))
+        time.sleep(self.wait)
+
+    @keyword("Write")
+    def write(self, txt: str) -> None:
+        """Send a string *and Enter* to the screen at the current cursor location.
+
+        Example:
+            | Write | something |
+        """
+        self._write(txt, enter=1)
+
+    @keyword("Write Bare")
+    def write_bare(self, txt: str) -> None:
+        """Send only the string to the screen at the current cursor location.
+
+        Example:
+            | Write Bare | something |
+        """
+        self._write(txt)
+
+    @keyword("Write In Position")
+    def write_in_position(self, txt: str, ypos: int, xpos: int) -> None:
+        """Send a string *and Enter* to the screen at screen co-ordinates ``ypos`` / ``xpos``.
+
+        Co-ordinates are 1 based, as listed in the status area of the
+        terminal.
+
+        Example:
+            | Write in Position | something | 9 | 11 |
+        """
+        self._write(txt, ypos, xpos, enter=1)
+
+    @keyword("Write Bare In Position")
+    def write_bare_in_position(self, txt: str, ypos: int, xpos: int):
+        """Send only the string to the screen at screen co-ordinates ``ypos`` / ``xpos``.
+
+        Co-ordinates are 1 based, as listed in the status area of the
+        terminal.
+
+        Example:
+            | Write Bare in Position | something | 9 | 11 |
+        """
+        self._write(txt, ypos, xpos)
+
+    def _write(
+        self,
+        txt: Any,
+        ypos: Optional[int] = None,
+        xpos: Optional[int] = None,
+        enter: int = 0,
+    ) -> None:
+        txt = txt.encode("unicode_escape")
+        if ypos is not None and xpos is not None:
+            self._check_limits(ypos, xpos)
+            self.mf.send_string(txt, ypos, xpos)
+        else:
+            self.mf.send_string(txt)
+        time.sleep(self.wait_write)
+        for i in range(enter):
+            self.mf.send_enter()
+            time.sleep(self.wait)
+
+    @keyword("Wait Until String")
+    def wait_until_string(
+        self, txt: str, timeout: timedelta = timedelta(seconds=5)
+    ) -> str:
+        """Wait until a string exists on the mainframe screen to perform the next step. If the string does not appear in
+        5 seconds, the keyword will raise an exception. You can define a different timeout.
+
+        Example:
+            | Wait Until String | something |
+            | Wait Until String | something | 10 |
+            | Wait Until String | something | 15 s |
+            | Wait Until String | something | 0:00:15 |
+        """
+        timeout = self._convert_timeout(timeout)
+        max_time = time.time() + timeout  # type: ignore
+        while time.time() < max_time:
+            result = self._search_string(str(txt))
+            if result:
+                return txt
+        raise Exception(f'String "{txt}" not found in {secs_to_timestr(timeout)}')
+
+    def _search_string(self, string: str, ignore_case: bool = False) -> bool:
+        """Search if a string exists on the mainframe screen and return True or False."""
+
+        def __read_screen(string: str, ignore_case: bool) -> bool:
+            for ypos in range(24):
+                line = self.mf.string_get(ypos + 1, 1, 80)
+                if ignore_case:
+                    line = line.lower()
+                if string in line:
+                    return True
+            return False
+
+        status = __read_screen(string, ignore_case)
+        return status
+
+    @keyword("Page Should Contain String")
+    def page_should_contain_string(
+        self, txt: str, ignore_case: bool = False, error_message: Optional[str] = None
+    ) -> None:
+        """Assert that a given string exists on the mainframe screen.
+
+        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
+
+        You can change the exception message by setting a custom string to error_message.
+
+        Example:
+            | Page Should Contain String | something |
+            | Page Should Contain String | someTHING | ignore_case=True                |
+            | Page Should Contain String | something | error_message=New error message |
+        """
+        message = f'The string "{txt}" was not found'
+        if error_message:
+            message = error_message
+        if ignore_case:
+            txt = txt.lower()
+        result = self._search_string(txt, ignore_case)
+        if not result:
+            raise Exception(message)
+        logger.info(f'The string "{txt}" was found')
+
+    @keyword("Page Should Not Contain String")
+    def page_should_not_contain_string(
+        self, txt: str, ignore_case: bool = False, error_message: Optional[str] = None
+    ) -> None:
+        """Assert that a given string does NOT exists on the mainframe screen.
+
+        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
+
+        You can change the exception message by setting a custom string to error_message.
+
+        Example:
+            | Page Should Not Contain String | something |
+            | Page Should Not Contain String | someTHING | ignore_case=True |
+            | Page Should Not Contain String | something | error_message=New error message |
+        """
+        message = f'The string "{txt}" was found'
+        if error_message:
+            message = error_message
+        if ignore_case:
+            txt = txt.lower()
+        result = self._search_string(txt, ignore_case)
+        if result:
+            raise Exception(message)
+
+    @keyword("Page Should Contain Any String")
+    def page_should_contain_any_string(
+        self,
+        list_string: List[str],
+        ignore_case: bool = False,
+        error_message: Optional[str] = None,
+    ) -> None:
+        """Assert that one of the strings in a given list exists on the mainframe screen.
+
+        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
+
+        You can change the exception message by setting a custom string to error_message.
+
+        Example:
+            | Page Should Contain Any String | ${list_of_string} |
+            | Page Should Contain Any String | ${list_of_string} | ignore_case=True |
+            | Page Should Contain Any String | ${list_of_string} | error_message=New error message |
+        """
+        message = f'The strings "{list_string}" were not found'
+        if error_message:
+            message = error_message
+        if ignore_case:
+            list_string = [item.lower() for item in list_string]
+        for string in list_string:
+            result = self._search_string(string, ignore_case)
+            if result:
+                break
+        if not result:
+            raise Exception(message)
+
+    @keyword("Page Should Not Contain Any String")
+    def page_should_not_contain_any_string(
+        self,
+        list_string: List[str],
+        ignore_case: bool = False,
+        error_message: Optional[str] = None,
+    ) -> None:
+        """Assert that none of the strings in a given list exists on the mainframe screen. If one or more of the
+        string are found, the keyword will raise a exception.
+
+        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
+
+        You can change the exception message by setting a custom string to error_message.
+
+        Example:
+            | Page Should Not Contain Any Strings | ${list_of_string} |
+            | Page Should Not Contain Any Strings | ${list_of_string} | ignore_case=True |
+            | Page Should Not Contain Any Strings | ${list_of_string} | error_message=New error message |
+        """
+        self._compare_all_list_with_screen_text(
+            list_string, ignore_case, error_message, should_match=False
+        )
+
+    @keyword("Page Should Contain All Strings")
+    def page_should_contain_all_strings(
+        self,
+        list_string: List[str],
+        ignore_case: bool = False,
+        error_message: Optional[str] = None,
+    ) -> None:
+        """Assert that all of the strings in a given list exist on the mainframe screen.
+
+        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
+
+        You can change the exception message by setting a custom string to error_message.
+
+        Example:
+            | Page Should Contain All Strings | ${list_of_string} |
+            | Page Should Contain All Strings | ${list_of_string} | ignore_case=True |
+            | Page Should Contain All Strings | ${list_of_string} | error_message=New error message |
+        """
+        self._compare_all_list_with_screen_text(
+            list_string, ignore_case, error_message, should_match=True
+        )
+
+    @keyword("Page Should Not Contain All Strings")
+    def page_should_not_contain_all_strings(
+        self,
+        list_string: List[str],
+        ignore_case: bool = False,
+        error_message: Optional[str] = None,
+    ) -> None:
+        """Fails if one of the strings in a given list exists on the mainframe screen. If one of the string
+        are found, the keyword will raise a exception.
+
+        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
+
+        You can change the exception message by setting a custom string to error_message.
+
+        Example:
+            | Page Should Not Contain All Strings | ${list_of_string} |
+            | Page Should Not Contain All Strings | ${list_of_string} | ignore_case=True |
+            | Page Should Not Contain All Strings | ${list_of_string} | error_message=New error message |
+        """
+        message = error_message
+        if ignore_case:
+            list_string = [item.lower() for item in list_string]
+        for string in list_string:
+            result = self._search_string(string, ignore_case)
+            if result:
+                if message is None:
+                    message = f'The string "{string}" was found'
+                raise Exception(message)
+
+    @keyword("Page Should Contain String X Times")
+    def page_should_contain_string_x_times(
+        self,
+        txt: str,
+        number: int,
+        ignore_case: bool = False,
+        error_message: Optional[str] = None,
+    ) -> None:
+        """Asserts that the entered string appears the desired number of times on the mainframe screen.
+
+        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
+
+        You can change the exception message by setting a custom string to error_message.
+
+        Example:
+               | Page Should Contain String X Times | something | 3 |
+               | Page Should Contain String X Times | someTHING | 3 | ignore_case=True |
+               | Page Should Contain String X Times | something | 3 | error_message=New error message |
+        """
+        message = error_message
+        number = number
+        all_screen = self._read_all_screen()
+        if ignore_case:
+            txt = txt.lower()
+            all_screen = all_screen.lower()
+        number_of_times = all_screen.count(txt)
+        if number_of_times != number:
+            if message is None:
+                message = f'The string "{txt}" was not found "{number}" times, it appears "{number_of_times}" times'
+            raise Exception(message)
+        logger.info(f'The string "{txt}" was found "{number}" times')
+
+    @keyword("Page Should Match Regex")
+    def page_should_match_regex(self, regex_pattern: str) -> None:
+        r"""Fails if string does not match pattern as a regular expression. Regular expression check is
+        implemented using the Python [https://docs.python.org/2/library/re.html|re module]. Python's
+        regular expression syntax is derived from Perl, and it is thus also very similar to the syntax used,
+        for example, in Java, Ruby and .NET.
+
+        Backslash is an escape character in the test data, and possible backslashes in the pattern must
+        thus be escaped with another backslash (e.g. \\d\\w+).
+        """
+        page_text = self._read_all_screen()
+        if not re.findall(regex_pattern, page_text, re.MULTILINE):
+            raise Exception(f'No matches found for "{regex_pattern}" pattern')
+
+    @keyword("Page Should Not Match Regex")
+    def page_should_not_match_regex(self, regex_pattern: str) -> None:
+        r"""Fails if string does match pattern as a regular expression. Regular expression check is
+        implemented using the Python [https://docs.python.org/2/library/re.html|re module]. Python's
+        regular expression syntax is derived from Perl, and it is thus also very similar to the syntax used,
+        for example, in Java, Ruby and .NET.
+
+        Backslash is an escape character in the test data, and possible backslashes in the pattern must
+        thus be escaped with another backslash (e.g. \\d\\w+).
+        """
+        page_text = self._read_all_screen()
+        if re.findall(regex_pattern, page_text, re.MULTILINE):
+            raise Exception(f'There are matches found for "{regex_pattern}" pattern')
+
+    @keyword("Page Should Contain Match")
+    def page_should_contain_match(
+        self, txt: str, ignore_case: bool = False, error_message: Optional[str] = None
+    ) -> None:
+        """Assert that the text displayed on the mainframe screen matches the given pattern.
+
+        Pattern matching is similar to matching files in a shell, and it is always case sensitive.
+        In the pattern, * matches anything and ? matches any single character.
+
+        Note that for this keyword the entire screen is considered a string. So if you want to search
+        for the string "something" and it is somewhere other than at the beginning or end of the screen, it
+        should be reported as follows: **something**
+
+        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
+
+        You can change the exception message by setting a custom string to error_message.
+
+        Example:
+            | Page Should Contain Match | **something** |
+            | Page Should Contain Match | **so???hing** |
+            | Page Should Contain Match | **someTHING** | ignore_case=True |
+            | Page Should Contain Match | **something** | error_message=New error message |
+        """
+        message = error_message
+        all_screen = self._read_all_screen()
+        if ignore_case:
+            txt = txt.lower()
+            all_screen = all_screen.lower()
+        matcher = Matcher(txt, caseless=False, spaceless=False)
+        result = matcher.match(all_screen)
+        if not result:
+            if message is None:
+                message = f'No matches found for "{txt}" pattern'
+            raise Exception(message)
+
+    @keyword("Page Should Not Contain Match")
+    def page_should_not_contain_match(
+        self, txt: str, ignore_case: bool = False, error_message: Optional[str] = None
+    ) -> None:
+        """Assert that the text displayed on the mainframe screen does NOT match the given pattern.
+
+        Pattern matching is similar to matching files in a shell, and it is always case sensitive.
+        In the pattern, * matches anything and ? matches any single character.
+
+        Note that for this keyword the entire screen is considered a string. So if you want to search
+        for the string "something" and it is somewhere other than at the beginning or end of the screen, it
+        should be reported as follows: **something**
+
+        The assertion is case sensitive. If you want it to be case insensitive, you can pass the argument ignore_case=True.
+
+        You can change the exception message by setting a custom string to error_message.
+
+        Example:
+            | Page Should Not Contain Match | **something** |
+            | Page Should Not Contain Match | **so???hing** |
+            | Page Should Not Contain Match | **someTHING** | ignore_case=True |
+            | Page Should Not Contain Match | **something** | error_message=New error message |
+        """
+        message = error_message
+        all_screen = self._read_all_screen()
+        if ignore_case:
+            txt = txt.lower()
+            all_screen = all_screen.lower()
+        matcher = Matcher(txt, caseless=False, spaceless=False)
+        result = matcher.match(all_screen)
+        if result:
+            if message is None:
+                message = f'There are matches found for "{txt}" pattern'
+            raise Exception(message)
+
+    def _read_all_screen(self) -> str:
+        """Read all the mainframe screen and return in a single string."""
+        full_text = ""
+        for ypos in range(24):
+            full_text += self.mf.string_get(ypos + 1, 1, 80)
+        return full_text
+
+    def _compare_all_list_with_screen_text(
+        self,
+        list_string: List[str],
+        ignore_case: bool,
+        message: Optional[str],
+        should_match: bool,
+    ) -> None:
+        if ignore_case:
+            list_string = [item.lower() for item in list_string]
+        for string in list_string:
+            result = self._search_string(string, ignore_case)
+            if not should_match and result:
+                if message is None:
+                    message = f'The string "{string}" was found'
+                raise Exception(message)
+            elif should_match and not result:
+                if message is None:
+                    message = f'The string "{string}" was not found'
+                raise Exception(message)
+
+    @staticmethod
+    def _check_limits(ypos: int, xpos: int):
+        """Checks if the user has passed some coordinate y / x greater than that existing in the mainframe"""
+        if ypos > 24:
+            raise Exception(
+                "You have exceeded the y-axis limit of the mainframe screen"
+            )
+        if xpos > 80:
+            raise Exception(
+                "You have exceeded the x-axis limit of the mainframe screen"
+            )
```

### Comparing `robotframework-mainframe3270-3.1/PKG-INFO` & `robotframework-mainframe3270-3.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,181 +1,157 @@
-Metadata-Version: 2.1
-Name: robotframework-mainframe3270
-Version: 3.1
-Summary: Mainframe Test library for Robot Framework
-Home-page: https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library
-Author: Altran Portugal
-Author-email: samuca@gmail.com
-License: MIT License
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Robot Framework
-Classifier: Framework :: Robot Framework :: Library
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: Acceptance
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: THIRD-PARTY-NOTICES.txt
-
-[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
-[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
-
-# Mainframe3270Library
-
-## Introduction
-
-Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
-
-## Compatibility
-Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
-
-## Installation
-
-In order to use this library, first install the package from PyPI.
-```commandline
-pip install robotframework-mainframe3270
-```
-
-Or you can upgrade with:
-```commandline
-pip install --upgrade robotframework-mainframe3270
-```
-
-Then, depending on your OS, proceed with the corresponding chapters in this README.
-
-### Windows
-
-You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
-
-The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
-
-### Unix
-
-You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
-```commandline
-sudo apt-get install x3270
-```
-or
-```commandline
-brew install x3270
-```
-
-More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
-
-## Example
-```RobotFramework
-*** Settings ***
-Library    Mainframe3270
-
-*** Test Cases ***
-Example
-    Open Connection    Hostname    LUname
-    Change Wait Time    0.4 seconds
-    Change Wait Time After Write    0.4 seconds
-    Set Screenshot Folder    C:\\Temp\\IMG
-    ${value}    Read    3    10    17
-    Page Should Contain String    ENTER APPLICATION
-    Wait Field Detected
-    Write Bare    applicationname
-    Send Enter
-    Take Screenshot
-    Close Connection
-```
-
-## Keyword Documentation
-
-You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
-
-## Importing
-
-Arguments:
-   - visible = True
-   - timeout = 30
-   - wait_time = 0.5
-   - wait_time_after_write = 0
-   - img_folder = .
-   - run_on_failure_keyword = Take Screenshot
-
-By default the emulator visibility is set to visible=True.
-In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
-You can change this by setting visible=False. Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
-This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
-
-Timeout, waits and screenshot folder are set on library import as shown above. However, they can be changed during runtime. To modify the ``wait_time``, see [Change Wait Time](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Wait%20Time),
-to modify the ``img_folder``, see [Set Screenshot Folder](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Set%20Screenshot%20Folder),
-and to modify the ``timeout``, see the [Change Timeout](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Timeout) keyword.
-Timeouts support all available Robot Framework [time formats](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format).
-
-By default, Mainframe3270 will take a screenshot on failure. You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option. If you pass ``None`` to this argument, no keyword will be run. To change the ``run_on_failure_keyword`` during runtime, see [Register Run On Failure Keyword](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Register%20Run%20On%20Failure%20Keyword).
-
-## Running with Docker
-
-The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker hub, so steps to use it
-- Build image:
-  ```
-  docker image build --build-arg BASE_IMAGE=3.7-alpine -t mainframe3270 .
-  ```
-
-  Here, `BASE_IMAGE` can be one of the available tags for the [python docker images](https://hub.docker.com/_/python). Please note that only alpine based images (e.g. 3.7-alpine) are supported.
-
-- Run all tests:
-  ```
-  docker container run --rm -it mainframe3270
-  ```
-
-Reports are saved to /reports. You can retrieve these by mapping the directory as volume. On Windows, run this command to mount your local _reports_ directory with the container:
-```
-docker container run --rm -it -v %cd%\reports:/reports mainframe3270
-```
-
-On Linux/MacOSX, run:
-```
-docker container run --rm -it -v ${pwd}/reports:/reports
-```
-
-If you want to run single/specific tests, they can be mentioned at the end of command. Currently, only a single argument can be given, so multiple tests need to be given with wildcards like:
-```
-docker container run --rm -it -v %cd%\reports:/reports mainframe3270 *PF*
-```
-
-When developing tests, source code and tests can alsp be mounted with the container. The command to run tests using current sources is:
-* Windows:
-```
-docker container run --rm -it -v %cd%\reports:/reports -v %cd%\atests:/tests -v %cd%\Mainframe3270:/usr/local/lib/python3.7/site-packages/Mainframe3270 mainframe3270
-```
-The _reports_ directory needs to be created beforehand.
-
-* Linux/MacOSX:
-```
-docker container run --rm -it -v ${pwd}/reports:/reports -v ${pwd}/atests:/tests -v ${pwd}/Mainframe3270:/usr/local/lib/python3.7/site-packages/Mainframe3270 mainframe3270
-```
-
-## Contributing to Robot-Framework-Mainframe3270-Library
-
-Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](COUNTRIBUTING.md) to help you get started.
-
-## Keyword Tests
-
-To run all the library tests, you will need to create a user on the [pub400](https://www.pub400.com/) website.
-
-## WIKI
-For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
-
-## Authors
-   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
-   - **Samuel Cabral**
-   - **Joao Gomes**
-   - **Bruno Calado**
-   - **Ricardo Morgado**
-
-## License
-This project is licensed under the MIT License - see [LICENSE.md](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
-
-
+Metadata-Version: 2.1
+Name: robotframework-mainframe3270
+Version: 3.2
+Summary: Mainframe Test library for Robot Framework
+Home-page: https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library
+Author: Altran Portugal
+Author-email: samuca@gmail.com
+License: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: THIRD-PARTY-NOTICES.txt
+
+[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
+[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
+
+# Mainframe3270Library
+
+## Introduction
+
+Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
+
+## Compatibility
+Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
+
+## Installation
+
+In order to use this library, first install the package from PyPI.
+```commandline
+pip install robotframework-mainframe3270
+```
+
+Or you can upgrade with:
+```commandline
+pip install --upgrade robotframework-mainframe3270
+```
+
+Then, depending on your OS, proceed with the corresponding chapters in this README.
+
+### Windows
+
+You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
+
+The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
+
+### Unix
+
+You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
+```commandline
+sudo apt-get install x3270
+```
+or
+```commandline
+brew install x3270
+```
+
+More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
+
+## Example
+```RobotFramework
+*** Settings ***
+Library    Mainframe3270
+
+*** Test Cases ***
+Example
+    Open Connection    Hostname    LUname
+    Change Wait Time    0.4 seconds
+    Change Wait Time After Write    0.4 seconds
+    Set Screenshot Folder    C:\\Temp\\IMG
+    ${value}    Read    3    10    17
+    Page Should Contain String    ENTER APPLICATION
+    Wait Field Detected
+    Write Bare    applicationname
+    Send Enter
+    Take Screenshot
+    Close Connection
+```
+
+## Keyword Documentation
+
+You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
+
+## Importing
+
+Arguments:
+   - visible = True
+   - timeout = 30
+   - wait_time = 0.5
+   - wait_time_after_write = 0
+   - img_folder = .
+   - run_on_failure_keyword = Take Screenshot
+
+By default the emulator visibility is set to visible=True.
+In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
+You can change this by setting visible=False. Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
+This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
+
+Timeout, waits and screenshot folder are set on library import as shown above. However, they can be changed during runtime. To modify the ``wait_time``, see [Change Wait Time](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Wait%20Time),
+to modify the ``img_folder``, see [Set Screenshot Folder](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Set%20Screenshot%20Folder),
+and to modify the ``timeout``, see the [Change Timeout](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Timeout) keyword.
+Timeouts support all available Robot Framework [time formats](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format).
+
+By default, Mainframe3270 will take a screenshot on failure. You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option. If you pass ``None`` to this argument, no keyword will be run. To change the ``run_on_failure_keyword`` during runtime, see [Register Run On Failure Keyword](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Register%20Run%20On%20Failure%20Keyword).
+
+## Running with Docker
+
+The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker Hub. In order to use it, perform the following steps.
+
+1. Download the Dockerfile sources
+```sh
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/Dockerfile
+
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/entrypoint.sh
+```
+
+2. Build the image:
+```sh
+docker build -t mainframe3270 .
+```
+
+3. Run the container
+```sh
+docker run --user mfuser -v /path/to/your/tests:/home/mfuser/tests mainframe3270 robot /home/mfuser/tests
+```
+
+## Contributing to Robot-Framework-Mainframe3270-Library
+
+Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](COUNTRIBUTING.md) to help you get started.
+
+## Keyword Tests
+
+To run all the library tests, you will need to create a user on the [pub400](https://www.pub400.com/) website.
+
+## WIKI
+For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
+
+## Authors
+   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
+   - **Samuel Cabral**
+   - **Joao Gomes**
+   - **Bruno Calado**
+   - **Ricardo Morgado**
+
+## License
+This project is licensed under the MIT License - see [LICENSE.md](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
```

### Comparing `robotframework-mainframe3270-3.1/README.md` & `robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,156 +1,157 @@
-[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
-[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
-
-# Mainframe3270Library
-
-## Introduction
-
-Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
-
-## Compatibility
-Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
-
-## Installation
-
-In order to use this library, first install the package from PyPI.
-```commandline
-pip install robotframework-mainframe3270
-```
-
-Or you can upgrade with:
-```commandline
-pip install --upgrade robotframework-mainframe3270
-```
-
-Then, depending on your OS, proceed with the corresponding chapters in this README.
-
-### Windows
-
-You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
-
-The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
-
-### Unix
-
-You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
-```commandline
-sudo apt-get install x3270
-```
-or
-```commandline
-brew install x3270
-```
-
-More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
-
-## Example
-```RobotFramework
-*** Settings ***
-Library    Mainframe3270
-
-*** Test Cases ***
-Example
-    Open Connection    Hostname    LUname
-    Change Wait Time    0.4 seconds
-    Change Wait Time After Write    0.4 seconds
-    Set Screenshot Folder    C:\\Temp\\IMG
-    ${value}    Read    3    10    17
-    Page Should Contain String    ENTER APPLICATION
-    Wait Field Detected
-    Write Bare    applicationname
-    Send Enter
-    Take Screenshot
-    Close Connection
-```
-
-## Keyword Documentation
-
-You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
-
-## Importing
-
-Arguments:
-   - visible = True
-   - timeout = 30
-   - wait_time = 0.5
-   - wait_time_after_write = 0
-   - img_folder = .
-   - run_on_failure_keyword = Take Screenshot
-
-By default the emulator visibility is set to visible=True.
-In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
-You can change this by setting visible=False. Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
-This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
-
-Timeout, waits and screenshot folder are set on library import as shown above. However, they can be changed during runtime. To modify the ``wait_time``, see [Change Wait Time](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Wait%20Time),
-to modify the ``img_folder``, see [Set Screenshot Folder](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Set%20Screenshot%20Folder),
-and to modify the ``timeout``, see the [Change Timeout](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Timeout) keyword.
-Timeouts support all available Robot Framework [time formats](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format).
-
-By default, Mainframe3270 will take a screenshot on failure. You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option. If you pass ``None`` to this argument, no keyword will be run. To change the ``run_on_failure_keyword`` during runtime, see [Register Run On Failure Keyword](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Register%20Run%20On%20Failure%20Keyword).
-
-## Running with Docker
-
-The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker hub, so steps to use it
-- Build image:
-  ```
-  docker image build --build-arg BASE_IMAGE=3.7-alpine -t mainframe3270 .
-  ```
-
-  Here, `BASE_IMAGE` can be one of the available tags for the [python docker images](https://hub.docker.com/_/python). Please note that only alpine based images (e.g. 3.7-alpine) are supported.
-
-- Run all tests:
-  ```
-  docker container run --rm -it mainframe3270
-  ```
-
-Reports are saved to /reports. You can retrieve these by mapping the directory as volume. On Windows, run this command to mount your local _reports_ directory with the container:
-```
-docker container run --rm -it -v %cd%\reports:/reports mainframe3270
-```
-
-On Linux/MacOSX, run:
-```
-docker container run --rm -it -v ${pwd}/reports:/reports
-```
-
-If you want to run single/specific tests, they can be mentioned at the end of command. Currently, only a single argument can be given, so multiple tests need to be given with wildcards like:
-```
-docker container run --rm -it -v %cd%\reports:/reports mainframe3270 *PF*
-```
-
-When developing tests, source code and tests can alsp be mounted with the container. The command to run tests using current sources is:
-* Windows:
-```
-docker container run --rm -it -v %cd%\reports:/reports -v %cd%\atests:/tests -v %cd%\Mainframe3270:/usr/local/lib/python3.7/site-packages/Mainframe3270 mainframe3270
-```
-The _reports_ directory needs to be created beforehand.
-
-* Linux/MacOSX:
-```
-docker container run --rm -it -v ${pwd}/reports:/reports -v ${pwd}/atests:/tests -v ${pwd}/Mainframe3270:/usr/local/lib/python3.7/site-packages/Mainframe3270 mainframe3270
-```
-
-## Contributing to Robot-Framework-Mainframe3270-Library
-
-Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](COUNTRIBUTING.md) to help you get started.
-
-## Keyword Tests
-
-To run all the library tests, you will need to create a user on the [pub400](https://www.pub400.com/) website.
-
-## WIKI
-For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
-
-## Authors
-   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
-   - **Samuel Cabral**
-   - **Joao Gomes**
-   - **Bruno Calado**
-   - **Ricardo Morgado**
-
-## License
-This project is licensed under the MIT License - see [LICENSE.md](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
+Metadata-Version: 2.1
+Name: robotframework-mainframe3270
+Version: 3.2
+Summary: Mainframe Test library for Robot Framework
+Home-page: https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library
+Author: Altran Portugal
+Author-email: samuca@gmail.com
+License: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: THIRD-PARTY-NOTICES.txt
+
+[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
+[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
+
+# Mainframe3270Library
+
+## Introduction
+
+Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
+
+## Compatibility
+Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
+
+## Installation
+
+In order to use this library, first install the package from PyPI.
+```commandline
+pip install robotframework-mainframe3270
+```
+
+Or you can upgrade with:
+```commandline
+pip install --upgrade robotframework-mainframe3270
+```
+
+Then, depending on your OS, proceed with the corresponding chapters in this README.
+
+### Windows
+
+You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
+
+The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
+
+### Unix
+
+You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
+```commandline
+sudo apt-get install x3270
+```
+or
+```commandline
+brew install x3270
+```
+
+More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
+
+## Example
+```RobotFramework
+*** Settings ***
+Library    Mainframe3270
+
+*** Test Cases ***
+Example
+    Open Connection    Hostname    LUname
+    Change Wait Time    0.4 seconds
+    Change Wait Time After Write    0.4 seconds
+    Set Screenshot Folder    C:\\Temp\\IMG
+    ${value}    Read    3    10    17
+    Page Should Contain String    ENTER APPLICATION
+    Wait Field Detected
+    Write Bare    applicationname
+    Send Enter
+    Take Screenshot
+    Close Connection
+```
+
+## Keyword Documentation
+
+You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
+
+## Importing
+
+Arguments:
+   - visible = True
+   - timeout = 30
+   - wait_time = 0.5
+   - wait_time_after_write = 0
+   - img_folder = .
+   - run_on_failure_keyword = Take Screenshot
+
+By default the emulator visibility is set to visible=True.
+In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
+You can change this by setting visible=False. Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
+This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
+
+Timeout, waits and screenshot folder are set on library import as shown above. However, they can be changed during runtime. To modify the ``wait_time``, see [Change Wait Time](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Wait%20Time),
+to modify the ``img_folder``, see [Set Screenshot Folder](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Set%20Screenshot%20Folder),
+and to modify the ``timeout``, see the [Change Timeout](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Timeout) keyword.
+Timeouts support all available Robot Framework [time formats](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format).
+
+By default, Mainframe3270 will take a screenshot on failure. You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option. If you pass ``None`` to this argument, no keyword will be run. To change the ``run_on_failure_keyword`` during runtime, see [Register Run On Failure Keyword](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Register%20Run%20On%20Failure%20Keyword).
+
+## Running with Docker
+
+The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker Hub. In order to use it, perform the following steps.
+
+1. Download the Dockerfile sources
+```sh
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/Dockerfile
+
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/entrypoint.sh
+```
+
+2. Build the image:
+```sh
+docker build -t mainframe3270 .
+```
+
+3. Run the container
+```sh
+docker run --user mfuser -v /path/to/your/tests:/home/mfuser/tests mainframe3270 robot /home/mfuser/tests
+```
+
+## Contributing to Robot-Framework-Mainframe3270-Library
+
+Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](COUNTRIBUTING.md) to help you get started.
+
+## Keyword Tests
+
+To run all the library tests, you will need to create a user on the [pub400](https://www.pub400.com/) website.
+
+## WIKI
+For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
+
+## Authors
+   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
+   - **Samuel Cabral**
+   - **Joao Gomes**
+   - **Bruno Calado**
+   - **Ricardo Morgado**
+
+## License
+This project is licensed under the MIT License - see [LICENSE.md](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
```

### Comparing `robotframework-mainframe3270-3.1/THIRD-PARTY-NOTICES.txt` & `robotframework-mainframe3270-3.2/THIRD-PARTY-NOTICES.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-Robot-Framework-Mainframe3270-Library uses third-party libraries or other resources that may be
-distributed under licenses different than the Robot-Framework-Mainframe3270-Library software.
-
-In the event that we accidentally failed to list a required notice, please
-bring it to our attention by posting an issue or making a pull request to our
-GitHub repository:
-
-https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/
-
-The attached notices are provided for information only.
-
-License notice for py3270
--------------------------
-Copyright (c) 2018, Randy Syring and contributors
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-    * Redistributions of source code must retain the above copyright
-      notice, this list of conditions and the following disclaimer.
-    * Redistributions in binary form must reproduce the above copyright
-      notice, this list of conditions and the following disclaimer in the
-      documentation and/or other materials provided with the distribution.
-    * Neither the name of the <organization> nor the
-      names of its contributors may be used to endorse or promote products
-      derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL <COPYRIGHT HOLDER> BE LIABLE FOR ANY
-DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Robot-Framework-Mainframe3270-Library uses third-party libraries or other resources that may be
+distributed under licenses different than the Robot-Framework-Mainframe3270-Library software.
+
+In the event that we accidentally failed to list a required notice, please
+bring it to our attention by posting an issue or making a pull request to our
+GitHub repository:
+
+https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/
+
+The attached notices are provided for information only.
+
+License notice for py3270
+-------------------------
+Copyright (c) 2018, Randy Syring and contributors
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+    * Redistributions of source code must retain the above copyright
+      notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above copyright
+      notice, this list of conditions and the following disclaimer in the
+      documentation and/or other materials provided with the distribution.
+    * Neither the name of the <organization> nor the
+      names of its contributors may be used to endorse or promote products
+      derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL <COPYRIGHT HOLDER> BE LIABLE FOR ANY
+DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `robotframework-mainframe3270-3.1/robotframework_mainframe3270.egg-info/PKG-INFO` & `robotframework-mainframe3270-3.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,181 +1,135 @@
-Metadata-Version: 2.1
-Name: robotframework-mainframe3270
-Version: 3.1
-Summary: Mainframe Test library for Robot Framework
-Home-page: https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library
-Author: Altran Portugal
-Author-email: samuca@gmail.com
-License: MIT License
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Robot Framework
-Classifier: Framework :: Robot Framework :: Library
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: Acceptance
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: THIRD-PARTY-NOTICES.txt
-
-[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
-[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
-
-# Mainframe3270Library
-
-## Introduction
-
-Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
-
-## Compatibility
-Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
-
-## Installation
-
-In order to use this library, first install the package from PyPI.
-```commandline
-pip install robotframework-mainframe3270
-```
-
-Or you can upgrade with:
-```commandline
-pip install --upgrade robotframework-mainframe3270
-```
-
-Then, depending on your OS, proceed with the corresponding chapters in this README.
-
-### Windows
-
-You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
-
-The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
-
-### Unix
-
-You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
-```commandline
-sudo apt-get install x3270
-```
-or
-```commandline
-brew install x3270
-```
-
-More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
-
-## Example
-```RobotFramework
-*** Settings ***
-Library    Mainframe3270
-
-*** Test Cases ***
-Example
-    Open Connection    Hostname    LUname
-    Change Wait Time    0.4 seconds
-    Change Wait Time After Write    0.4 seconds
-    Set Screenshot Folder    C:\\Temp\\IMG
-    ${value}    Read    3    10    17
-    Page Should Contain String    ENTER APPLICATION
-    Wait Field Detected
-    Write Bare    applicationname
-    Send Enter
-    Take Screenshot
-    Close Connection
-```
-
-## Keyword Documentation
-
-You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
-
-## Importing
-
-Arguments:
-   - visible = True
-   - timeout = 30
-   - wait_time = 0.5
-   - wait_time_after_write = 0
-   - img_folder = .
-   - run_on_failure_keyword = Take Screenshot
-
-By default the emulator visibility is set to visible=True.
-In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
-You can change this by setting visible=False. Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
-This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
-
-Timeout, waits and screenshot folder are set on library import as shown above. However, they can be changed during runtime. To modify the ``wait_time``, see [Change Wait Time](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Wait%20Time),
-to modify the ``img_folder``, see [Set Screenshot Folder](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Set%20Screenshot%20Folder),
-and to modify the ``timeout``, see the [Change Timeout](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Timeout) keyword.
-Timeouts support all available Robot Framework [time formats](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format).
-
-By default, Mainframe3270 will take a screenshot on failure. You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option. If you pass ``None`` to this argument, no keyword will be run. To change the ``run_on_failure_keyword`` during runtime, see [Register Run On Failure Keyword](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Register%20Run%20On%20Failure%20Keyword).
-
-## Running with Docker
-
-The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker hub, so steps to use it
-- Build image:
-  ```
-  docker image build --build-arg BASE_IMAGE=3.7-alpine -t mainframe3270 .
-  ```
-
-  Here, `BASE_IMAGE` can be one of the available tags for the [python docker images](https://hub.docker.com/_/python). Please note that only alpine based images (e.g. 3.7-alpine) are supported.
-
-- Run all tests:
-  ```
-  docker container run --rm -it mainframe3270
-  ```
-
-Reports are saved to /reports. You can retrieve these by mapping the directory as volume. On Windows, run this command to mount your local _reports_ directory with the container:
-```
-docker container run --rm -it -v %cd%\reports:/reports mainframe3270
-```
-
-On Linux/MacOSX, run:
-```
-docker container run --rm -it -v ${pwd}/reports:/reports
-```
-
-If you want to run single/specific tests, they can be mentioned at the end of command. Currently, only a single argument can be given, so multiple tests need to be given with wildcards like:
-```
-docker container run --rm -it -v %cd%\reports:/reports mainframe3270 *PF*
-```
-
-When developing tests, source code and tests can alsp be mounted with the container. The command to run tests using current sources is:
-* Windows:
-```
-docker container run --rm -it -v %cd%\reports:/reports -v %cd%\atests:/tests -v %cd%\Mainframe3270:/usr/local/lib/python3.7/site-packages/Mainframe3270 mainframe3270
-```
-The _reports_ directory needs to be created beforehand.
-
-* Linux/MacOSX:
-```
-docker container run --rm -it -v ${pwd}/reports:/reports -v ${pwd}/atests:/tests -v ${pwd}/Mainframe3270:/usr/local/lib/python3.7/site-packages/Mainframe3270 mainframe3270
-```
-
-## Contributing to Robot-Framework-Mainframe3270-Library
-
-Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](COUNTRIBUTING.md) to help you get started.
-
-## Keyword Tests
-
-To run all the library tests, you will need to create a user on the [pub400](https://www.pub400.com/) website.
-
-## WIKI
-For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
-
-## Authors
-   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
-   - **Samuel Cabral**
-   - **Joao Gomes**
-   - **Bruno Calado**
-   - **Ricardo Morgado**
-
-## License
-This project is licensed under the MIT License - see [LICENSE.md](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
-
-
+[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
+[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
+
+# Mainframe3270Library
+
+## Introduction
+
+Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
+
+## Compatibility
+Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
+
+## Installation
+
+In order to use this library, first install the package from PyPI.
+```commandline
+pip install robotframework-mainframe3270
+```
+
+Or you can upgrade with:
+```commandline
+pip install --upgrade robotframework-mainframe3270
+```
+
+Then, depending on your OS, proceed with the corresponding chapters in this README.
+
+### Windows
+
+You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
+
+The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
+
+### Unix
+
+You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
+```commandline
+sudo apt-get install x3270
+```
+or
+```commandline
+brew install x3270
+```
+
+More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
+
+## Example
+```RobotFramework
+*** Settings ***
+Library    Mainframe3270
+
+*** Test Cases ***
+Example
+    Open Connection    Hostname    LUname
+    Change Wait Time    0.4 seconds
+    Change Wait Time After Write    0.4 seconds
+    Set Screenshot Folder    C:\\Temp\\IMG
+    ${value}    Read    3    10    17
+    Page Should Contain String    ENTER APPLICATION
+    Wait Field Detected
+    Write Bare    applicationname
+    Send Enter
+    Take Screenshot
+    Close Connection
+```
+
+## Keyword Documentation
+
+You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
+
+## Importing
+
+Arguments:
+   - visible = True
+   - timeout = 30
+   - wait_time = 0.5
+   - wait_time_after_write = 0
+   - img_folder = .
+   - run_on_failure_keyword = Take Screenshot
+
+By default the emulator visibility is set to visible=True.
+In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
+You can change this by setting visible=False. Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
+This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
+
+Timeout, waits and screenshot folder are set on library import as shown above. However, they can be changed during runtime. To modify the ``wait_time``, see [Change Wait Time](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Wait%20Time),
+to modify the ``img_folder``, see [Set Screenshot Folder](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Set%20Screenshot%20Folder),
+and to modify the ``timeout``, see the [Change Timeout](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Timeout) keyword.
+Timeouts support all available Robot Framework [time formats](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format).
+
+By default, Mainframe3270 will take a screenshot on failure. You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option. If you pass ``None`` to this argument, no keyword will be run. To change the ``run_on_failure_keyword`` during runtime, see [Register Run On Failure Keyword](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Register%20Run%20On%20Failure%20Keyword).
+
+## Running with Docker
+
+The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker Hub. In order to use it, perform the following steps.
+
+1. Download the Dockerfile sources
+```sh
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/Dockerfile
+
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/entrypoint.sh
+```
+
+2. Build the image:
+```sh
+docker build -t mainframe3270 .
+```
+
+3. Run the container
+```sh
+docker run --user mfuser -v /path/to/your/tests:/home/mfuser/tests mainframe3270 robot /home/mfuser/tests
+```
+
+## Contributing to Robot-Framework-Mainframe3270-Library
+
+Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](COUNTRIBUTING.md) to help you get started.
+
+## Keyword Tests
+
+To run all the library tests, you will need to create a user on the [pub400](https://www.pub400.com/) website.
+
+## WIKI
+For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
+
+## Authors
+   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
+   - **Samuel Cabral**
+   - **Joao Gomes**
+   - **Bruno Calado**
+   - **Ricardo Morgado**
+
+## License
+This project is licensed under the MIT License - see [LICENSE.md](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
```

### Comparing `robotframework-mainframe3270-3.1/setup.py` & `robotframework-mainframe3270-3.2/setup.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from os.path import abspath, dirname, join
-
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
-
-VERSION = None
-version_file = join(dirname(abspath(__file__)), "Mainframe3270", "version.py")
-
-with open(version_file) as file:
-    code = compile(file.read(), version_file, "exec")
-    exec(code)
-
-with open("README.md", encoding="utf-8") as file:
-    long_description = file.read()
-
-
-package_kwargs = {
-    "name": "robotframework-mainframe3270",
-    "version": VERSION,
-    "description": "Mainframe Test library for Robot Framework",
-    "long_description": long_description,
-    "long_description_content_type": "text/markdown",
-    "author": "Altran Portugal",
-    "author_email": "samuca@gmail.com",
-    "license": "MIT License",
-    "license_files": ["LICENSE.md", "THIRD-PARTY-NOTICES.txt"],
-    "url": "https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library",
-    "packages": ["Mainframe3270"],
-    "install_requires": ["robotframework", "robotframework-pythonlibcore"],
-    "classifiers": [
-        "Development Status :: 5 - Production/Stable",
-        "Framework :: Robot Framework",
-        "Framework :: Robot Framework :: Library",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Topic :: Software Development :: Testing",
-        "Topic :: Software Development :: Testing :: Acceptance",
-    ],
-}
-
-setup(**package_kwargs)
+from os.path import abspath, dirname, join
+
+try:
+    from setuptools import setup
+except ImportError:
+    from distutils.core import setup
+
+VERSION = None
+version_file = join(dirname(abspath(__file__)), "Mainframe3270", "version.py")
+
+with open(version_file) as file:
+    code = compile(file.read(), version_file, "exec")
+    exec(code)
+
+with open("README.md", encoding="utf-8") as file:
+    long_description = file.read()
+
+
+package_kwargs = {
+    "name": "robotframework-mainframe3270",
+    "version": VERSION,
+    "description": "Mainframe Test library for Robot Framework",
+    "long_description": long_description,
+    "long_description_content_type": "text/markdown",
+    "author": "Altran Portugal",
+    "author_email": "samuca@gmail.com",
+    "license": "MIT License",
+    "license_files": ["LICENSE.md", "THIRD-PARTY-NOTICES.txt"],
+    "url": "https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library",
+    "packages": ["Mainframe3270"],
+    "install_requires": ["robotframework", "robotframework-pythonlibcore"],
+    "classifiers": [
+        "Development Status :: 5 - Production/Stable",
+        "Framework :: Robot Framework",
+        "Framework :: Robot Framework :: Library",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Topic :: Software Development :: Testing",
+        "Topic :: Software Development :: Testing :: Acceptance",
+    ],
+}
+
+setup(**package_kwargs)
```


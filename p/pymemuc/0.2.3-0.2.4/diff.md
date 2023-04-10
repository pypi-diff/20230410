# Comparing `tmp/pymemuc-0.2.3.tar.gz` & `tmp/pymemuc-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.2.3.tar", max compression
+gzip compressed data, was "pymemuc-0.2.4.tar", max compression
```

## Comparing `pymemuc-0.2.3.tar` & `pymemuc-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-04-06 21:52:46.040773 pymemuc-0.2.3/LICENSE
--rw-r--r--   0        0        0     1577 2023-04-06 21:52:46.040773 pymemuc-0.2.3/README.md
--rw-r--r--   0        0        0      386 2023-04-06 21:52:46.040773 pymemuc-0.2.3/pymemuc/__init__.py
--rw-r--r--   0        0        0    22468 2023-04-06 21:52:46.040773 pymemuc-0.2.3/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-04-06 21:52:46.040773 pymemuc-0.2.3/pymemuc/_constants.py
--rw-r--r--   0        0        0     4941 2023-04-06 21:52:46.040773 pymemuc-0.2.3/pymemuc/_control.py
--rw-r--r--   0        0        0     1150 2023-04-06 21:52:46.040773 pymemuc-0.2.3/pymemuc/_decorators.py
--rw-r--r--   0        0        0    12559 2023-04-06 21:52:46.040773 pymemuc-0.2.3/pymemuc/_manage.py
--rw-r--r--   0        0        0     3937 2023-04-06 21:52:46.040773 pymemuc-0.2.3/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-04-06 21:52:46.044774 pymemuc-0.2.3/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2194 2023-04-06 21:52:46.044774 pymemuc-0.2.3/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-04-06 21:52:46.044774 pymemuc-0.2.3/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1632 2023-04-06 21:53:05.444241 pymemuc-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 pymemuc-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-10 19:07:05.128549 pymemuc-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1577 2023-04-10 19:07:05.128549 pymemuc-0.2.4/README.md
+-rw-r--r--   0        0        0      386 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/__init__.py
+-rw-r--r--   0        0        0    22754 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_constants.py
+-rw-r--r--   0        0        0     4984 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_control.py
+-rw-r--r--   0        0        0     1150 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    12663 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_manage.py
+-rw-r--r--   0        0        0     3937 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     2194 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1632 2023-04-10 19:07:25.492846 pymemuc-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 pymemuc-0.2.4/PKG-INFO
```

### Comparing `pymemuc-0.2.3/LICENSE` & `pymemuc-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.3/README.md` & `pymemuc-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.3/pymemuc/_command.py` & `pymemuc-0.2.4/pymemuc/_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """This module contains functions for commanding running virtual machines with memuc.exe.
 Functions for interacting with running VMs are defined here."""
-from typing import TYPE_CHECKING, Literal
+from typing import TYPE_CHECKING, Literal, Union
 
 from .exceptions import PyMemucError, PyMemucIndexError, PyMemucTimeoutExpired
 
 if TYPE_CHECKING:
     from pymemuc import PyMemuc
 
 
@@ -21,16 +21,16 @@
     return True
 
 
 # TODO: look into bindings with https://github.com/egirault/googleplay-api
 def install_apk_vm(
     self: "PyMemuc",
     apk_path,
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
     create_shortcut=False,
 ) -> Literal[True]:
     """Install an APK on a VM, must specify either a vm index or a vm name
 
     :param apk_path: Path to the APK
     :type apk_path: str
     :param vm_index: VM index. Defaults to None.
@@ -70,16 +70,16 @@
         raise PyMemucError(f"Failed to install APK: {output}")
     return True
 
 
 def uninstall_apk_vm(
     self: "PyMemuc",
     package_name,
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> Literal[True]:
     """Uninstall an APK on a VM, must specify either a vm index or a vm name
 
     :param package_name: Package name of the APK
     :type package_name: str
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -102,16 +102,16 @@
         raise PyMemucError(f"Failed to uninstall APK: {output}")
     return True
 
 
 def start_app_vm(
     self: "PyMemuc",
     package_name,
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> Literal[True]:
     """Start an app on a VM, must specify either a vm index or a vm name
 
     :param package_name: Package name of the APK
     :type package_name: str
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -132,16 +132,16 @@
         raise PyMemucError(f"Failed to start app: {output}")
     return True
 
 
 def stop_app_vm(
     self: "PyMemuc",
     package_name,
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> Literal[True]:
     """Stop an app on a VM, must specify either a vm index or a vm name
 
     :param package_name: Package name of the APK
     :type package_name: str
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -162,16 +162,16 @@
         raise PyMemucError(f"Failed to stop app: {output}")
     return True
 
 
 def trigger_keystroke_vm(
     self: "PyMemuc",
     key: Literal["back", "home", "menu", "volumeup", "volumedown"],
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> Literal[True]:
     """Trigger a keystroke on a VM, must specify either a vm index or a vm name
 
     :param key: Key to trigger
     :type key: Literal["back", "home", "menu", "volumeup", "volumedown"]
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -190,15 +190,15 @@
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to trigger keystroke: {output}")
     return True
 
 
 def trigger_shake_vm(
-    self: "PyMemuc", vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc", vm_index: Union[int, None] = None, vm_name: Union[str, None] = None
 ) -> Literal[True]:
     """Trigger a shake on a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
@@ -215,15 +215,15 @@
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to trigger shake: {output}")
     return True
 
 
 def connect_internet_vm(
-    self: "PyMemuc", vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc", vm_index: Union[int, None] = None, vm_name: Union[str, None] = None
 ) -> Literal[True]:
     """Connect the internet on a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
@@ -240,15 +240,15 @@
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to connect internet: {output}")
     return True
 
 
 def disconnect_internet_vm(
-    self: "PyMemuc", vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc", vm_index: Union[int, None] = None, vm_name: Union[str, None] = None
 ) -> Literal[True]:
     """Disconnect the internet on a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
@@ -265,15 +265,18 @@
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to disconnect internet: {output}")
     return True
 
 
 def input_text_vm(
-    self: "PyMemuc", text, vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc",
+    text,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> Literal[True]:
     """Input text on a VM, must specify either a vm index or a vm name
 
     :param text: Text to input
     :type text: str
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -292,15 +295,15 @@
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to input text: {output}")
     return True
 
 
 def rotate_window_vm(
-    self: "PyMemuc", vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc", vm_index: Union[int, None] = None, vm_name: Union[str, None] = None
 ) -> Literal[True]:
     """Rotate the window on a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :raises PyMemucIndexError: an error if neither a vm index or a vm name is specified
     :return: True if the vm window rotation was successful
@@ -315,15 +318,18 @@
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to rotate window: {output}")
     return True
 
 
 def execute_command_vm(
-    self: "PyMemuc", command, vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc",
+    command,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> tuple[int, str]:
     """Execute a command on a VM, must specify either a vm index or a vm name
 
     :param command: Command to execute
     :type command: str
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -340,16 +346,16 @@
     raise PyMemucIndexError("Please specify either a vm index or a vm name")
 
 
 def change_gps_vm(
     self: "PyMemuc",
     latitude: float,
     longitude: float,
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> Literal[True]:
     """Change the GPS location on a VM, must specify either a vm index or a vm name
 
     :param latitude: Latitude
     :type latitude: float
     :param longitude: Longitude
     :type longitude: float
@@ -375,15 +381,15 @@
     if not success:
         raise PyMemucError(f"Failed to change GPS location: {output}")
     return True
 
 
 # TODO: fix parsing of the output
 def get_public_ip_vm(
-    self: "PyMemuc", vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc", vm_index: Union[int, None] = None, vm_name: Union[str, None] = None
 ) -> tuple[int, str]:
     """Get the public IP of a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
@@ -399,15 +405,15 @@
         return self.memuc_run(
             ["-n", vm_name, 'execcmd "wget -O- whatismyip.akamai.com"']
         )
     raise PyMemucIndexError("Please specify either a vm index or a vm name")
 
 
 def zoom_in_vm(
-    self: "PyMemuc", vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc", vm_index: Union[int, None] = None, vm_name: Union[str, None] = None
 ) -> Literal[True]:
     """Zoom in on a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
@@ -424,15 +430,15 @@
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to zoom in: {output}")
     return True
 
 
 def zoom_out_vm(
-    self: "PyMemuc", vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc", vm_index: Union[int, None] = None, vm_name: Union[str, None] = None
 ) -> Literal[True]:
     """Zoom out on a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
@@ -449,15 +455,18 @@
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to zoom in: {output}")
     return True
 
 
 def get_app_info_list_vm(
-    self: "PyMemuc", vm_index: int | None = None, vm_name: str | None = None, timeout=10
+    self: "PyMemuc",
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
+    timeout=10,
 ) -> list[str]:
     """Get the list of apps installed on a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
@@ -489,16 +498,16 @@
         return []
 
 
 # TODO: debug this, it doesn't work
 def set_accelerometer_vm(
     self: "PyMemuc",
     value: tuple[float, float, float],
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> tuple[int, str]:
     """Set the accelerometer on a VM, must specify either a vm index or a vm name
 
     :param value: the accelerometer value to set
     :type value: tuple[float, float, float]
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -533,16 +542,16 @@
         )
     raise PyMemucIndexError("Please specify either a vm index or a vm name")
 
 
 def create_app_shortcut_vm(
     self: "PyMemuc",
     package_name: str,
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> tuple[int, str]:
     """Create an app shortcut on a VM, must specify either a vm index or a vm name
 
     :param package_name: Package name
     :type package_name: str
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -567,18 +576,18 @@
         )  # can raise timeout
     raise PyMemucIndexError("Please specify either a vm index or a vm name")
 
 
 # TODO: parse the output to confirm that the command was ran successfully
 def send_adb_command_vm(
     self: "PyMemuc",
-    command: str | list[str],
-    vm_index: int | None = None,
-    vm_name: str | None = None,
-    timeout: int | None = None,
+    command: Union[str, list[str]],
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
+    timeout: Union[int, None] = None,
 ) -> str:
     """Send an ADB command to a VM, must specify either a vm index or a vm name
 
     :param command: ADB command
     :type command: str | list[str]
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
```

### Comparing `pymemuc-0.2.3/pymemuc/_control.py` & `pymemuc-0.2.4/pymemuc/_control.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """This module contains functions for controlling the VMs.
 Functions for starting and stopping VMs are defined here.
 """
-from typing import TYPE_CHECKING, Literal
+from typing import TYPE_CHECKING, Literal, Union
 
 from ._decorators import _retryable
 from .exceptions import PyMemucError, PyMemucIndexError
 
 if TYPE_CHECKING:
     from pymemuc import PyMemuc
 
 
 @_retryable
 def start_vm(
     self: "PyMemuc",
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
     non_blocking=False,
     timeout=None,
 ) -> Literal[True]:
     """Start a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -45,16 +45,16 @@
         raise PyMemucError(f"Failed to start VM: {output}")
     return True
 
 
 @_retryable
 def stop_vm(
     self: "PyMemuc",
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
     non_blocking=False,
     timeout=None,
 ) -> Literal[True]:
     """Stop a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -99,16 +99,16 @@
     if not success:
         raise PyMemucError(f"Failed to stop all VMs: {output}")
     return True
 
 
 def reboot_vm(
     self: "PyMemuc",
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
     non_blocking=False,
 ) -> Literal[True]:
     """Reboot a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
```

### Comparing `pymemuc-0.2.3/pymemuc/_decorators.py` & `pymemuc-0.2.4/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.3/pymemuc/_manage.py` & `pymemuc-0.2.4/pymemuc/_manage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module contains functions for managing the VMs.
 Functions for creating, deleting, and listing VMs are defined here.
 """
 import re
 from os.path import abspath, expanduser, expandvars
-from typing import TYPE_CHECKING, Literal
+from typing import TYPE_CHECKING, Literal, Union
 
 from ._decorators import _retryable
 from .exceptions import PyMemucError, PyMemucIndexError, PyMemucTimeoutExpired
 from .vminfo import VMInfo
 
 if TYPE_CHECKING:
     from pymemuc import PyMemuc
@@ -32,15 +32,15 @@
         return -1 if indecies is None else int(indecies[1])
     except AttributeError:
         return -1
 
 
 @_retryable
 def delete_vm(
-    self: "PyMemuc", vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc", vm_index: Union[int, None] = None, vm_name: Union[str, None] = None
 ) -> Literal[True]:
     """Delete a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
@@ -58,16 +58,16 @@
     if not success:
         raise PyMemucError(f"Failed to delete VM: {output}")
     return True
 
 
 def clone_vm(
     self: "PyMemuc",
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
     new_name=None,
 ) -> Literal[True]:
     """Clone a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
@@ -90,16 +90,16 @@
         raise PyMemucError(f"Failed to clone VM: {output}")
     return True
 
 
 # TODO: verify functionality
 def export_vm(
     self: "PyMemuc",
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
     file_name="vm.ova",
     non_blocking=False,
 ):
     """Export a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -140,16 +140,16 @@
         raise PyMemucError(f"Failed to import VM: {output}")
     return True
 
 
 @_retryable
 def rename_vm(
     self: "PyMemuc",
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
     new_name=None,
 ) -> Literal[True]:
     """Rename a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
@@ -178,16 +178,16 @@
         return True
     except PyMemucTimeoutExpired as err:
         raise PyMemucError("Failed to rename VM: Timeout expired") from err
 
 
 def list_vm_info(
     self: "PyMemuc",
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
     running=False,
     disk_info=False,
 ) -> list[VMInfo]:
     """List VM info, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
@@ -269,15 +269,18 @@
     :rtype: bool
     """
     _, output = self.memuc_run(["-i", str(vm_index), "isrunning"])
     return "Running" in output
 
 
 def get_configuration_vm(
-    self: "PyMemuc", config_key, vm_index: int | None = None, vm_name: str | None = None
+    self: "PyMemuc",
+    config_key,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> str:
     """Get a VM configuration, must specify either a vm index or a vm name
 
     :param config_key: Configuration key, keys are noted in `configuration keys table
         <https://pymemuc.readthedocs.io/pymemuc.html#the-vm-configuration-keys-table>`_
     :type config_key: str
     :param vm_index: VM index. Defaults to None.
@@ -302,16 +305,16 @@
     return output.split("Value: ")[1].replace("\n", "").replace("\r", "")
 
 
 def set_configuration_vm(
     self: "PyMemuc",
     config_key: str,
     config_value: str,
-    vm_index: int | None = None,
-    vm_name: str | None = None,
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
 ) -> Literal[True]:
     """Set a VM configuration, must specify either a vm index or a vm name
 
     :param config_key: Configuration key, keys are noted in `configuration keys table
         <https://pymemuc.readthedocs.io/pymemuc.html#the-vm-configuration-keys-table>`_
     :type config_key: str
     :param config_value: Configuration value
```

### Comparing `pymemuc-0.2.3/pymemuc/_memuc.py` & `pymemuc-0.2.4/pymemuc/_memuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.3/pymemuc/exceptions.py` & `pymemuc-0.2.4/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.3/pymemuc/pymemuc.py` & `pymemuc-0.2.4/pymemuc/pymemuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.3/pyproject.toml` & `pymemuc-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.2.3"
+version = "v0.2.4"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -17,15 +17,15 @@
 ]
 keywords = ["memu", "memuc", "wrapper", "api"]
 repository = "https://github.com/marmig0404/pymemuc"
 documentation = "https://pymemuc.readthedocs.io/"
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.1"
 black = "^23.1.0"
 prospector = "^1.9.0"
 ipykernel = "^6.22.0"
```

### Comparing `pymemuc-0.2.3/PKG-INFO` & `pymemuc-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/marmig0404/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Documentation, https://pymemuc.readthedocs.io/
 Project-URL: Repository, https://github.com/marmig0404/pymemuc
```


# Comparing `tmp/pyhOn-0.5.0.tar.gz` & `tmp/pyhOn-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.5.0.tar", last modified: Sat Apr  8 02:09:41 2023, max compression
+gzip compressed data, was "pyhOn-0.6.0.tar", last modified: Mon Apr 10 04:55:12 2023, max compression
```

## Comparing `pyhOn-0.5.0.tar` & `pyhOn-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:09:41.747518 pyhOn-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 02:09:32.000000 pyhOn-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-08 02:09:41.747518 pyhOn-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-08 02:09:32.000000 pyhOn-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:09:41.743518 pyhOn-0.5.0/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-08 02:09:41.000000 pyhOn-0.5.0/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-08 02:09:41.000000 pyhOn-0.5.0/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 02:09:41.000000 pyhOn-0.5.0/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 02:09:41.000000 pyhOn-0.5.0/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 02:09:41.000000 pyhOn-0.5.0/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 02:09:41.000000 pyhOn-0.5.0/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:09:41.743518 pyhOn-0.5.0/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4754 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:09:41.747518 pyhOn-0.5.0/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-08 02:09:32.000000 pyhOn-0.5.0/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 02:09:41.747518 pyhOn-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-08 02:09:32.000000 pyhOn-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:12.230599 pyhOn-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 04:55:02.000000 pyhOn-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 04:55:12.230599 pyhOn-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-10 04:55:02.000000 pyhOn-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:12.230599 pyhOn-0.6.0/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:12.230599 pyhOn-0.6.0/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4839 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:12.230599 pyhOn-0.6.0/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:12.230599 pyhOn-0.6.0/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/connection/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/connection/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 04:55:12.230599 pyhOn-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-10 04:55:02.000000 pyhOn-0.6.0/setup.py
```

### Comparing `pyhOn-0.5.0/LICENSE` & `pyhOn-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.5.0/PKG-INFO` & `pyhOn-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.5.0
+Version: 0.6.0
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -64,36 +64,36 @@
       ...
 ```
 
 ## Python-API
 ### List devices
 ```python
 import asyncio
-from pyhon import HonConnection
+from pyhon import Hon
 
 async def devices_example():
-    async with HonConnection(USER, PASSWORD) as hon:
-        for device in hon.devices:
-            print(device.nick_name)
+    async with Hon(USER, PASSWORD) as hon:
+        for appliance in hon.appliances:
+            print(appliance.nick_name)
 
 asyncio.run(devices_example())
 ```
 
 ### Execute a command
 ```python
-async with HonConnection(USER, PASSWORD) as hon:
-    washing_machine = hon.devices[0]
+async with Hon(USER, PASSWORD) as hon:
+    washing_machine = hon.appliances[0]
     pause_command = washing_machine.commands["pauseProgram"]
     await pause_command.send()
 ```
 
 ### Set command parameter
 ```python
-async with HonConnection(USER, PASSWORD) as hon:
-    washing_machine = hon.devices[0]
+async with Hon(USER, PASSWORD) as hon:
+    washing_machine = hon.appliances[0]
     start_command = washing_machine.commands["startProgram"]
     for name, setting in start_command.settings:
         print("Setting", name)
         print("Current value", setting.value)
         if setting.typology == "enum":
             print("Available values", setting.values)
             setting.value = setting.values[0]
```

### Comparing `pyhOn-0.5.0/README.md` & `pyhOn-0.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -43,36 +43,36 @@
       ...
 ```
 
 ## Python-API
 ### List devices
 ```python
 import asyncio
-from pyhon import HonConnection
+from pyhon import Hon
 
 async def devices_example():
-    async with HonConnection(USER, PASSWORD) as hon:
-        for device in hon.devices:
-            print(device.nick_name)
+    async with Hon(USER, PASSWORD) as hon:
+        for appliance in hon.appliances:
+            print(appliance.nick_name)
 
 asyncio.run(devices_example())
 ```
 
 ### Execute a command
 ```python
-async with HonConnection(USER, PASSWORD) as hon:
-    washing_machine = hon.devices[0]
+async with Hon(USER, PASSWORD) as hon:
+    washing_machine = hon.appliances[0]
     pause_command = washing_machine.commands["pauseProgram"]
     await pause_command.send()
 ```
 
 ### Set command parameter
 ```python
-async with HonConnection(USER, PASSWORD) as hon:
-    washing_machine = hon.devices[0]
+async with Hon(USER, PASSWORD) as hon:
+    washing_machine = hon.appliances[0]
     start_command = washing_machine.commands["startProgram"]
     for name, setting in start_command.settings:
         print("Setting", name)
         print("Current value", setting.value)
         if setting.typology == "enum":
             print("Available values", setting.values)
             setting.value = setting.values[0]
```

### Comparing `pyhOn-0.5.0/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.6.0/pyhOn.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.5.0
+Version: 0.6.0
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -64,36 +64,36 @@
       ...
 ```
 
 ## Python-API
 ### List devices
 ```python
 import asyncio
-from pyhon import HonConnection
+from pyhon import Hon
 
 async def devices_example():
-    async with HonConnection(USER, PASSWORD) as hon:
-        for device in hon.devices:
-            print(device.nick_name)
+    async with Hon(USER, PASSWORD) as hon:
+        for appliance in hon.appliances:
+            print(appliance.nick_name)
 
 asyncio.run(devices_example())
 ```
 
 ### Execute a command
 ```python
-async with HonConnection(USER, PASSWORD) as hon:
-    washing_machine = hon.devices[0]
+async with Hon(USER, PASSWORD) as hon:
+    washing_machine = hon.appliances[0]
     pause_command = washing_machine.commands["pauseProgram"]
     await pause_command.send()
 ```
 
 ### Set command parameter
 ```python
-async with HonConnection(USER, PASSWORD) as hon:
-    washing_machine = hon.devices[0]
+async with Hon(USER, PASSWORD) as hon:
+    washing_machine = hon.appliances[0]
     start_command = washing_machine.commands["startProgram"]
     for name, setting in start_command.settings:
         print("Setting", name)
         print("Current value", setting.value)
         if setting.typology == "enum":
             print("Available values", setting.values)
             setting.value = setting.values[0]
```

### Comparing `pyhOn-0.5.0/pyhon/__main__.py` & `pyhOn-0.6.0/pyhon/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 import argparse
 import asyncio
 import json
 import logging
 import sys
 from getpass import getpass
 from pathlib import Path
-from pprint import pprint
 
 if __name__ == "__main__":
     sys.path.insert(0, str(Path(__file__).parent.parent))
 
-from pyhon import HonConnection
+from pyhon import Hon, HonAPI
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def get_arguments():
     """Get parsed arguments."""
     parser = argparse.ArgumentParser(description="pyhOn: Command Line Utility")
     parser.add_argument("-u", "--user", help="user for haier hOn account")
     parser.add_argument("-p", "--password", help="password for haier hOn account")
     subparser = parser.add_subparsers(title="commands", metavar="COMMAND")
     keys = subparser.add_parser("keys", help="print as key format")
     keys.add_argument("keys", help="print as key format", action="store_true")
     keys.add_argument("--all", help="print also full keys", action="store_true")
-    translate = subparser.add_parser("translate", help="print available translation keys")
-    translate.add_argument("translate", help="language (de, en, fr...)", metavar="LANGUAGE")
+    translate = subparser.add_parser(
+        "translate", help="print available translation keys"
+    )
+    translate.add_argument(
+        "translate", help="language (de, en, fr...)", metavar="LANGUAGE"
+    )
     translate.add_argument("--json", help="print as json", action="store_true")
     return vars(parser.parse_args())
 
 
 # yaml.dump() would be done the same, but needs an additional dependency...
 def pretty_print(data, key="", intend=0, is_list=False):
     if type(data) is list:
@@ -47,15 +50,17 @@
             if is_list and not i:
                 pretty_print(value, key=key, intend=intend, is_list=True)
             elif is_list:
                 pretty_print(value, key=key, intend=intend + 1)
             else:
                 pretty_print(value, key=key, intend=intend)
     else:
-        print(f"{'  ' * intend}{'- ' if is_list else ''}{key}{': ' if key else ''}{data}")
+        print(
+            f"{'  ' * intend}{'- ' if is_list else ''}{key}{': ' if key else ''}{data}"
+        )
 
 
 def key_print(data, key="", start=True):
     if type(data) is list:
         for i, value in enumerate(data):
             key_print(value, key=f"{key}.{i}", start=False)
     elif type(data) is dict:
@@ -81,35 +86,40 @@
                 result[name][parameter] = value
             else:
                 result[f"{name}.{parameter}"] = value
     return result
 
 
 async def translate(language, json_output=False):
-    async with HonConnection() as hon:
+    async with HonAPI(anonymous=True) as hon:
         keys = await hon.translation_keys(language)
     if json_output:
         print(json.dumps(keys, indent=4))
     else:
-        clean_keys = json.dumps(keys).replace("\\n", "\\\\n").replace("\\\\r", "").replace("\\r", "")
+        clean_keys = (
+            json.dumps(keys)
+            .replace("\\n", "\\\\n")
+            .replace("\\\\r", "")
+            .replace("\\r", "")
+        )
         keys = json.loads(clean_keys)
         pretty_print(keys)
 
 
 async def main():
     args = get_arguments()
     if language := args.get("translate"):
         await translate(language, json_output=args.get("json"))
         return
     if not (user := args["user"]):
         user = input("User for hOn account: ")
     if not (password := args["password"]):
         password = getpass("Password for hOn account: ")
-    async with HonConnection(user, password) as hon:
-        for device in hon.devices:
+    async with Hon(user, password) as hon:
+        for device in hon.appliances:
             print("=" * 10, device.appliance_type, "-", device.nick_name, "=" * 10)
             if args.get("keys"):
                 data = device.data.copy()
                 attr = "get" if args.get("all") else "pop"
                 key_print(data["attributes"].__getattribute__(attr)("parameters"))
                 key_print(data.__getattribute__(attr)("appliance"))
                 key_print(data)
@@ -122,9 +132,9 @@
 def start():
     try:
         asyncio.run(main())
     except KeyboardInterrupt:
         print("Aborted.")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     start()
```

### Comparing `pyhOn-0.5.0/pyhon/appliances/ov.py` & `pyhOn-0.6.0/pyhon/appliances/ov.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from pyhon.parameter import HonParameterEnum
 
 
 class Appliance:
+    _FILTERS = {
+        "default": "^(?!iot_(?:recipe|guided))\\S+$",
+        "recipe": "iot_recipe_",
+        "guided": "iot_guided_",
+    }
+
     def __init__(self):
-        filters = ["receipt", "standard, special"]
-        data = {'defaultValue': filters[0], 'enumValues': filters}
+        filters = list(self._FILTERS.values())
+        data = {"defaultValue": filters[0], "enumValues": filters}
         self._program_filter = HonParameterEnum("program_filter", data)
 
     def data(self, data):
         return data
 
     def settings(self, settings):
         settings["program_filter"] = self._program_filter
-        settings["startProgram.program"].filter = self._program_filter.value
+        value = self._FILTERS[self._program_filter.value]
+        settings["startProgram.program"].filter = value
         return settings
```

### Comparing `pyhOn-0.5.0/pyhon/auth.py` & `pyhOn-0.6.0/pyhon/connection/auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import json
 import logging
 import re
 import secrets
 import urllib
+from pprint import pformat
 from urllib import parse
 
-import aiohttp as aiohttp
 from yarl import URL
 
 from pyhon import const
 
 _LOGGER = logging.getLogger()
 
 
 class HonAuth:
-    def __init__(self) -> None:
+    def __init__(self, session, email, password, device) -> None:
+        self._session = session
+        self._email = email
+        self._password = password
         self._access_token = ""
         self._refresh_token = ""
         self._cognito_token = ""
         self._id_token = ""
+        self._device = device
 
     @property
     def cognito_token(self):
         return self._cognito_token
 
     @property
     def id_token(self):
@@ -32,126 +36,165 @@
     def access_token(self):
         return self._access_token
 
     @property
     def refresh_token(self):
         return self._refresh_token
 
-    async def _load_login(self, session):
+    async def _load_login(self):
         nonce = secrets.token_hex(16)
         nonce = f"{nonce[:8]}-{nonce[8:12]}-{nonce[12:16]}-{nonce[16:20]}-{nonce[20:]}"
         params = {
             "response_type": "token+id_token",
             "client_id": const.CLIENT_ID,
-            "redirect_uri": urllib.parse.quote(f"{const.APP}://mobilesdk/detect/oauth/done"),
+            "redirect_uri": urllib.parse.quote(
+                f"{const.APP}://mobilesdk/detect/oauth/done"
+            ),
             "display": "touch",
             "scope": "api openid refresh_token web",
-            "nonce": nonce
+            "nonce": nonce,
         }
         params = "&".join([f"{k}={v}" for k, v in params.items()])
-        async with session.get(f"{const.AUTH_API}/services/oauth2/authorize/expid_Login?{params}") as resp:
+        async with self._session.get(
+            f"{const.AUTH_API}/services/oauth2/authorize/expid_Login?{params}"
+        ) as resp:
             if not (login_url := re.findall("url = '(.+?)'", await resp.text())):
                 return False
-        async with session.get(login_url[0], allow_redirects=False) as redirect1:
+        async with self._session.get(login_url[0], allow_redirects=False) as redirect1:
             if not (url := redirect1.headers.get("Location")):
                 return False
-        async with session.get(url, allow_redirects=False) as redirect2:
-            if not (url := redirect2.headers.get("Location") + "&System=IoT_Mobile_App&RegistrationSubChannel=hOn"):
-                return False
-        async with session.get(URL(url, encoded=True)) as login_screen:
-            if context := re.findall('"fwuid":"(.*?)","loaded":(\\{.*?})', await login_screen.text()):
+        async with self._session.get(url, allow_redirects=False) as redirect2:
+            if not (
+                url := redirect2.headers.get("Location")
+                + "&System=IoT_Mobile_App&RegistrationSubChannel=hOn"
+            ):
+                return False
+        async with self._session.get(URL(url, encoded=True)) as login_screen:
+            if context := re.findall(
+                '"fwuid":"(.*?)","loaded":(\\{.*?})', await login_screen.text()
+            ):
                 fw_uid, loaded_str = context[0]
                 loaded = json.loads(loaded_str)
-                login_url = login_url[0].replace("/".join(const.AUTH_API.split("/")[:-1]), "")
+                login_url = login_url[0].replace(
+                    "/".join(const.AUTH_API.split("/")[:-1]), ""
+                )
                 return fw_uid, loaded, login_url
         return False
 
-    async def _login(self, session, email, password, fw_uid, loaded, login_url):
+    async def _login(self, fw_uid, loaded, login_url):
         data = {
             "message": {
                 "actions": [
                     {
                         "id": "79;a",
                         "descriptor": "apex://LightningLoginCustomController/ACTION$login",
                         "callingDescriptor": "markup://c:loginForm",
                         "params": {
-                            "username": email,
-                            "password": password,
-                            "startUrl": parse.unquote(login_url.split("startURL=")[-1]).split("%3D")[0]
-                        }
+                            "username": self._email,
+                            "password": self._password,
+                            "startUrl": parse.unquote(
+                                login_url.split("startURL=")[-1]
+                            ).split("%3D")[0],
+                        },
                     }
                 ]
             },
             "aura.context": {
                 "mode": "PROD",
                 "fwuid": fw_uid,
                 "app": "siteforce:loginApp2",
                 "loaded": loaded,
                 "dn": [],
                 "globals": {},
-                "uad": False},
+                "uad": False,
+            },
             "aura.pageURI": login_url,
-            "aura.token": None}
-
+            "aura.token": None,
+        }
         params = {"r": 3, "other.LightningLoginCustom.login": 1}
-        async with session.post(
-                const.AUTH_API + "/s/sfsites/aura",
-                headers={"Content-Type": "application/x-www-form-urlencoded"},
-                data="&".join(f"{k}={json.dumps(v)}" for k, v in data.items()),
-                params=params
+        async with self._session.post(
+            const.AUTH_API + "/s/sfsites/aura",
+            headers={"Content-Type": "application/x-www-form-urlencoded"},
+            data="&".join(f"{k}={json.dumps(v)}" for k, v in data.items()),
+            params=params,
         ) as response:
             if response.status == 200:
                 try:
-                    return (await response.json())["events"][0]["attributes"]["values"]["url"]
+                    data = await response.json()
+                    return data["events"][0]["attributes"]["values"]["url"]
                 except json.JSONDecodeError:
                     pass
-            _LOGGER.error("Unable to login: %s\n%s", response.status, await response.text())
+                except KeyError:
+                    _LOGGER.error(
+                        "Can't get login url - %s", pformat(await response.json())
+                    )
+            _LOGGER.error(
+                "Unable to login: %s\n%s", response.status, await response.text()
+            )
             return ""
 
-    async def _get_token(self, session, url):
-        async with session.get(url) as resp:
+    async def _get_token(self, url):
+        async with self._session.get(url) as resp:
             if resp.status != 200:
                 _LOGGER.error("Unable to get token: %s", resp.status)
                 return False
-            url = re.findall("href\\s*=\\s*[\"'](.*?)[\"']", await resp.text())
-        async with session.get(url[0]) as resp:
+            url = re.findall("href\\s*=\\s*[\"'](http.+?)[\"']", await resp.text())
+            if not url:
+                _LOGGER.error("Can't get login url - \n%s", await resp.text())
+                raise PermissionError
+        async with self._session.get(url[0]) as resp:
             if resp.status != 200:
                 _LOGGER.error("Unable to get token: %s", resp.status)
                 return False
             url = re.findall("href\\s*=\\s*[\"'](.*?)[\"']", await resp.text())
             url = "/".join(const.AUTH_API.split("/")[:-1]) + url[0]
-        async with session.get(url) as resp:
+        async with self._session.get(url) as resp:
             if resp.status != 200:
                 _LOGGER.error("Unable to connect to the login service: %s", resp.status)
                 return False
             text = await resp.text()
         if access_token := re.findall("access_token=(.*?)&", text):
             self._access_token = access_token[0]
         if refresh_token := re.findall("refresh_token=(.*?)&", text):
             self._refresh_token = refresh_token[0]
         if id_token := re.findall("id_token=(.*?)&", text):
             self._id_token = id_token[0]
         return True
 
-    async def authorize(self, email, password, mobile_id):
-        headers = {"user-agent": const.USER_AGENT}
-        async with aiohttp.ClientSession(headers=headers) as session:
-            if login_site := await self._load_login(session):
-                fw_uid, loaded, login_url = login_site
-            else:
-                return False
-            if not (url := await self._login(session, email, password, fw_uid, loaded, login_url)):
-                return False
-            if not await self._get_token(session, url):
-                return False
-
-            post_headers = {"Content-Type": "application/json", "id-token": self._id_token}
-            data = {"appVersion": const.APP_VERSION, "mobileId": mobile_id, "osVersion": const.OS_VERSION,
-                    "os": const.OS, "deviceModel": const.DEVICE_MODEL}
-            async with session.post(f"{const.API_URL}/auth/v1/login", headers=post_headers, json=data) as resp:
-                try:
-                    json_data = await resp.json()
-                except json.JSONDecodeError:
-                    _LOGGER.error("No JSON Data after POST: %s", await resp.text())
-                    return False
-                self._cognito_token = json_data["cognitoUser"]["Token"]
+    async def authorize(self):
+        if login_site := await self._load_login():
+            fw_uid, loaded, login_url = login_site
+        else:
+            return False
+        if not (url := await self._login(fw_uid, loaded, login_url)):
+            return False
+        if not await self._get_token(url):
+            return False
+
+        post_headers = {"id-token": self._id_token}
+        data = self._device.get()
+        async with self._session.post(
+            f"{const.API_URL}/auth/v1/login", headers=post_headers, json=data
+        ) as resp:
+            try:
+                json_data = await resp.json()
+            except json.JSONDecodeError:
+                _LOGGER.error("No JSON Data after POST: %s", await resp.text())
+                return False
+            self._cognito_token = json_data["cognitoUser"]["Token"]
+        return True
+
+    async def refresh(self):
+        params = {
+            "client_id": const.CLIENT_ID,
+            "refresh_token": self._refresh_token,
+            "grant_type": "refresh_token",
+        }
+        async with self._session.post(
+            f"{const.AUTH_API}/services/oauth2/token", params=params
+        ) as resp:
+            if resp.status >= 400:
+                return False
+            data = await resp.json()
+        self._id_token = data["id_token"]
+        self._access_token = data["access_token"]
         return True
```

### Comparing `pyhOn-0.5.0/pyhon/commands.py` & `pyhOn-0.6.0/pyhon/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-from pyhon.parameter import HonParameterFixed, HonParameterEnum, HonParameterRange, HonParameterProgram
+from pyhon.parameter import (
+    HonParameterFixed,
+    HonParameterEnum,
+    HonParameterRange,
+    HonParameterProgram,
+)
 
 
 class HonCommand:
     def __init__(self, name, attributes, connector, device, multi=None, program=""):
         self._connector = connector
         self._device = device
         self._name = name
         self._multi = multi or {}
         self._program = program
         self._description = attributes.get("description", "")
         self._parameters = self._create_parameters(attributes.get("parameters", {}))
-        self._ancillary_parameters = self._create_parameters(attributes.get("ancillaryParameters", {}))
+        self._ancillary_parameters = self._create_parameters(
+            attributes.get("ancillaryParameters", {})
+        )
 
     def __repr__(self):
         return f"{self._name} command"
 
     def _create_parameters(self, parameters):
         result = {}
         for parameter, attributes in parameters.items():
@@ -31,19 +38,26 @@
 
     @property
     def parameters(self):
         return self._parameters
 
     @property
     def ancillary_parameters(self):
-        return {key: parameter.value for key, parameter in self._ancillary_parameters.items()}
+        return {
+            key: parameter.value
+            for key, parameter in self._ancillary_parameters.items()
+        }
 
     async def send(self):
-        parameters = {name: parameter.value for name, parameter in self._parameters.items()}
-        return await self._connector.send_command(self._device, self._name, parameters, self.ancillary_parameters)
+        parameters = {
+            name: parameter.value for name, parameter in self._parameters.items()
+        }
+        return await self._connector.send_command(
+            self._device, self._name, parameters, self.ancillary_parameters
+        )
 
     def get_programs(self):
         return self._multi
 
     def set_program(self, program):
         self._device.commands[self._name] = self._multi[program]
 
@@ -57,15 +71,20 @@
                 keys.append(key)
         return keys
 
     @property
     def setting_keys(self):
         if not self._multi:
             return self._get_settings_keys()
-        result = [key for cmd in self._multi.values() for key in self._get_settings_keys(cmd)]
+        result = [
+            key for cmd in self._multi.values() for key in self._get_settings_keys(cmd)
+        ]
         return list(set(result + ["program"]))
 
     @property
     def settings(self):
         """Parameters with typology enum and range"""
-        return {s: self._parameters.get(s) for s in self.setting_keys if self._parameters.get(s) is not None}
-
+        return {
+            s: self._parameters.get(s)
+            for s in self.setting_keys
+            if self._parameters.get(s) is not None
+        }
```

### Comparing `pyhOn-0.5.0/pyhon/device.py` & `pyhOn-0.6.0/pyhon/appliance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import importlib
 from contextlib import suppress
 
 from pyhon.commands import HonCommand
 from pyhon.parameter import HonParameterFixed
 
 
-class HonDevice:
-    def __init__(self, connector, appliance):
-        if attributes := appliance.get("attributes"):
-            appliance["attributes"] = {v["parName"]: v["parValue"] for v in attributes}
-        self._appliance = appliance
-        self._connector = connector
+class HonAppliance:
+    def __init__(self, api, info):
+        if attributes := info.get("attributes"):
+            info["attributes"] = {v["parName"]: v["parValue"] for v in attributes}
+        self._info = info
+        self._api = api
         self._appliance_model = {}
 
         self._commands = {}
         self._statistics = {}
         self._attributes = {}
 
         try:
-            self._extra = importlib.import_module(f'pyhon.appliances.{self.appliance_type.lower()}').Appliance()
+            self._extra = importlib.import_module(
+                f"pyhon.appliances.{self.appliance_type.lower()}"
+            ).Appliance()
         except ModuleNotFoundError:
             self._extra = None
 
     def __getitem__(self, item):
         if "." in item:
             result = self.data
             for key in item.split("."):
@@ -32,41 +34,41 @@
                     result = result[key]
             return result
         else:
             if item in self.data:
                 return self.data[item]
             if item in self.attributes["parameters"]:
                 return self.attributes["parameters"].get(item)
-            return self.appliance[item]
+            return self.info[item]
 
     def get(self, item, default=None):
         try:
             return self[item]
         except (KeyError, IndexError):
             return default
 
     @property
     def appliance_model_id(self):
-        return self._appliance.get("applianceModelId")
+        return self._info.get("applianceModelId")
 
     @property
     def appliance_type(self):
-        return self._appliance.get("applianceTypeName")
+        return self._info.get("applianceTypeName")
 
     @property
     def mac_address(self):
-        return self._appliance.get("macAddress")
+        return self._info.get("macAddress")
 
     @property
     def model_name(self):
-        return self._appliance.get("modelName")
+        return self._info.get("modelName")
 
     @property
     def nick_name(self):
-        return self._appliance.get("nickName")
+        return self._info.get("nickName")
 
     @property
     def commands_options(self):
         return self._appliance_model.get("options")
 
     @property
     def commands(self):
@@ -77,46 +79,58 @@
         return self._attributes
 
     @property
     def statistics(self):
         return self._statistics
 
     @property
-    def appliance(self):
-        return self._appliance
+    def info(self):
+        return self._info
 
     async def _recover_last_command_states(self, commands):
-        command_history = await self._connector.command_history(self)
+        command_history = await self._api.command_history(self)
         for name, command in commands.items():
-            last = next((index for (index, d) in enumerate(command_history) if d.get("command", {}).get("commandName") == name), None)
+            last = next(
+                (
+                    index
+                    for (index, d) in enumerate(command_history)
+                    if d.get("command", {}).get("commandName") == name
+                ),
+                None,
+            )
             if last is None:
                 continue
             parameters = command_history[last].get("command", {}).get("parameters", {})
             if command._multi and parameters.get("program"):
                 command.set_program(parameters.pop("program").split(".")[-1].lower())
                 command = self.commands[name]
             for key, data in command.settings.items():
-                if not isinstance(data, HonParameterFixed) and parameters.get(key) is not None:
+                if (
+                    not isinstance(data, HonParameterFixed)
+                    and parameters.get(key) is not None
+                ):
                     with suppress(ValueError):
                         data.value = parameters.get(key)
 
     async def load_commands(self):
-        raw = await self._connector.load_commands(self)
+        raw = await self._api.load_commands(self)
         self._appliance_model = raw.pop("applianceModel")
         for item in ["settings", "options", "dictionaryId"]:
             raw.pop(item)
         commands = {}
         for command, attr in raw.items():
             if "parameters" in attr:
-                commands[command] = HonCommand(command, attr, self._connector, self)
+                commands[command] = HonCommand(command, attr, self._api, self)
             elif "parameters" in attr[list(attr)[0]]:
                 multi = {}
                 for program, attr2 in attr.items():
                     program = program.split(".")[-1].lower()
-                    cmd = HonCommand(command, attr2, self._connector, self, multi=multi, program=program)
+                    cmd = HonCommand(
+                        command, attr2, self._api, self, multi=multi, program=program
+                    )
                     multi[program] = cmd
                     commands[command] = cmd
         self._commands = commands
         await self._recover_last_command_states(commands)
 
     @property
     def settings(self):
@@ -133,24 +147,28 @@
         result = {}
         for name, command in self._commands.items():
             for key, parameter in command.parameters.items():
                 result.setdefault(name, {})[key] = parameter.value
         return result
 
     async def load_attributes(self):
-        self._attributes = await self._connector.load_attributes(self)
+        self._attributes = await self._api.load_attributes(self)
         for name, values in self._attributes.pop("shadow").get("parameters").items():
             self._attributes.setdefault("parameters", {})[name] = values["parNewVal"]
 
     async def load_statistics(self):
-        self._statistics = await self._connector.load_statistics(self)
+        self._statistics = await self._api.load_statistics(self)
 
     async def update(self):
         await self.load_attributes()
 
     @property
     def data(self):
-        result = {"attributes": self.attributes, "appliance": self.appliance, "statistics": self.statistics,
-                  **self.parameters}
+        result = {
+            "attributes": self.attributes,
+            "appliance": self.info,
+            "statistics": self.statistics,
+            **self.parameters,
+        }
         if self._extra:
             return self._extra.data(result)
         return result
```

### Comparing `pyhOn-0.5.0/pyhon/parameter.py` & `pyhOn-0.6.0/pyhon/parameter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import re
+
+
 class HonParameter:
     def __init__(self, key, attributes):
         self._key = key
         self._category = attributes.get("category")
         self._typology = attributes.get("typology")
         self._mandatory = attributes.get("mandatory")
         self._value = ""
@@ -75,15 +78,17 @@
 
     @value.setter
     def value(self, value):
         value = int(value)
         if self._min <= value <= self._max and not value % self._step:
             self._value = value
         else:
-            raise ValueError(f"Allowed: min {self._min} max {self._max} step {self._step}")
+            raise ValueError(
+                f"Allowed: min {self._min} max {self._max} step {self._step}"
+            )
 
 
 class HonParameterEnum(HonParameter):
     def __init__(self, key, attributes):
         super().__init__(key, attributes)
         self._default = attributes.get("defaultValue")
         self._value = self._default or "0"
@@ -134,8 +139,12 @@
 
     @filter.setter
     def filter(self, filter):
         self._filter = filter
 
     @property
     def values(self):
-        return sorted([str(value) for value in self._values if not self._filter or self._filter in str(value)])
+        values = []
+        for value in self._values:
+            if not self._filter or re.findall(self._filter, str(value)):
+                values.append(str(value))
+        return sorted(values)
```

### Comparing `pyhOn-0.5.0/setup.py` & `pyhOn-0.6.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.5.0",
+    version="0.6.0",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
     },
     license="MIT",
     platforms="any",
     packages=find_packages(),
@@ -29,12 +29,12 @@
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     entry_points={
-        'console_scripts': [
-            'pyhOn = pyhon.__main__:start',
+        "console_scripts": [
+            "pyhOn = pyhon.__main__:start",
         ]
-    }
+    },
 )
```


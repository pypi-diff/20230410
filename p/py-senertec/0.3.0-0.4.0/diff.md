# Comparing `tmp/py-senertec-0.3.0.tar.gz` & `tmp/py-senertec-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-senertec-0.3.0.tar", last modified: Tue Dec 20 17:04:41 2022, max compression
+gzip compressed data, was "py-senertec-0.4.0.tar", last modified: Mon Apr 10 19:39:48 2023, max compression
```

## Comparing `py-senertec-0.3.0.tar` & `py-senertec-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 17:04:41.508406 py-senertec-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-20 17:04:31.000000 py-senertec-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2022-12-20 17:04:41.508406 py-senertec-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2022-12-20 17:04:31.000000 py-senertec-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-20 17:04:31.000000 py-senertec-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 17:04:41.508406 py-senertec-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      896 2022-12-20 17:04:31.000000 py-senertec-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 17:04:41.500406 py-senertec-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 17:04:41.504407 py-senertec-0.3.0/src/py_senertec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2022-12-20 17:04:41.000000 py-senertec-0.3.0/src/py_senertec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2022-12-20 17:04:41.000000 py-senertec-0.3.0/src/py_senertec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 17:04:41.000000 py-senertec-0.3.0/src/py_senertec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-20 17:04:41.000000 py-senertec-0.3.0/src/py_senertec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-20 17:04:41.000000 py-senertec-0.3.0/src/py_senertec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 17:04:41.508406 py-senertec-0.3.0/src/senertec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 17:04:31.000000 py-senertec-0.3.0/src/senertec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2022-12-20 17:04:31.000000 py-senertec-0.3.0/src/senertec/board.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2022-12-20 17:04:31.000000 py-senertec-0.3.0/src/senertec/canipError.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2022-12-20 17:04:31.000000 py-senertec-0.3.0/src/senertec/canipValue.py
--rw-r--r--   0 runner    (1001) docker     (123)    19921 2022-12-20 17:04:31.000000 py-senertec-0.3.0/src/senertec/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2022-12-20 17:04:31.000000 py-senertec-0.3.0/src/senertec/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2022-12-20 17:04:31.000000 py-senertec-0.3.0/src/senertec/energyUnit.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-20 17:04:31.000000 py-senertec-0.3.0/src/senertec/lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:48.393090 py-senertec-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 19:39:38.000000 py-senertec-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-10 19:39:48.393090 py-senertec-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-10 19:39:38.000000 py-senertec-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 19:39:38.000000 py-senertec-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:39:48.393090 py-senertec-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-10 19:39:41.000000 py-senertec-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:48.389090 py-senertec-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:48.393090 py-senertec-0.4.0/src/py_senertec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-10 19:39:48.000000 py-senertec-0.4.0/src/py_senertec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 19:39:48.000000 py-senertec-0.4.0/src/py_senertec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:39:48.000000 py-senertec-0.4.0/src/py_senertec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:39:48.000000 py-senertec-0.4.0/src/py_senertec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 19:39:48.000000 py-senertec-0.4.0/src/py_senertec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:48.393090 py-senertec-0.4.0/src/senertec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/canipError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/canipValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/energyUnit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/obdClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:48.393090 py-senertec-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-10 19:39:38.000000 py-senertec-0.4.0/tests/test_base.py
```

### Comparing `py-senertec-0.3.0/LICENSE` & `py-senertec-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-senertec-0.3.0/PKG-INFO` & `py-senertec-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-senertec
-Version: 0.3.0
+Version: 0.4.0
 Summary: Senertec energy system gen2 interface.
 Home-page: https://github.com/Kleinrotti/py-senertec
 Author: Kleinrotti
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/Kleinrotti/py-senertec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,21 +21,22 @@
 ## Description
 
 The **py-senertec** library provides a way to communicate with Senertec Dachsportal2 to monitor your energy unit.
 This library supports read-only communication. So *changing* values for your energy unit isn't implemented and not planned yet.
 
 ## Requirements
 
-*   **Python 3.6+**
+*   **Python 3.9+**
 *   **Account for Senertec Dachsportal2/Remeha KWK**
 
 ## Tested with this devices
 
 I could test with this devices but others should also work:  
 *   Senertec Dachs 0.8
+*   Senertec Dachs InnoGen
 *   Senertec Dachs Gen2 F5.5
 *   Remeha eLecta 300 (technically same as Senertec Dachs 0.8)
 
 
 ## Installation
 
 ```sh
@@ -99,7 +100,11 @@
 ## Filtering (recommended)
 If you specify a json string in the senertec contructor you can limit what datapoints should be received.
 This is pretty usefull if you know what data you want from your heating system e.g. power, temperature.
 By default all datapoints are included which are more than 400 in most cases and receiving them takes some time.
 This json string should look like [this](https://github.com/Kleinrotti/py-senertec/blob/main/examples/datapointFilter.json).
 The json string contains the productGroup at the top and below the datapoints which should be included.
 You get the productGroup from the getUnits() function.
+
+## What are these datapoints?
+Take a look at this manual from [Remeha](https://mediacdn.remeha.de/-/media/websites/remehade/downloads/produkte/regenerative-hybrid/gas-hybrid-waerme-und-strom/electa-ace-300/electaace300_bedienungsanleitung_02-23.pdf?v=1&d=20230228T114400Z) (Page 39).
+There is already a good explanation of how these datapoints are composed.
```

### Comparing `py-senertec-0.3.0/README.md` & `py-senertec-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 ## Description
 
 The **py-senertec** library provides a way to communicate with Senertec Dachsportal2 to monitor your energy unit.
 This library supports read-only communication. So *changing* values for your energy unit isn't implemented and not planned yet.
 
 ## Requirements
 
-*   **Python 3.6+**
+*   **Python 3.9+**
 *   **Account for Senertec Dachsportal2/Remeha KWK**
 
 ## Tested with this devices
 
 I could test with this devices but others should also work:  
 *   Senertec Dachs 0.8
+*   Senertec Dachs InnoGen
 *   Senertec Dachs Gen2 F5.5
 *   Remeha eLecta 300 (technically same as Senertec Dachs 0.8)
 
 
 ## Installation
 
 ```sh
@@ -83,8 +84,12 @@
 
 ## Filtering (recommended)
 If you specify a json string in the senertec contructor you can limit what datapoints should be received.
 This is pretty usefull if you know what data you want from your heating system e.g. power, temperature.
 By default all datapoints are included which are more than 400 in most cases and receiving them takes some time.
 This json string should look like [this](https://github.com/Kleinrotti/py-senertec/blob/main/examples/datapointFilter.json).
 The json string contains the productGroup at the top and below the datapoints which should be included.
-You get the productGroup from the getUnits() function.
+You get the productGroup from the getUnits() function.
+
+## What are these datapoints?
+Take a look at this manual from [Remeha](https://mediacdn.remeha.de/-/media/websites/remehade/downloads/produkte/regenerative-hybrid/gas-hybrid-waerme-und-strom/electa-ace-300/electaace300_bedienungsanleitung_02-23.pdf?v=1&d=20230228T114400Z) (Page 39).
+There is already a good explanation of how these datapoints are composed.
```

### Comparing `py-senertec-0.3.0/setup.py` & `py-senertec-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py-senertec",
-    version="0.3.0",
+    version="0.4.0",
     author="Kleinrotti",
     author_email="",
     package_dir={"": "src"},
     packages=setuptools.find_packages("src"),
     description="Senertec energy system gen2 interface.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `py-senertec-0.3.0/src/py_senertec.egg-info/PKG-INFO` & `py-senertec-0.4.0/src/py_senertec.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-senertec
-Version: 0.3.0
+Version: 0.4.0
 Summary: Senertec energy system gen2 interface.
 Home-page: https://github.com/Kleinrotti/py-senertec
 Author: Kleinrotti
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/Kleinrotti/py-senertec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,21 +21,22 @@
 ## Description
 
 The **py-senertec** library provides a way to communicate with Senertec Dachsportal2 to monitor your energy unit.
 This library supports read-only communication. So *changing* values for your energy unit isn't implemented and not planned yet.
 
 ## Requirements
 
-*   **Python 3.6+**
+*   **Python 3.9+**
 *   **Account for Senertec Dachsportal2/Remeha KWK**
 
 ## Tested with this devices
 
 I could test with this devices but others should also work:  
 *   Senertec Dachs 0.8
+*   Senertec Dachs InnoGen
 *   Senertec Dachs Gen2 F5.5
 *   Remeha eLecta 300 (technically same as Senertec Dachs 0.8)
 
 
 ## Installation
 
 ```sh
@@ -99,7 +100,11 @@
 ## Filtering (recommended)
 If you specify a json string in the senertec contructor you can limit what datapoints should be received.
 This is pretty usefull if you know what data you want from your heating system e.g. power, temperature.
 By default all datapoints are included which are more than 400 in most cases and receiving them takes some time.
 This json string should look like [this](https://github.com/Kleinrotti/py-senertec/blob/main/examples/datapointFilter.json).
 The json string contains the productGroup at the top and below the datapoints which should be included.
 You get the productGroup from the getUnits() function.
+
+## What are these datapoints?
+Take a look at this manual from [Remeha](https://mediacdn.remeha.de/-/media/websites/remehade/downloads/produkte/regenerative-hybrid/gas-hybrid-waerme-und-strom/electa-ace-300/electaace300_bedienungsanleitung_02-23.pdf?v=1&d=20230228T114400Z) (Page 39).
+There is already a good explanation of how these datapoints are composed.
```

### Comparing `py-senertec-0.3.0/src/senertec/board.py` & `py-senertec-0.4.0/src/senertec/datapoint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,22 @@
-from .datapoint import datapoint
+from .obdClass import obdClass
 
 
-class board(object):
-    """Represents an electronic board of the energy unit."""
+class datapoint(object):
+    """Represents a datapoint of a board."""
     def __init__(self):
-        self.boardName = str()
-        """Name of the board."""
+        self.id = str()
+        """Unique datapoint id. This id is random and changes every session."""
+        self.sourceId = str()
+        """Name of the datapoint e.g. BM001."""
         self.friendlyName = str()
-        """Human readable name of the board."""
-        self.datapoints = [datapoint()]
-        """Stores datapoints of the board."""
-        self.datapoints.pop()  # remove default element
-
-    def getFullDatapoint(self, index: int):
-        """Get the full datapoint string."""
-        return self.boardName + "." + self.datapoints[index]
-
-    def getDatapointByName(self, name: str):
-        """Get a datapoint by its name. Not case sensitive."""
-        for point in self.datapoints:
-            if name.lower() in point.friendlyName.lower():
-                return point
-
-    def getFullDataPointIds(self):
-        """Get all datapoints."""
-        lst = []
-        for i in self.datapoints:
-            lst.append(self.boardName + "." + i.id)
-        return lst
+        """Human readable name of the datapoint."""
+        self.unit = str()
+        """Unit of the datapoint."""
+        self.gain = int()
+        """Scaling of interger or float values."""
+        self.enumName = str()
+        """If the datapoint is an enum, this value is set."""
+        self.type = obdClass
+        """The datapoint obdClass."""
+        self.array = bool
+        """Indicates if this datapoint is an array."""
```

### Comparing `py-senertec-0.3.0/src/senertec/canipValue.py` & `py-senertec-0.4.0/src/senertec/canipValue.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,7 +9,11 @@
         """Value"""
         self.dataUnit = str()
         """Unit of the value."""
         self.friendlyDataName = str()
         """Human readable data value name."""
         self.sourceDatapoint = str()
         """Id of datapoint which was requested."""
+        self.array = bool()
+        """Indicates if this canipValue is part of an array."""
+        self.deviceSerial = str()
+        """The serial of the device this canipValue belongs to."""
```

### Comparing `py-senertec-0.3.0/src/senertec/client.py` & `py-senertec-0.4.0/src/senertec/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,469 +1,487 @@
-from asyncio.log import logger
-import inspect
-import json
-import logging
-from threading import Thread
-import requests
-import websocket
-from bs4 import BeautifulSoup
-from .energyUnit import energyUnit
-from .lang import lang
-from .canipError import canipError
-from .canipValue import canipValue
-from .board import board
-from .datapoint import datapoint
-
-
-class basesocketclient:
-    """Base class which provides logic for a senertec websocket connection."""
-
-    def __init__(self, level=logging.WARN):
-        self.logger = logging.getLogger(__name__)
-        self.logger.setLevel(level)
-        self.WS_HOST = "wss://dachsconnect.senertec.com/ws"
-        self.__is_ws_connected__ = False
-        self.__messages__ = [str()]
-        self.__thread__ = None
-        self.ws = None
-        self.boards = [board()]
-        """All available boards with datapoints which can be used in request function"""
-
-    def __on_message__(self, ws, message):
-        j = json.loads(message)
-        action = j["action"]
-        data = j["data"]
-        if action == "CanipValue":
-            self.logger.debug("Received new CanipValue from websocket.")
-            for b in self.boards:
-                if b.boardName == data["boardName"]:
-                    value = canipValue()
-                    value.boardName = b.boardName
-                    for point in b.datapoints:
-                        if point.id == data["dataPointName"]:
-                            value.friendlyDataName = point.friendlyName
-                            value.sourceDatapoint = point.sourceId
-                            tempValue = data["value"]
-                            if point.enumName != None:
-                                for enum in self.__enumTranslations__:
-                                    if point.enumName == enum["name"]:
-                                        try:
-                                            value.dataValue = enum["translations"][f"{tempValue}"]
-                                        except KeyError:
-                                            self.logger.warning(
-                                                f"No enum translation found for datapoint '{point.friendlyName}'.")
-                                            value.dataValue = "Unknown"
-                            elif point.gain != 0 and point.gain != 1:
-                                value.dataValue = tempValue * \
-                                    point.gain
-                            else:
-                                value.dataValue = tempValue
-                            if point.unit != None:
-                                value.dataUnit = point.unit
-                            else:
-                                value.dataUnit = ""
-                            self.messagecallback(value)
-                            break
-        elif action == "HkaStore" and data["updateType"] == "remove":
-            sn = j["sn"]
-            self.logger.info(
-                f"Unit with serial {sn} got disconnected.")
-        else:
-            self.logger.debug(f"Received new websocket message {action}.")
-            self.__messages__.append(message)
-
-    def __on_error__(self, ws, error):
-        self.logger.error(f"error : {error}")
-
-    def __on_close__(self, ws, close_status_code, close_msg):
-        self.logger.info(
-            f"Senertec Websocket closed with code {close_status_code}")
-        self.__is_ws_connected__ = False
-
-    def __on_open__(self, ws):
-        self.logger.info("Connected to Senertec websocket")
-        self.__is_ws_connected__ = True
-
-    def __create_websocket__(self):
-        cookies = self.__getCookies__(
-            self.__session__.cookies, "dachsconnect.senertec.com")
-        self.logger.debug("Creating websocket connection..")
-        self.ws = websocket.WebSocketApp(self.WS_HOST,
-                                         on_message=self.__on_message__,
-                                         on_error=self.__on_error__,
-                                         on_close=self.__on_close__,
-                                         on_open=self.__on_open__,
-                                         cookie=cookies)
-        self.__thread__ = Thread(
-            target=self.ws.run_forever, kwargs={
-                "ping_interval": 60, "ping_timeout": 5}
-        )
-        self.__thread__.daemon = True
-        self.__thread__.setName("senertec-websocket")
-        self.__thread__.start()
-        self.logger.debug("Websocket connection started.")
-
-
-class senertec(basesocketclient):
-    """Class to communicate with Senertec and handle network calls"""
-
-    def __init__(self, datapointList=None, email: str = None, password: str = None, language=lang.English, level=logging.INFO):
-        """Constructor, create instance of senertec client.
-
-        ``datapointList`` Json string to add only these datapoints instead of everything.
-
-        ``language`` Set to your language.
-        """
-        if email is None or password is None:
-            raise ValueError(
-                "Arguments 'email', 'passwords'"
-            )
-        super().__init__(level)
-        logging.basicConfig(
-            level=level,
-            format='py-senertec: %(asctime)s %(levelname)-8s %(message)s',
-            datefmt='%Y-%m-%d %H:%M:%S'
-        )
-        self.AUTHENTICATION_HOST = "https://dachsconnect.senertec.com"
-        self.SSO_HOST = "https://sso-portal.senertec.com"
-        self.email = email
-        self.__session__ = None
-        self.language = language
-        self.password = password
-        self.level = level
-        self.__filteredDatapoints__ = datapointList
-        self.__enums__ = []
-        self.__metaDataPoints__ = []
-        self.__metaDataTranslations__ = []
-        self.__enumTranslations__ = []
-        self.__errorTranslations__ = []
-        self.__connectedUnit__ = []
-        self.__appVersion__ = ""
-        self.messagecallback = (canipValue())
-        """Set your callback function to get the data values. Function has to be overloaded with data type ``canipValue``"""
-        self.logger = logging.getLogger(__name__)
-        self.logger.setLevel(level)
-
-    def __create_headers__(self):
-        headers = {"Content-Type": "application/json"}
-        return headers
-
-    def __getCookies__(self, cookie_jar, domain):
-        cookie_dict = cookie_jar.get_dict(domain=domain)
-        found = ['%s=%s' % (name, value)
-                 for (name, value) in cookie_dict.items()]
-        return ';'.join(found)
-
-    def __post__(self, urlPath: str, payload: str):
-        url = self.AUTHENTICATION_HOST + urlPath
-        response = self.__session__.post(
-            url, data=payload, headers=self.__create_headers__())
-        if (response.status_code >= 400 and response.status_code <= 599):
-            logger.error("Error in post request by function: " + inspect.stack()
-                         [1].function + " HTTP response: " + response.text)
-        return response
-
-    def __get__(self, urlPath: str):
-        url = self.AUTHENTICATION_HOST + urlPath
-        response = self.__session__.get(
-            url, headers=self.__create_headers__())
-        if (response.status_code >= 400 and response.status_code <= 599):
-            logger.error("Error in get request by function: {" + inspect.stack()
-                         [1].function + "} HTTP response: " + response.text)
-        return response
-
-    def __parseDataPoints__(self):
-        """Parse all available datapoints for connected unit."""
-        self.logger.debug("Starting to parse datapoints..")
-        dataPointCount = 0
-        metaData = self.__metaDataPoints__
-        allPoints = []
-        boardList = []
-
-        # first collect all available datapoints
-        for point in metaData:
-            if metaData[point]["friendlyName"] is not None:
-                datap = datapoint()
-                datap.sourceId = metaData[point]["friendlyName"]
-                datap.friendlyName = self.__metaDataTranslations__[
-                    metaData[point]["name"]]
-                datap.id = metaData[point]["name"]
-                datap.gain = metaData[point]["gain"]
-                datap.unit = metaData[point]["unit"]
-                datap.enumName = metaData[point]["enumName"]
-                allPoints.append(datap)
-                # loop through all boards of unit
-                for b in self.__connectedUnit__["boards"]:
-                    # add board to the collection if its not already included
-                    if not any(x for x in boardList if x.boardName == b["name"]):
-                        device = board()
-                        device.boardName = b["name"]
-                        boardList.append(device)
-                    # loop through datapoints of that board and add available points
-                    for at in b["attributes"]:
-                        if at == datap.id:
-                            for b1 in boardList:
-                                if b1.boardName == b["name"]:
-                                    dataPointCount += 1
-                                    b1.datapoints.append(datap)
-                            break
-        self.logger.debug(
-            f"Finished datapoints parsing. Found {len(boardList)} boards with {dataPointCount} datapoints in total.")
-        self.boards = boardList
-        return
-
-    def __parseDataPointsFiltered__(self):
-        """Use this function to include only datapoints of datapointList which was set in class constructor."""
-        self.logger.debug("Starting to parse datapoints..")
-        metaData = self.__metaDataPoints__
-        blist = []
-        dataPointCount = 0
-        boardname = ""
-        for a in metaData:
-            for element in self.__filteredDatapoints__[self.__connectedUnit__["productGroup"]]:
-                if metaData[a]["friendlyName"] == element:
-                    for l in self.__connectedUnit__["boards"]:
-                        for o in l["attributes"]:
-                            if o == metaData[a]["name"]:
-                                boardname = l["name"]
-                    datap = datapoint()
-                    datap.sourceId = element
-                    datap.id = metaData[a]["name"]
-                    datap.friendlyName = self.__metaDataTranslations__[
-                        metaData[a]["name"]]
-                    datap.unit = metaData[a]["unit"]
-                    datap.gain = metaData[a]["gain"]
-                    datap.enumName = metaData[a]["enumName"]
-                    dataPointCount += 1
-                    # avoid doubled board entries
-                    if not any(x for x in blist if x.boardName == boardname):
-                        b = board()
-                        b.boardName = boardname
-                        b.datapoints.append(datap)
-                        blist.append(b)
-                    else:
-                        for b in blist:
-                            if b.boardName == boardname:
-                                b.datapoints.append(datap)
-        self.boards = blist
-        self.logger.debug(
-            f"Finished datapoints parsing. Found {len(blist)} boards with {dataPointCount} datapoints in total.")
-
-    @property
-    def portalVersion(self) -> str:
-        """Returns Senertec Dachsportal version.
-
-        Init function has to be called first.
-        """
-        return self.__appVersion__
-
-    def login(self):
-        """
-        Login.
-
-        This function needs to be called first.
-
-        Returns True on success, False on failure.
-        """
-        self.logger.info("Logging in..")
-        self.__session__ = requests.Session()
-        loginSSOResponse = self.__session__.get(
-            self.AUTHENTICATION_HOST + "/rest/saml2/login")
-
-        authState = loginSSOResponse.url.split("loginuserpass.php?")[1]
-        head = {"Content-Type": "application/x-www-form-urlencoded"}
-        userData = f"username={self.email}&password={self.password}&{authState}"
-        # submit credentials
-        loginResponse = self.__session__.post(self.SSO_HOST + "/simplesaml/module.php/core/loginuserpass.php?",
-                                              data=userData, headers=head)
-
-        # filter out samlresponse and relaystate for ACS request
-        soup = BeautifulSoup(loginResponse.text, features="html.parser")
-        try:
-            samlResponse = soup.findAll(
-                "input", {"name": "SAMLResponse"})[0]["value"]
-            relayState = soup.findAll(
-                "input", {"name": "RelayState"})[0]["value"]
-        except IndexError:
-            self.logger.error("Login failed, username or password wrong.")
-            return False
-        acsData = {'SAMLResponse': {samlResponse}, 'RelayState': {relayState}}
-
-        # do assertion consumer service request with received saml response
-        acs = self.__session__.post(
-            self.AUTHENTICATION_HOST + "/rest/saml2/acs", data=acsData, headers=head)
-
-        if acs.history[0].status_code != 302:
-            self.logger.error("Login failed at ACS request, got no redirect.")
-            return False
-        self.logger.info("Login was successful.")
-        return True
-
-    def logout(self):
-        """
-        Logout from senertec.
-
-        Returns True on success, False on failure.
-        """
-        self.logger.info("Logging out..")
-        response = self.__get__("/logout")
-        if self.ws:
-            self.ws.close()
-        self.__session__.close()
-        if response.status_code == 200:
-            self.logger.debug("Logout was successful.")
-            return True
-        else:
-            return False
-
-    def init(self):
-        """
-        Initialize Senertec platform and connect to websocket.
-
-        This function needs to be called after login.
-
-        Returns True on success, False on failure.
-        """
-        self.logger.info("Initializing senertec platform...")
-        response = self.__get__("/rest/info/init")
-        if response.status_code == 200:
-            self.__create_websocket__()
-            j = json.loads(response.text)
-            self.__metaDataPoints__ = j["metaDataPoints"]
-            self.__enums__ = j["enums"]
-            self.__enumTranslations__ = j["translations"][f"{self.language.value}"]["enums"]
-            self.__metaDataTranslations__ = j["translations"][
-                f"{self.language.value}"]["metaDataPoints"]["translations"]
-            self.__errorTranslations__ = j["translations"][f"{self.language.value}"]["errorCategories"]
-            self.__appVersion__ = j["app"]["version"]
-            return True
-        else:
-            return False
-
-    def getUnits(self) -> list[energyUnit]:
-        """
-        Get all units.
-
-        Returns all energy units of this account as object list.
-        """
-        response = self.__post__(
-            "/rest/info/units", json.dumps({"limit": 10, "offset": 0, "filter": {}}))
-        if response.status_code == 200:
-            values = json.loads(response.text)
-            units = []
-            for x in values["units"]:
-                unit = energyUnit()
-                unit.model = x["benennung"]
-                unit.serial = x["seriennummer"]
-                unit.connected = x["connected"]
-                unit.online = x["online"]
-                unit.itemNumber = x["artikelNummer"]
-                unit.contact = x["standortAnsprech"]
-                unit.city = x["standortOrt"]
-                unit.locationName = x["standortName"]
-                unit.postalCode = x["standortPlz"]
-                unit.street = x["standortAdresse"]
-                unit.productGroup = x["productGroup"]
-                units.append(unit)
-            self.logger.debug(
-                f"Successful received a list of {len(units)} units.")
-            return units
-        else:
-            return None
-
-    def connectUnit(self, serial: str):
-        """
-        This function connects to a unit and enables receiving data for that unit.
-
-        ``serial`` Serial number of energy unit. Can be received with getUnits() method.
-
-        Returns True on success, False on failure.
-        """
-        response = self.__get__(f"/rest/canip/{serial}")
-        if response.status_code == 200:
-            self.__connectedUnit__ = json.loads(response.text)
-            # if no supported items were set in constructor, do not filter and parse every datapoint
-            if self.__filteredDatapoints__ is None:
-                self.__parseDataPoints__()
-            else:
-                self.__parseDataPointsFiltered__()
-            return True
-        else:
-            return False
-
-    def disconnectUnit(self):
-        """
-        Disconnect from a unit.
-
-        Returns True on success, False on failure.
-        """
-        sn = self.__connectedUnit__["seriennummer"]
-        response = self.__get__(f"/rest/canip/{sn}/disconnect")
-        if response.status_code == 200:
-            return True
-        else:
-            return False
-
-    def getChart(self, chartname: str):
-        """
-        Get a history chart of the connected unit.
-        """
-        sn = self.__connectedUnit__["seriennummer"]
-        response = self.__post__(
-            f"/rest/charts/{sn}/data", json.dumps(
-                {"start": 1641596400000, "end": None, "parameters": {}, "chartName": chartname, "sn": sn}))
-        if response.status_code == 200:
-            return json.loads(response.text)
-
-    def request(self, dataPoints: list):
-        """
-        Request data from specific datapoints of the connected unit.
-
-        Data wil be received through websocket.
-
-        ``dataPoints`` List of datapoint strings
-
-        Returns True on success, False on failure.
-        """
-        sn = self.__connectedUnit__["seriennummer"]
-        j = json.dumps(
-            {"seriennummer": sn, "keys": dataPoints})
-        response = self.__post__(
-            f"/rest/canip/{sn}/request", j)
-        result = json.loads(response.text)
-        if response.status_code == 200 and result["success"] and not result["errorKeys"]:
-            return True
-        else:
-            return False
-
-    def getBoardList(self):
-        """Get all boards of the connected unit"""
-        lst = [str()]
-        for b in self.__connectedUnit__["boards"]:
-            lst.append(b["name"])
-        return lst
-
-    def getErrors(self, onlyCurrentErrors: bool = True) -> list[canipError]:
-        """Get an error history of the connected unit.
-
-        ``onlyCurrentErrors`` Return only errors which are present now. Set to false if you want error history.
-
-        This gets loaded when a unit gets connected."""
-        lst = []
-        for b in self.__connectedUnit__["boards"]:
-            for e in b["canipErrors"]:
-                if onlyCurrentErrors and not e["currentError"]:
-                    continue
-                error = canipError()
-                error.boardName = e["boardName"]
-                error.code = e["codeText"]
-                error.counter = e["counter"]
-                error.currentError = e["currentError"]
-                error.timestamp = e["timestamp"]
-                cat = e["errorCode"]["category"]
-                code = e["errorCode"]["code"]
-                error.errorCategory = self.__errorTranslations__[
-                    f"{cat}"]["translationMedium"]
-                error.errorTranslation = self.__errorTranslations__[
-                    f"{cat}"]["translations"][f"{code}"]
-                lst.append(error)
-        return lst
+from asyncio.log import logger
+import inspect
+import json
+import logging
+from threading import Thread
+import requests
+import websocket
+from bs4 import BeautifulSoup
+
+from .obdClass import obdClass
+from .energyUnit import energyUnit
+from .lang import lang
+from .canipError import canipError
+from .canipValue import canipValue
+from .board import board
+from .datapoint import datapoint
+
+
+class basesocketclient:
+    """Base class which provides logic for a senertec websocket connection."""
+
+    def __init__(self, level=logging.WARN):
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(level)
+        self.WS_HOST = "wss://dachsconnect.senertec.com/ws"
+        self.__is_ws_connected__ = False
+        self.__messages__ = [str()]
+        self.__thread__ = None
+        self.ws = None
+        self.boards = [board()]
+        """All available boards with datapoints which can be used in request function"""
+
+    def __on_message__(self, ws, message):
+        j = json.loads(message)
+        action = j["action"]
+        data = j["data"]
+        if action == "CanipValue":
+            self.logger.debug("Received new CanipValue from websocket.")
+            # skip old values and array size indicators
+            if (data["age"] != 0 or data["size"] == True):
+                return
+            for b in self.boards:
+                if b.boardName == data["boardName"]:
+                    value = canipValue()
+                    value.boardName = b.boardName
+                    value.array = data["array"]
+                    value.deviceSerial = data["sn"]
+                    for point in b.datapoints:
+                        if point.id == data["dataPointName"]:
+                            #if the data is an array, add the index to the name
+                            if (data["index"] != None):
+                                value.friendlyDataName = point.friendlyName + \
+                                    " " + data["index"].__str__()
+                                value.sourceDatapoint = point.sourceId + \
+                                    "_" + data["index"].__str__()
+                            else:
+                                value.friendlyDataName = point.friendlyName
+                                value.sourceDatapoint = point.sourceId
+                            tempValue = data["value"]
+                            if point.enumName != None:
+                                for enum in self.__enumTranslations__:
+                                    if point.enumName == enum["name"]:
+                                        try:
+                                            value.dataValue = enum["translations"][f"{tempValue}"]
+                                        except KeyError:
+                                            self.logger.warning(
+                                                f"No enum translation found for datapoint '{point.friendlyName}'.")
+                                            value.dataValue = "Unknown"
+                            elif point.gain != 0:
+                                value.dataValue = round(tempValue *
+                                                        point.gain, 2)
+                            else:
+                                value.dataValue = tempValue
+                            if point.unit != None:
+                                value.dataUnit = point.unit
+                            else:
+                                value.dataUnit = ""
+                            self.messagecallback(value)
+                            break
+        elif action == "HkaStore" and data["updateType"] == "remove":
+            sn = j["sn"]
+            self.logger.info(
+                f"Unit with serial {sn} got disconnected.")
+        else:
+            self.logger.debug(f"Received new websocket message {action}.")
+            self.__messages__.append(message)
+
+    def __on_error__(self, ws, error):
+        self.logger.error(f"error : {error}")
+
+    def __on_close__(self, ws, close_status_code, close_msg):
+        self.logger.info(
+            f"Senertec Websocket closed with code {close_status_code}")
+        self.__is_ws_connected__ = False
+
+    def __on_open__(self, ws):
+        self.logger.info("Connected to Senertec websocket")
+        self.__is_ws_connected__ = True
+
+    def __create_websocket__(self):
+        cookies = self.__getCookies__(
+            self.__session__.cookies, "dachsconnect.senertec.com")
+        self.logger.debug("Creating websocket connection..")
+        self.ws = websocket.WebSocketApp(self.WS_HOST,
+                                         on_message=self.__on_message__,
+                                         on_error=self.__on_error__,
+                                         on_close=self.__on_close__,
+                                         on_open=self.__on_open__,
+                                         cookie=cookies)
+        self.__thread__ = Thread(
+            target=self.ws.run_forever, kwargs={
+                "ping_interval": 60, "ping_timeout": 5}
+        )
+        self.__thread__.daemon = True
+        self.__thread__.setName("senertec-websocket")
+        self.__thread__.start()
+        self.logger.debug("Websocket connection started.")
+
+
+class senertec(basesocketclient):
+    """Class to communicate with Senertec and handle network calls"""
+
+    def __init__(self, datapointList=None, email: str = None, password: str = None, language=lang.English, level=logging.INFO):
+        """Constructor, create instance of senertec client.
+
+        ``datapointList`` Json string to add only these datapoints instead of everything.
+
+        ``language`` Set to your language.
+        """
+        if email is None or password is None:
+            raise ValueError(
+                "Arguments 'email', 'passwords'"
+            )
+        super().__init__(level)
+        logging.basicConfig(
+            level=level,
+            format='py-senertec: %(asctime)s %(levelname)-8s %(message)s',
+            datefmt='%Y-%m-%d %H:%M:%S'
+        )
+        self.AUTHENTICATION_HOST = "https://dachsconnect.senertec.com"
+        self.SSO_HOST = "https://sso-portal.senertec.com"
+        self.email = email
+        self.__session__ = None
+        self.language = language
+        self.password = password
+        self.level = level
+        self.__filteredDatapoints__ = datapointList
+        self.__enums__ = []
+        self.__metaDataPoints__ = []
+        self.__metaDataTranslations__ = []
+        self.__enumTranslations__ = []
+        self.__errorTranslations__ = []
+        self.__connectedUnit__ = []
+        self.__appVersion__ = ""
+        self.messagecallback = (canipValue())
+        """Set your callback function to get the data values. Function has to be overloaded with data type ``canipValue``"""
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(level)
+
+    def __create_headers__(self):
+        headers = {"Content-Type": "application/json"}
+        return headers
+
+    def __getCookies__(self, cookie_jar, domain):
+        cookie_dict = cookie_jar.get_dict(domain=domain)
+        found = ['%s=%s' % (name, value)
+                 for (name, value) in cookie_dict.items()]
+        return ';'.join(found)
+
+    def __post__(self, urlPath: str, payload: str):
+        url = self.AUTHENTICATION_HOST + urlPath
+        response = self.__session__.post(
+            url, data=payload, headers=self.__create_headers__())
+        if (response.status_code >= 400 and response.status_code <= 599):
+            logger.error("Error in post request by function: " + inspect.stack()
+                         [1].function + " HTTP response: " + response.text)
+        return response
+
+    def __get__(self, urlPath: str):
+        url = self.AUTHENTICATION_HOST + urlPath
+        response = self.__session__.get(
+            url, headers=self.__create_headers__())
+        if (response.status_code >= 400 and response.status_code <= 599):
+            logger.error("Error in get request by function: {" + inspect.stack()
+                         [1].function + "} HTTP response: " + response.text)
+        return response
+
+    def __parseDataPoints__(self):
+        """Parse all available datapoints for connected unit."""
+        self.logger.debug("Starting to parse datapoints..")
+        dataPointCount = 0
+        metaData = self.__metaDataPoints__
+        allPoints = []
+        boardList = []
+
+        # first collect all available datapoints
+        for point in metaData:
+            if metaData[point]["friendlyName"] is not None:
+                datap = datapoint()
+                datap.sourceId = metaData[point]["friendlyName"]
+                datap.friendlyName = self.__metaDataTranslations__[
+                    metaData[point]["name"]]
+                datap.id = metaData[point]["name"]
+                datap.gain = metaData[point]["gain"]
+                datap.unit = metaData[point]["unit"]
+                datap.enumName = metaData[point]["enumName"]
+                datap.array = metaData[point]["array"]
+                datap.type = obdClass(metaData[point]["obdClass"])
+                allPoints.append(datap)
+                # loop through all boards of unit
+                for b in self.__connectedUnit__["boards"]:
+                    # add board to the collection if its not already included
+                    if not any(x for x in boardList if x.boardName == b["name"]):
+                        device = board()
+                        device.__boardName__ = b["name"]
+                        boardList.append(device)
+                    # loop through datapoints of that board and add available points
+                    for at in b["attributes"]:
+                        if at == datap.id:
+                            for b1 in boardList:
+                                if b1.boardName == b["name"]:
+                                    dataPointCount += 1
+                                    b1.__datapoints__.append(datap)
+                            break
+        self.logger.debug(
+            f"Finished datapoints parsing. Found {len(boardList)} boards with {dataPointCount} datapoints in total.")
+        self.boards = boardList
+        return
+
+    def __parseDataPointsFiltered__(self):
+        """Use this function to include only datapoints of datapointList which was set in class constructor."""
+        self.logger.debug("Starting to parse datapoints..")
+        metaData = self.__metaDataPoints__
+        blist = []
+        dataPointCount = 0
+        boardname = ""
+        for a in metaData:
+            for element in self.__filteredDatapoints__[self.__connectedUnit__["productGroup"]]:
+                if metaData[a]["friendlyName"] == element:
+                    for l in self.__connectedUnit__["boards"]:
+                        for o in l["attributes"]:
+                            if o == metaData[a]["name"]:
+                                boardname = l["name"]
+                    datap = datapoint()
+                    datap.sourceId = element
+                    datap.id = metaData[a]["name"]
+                    datap.friendlyName = self.__metaDataTranslations__[
+                        metaData[a]["name"]]
+                    datap.unit = metaData[a]["unit"]
+                    datap.gain = metaData[a]["gain"]
+                    datap.enumName = metaData[a]["enumName"]
+                    datap.array = metaData[a]["array"]
+                    datap.type = obdClass(metaData[a]["obdClass"])
+                    dataPointCount += 1
+                    # avoid doubled board entries
+                    if not any(x for x in blist if x.boardName == boardname):
+                        b = board()
+                        b.__boardName__ = boardname
+                        b.__datapoints__.append(datap)
+                        blist.append(b)
+                    else:
+                        for b in blist:
+                            if b.boardName == boardname:
+                                b.__datapoints__.append(datap)
+        self.boards = blist
+        self.logger.debug(
+            f"Finished datapoints parsing. Found {len(blist)} boards with {dataPointCount} datapoints in total.")
+
+    @property
+    def portalVersion(self) -> str:
+        """Returns Senertec Dachsportal version.
+
+        Init function has to be called first.
+        """
+        return self.__appVersion__
+
+    def login(self):
+        """
+        Login.
+
+        This function needs to be called first.
+
+        Returns True on success, False on failure.
+        """
+        self.logger.info("Logging in..")
+        self.__session__ = requests.Session()
+        loginSSOResponse = self.__session__.get(
+            self.AUTHENTICATION_HOST + "/rest/saml2/login")
+
+        authState = loginSSOResponse.url.split("loginuserpass.php?")[1]
+        head = {"Content-Type": "application/x-www-form-urlencoded"}
+        userData = f"username={self.email}&password={self.password}&{authState}"
+        # submit credentials
+        loginResponse = self.__session__.post(self.SSO_HOST + "/simplesaml/module.php/core/loginuserpass.php?",
+                                              data=userData, headers=head)
+
+        # filter out samlresponse and relaystate for ACS request
+        soup = BeautifulSoup(loginResponse.text, features="html.parser")
+        try:
+            samlResponse = soup.findAll(
+                "input", {"name": "SAMLResponse"})[0]["value"]
+            relayState = soup.findAll(
+                "input", {"name": "RelayState"})[0]["value"]
+        except IndexError:
+            self.logger.error("Login failed, username or password wrong.")
+            return False
+        acsData = {'SAMLResponse': {samlResponse}, 'RelayState': {relayState}}
+
+        # do assertion consumer service request with received saml response
+        acs = self.__session__.post(
+            self.AUTHENTICATION_HOST + "/rest/saml2/acs", data=acsData, headers=head)
+
+        if acs.history[0].status_code != 302:
+            self.logger.error("Login failed at ACS request, got no redirect.")
+            return False
+        self.logger.info("Login was successful.")
+        return True
+
+    def logout(self):
+        """
+        Logout from senertec.
+
+        Returns True on success, False on failure.
+        """
+        self.logger.info("Logging out..")
+        response = self.__get__("/logout")
+        if self.ws:
+            self.ws.close()
+        self.__session__.close()
+        if response.status_code == 200:
+            self.logger.debug("Logout was successful.")
+            return True
+        else:
+            return False
+
+    def init(self):
+        """
+        Initialize Senertec platform and connect to websocket.
+
+        This function needs to be called after login.
+
+        Returns True on success, False on failure.
+        """
+        self.logger.info("Initializing senertec platform...")
+        response = self.__get__("/rest/info/init")
+        if response.status_code == 200:
+            self.__create_websocket__()
+            j = json.loads(response.text)
+            self.__metaDataPoints__ = j["metaDataPoints"]
+            self.__enums__ = j["enums"]
+            self.__enumTranslations__ = j["translations"][f"{self.language.value}"]["enums"]
+            self.__metaDataTranslations__ = j["translations"][
+                f"{self.language.value}"]["metaDataPoints"]["translations"]
+            self.__errorTranslations__ = j["translations"][f"{self.language.value}"]["errorCategories"]
+            self.__appVersion__ = j["app"]["version"]
+            return True
+        else:
+            return False
+
+    def getUnits(self) -> list[energyUnit]:
+        """
+        Get all units.
+
+        Returns all energy units of this account as object list.
+        """
+        response = self.__post__(
+            "/rest/info/units", json.dumps({"limit": 10, "offset": 0, "filter": {}}))
+        if response.status_code == 200:
+            values = json.loads(response.text)
+            units = []
+            for x in values["units"]:
+                unit = energyUnit()
+                unit.model = x["benennung"]
+                unit.serial = x["seriennummer"]
+                unit.connected = x["connected"]
+                unit.online = x["online"]
+                unit.itemNumber = x["artikelNummer"]
+                unit.contact = x["standortAnsprech"]
+                unit.city = x["standortOrt"]
+                unit.locationName = x["standortName"]
+                unit.postalCode = x["standortPlz"]
+                unit.street = x["standortAdresse"]
+                unit.productGroup = x["productGroup"]
+                units.append(unit)
+            self.logger.debug(
+                f"Successful received a list of {len(units)} units.")
+            return units
+        else:
+            return None
+
+    def connectUnit(self, serial: str):
+        """
+        This function connects to a unit and enables receiving data for that unit.
+
+        ``serial`` Serial number of energy unit. Can be received with getUnits() method.
+
+        Returns True on success, False on failure.
+        """
+        response = self.__get__(f"/rest/canip/{serial}")
+        if response.status_code == 200:
+            self.__connectedUnit__ = json.loads(response.text)
+            # if no supported items were set in constructor, do not filter and parse every datapoint
+            if self.__filteredDatapoints__ is None:
+                self.__parseDataPoints__()
+            else:
+                self.__parseDataPointsFiltered__()
+            return True
+        else:
+            return False
+
+    def disconnectUnit(self):
+        """
+        Disconnect from a unit.
+
+        Returns True on success, False on failure.
+        """
+        sn = self.__connectedUnit__["seriennummer"]
+        response = self.__get__(f"/rest/canip/{sn}/disconnect")
+        if response.status_code == 200:
+            return True
+        else:
+            return False
+
+    def getChart(self, chartname: str):
+        """
+        Get a history chart of the connected unit.
+        """
+        sn = self.__connectedUnit__["seriennummer"]
+        response = self.__post__(
+            f"/rest/charts/{sn}/data", json.dumps(
+                {"start": 1641596400000, "end": None, "parameters": {}, "chartName": chartname, "sn": sn}))
+        if response.status_code == 200:
+            return json.loads(response.text)
+
+    def request(self, dataPoints: list):
+        """
+        Request data from specific datapoints of the connected unit.
+
+        Data wil be received through websocket.
+
+        ``dataPoints`` List of datapoint strings
+
+        Returns True on success, False on failure.
+        """
+        sn = self.__connectedUnit__["seriennummer"]
+        j = json.dumps(
+            {"seriennummer": sn, "keys": dataPoints})
+        response = self.__post__(
+            f"/rest/canip/{sn}/request", j)
+        result = json.loads(response.text)
+        if response.status_code == 200 and result["success"] and not result["errorKeys"]:
+            return True
+        else:
+            return False
+
+    def getBoardList(self):
+        """Get all boards of the connected unit"""
+        lst = [str()]
+        for b in self.__connectedUnit__["boards"]:
+            lst.append(b["name"])
+        return lst
+
+    def getErrors(self, onlyCurrentErrors: bool = True) -> list[canipError]:
+        """Get an error history of the connected unit.
+
+        ``onlyCurrentErrors`` Return only errors which are present now. Set to false if you want error history.
+
+        This gets loaded when a unit gets connected."""
+        lst = []
+        for b in self.__connectedUnit__["boards"]:
+            for e in b["canipErrors"]:
+                if onlyCurrentErrors and not e["currentError"]:
+                    continue
+                error = canipError()
+                error.__boardName__ = e["boardName"]
+                error.__code__ = e["codeText"]
+                error.__counter__ = e["counter"]
+                error.__currentError__ = e["currentError"]
+                error.__timestamp__ = e["timestamp"]
+                cat = e["errorCode"]["category"]
+                code = e["errorCode"]["code"]
+                error.__errorCategory__ = self.__errorTranslations__[
+                    f"{cat}"]["translationMedium"]
+                error.__errorTranslation__ = self.__errorTranslations__[
+                    f"{cat}"]["translations"][f"{code}"]
+                lst.append(error)
+        return lst
```

### Comparing `py-senertec-0.3.0/src/senertec/energyUnit.py` & `py-senertec-0.4.0/src/senertec/energyUnit.py`

 * *Files identical despite different names*


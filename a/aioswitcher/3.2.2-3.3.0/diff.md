# Comparing `tmp/aioswitcher-3.2.2.tar.gz` & `tmp/aioswitcher-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioswitcher-3.2.2.tar", max compression
+gzip compressed data, was "aioswitcher-3.3.0.tar", max compression
```

## Comparing `aioswitcher-3.2.2.tar` & `aioswitcher-3.3.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-02-04 09:10:01.922601 aioswitcher-3.2.2/LICENSE
--rw-r--r--   0        0        0     9671 2023-02-04 09:10:01.922601 aioswitcher-3.2.2/README.md
--rw-r--r--   0        0        0        0 2023-02-04 09:10:01.926601 aioswitcher-3.2.2/py.typed
--rw-r--r--   0        0        0     3131 2023-02-04 09:10:20.686788 aioswitcher-3.2.2/pyproject.toml
--rwxr-xr-x   0        0        0      818 2023-02-04 09:10:01.926601 aioswitcher-3.2.2/src/aioswitcher/__init__.py
--rw-r--r--   0        0        0    27812 2023-02-04 09:10:01.926601 aioswitcher-3.2.2/src/aioswitcher/api/__init__.py
--rw-r--r--   0        0        0     9461 2023-02-04 09:10:01.926601 aioswitcher-3.2.2/src/aioswitcher/api/messages.py
--rw-r--r--   0        0        0     3924 2023-02-04 09:10:01.926601 aioswitcher-3.2.2/src/aioswitcher/api/packets.py
--rw-r--r--   0        0        0    15903 2023-02-04 09:10:01.926601 aioswitcher-3.2.2/src/aioswitcher/api/remotes.py
--rw-r--r--   0        0        0    15858 2023-02-04 09:10:01.926601 aioswitcher-3.2.2/src/aioswitcher/bridge.py
--rw-r--r--   0        0        0    11461 2023-02-04 09:10:01.926601 aioswitcher-3.2.2/src/aioswitcher/device/__init__.py
--rw-r--r--   0        0        0     4320 2023-02-04 09:10:01.926601 aioswitcher-3.2.2/src/aioswitcher/device/tools.py
--rw-r--r--   0        0        0 12418831 2023-02-04 09:10:01.954601 aioswitcher-3.2.2/src/aioswitcher/resources/irset_db.json
--rw-r--r--   0        0        0     2054 2023-02-04 09:10:01.954601 aioswitcher-3.2.2/src/aioswitcher/schedule/__init__.py
--rw-r--r--   0        0        0     4047 2023-02-04 09:10:01.954601 aioswitcher-3.2.2/src/aioswitcher/schedule/parser.py
--rw-r--r--   0        0        0     5683 2023-02-04 09:10:01.954601 aioswitcher-3.2.2/src/aioswitcher/schedule/tools.py
--rw-r--r--   0        0        0    10605 1970-01-01 00:00:00.000000 aioswitcher-3.2.2/setup.py
--rw-r--r--   0        0        0    10640 1970-01-01 00:00:00.000000 aioswitcher-3.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 18:44:09.095507 aioswitcher-3.3.0/LICENSE
+-rw-r--r--   0        0        0    10703 2023-04-10 18:44:09.095507 aioswitcher-3.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/py.typed
+-rw-r--r--   0        0        0     3198 2023-04-10 18:44:34.064273 aioswitcher-3.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0      818 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/__init__.py
+-rw-r--r--   0        0        0    27808 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/api/__init__.py
+-rw-r--r--   0        0        0     9461 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/api/messages.py
+-rw-r--r--   0        0        0     3924 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/api/packets.py
+-rw-r--r--   0        0        0    15903 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/api/remotes.py
+-rw-r--r--   0        0        0    16048 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/bridge.py
+-rw-r--r--   0        0        0    11461 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/device/__init__.py
+-rw-r--r--   0        0        0     4320 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/device/tools.py
+-rw-r--r--   0        0        0 12418831 2023-04-10 18:44:09.131508 aioswitcher-3.3.0/src/aioswitcher/resources/irset_db.json
+-rw-r--r--   0        0        0     2054 2023-04-10 18:44:09.131508 aioswitcher-3.3.0/src/aioswitcher/schedule/__init__.py
+-rw-r--r--   0        0        0     4047 2023-04-10 18:44:09.131508 aioswitcher-3.3.0/src/aioswitcher/schedule/parser.py
+-rw-r--r--   0        0        0     5683 2023-04-10 18:44:09.131508 aioswitcher-3.3.0/src/aioswitcher/schedule/tools.py
+-rw-r--r--   0        0        0    11672 1970-01-01 00:00:00.000000 aioswitcher-3.3.0/PKG-INFO
```

### Comparing `aioswitcher-3.2.2/LICENSE` & `aioswitcher-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/README.md` & `aioswitcher-3.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,19 @@
-<!-- markdownlint-disable MD033 -->
+# Help Wanted
+
+<p align="left">
+<strong>
+Aioswitcher project is looking for maintainers and contributors!<br/>
+For various reasons, I can only keep maintaining this project as far as dependency bumps and publishing.<br/>
+As for new features and the occasional bug support, these will require other maintainers/contributors.<br/>
+<br/>
+If that's you - please feel free to ping me and I will do all I can to make the onboarding process easy.
+</strong>
+</p>
+
 # Switcher Python Integration</br>[![pypi-version]][11] [![pypi-downloads]][11] [![license-badge]][4]
 
 [![gh-build-status]][7] [![gh-pages-status]][8] [![codecov]][3]
 
 PyPi module integrating with various [Switcher][12] devices.</br>
 Check out the [wiki pages][0] for a list of supported devices.
 
@@ -153,26 +164,27 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center"><a href="https://github.com/aviadgolan"><img src="https://avatars.githubusercontent.com/u/17742111?v=4?s=100" width="100px;" alt="Aviad Golan"/><br /><sub><b>Aviad Golan</b></sub></a><br /><a href="#data-AviadGolan" title="Data">🔣</a></td>
-      <td align="center"><a href="https://github.com/dolby360"><img src="https://avatars.githubusercontent.com/u/22151399?v=4?s=100" width="100px;" alt="Dolev Ben Aharon"/><br /><sub><b>Dolev Ben Aharon</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=dolby360" title="Documentation">📖</a></td>
-      <td align="center"><a href="http://fabian-affolter.ch/blog/"><img src="https://avatars.githubusercontent.com/u/116184?v=4?s=100" width="100px;" alt="Fabian Affolter"/><br /><sub><b>Fabian Affolter</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=fabaff" title="Code">💻</a></td>
-      <td align="center"><a href="https://github.com/oranja"><img src="https://avatars.githubusercontent.com/u/679184?v=4?s=100" width="100px;" alt="Itzik Ephraim"/><br /><sub><b>Itzik Ephraim</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=oranja" title="Code">💻</a></td>
-      <td align="center"><a href="https://github.com/Kesav890"><img src="https://avatars.githubusercontent.com/u/82559951?v=4?s=100" width="100px;" alt="Kesav890"/><br /><sub><b>Kesav890</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=Kesav890" title="Documentation">📖</a></td>
-      <td align="center"><a href="https://github.com/OrBin"><img src="https://avatars.githubusercontent.com/u/6897234?v=4?s=100" width="100px;" alt="Or Bin"/><br /><sub><b>Or Bin</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=OrBin" title="Code">💻</a></td>
-      <td align="center"><a href="http://exploit.co.il"><img src="https://avatars.githubusercontent.com/u/1768915?v=4?s=100" width="100px;" alt="Shai rod"/><br /><sub><b>Shai rod</b></sub></a><br /><a href="#data-nightrang3r" title="Data">🔣</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/aviadgolan"><img src="https://avatars.githubusercontent.com/u/17742111?v=4?s=100" width="100px;" alt="Aviad Golan"/><br /><sub><b>Aviad Golan</b></sub></a><br /><a href="#data-AviadGolan" title="Data">🔣</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dolby360"><img src="https://avatars.githubusercontent.com/u/22151399?v=4?s=100" width="100px;" alt="Dolev Ben Aharon"/><br /><sub><b>Dolev Ben Aharon</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=dolby360" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://fabian-affolter.ch/blog/"><img src="https://avatars.githubusercontent.com/u/116184?v=4?s=100" width="100px;" alt="Fabian Affolter"/><br /><sub><b>Fabian Affolter</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=fabaff" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/oranja"><img src="https://avatars.githubusercontent.com/u/679184?v=4?s=100" width="100px;" alt="Itzik Ephraim"/><br /><sub><b>Itzik Ephraim</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=oranja" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Kesav890"><img src="https://avatars.githubusercontent.com/u/82559951?v=4?s=100" width="100px;" alt="Kesav890"/><br /><sub><b>Kesav890</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=Kesav890" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://liad.avrah.am"><img src="https://avatars.githubusercontent.com/u/7263223?v=4?s=100" width="100px;" alt="Liad Avraham"/><br /><sub><b>Liad Avraham</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=liadav" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/OrBin"><img src="https://avatars.githubusercontent.com/u/6897234?v=4?s=100" width="100px;" alt="Or Bin"/><br /><sub><b>Or Bin</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=OrBin" title="Code">💻</a></td>
     </tr>
     <tr>
-      <td align="center"><a href="https://github.com/thecode"><img src="https://avatars.githubusercontent.com/u/1858925?v=4?s=100" width="100px;" alt="Shay Levy"/><br /><sub><b>Shay Levy</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=thecode" title="Code">💻</a> <a href="#ideas-thecode" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-thecode" title="Maintenance">🚧</a></td>
-      <td align="center"><a href="https://github.com/dmatik"><img src="https://avatars.githubusercontent.com/u/5577386?v=4?s=100" width="100px;" alt="dmatik"/><br /><sub><b>dmatik</b></sub></a><br /><a href="#blog-dmatik" title="Blogposts">📝</a> <a href="#ideas-dmatik" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-dmatik" title="User Testing">📓</a></td>
-      <td align="center"><a href="https://github.com/jafar-atili"><img src="https://avatars.githubusercontent.com/u/19508787?v=4?s=100" width="100px;" alt="jafar-atili"/><br /><sub><b>jafar-atili</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Code">💻</a> <a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://exploit.co.il"><img src="https://avatars.githubusercontent.com/u/1768915?v=4?s=100" width="100px;" alt="Shai rod"/><br /><sub><b>Shai rod</b></sub></a><br /><a href="#data-nightrang3r" title="Data">🔣</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/thecode"><img src="https://avatars.githubusercontent.com/u/1858925?v=4?s=100" width="100px;" alt="Shay Levy"/><br /><sub><b>Shay Levy</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=thecode" title="Code">💻</a> <a href="#ideas-thecode" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-thecode" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dmatik"><img src="https://avatars.githubusercontent.com/u/5577386?v=4?s=100" width="100px;" alt="dmatik"/><br /><sub><b>dmatik</b></sub></a><br /><a href="#blog-dmatik" title="Blogposts">📝</a> <a href="#ideas-dmatik" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-dmatik" title="User Testing">📓</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jafar-atili"><img src="https://avatars.githubusercontent.com/u/19508787?v=4?s=100" width="100px;" alt="jafar-atili"/><br /><sub><b>jafar-atili</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Code">💻</a> <a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `aioswitcher-3.2.2/pyproject.toml` & `aioswitcher-3.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioswitcher"
-version = "3.2.2"
+version = "3.3.0"
 description = "Switcher Python Integration."
 license = "Apache-2.0"
 authors = [ "Tomer Figenblat <tomer@tomfi.info>" ]
 maintainers = [ "Shay Levy" ]
 readme = "README.md"
 homepage = "https://pypi.org/project/aioswitcher/"
 repository = "https://github.com/tomerfi/aioswitcher"
@@ -21,38 +21,38 @@
 exclude = [ ]
 
   [tool.poetry.dependencies]
   python = "^3.9.0"
 
 [tool.poetry.group.dev.dependencies]
 assertpy = "^1.1"
-black = "^22.8"
+black = ">=22.8,<24.0"
 codecov = "^2.1.12"
-flake8 = "^5.0.4"
+flake8 = ">=5.0.4,<7.0.0"
 flake8-docstrings = "^1.6.0"
 Flake8-pyproject = "^1.1.0.post0"
 isort = "^5.10.1"
-mypy = "^0.971"
-poethepoet = "^0.16.1"
+mypy = ">=0.971,<1.3"
+poethepoet = ">=0.16.1,<0.20.0"
 pytest = "^7.1.2"
-pytest-asyncio = "^0.19.0"
-pytest-cov = "^3.0.0"
+pytest-asyncio = ">=0.19,<0.22"
+pytest-cov = ">=3,<5"
 pytest-resource-path = "^1.3.0"
 pytest-mockservers = "^0.6.0"
 pytest-sugar = "^0.9.4"
 time-machine = "^2.7.0"
 yamllint = "^1.26.3"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.3.0"
 mkdocs-git-revision-date-plugin = "^0.3.2"
-mkdocs-material = "^8.3.8"
-mkdocstrings = "^0.19.0"
-mkdocstrings-python = "^0.7.1"
-poethepoet = "^0.16.1"
+mkdocs-material = ">=8.3.8,<10.0.0"
+mkdocstrings = ">=0.19,<0.22"
+mkdocstrings-python = ">=0.7.1,<0.10.0"
+poethepoet = ">=0.16.1,<0.20.0"
 
 [tool.poe.tasks]
 install = "poetry install --no-interaction"
 test = "poetry run pytest -v"
 test_cov = "poetry run pytest -v --cov --cov-report=term"
 test_rep = "poetry run pytest -v --cov --cov-report=xml:coverage.xml --junit-xml junit.xml"
 test_pub = "poetry publish --build --repository testpypi"
```

### Comparing `aioswitcher-3.2.2/src/aioswitcher/__init__.py` & `aioswitcher-3.3.0/src/aioswitcher/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/src/aioswitcher/api/__init__.py` & `aioswitcher-3.3.0/src/aioswitcher/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -617,15 +617,14 @@
                     mode.value,
                     target_temp,
                     fan_level.value,
                     set_swing.value,
                 )
                 logger.debug("sending a set status packet")
             else:
-
                 command = remote.build_command(
                     state, mode, target_temp, fan_level, set_swing, current_state.state
                 )
 
                 packet = packets.BREEZE_COMMAND_PACKET.format(
                     login_resp.session_id,
                     timestamp,
@@ -763,15 +762,14 @@
 
         Returns:
             An instance of ``SwitcherShutterStateResponse``.
 
         """
         timestamp, login_resp = await self._login(DeviceType.RUNNER)
         if login_resp.successful:
-
             packet = packets.GET_STATE_PACKET2_TYPE2.format(
                 login_resp.session_id, timestamp, self._device_id
             )
 
             signed_packet = sign_packet_with_crc_key(packet)
 
             logger.debug("sending a get state packet")
```

### Comparing `aioswitcher-3.2.2/src/aioswitcher/api/messages.py` & `aioswitcher-3.3.0/src/aioswitcher/api/messages.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/src/aioswitcher/api/packets.py` & `aioswitcher-3.3.0/src/aioswitcher/api/packets.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/src/aioswitcher/api/remotes.py` & `aioswitcher-3.3.0/src/aioswitcher/api/remotes.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/src/aioswitcher/bridge.py` & `aioswitcher-3.3.0/src/aioswitcher/bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 __all__ = ["SwitcherBridge"]
 logger = getLogger(__name__)
 
 
 # Protocol type 1 devices: V2, Touch, V4, Mini, Power Plug
 SWITCHER_UDP_PORT_TYPE1 = 20002
+SWITCHER_UDP_PORT_TYPE1_NEW_VERSION = 10002
 # Protocol type 2 devices: Breeze, Runner, Runner Mini
 SWITCHER_UDP_PORT_TYPE2 = 20003
 
 SWITCHER_DEVICE_TO_UDP_PORT = {
     DeviceCategory.WATER_HEATER: SWITCHER_UDP_PORT_TYPE1,
     DeviceCategory.POWER_PLUG: SWITCHER_UDP_PORT_TYPE1,
     DeviceCategory.THERMOSTAT: SWITCHER_UDP_PORT_TYPE2,
@@ -162,22 +163,27 @@
 @final
 class SwitcherBridge:
     """Use for running a UDP client for bridging Switcher devices broadcast messages.
 
     Args:
         on_device: a callable to which every new SwitcherBase device found will be send.
         broadcast_ports: broadcast ports list, default for type 1 devices is 20002,
-            default for type 2 devices is 20003
+            default for type 2 devices is 20003.
+            On newer type1 devices, the port is 10002.
 
     """
 
     def __init__(
         self,
         on_device: Callable[[SwitcherBase], Any],
-        broadcast_ports: List[int] = [SWITCHER_UDP_PORT_TYPE1, SWITCHER_UDP_PORT_TYPE2],
+        broadcast_ports: List[int] = [
+            SWITCHER_UDP_PORT_TYPE1,
+            SWITCHER_UDP_PORT_TYPE1_NEW_VERSION,
+            SWITCHER_UDP_PORT_TYPE2,
+        ],
     ) -> None:
         """Initialize the switcher bridge."""
         self._on_device = on_device
         self._broadcast_ports = broadcast_ports
         self._is_running = False
         self._transports: Dict[int, Optional[BaseTransport]] = {}
```

### Comparing `aioswitcher-3.2.2/src/aioswitcher/device/__init__.py` & `aioswitcher-3.3.0/src/aioswitcher/device/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/src/aioswitcher/device/tools.py` & `aioswitcher-3.3.0/src/aioswitcher/device/tools.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/src/aioswitcher/resources/irset_db.json` & `aioswitcher-3.3.0/src/aioswitcher/resources/irset_db.json`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/src/aioswitcher/schedule/__init__.py` & `aioswitcher-3.3.0/src/aioswitcher/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/src/aioswitcher/schedule/parser.py` & `aioswitcher-3.3.0/src/aioswitcher/schedule/parser.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/src/aioswitcher/schedule/tools.py` & `aioswitcher-3.3.0/src/aioswitcher/schedule/tools.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.2.2/setup.py` & `aioswitcher-3.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,663 +1,730 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 655f 6469  etup..package_di
-00000040: 7220 3d20 5c0a 7b27 273a 2027 7372 6327  r = \.{'': 'src'
-00000050: 7d0a 0a70 6163 6b61 6765 7320 3d20 5c0a  }..packages = \.
-00000060: 5b27 6169 6f73 7769 7463 6865 7227 2c20  ['aioswitcher', 
-00000070: 2761 696f 7377 6974 6368 6572 2e61 7069  'aioswitcher.api
-00000080: 272c 2027 6169 6f73 7769 7463 6865 722e  ', 'aioswitcher.
-00000090: 6465 7669 6365 272c 2027 6169 6f73 7769  device', 'aioswi
-000000a0: 7463 6865 722e 7363 6865 6475 6c65 275d  tcher.schedule']
-000000b0: 0a0a 7061 636b 6167 655f 6461 7461 203d  ..package_data =
-000000c0: 205c 0a7b 2727 3a20 5b27 2a27 5d2c 2027   \.{'': ['*'], '
-000000d0: 6169 6f73 7769 7463 6865 7227 3a20 5b27  aioswitcher': ['
-000000e0: 7265 736f 7572 6365 732f 2a27 5d7d 0a0a  resources/*']}..
-000000f0: 7365 7475 705f 6b77 6172 6773 203d 207b  setup_kwargs = {
-00000100: 0a20 2020 2027 6e61 6d65 273a 2027 6169  .    'name': 'ai
-00000110: 6f73 7769 7463 6865 7227 2c0a 2020 2020  oswitcher',.    
-00000120: 2776 6572 7369 6f6e 273a 2027 332e 322e  'version': '3.2.
-00000130: 3227 2c0a 2020 2020 2764 6573 6372 6970  2',.    'descrip
-00000140: 7469 6f6e 273a 2027 5377 6974 6368 6572  tion': 'Switcher
-00000150: 2050 7974 686f 6e20 496e 7465 6772 6174   Python Integrat
-00000160: 696f 6e2e 272c 0a20 2020 2027 6c6f 6e67  ion.',.    'long
-00000170: 5f64 6573 6372 6970 7469 6f6e 273a 2027  _description': '
-00000180: 3c21 2d2d 206d 6172 6b64 6f77 6e6c 696e  <!-- markdownlin
-00000190: 742d 6469 7361 626c 6520 4d44 3033 3320  t-disable MD033 
-000001a0: 2d2d 3e5c 6e23 2053 7769 7463 6865 7220  -->\n# Switcher 
-000001b0: 5079 7468 6f6e 2049 6e74 6567 7261 7469  Python Integrati
-000001c0: 6f6e 3c2f 6272 3e5b 215b 7079 7069 2d76  on</br>[![pypi-v
-000001d0: 6572 7369 6f6e 5d5d 5b31 315d 205b 215b  ersion]][11] [![
-000001e0: 7079 7069 2d64 6f77 6e6c 6f61 6473 5d5d  pypi-downloads]]
-000001f0: 5b31 315d 205b 215b 6c69 6365 6e73 652d  [11] [![license-
-00000200: 6261 6467 655d 5d5b 345d 5c6e 5c6e 5b21  badge]][4]\n\n[!
-00000210: 5b67 682d 6275 696c 642d 7374 6174 7573  [gh-build-status
-00000220: 5d5d 5b37 5d20 5b21 5b67 682d 7061 6765  ]][7] [![gh-page
-00000230: 732d 7374 6174 7573 5d5d 5b38 5d20 5b21  s-status]][8] [!
-00000240: 5b63 6f64 6563 6f76 5d5d 5b33 5d5c 6e5c  [codecov]][3]\n\
-00000250: 6e50 7950 6920 6d6f 6475 6c65 2069 6e74  nPyPi module int
-00000260: 6567 7261 7469 6e67 2077 6974 6820 7661  egrating with va
-00000270: 7269 6f75 7320 5b53 7769 7463 6865 725d  rious [Switcher]
-00000280: 5b31 325d 2064 6576 6963 6573 2e3c 2f62  [12] devices.</b
-00000290: 723e 5c6e 4368 6563 6b20 6f75 7420 7468  r>\nCheck out th
-000002a0: 6520 5b77 696b 6920 7061 6765 735d 5b30  e [wiki pages][0
-000002b0: 5d20 666f 7220 6120 6c69 7374 206f 6620  ] for a list of 
-000002c0: 7375 7070 6f72 7465 6420 6465 7669 6365  supported device
-000002d0: 732e 5c6e 5c6e 6060 6073 6865 6c6c 5c6e  s.\n\n```shell\n
-000002e0: 7069 7020 696e 7374 616c 6c20 6169 6f73  pip install aios
-000002f0: 7769 7463 6865 725c 6e60 6060 5c6e 5c6e  witcher\n```\n\n
-00000300: 3c74 6162 6c65 3e5c 6e20 203c 7464 3e3c  <table>\n  <td><
-00000310: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000320: 6169 6f73 7769 7463 6865 722e 746f 6d66  aioswitcher.tomf
-00000330: 692e 696e 666f 2f22 3e44 6f63 756d 656e  i.info/">Documen
-00000340: 7461 7469 6f6e 3c2f 613e 3c2f 7464 3e5c  tation</a></td>\
-00000350: 6e20 203c 7464 3e3c 6120 6872 6566 3d22  n  <td><a href="
-00000360: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000370: 6f6d 2f54 6f6d 6572 4669 2f61 696f 7377  om/TomerFi/aiosw
-00000380: 6974 6368 6572 2f77 696b 6922 3e57 696b  itcher/wiki">Wik
-00000390: 693c 2f61 3e3c 2f74 643e 5c6e 2020 3c74  i</a></td>\n  <t
-000003a0: 643e 3c61 2068 7265 663d 2268 7474 7073  d><a href="https
-000003b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
-000003c0: 6d65 7246 692f 6169 6f73 7769 7463 6865  merFi/aioswitche
-000003d0: 722f 626c 6f62 2f64 6576 2f43 4f4e 5452  r/blob/dev/CONTR
-000003e0: 4942 5554 494e 472e 6d64 223e 436f 6e74  IBUTING.md">Cont
-000003f0: 7269 6275 7469 6e67 3c2f 613e 3c2f 7464  ributing</a></td
-00000400: 3e5c 6e3c 2f74 6162 6c65 3e5c 6e5c 6e23  >\n</table>\n\n#
-00000410: 2320 4578 616d 706c 6520 5573 6167 655c  # Example Usage\
-00000420: 6e5c 6e3c 6465 7461 696c 733e 5c6e 2020  n\n<details>\n  
-00000430: 3c73 756d 6d61 7279 3e53 7461 7465 2042  <summary>State B
-00000440: 7269 6467 653c 2f73 756d 6d61 7279 3e5c  ridge</summary>\
-00000450: 6e5c 6e60 6060 7079 7468 6f6e 5c6e 6173  n\n```python\nas
-00000460: 796e 6320 6465 6620 7072 696e 745f 6465  ync def print_de
-00000470: 7669 6365 7328 6465 6c61 7929 3a5c 6e20  vices(delay):\n 
-00000480: 2020 2064 6566 206f 6e5f 6465 7669 6365     def on_device
-00000490: 5f66 6f75 6e64 5f63 616c 6c62 6163 6b28  _found_callback(
-000004a0: 6465 7669 6365 293a 5c6e 2020 2020 2020  device):\n      
-000004b0: 2020 2320 6120 7377 6974 6368 6572 2064    # a switcher d
-000004c0: 6576 6963 6520 7769 6c6c 2062 726f 6164  evice will broad
-000004d0: 6361 7374 2061 2073 7461 7465 206d 6573  cast a state mes
-000004e0: 7361 6765 2061 7070 726f 7869 6d61 7465  sage approximate
-000004f0: 6c79 2065 7665 7279 2034 2073 6563 6f6e  ly every 4 secon
-00000500: 6473 5c6e 2020 2020 2020 2020 7072 696e  ds\n        prin
-00000510: 7428 6173 6469 6374 2864 6576 6963 6529  t(asdict(device)
-00000520: 295c 6e5c 6e20 2020 2061 7379 6e63 2077  )\n\n    async w
-00000530: 6974 6820 5377 6974 6368 6572 4272 6964  ith SwitcherBrid
-00000540: 6765 286f 6e5f 6465 7669 6365 5f66 6f75  ge(on_device_fou
-00000550: 6e64 5f63 616c 6c62 6163 6b29 3a5c 6e20  nd_callback):\n 
-00000560: 2020 2020 2020 2061 7761 6974 2061 7379         await asy
-00000570: 6e63 696f 2e73 6c65 6570 2864 656c 6179  ncio.sleep(delay
-00000580: 295c 6e5c 6e23 2072 756e 2074 6865 2062  )\n\n# run the b
-00000590: 7269 6467 6520 666f 7220 3630 2073 6563  ridge for 60 sec
-000005a0: 6f6e 6473 5c6e 6173 796e 6369 6f2e 7275  onds\nasyncio.ru
-000005b0: 6e28 7072 696e 745f 6465 7669 6365 7328  n(print_devices(
-000005c0: 3630 2929 5c6e 6060 605c 6e5c 6e3c 2f64  60))\n```\n\n</d
-000005d0: 6574 6169 6c73 3e5c 6e5c 6e3c 6465 7461  etails>\n\n<deta
-000005e0: 696c 733e 5c6e 2020 3c73 756d 6d61 7279  ils>\n  <summary
-000005f0: 3e50 6f77 6572 2050 6c75 6720 4150 493c  >Power Plug API<
-00000600: 2f73 756d 6d61 7279 3e5c 6e5c 6e20 2060  /summary>\n\n  `
-00000610: 6060 7079 7468 6f6e 5c6e 2020 6173 796e  ``python\n  asyn
-00000620: 6320 6465 6620 636f 6e74 726f 6c5f 706f  c def control_po
-00000630: 7765 725f 706c 7567 2864 6576 6963 655f  wer_plug(device_
-00000640: 6970 2c20 6465 7669 6365 5f69 6429 203a  ip, device_id) :
-00000650: 5c6e 2020 2020 2020 2320 666f 7220 636f  \n      # for co
-00000660: 6e6e 6563 7469 6e67 2074 6f20 6120 6465  nnecting to a de
-00000670: 7669 6365 2077 6520 6e65 6564 2069 7473  vice we need its
-00000680: 2069 6420 616e 6420 6970 2061 6464 7265   id and ip addre
-00000690: 7373 5c6e 2020 2020 2020 6173 796e 6320  ss\n      async 
-000006a0: 7769 7468 2053 7769 7463 6865 7254 7970  with SwitcherTyp
-000006b0: 6531 4170 6928 6465 7669 6365 5f69 702c  e1Api(device_ip,
-000006c0: 2064 6576 6963 655f 6964 2920 6173 2061   device_id) as a
-000006d0: 7069 3a5c 6e20 2020 2020 2020 2020 2023  pi:\n          #
-000006e0: 2067 6574 2074 6865 2064 6576 6963 6520   get the device 
-000006f0: 6375 7272 656e 7420 7374 6174 655c 6e20  current state\n 
-00000700: 2020 2020 2020 2020 2061 7761 6974 2061           await a
-00000710: 7069 2e67 6574 5f73 7461 7465 2829 5c6e  pi.get_state()\n
-00000720: 2020 2020 2020 2020 2020 2320 7475 726e            # turn
-00000730: 2074 6865 2064 6576 6963 6520 6f6e 5c6e   the device on\n
-00000740: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00000750: 6170 692e 636f 6e74 726f 6c5f 6465 7669  api.control_devi
-00000760: 6365 2843 6f6d 6d61 6e64 2e4f 4e29 5c6e  ce(Command.ON)\n
-00000770: 2020 2020 2020 2020 2020 2320 7475 726e            # turn
-00000780: 2074 6865 2064 6576 6963 6520 6f66 665c   the device off\
-00000790: 6e20 2020 2020 2020 2020 2061 7761 6974  n          await
-000007a0: 2061 7069 2e63 6f6e 7472 6f6c 5f64 6576   api.control_dev
-000007b0: 6963 6528 436f 6d6d 616e 642e 4f46 4629  ice(Command.OFF)
-000007c0: 5c6e 2020 2020 2020 2020 2020 2320 7365  \n          # se
-000007d0: 7420 7468 6520 6465 7669 6365 206e 616d  t the device nam
-000007e0: 6520 746f 205c 276d 7920 6e65 7720 6e61  e to \'my new na
-000007f0: 6d65 5c27 5c6e 2020 2020 2020 2020 2020  me\'\n          
-00000800: 6177 6169 7420 6170 692e 7365 745f 6465  await api.set_de
-00000810: 7669 6365 5f6e 616d 6528 226d 7920 6e65  vice_name("my ne
-00000820: 7720 6e61 6d65 2229 5c6e 5c6e 2020 6173  w name")\n\n  as
-00000830: 796e 6369 6f2e 7275 6e28 636f 6e74 726f  yncio.run(contro
-00000840: 6c5f 706f 7765 725f 706c 7567 2822 3131  l_power_plug("11
-00000850: 312e 3232 322e 3131 2e32 3222 2c20 2261  1.222.11.22", "a
-00000860: 6231 6332 6422 2929 5c6e 2020 6060 605c  b1c2d"))\n  ```\
-00000870: 6e5c 6e3c 2f64 6574 6169 6c73 3e5c 6e5c  n\n</details>\n\
-00000880: 6e3c 6465 7461 696c 733e 5c6e 2020 3c73  n<details>\n  <s
-00000890: 756d 6d61 7279 3e57 6174 6572 2048 6561  ummary>Water Hea
-000008a0: 7465 7220 4150 493c 2f73 756d 6d61 7279  ter API</summary
-000008b0: 3e5c 6e5c 6e20 2060 6060 7079 7468 6f6e  >\n\n  ```python
-000008c0: 5c6e 2020 6173 796e 6320 6465 6620 636f  \n  async def co
-000008d0: 6e74 726f 6c5f 7761 7465 725f 6865 6174  ntrol_water_heat
-000008e0: 6572 2864 6576 6963 655f 6970 2c20 6465  er(device_ip, de
-000008f0: 7669 6365 5f69 6429 203a 5c6e 2020 2020  vice_id) :\n    
-00000900: 2020 2320 666f 7220 636f 6e6e 6563 7469    # for connecti
-00000910: 6e67 2074 6f20 6120 6465 7669 6365 2077  ng to a device w
-00000920: 6520 6e65 6564 2069 7473 2069 6420 616e  e need its id an
-00000930: 6420 6970 2061 6464 7265 7373 5c6e 2020  d ip address\n  
-00000940: 2020 2020 6173 796e 6320 7769 7468 2053      async with S
-00000950: 7769 7463 6865 7254 7970 6531 4170 6928  witcherType1Api(
-00000960: 6465 7669 6365 5f69 702c 2064 6576 6963  device_ip, devic
-00000970: 655f 6964 2920 6173 2061 7069 3a5c 6e20  e_id) as api:\n 
-00000980: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
-00000990: 6865 2064 6576 6963 6520 6375 7272 656e  he device curren
-000009a0: 7420 7374 6174 655c 6e20 2020 2020 2020  t state\n       
-000009b0: 2020 2061 7761 6974 2061 7069 2e67 6574     await api.get
-000009c0: 5f73 7461 7465 2829 5c6e 2020 2020 2020  _state()\n      
-000009d0: 2020 2020 2320 7475 726e 2074 6865 2064      # turn the d
-000009e0: 6576 6963 6520 6f6e 2066 6f72 2031 3520  evice on for 15 
-000009f0: 6d69 6e75 7465 735c 6e20 2020 2020 2020  minutes\n       
-00000a00: 2020 2061 7761 6974 2061 7069 2e63 6f6e     await api.con
-00000a10: 7472 6f6c 5f64 6576 6963 6528 436f 6d6d  trol_device(Comm
-00000a20: 616e 642e 4f4e 2c20 3135 295c 6e20 2020  and.ON, 15)\n   
-00000a30: 2020 2020 2020 2023 2074 7572 6e20 7468         # turn th
-00000a40: 6520 6465 7669 6365 206f 6666 5c6e 2020  e device off\n  
-00000a50: 2020 2020 2020 2020 6177 6169 7420 6170          await ap
-00000a60: 692e 636f 6e74 726f 6c5f 6465 7669 6365  i.control_device
-00000a70: 2843 6f6d 6d61 6e64 2e4f 4646 295c 6e20  (Command.OFF)\n 
-00000a80: 2020 2020 2020 2020 2023 2073 6574 2074           # set t
-00000a90: 6865 2064 6576 6963 6520 6e61 6d65 2074  he device name t
-00000aa0: 6f20 5c27 6d79 206e 6577 206e 616d 655c  o \'my new name\
-00000ab0: 275c 6e20 2020 2020 2020 2020 2061 7761  '\n          awa
-00000ac0: 6974 2061 7069 2e73 6574 5f64 6576 6963  it api.set_devic
-00000ad0: 655f 6e61 6d65 2822 6d79 206e 6577 206e  e_name("my new n
-00000ae0: 616d 6522 295c 6e20 2020 2020 2020 2020  ame")\n         
-00000af0: 2023 2063 6f6e 6669 6775 7265 2074 6865   # configure the
-00000b00: 2064 6576 6963 6520 666f 7220 3032 3a33   device for 02:3
-00000b10: 3020 6175 746f 2073 6875 7464 6f77 6e5c  0 auto shutdown\
-00000b20: 6e20 2020 2020 2020 2020 2061 7761 6974  n          await
-00000b30: 2061 7069 2e73 6574 5f61 7574 6f5f 7368   api.set_auto_sh
-00000b40: 7574 646f 776e 2874 696d 6564 656c 7461  utdown(timedelta
-00000b50: 2868 6f75 7273 3d32 2c20 6d69 6e75 7465  (hours=2, minute
-00000b60: 733d 3330 2929 5c6e 2020 2020 2020 2020  s=30))\n        
-00000b70: 2020 2320 6765 7420 7468 6520 7363 6865    # get the sche
-00000b80: 6475 6c65 7320 6672 6f6d 2074 6865 2064  dules from the d
-00000b90: 6576 6963 655c 6e20 2020 2020 2020 2020  evice\n         
-00000ba0: 2061 7761 6974 2061 7069 2e67 6574 5f73   await api.get_s
-00000bb0: 6368 6564 756c 6573 2829 5c6e 2020 2020  chedules()\n    
-00000bc0: 2020 2020 2020 2320 6465 6c65 7465 2061        # delete a
-00000bd0: 6e64 2065 7869 7374 696e 6720 7363 6865  nd existing sche
-00000be0: 6475 6c65 2077 6974 6820 6964 2031 5c6e  dule with id 1\n
-00000bf0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00000c00: 6170 692e 6465 6c65 7465 5f73 6368 6564  api.delete_sched
-00000c10: 756c 6528 2231 2229 5c6e 2020 2020 2020  ule("1")\n      
-00000c20: 2020 2020 2320 6372 6561 7465 2061 206e      # create a n
-00000c30: 6577 2072 6563 7572 7269 6e67 2073 6368  ew recurring sch
-00000c40: 6564 756c 6520 666f 7220 3133 3a30 302d  edule for 13:00-
-00000c50: 3134 3a33 305c 6e20 2020 2020 2020 2020  14:30\n         
-00000c60: 2023 2065 7865 6375 7469 6e67 206f 6e20   # executing on 
-00000c70: 7375 6e64 6179 2061 6e64 2066 7269 6461  sunday and frida
-00000c80: 795c 6e20 2020 2020 2020 2020 2061 7761  y\n          awa
-00000c90: 6974 2061 7069 2e63 7265 6174 655f 7363  it api.create_sc
-00000ca0: 6865 6475 6c65 2822 3133 3a30 3022 2c20  hedule("13:00", 
-00000cb0: 2231 343a 3330 222c 207b 4461 7973 2e53  "14:30", {Days.S
-00000cc0: 554e 4441 592c 2044 6179 732e 4652 4944  UNDAY, Days.FRID
-00000cd0: 4159 7d29 5c6e 5c6e 2020 6173 796e 6369  AY})\n\n  asynci
-00000ce0: 6f2e 7275 6e28 636f 6e74 726f 6c5f 7761  o.run(control_wa
-00000cf0: 7465 725f 6865 6174 6572 2822 3131 312e  ter_heater("111.
-00000d00: 3232 322e 3131 2e32 3222 2c20 2261 6231  222.11.22", "ab1
-00000d10: 6332 6422 2929 5c6e 2020 6060 605c 6e5c  c2d"))\n  ```\n\
-00000d20: 6e3c 2f64 6574 6169 6c73 3e5c 6e5c 6e3c  n</details>\n\n<
-00000d30: 6465 7461 696c 733e 5c6e 2020 3c73 756d  details>\n  <sum
-00000d40: 6d61 7279 3e52 756e 6e65 7220 4150 493c  mary>Runner API<
-00000d50: 2f73 756d 6d61 7279 3e5c 6e5c 6e20 2060  /summary>\n\n  `
-00000d60: 6060 7079 7468 6f6e 5c6e 2020 6173 796e  ``python\n  asyn
-00000d70: 6320 6465 6620 636f 6e74 726f 6c5f 7275  c def control_ru
-00000d80: 6e6e 6572 2864 6576 6963 655f 6970 2c20  nner(device_ip, 
-00000d90: 6465 7669 6365 5f69 6429 203a 5c6e 2020  device_id) :\n  
-00000da0: 2020 2020 2320 666f 7220 636f 6e6e 6563      # for connec
-00000db0: 7469 6e67 2074 6f20 6120 6465 7669 6365  ting to a device
-00000dc0: 2077 6520 6e65 6564 2069 7473 2069 6420   we need its id 
-00000dd0: 616e 6420 6970 2061 6464 7265 7373 5c6e  and ip address\n
-00000de0: 2020 2020 2020 6173 796e 6320 7769 7468        async with
-00000df0: 2053 7769 7463 6865 7254 7970 6532 4170   SwitcherType2Ap
-00000e00: 6928 6465 7669 6365 5f69 702c 2064 6576  i(device_ip, dev
-00000e10: 6963 655f 6964 2920 6173 2061 7069 3a5c  ice_id) as api:\
-00000e20: 6e20 2020 2020 2020 2020 2023 2067 6574  n          # get
-00000e30: 2074 6865 2064 6576 6963 6520 6375 7272   the device curr
-00000e40: 656e 7420 7374 6174 655c 6e20 2020 2020  ent state\n     
-00000e50: 2020 2020 2061 7761 6974 2061 7069 2e67       await api.g
-00000e60: 6574 5f73 6875 7474 6572 5f73 7461 7465  et_shutter_state
-00000e70: 2829 5c6e 2020 2020 2020 2020 2020 2320  ()\n          # 
-00000e80: 6f70 656e 2074 6865 2073 6875 7474 6572  open the shutter
-00000e90: 2074 6f20 3330 255c 6e20 2020 2020 2020   to 30%\n       
-00000ea0: 2020 2061 7761 6974 2061 7069 2e73 6574     await api.set
-00000eb0: 5f70 6f73 6974 696f 6e28 3330 295c 6e20  _position(30)\n 
-00000ec0: 2020 2020 2020 2020 2023 2073 746f 7020           # stop 
-00000ed0: 7468 6520 7368 7574 7465 7220 6966 2063  the shutter if c
-00000ee0: 7572 7265 6e74 6c79 2072 6f6c 6c69 6e67  urrently rolling
-00000ef0: 5c6e 2020 2020 2020 2020 2020 6177 6169  \n          awai
-00000f00: 7420 6170 692e 7374 6f70 2829 5c6e 5c6e  t api.stop()\n\n
-00000f10: 2020 6173 796e 6369 6f2e 7275 6e28 636f    asyncio.run(co
-00000f20: 6e74 726f 6c5f 7275 6e6e 6572 2822 3131  ntrol_runner("11
-00000f30: 312e 3232 322e 3131 2e32 3222 2c20 2261  1.222.11.22", "a
-00000f40: 6231 6332 6422 2929 5c6e 2020 6060 605c  b1c2d"))\n  ```\
-00000f50: 6e5c 6e3c 2f64 6574 6169 6c73 3e5c 6e5c  n\n</details>\n\
-00000f60: 6e3c 6465 7461 696c 733e 5c6e 2020 3c73  n<details>\n  <s
-00000f70: 756d 6d61 7279 3e42 7265 657a 6520 4150  ummary>Breeze AP
-00000f80: 493c 2f73 756d 6d61 7279 3e5c 6e5c 6e20  I</summary>\n\n 
-00000f90: 2060 6060 7079 7468 6f6e 5c6e 2020 6173   ```python\n  as
-00000fa0: 796e 6320 6465 6620 636f 6e74 726f 6c5f  ync def control_
-00000fb0: 6272 6565 7a65 2864 6576 6963 655f 6970  breeze(device_ip
-00000fc0: 2c20 6465 7669 6365 5f69 642c 2072 656d  , device_id, rem
-00000fd0: 6f74 655f 6d61 6e61 6765 722c 2072 656d  ote_manager, rem
-00000fe0: 6f74 655f 6964 2920 3a5c 6e20 2020 2020  ote_id) :\n     
-00000ff0: 2023 2066 6f72 2063 6f6e 6e65 6374 696e   # for connectin
-00001000: 6720 746f 2061 2064 6576 6963 6520 7765  g to a device we
-00001010: 206e 6565 6420 6974 7320 6964 2061 6e64   need its id and
-00001020: 2069 7020 6164 6472 6573 735c 6e20 2020   ip address\n   
-00001030: 2020 2061 7379 6e63 2077 6974 6820 5377     async with Sw
-00001040: 6974 6368 6572 5479 7065 3241 7069 2864  itcherType2Api(d
-00001050: 6576 6963 655f 6970 2c20 6465 7669 6365  evice_ip, device
-00001060: 5f69 6429 2061 7320 6170 693a 5c6e 2020  _id) as api:\n  
-00001070: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-00001080: 6520 6465 7669 6365 2063 7572 7265 6e74  e device current
-00001090: 2073 7461 7465 5c6e 2020 2020 2020 2020   state\n        
-000010a0: 2020 6177 6169 7420 6170 692e 6765 745f    await api.get_
-000010b0: 6272 6565 7a65 5f73 7461 7465 2829 5c6e  breeze_state()\n
-000010c0: 2020 2020 2020 2020 2020 2320 696e 6974            # init
-000010d0: 6961 6c69 7a65 2074 6865 2042 7265 657a  ialize the Breez
-000010e0: 6520 5265 6d6f 7465 4d61 6e61 6765 7220  e RemoteManager 
-000010f0: 616e 6420 6765 7420 7468 6520 7265 6d6f  and get the remo
-00001100: 7465 5c6e 2020 2020 2020 2020 2020 7265  te\n          re
-00001110: 6d6f 7465 203d 2072 656d 6f74 655f 6d61  mote = remote_ma
-00001120: 6e61 6765 722e 6765 745f 7265 6d6f 7465  nager.get_remote
-00001130: 2872 656d 6f74 655f 6964 295c 6e20 2020  (remote_id)\n   
-00001140: 2020 2020 2020 2023 2070 7265 7061 7265         # prepare
-00001150: 2061 2063 6f6e 7472 6f6c 2063 6f6d 6d61   a control comma
-00001160: 6e64 2074 6861 7420 7475 726e 7320 6f6e  nd that turns on
-00001170: 2074 6865 2042 7265 657a 655c 6e20 2020   the Breeze\n   
-00001180: 2020 2020 2020 2023 2073 6574 2074 6f20         # set to 
-00001190: 3234 2064 6567 7265 6520 2843 656c 7369  24 degree (Celsi
-000011a0: 7573 2920 636f 6f6c 696e 6720 7769 7468  us) cooling with
-000011b0: 2076 6572 7469 6361 6c20 7377 696e 675c   vertical swing\
-000011c0: 6e20 2020 2020 2020 2020 2023 2073 656e  n          # sen
-000011d0: 6420 636f 6d6d 616e 6420 746f 2074 6865  d command to the
-000011e0: 2064 6576 6963 655c 6e20 2020 2020 2020   device\n       
-000011f0: 2020 2061 7761 6974 2061 7069 2e63 6f6e     await api.con
-00001200: 7472 6f6c 5f62 7265 657a 655f 6465 7669  trol_breeze_devi
-00001210: 6365 285c 6e20 2020 2020 2020 2020 2020  ce(\n           
-00001220: 2020 2072 656d 6f74 652c 5c6e 2020 2020     remote,\n    
-00001230: 2020 2020 2020 2020 2020 4465 7669 6365            Device
-00001240: 5374 6174 652e 4f4e 2c5c 6e20 2020 2020  State.ON,\n     
-00001250: 2020 2020 2020 2020 2054 6865 726d 6f73           Thermos
-00001260: 7461 744d 6f64 652e 434f 4f4c 2c5c 6e20  tatMode.COOL,\n 
-00001270: 2020 2020 2020 2020 2020 2020 2032 342c               24,
-00001280: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00001290: 5468 6572 6d6f 7374 6174 4661 6e4c 6576  ThermostatFanLev
-000012a0: 656c 2e4d 4544 4955 4d2c 5c6e 2020 2020  el.MEDIUM,\n    
-000012b0: 2020 2020 2020 2020 2020 5468 6572 6d6f            Thermo
-000012c0: 7374 6174 5377 696e 672e 4f4e 2c5c 6e20  statSwing.ON,\n 
-000012d0: 2020 2020 2020 2020 2029 5c6e 5c6e 2020           )\n\n  
-000012e0: 2320 6372 6561 7465 2074 6865 2072 656d  # create the rem
-000012f0: 6f74 6520 6d61 6e61 6765 7220 6f75 7473  ote manager outs
-00001300: 6964 6520 7468 6520 636f 6e74 6578 7420  ide the context 
-00001310: 666f 7220 7265 2d75 7369 6e67 5c6e 2020  for re-using\n  
-00001320: 7265 6d6f 7465 5f6d 616e 6167 6572 203d  remote_manager =
-00001330: 2053 7769 7463 6865 7242 7265 657a 6552   SwitcherBreezeR
-00001340: 656d 6f74 654d 616e 6167 6572 2829 5c6e  emoteManager()\n
-00001350: 2020 6173 796e 6369 6f2e 7275 6e28 636f    asyncio.run(co
-00001360: 6e74 726f 6c5f 6272 6565 7a65 2822 3131  ntrol_breeze("11
-00001370: 312e 3232 322e 3131 2e32 3222 2c20 2261  1.222.11.22", "a
-00001380: 6231 6332 6422 2c20 7265 6d6f 7465 5f6d  b1c2d", remote_m
-00001390: 616e 6167 6572 2c20 2244 4c4b 3635 3836  anager, "DLK6586
-000013a0: 3322 2929 5c6e 2020 6060 605c 6e5c 6e3c  3"))\n  ```\n\n<
-000013b0: 2f64 6574 6169 6c73 3e5c 6e5c 6e23 2320  /details>\n\n## 
-000013c0: 436f 6d6d 616e 6420 4c69 6e65 2048 656c  Command Line Hel
-000013d0: 7065 7220 5363 7269 7074 735c 6e5c 6e2d  per Scripts\n\n-
-000013e0: 205b 6469 7363 6f76 6572 5f64 6576 6963   [discover_devic
-000013f0: 6573 2e70 795d 2868 7474 7073 3a2f 2f67  es.py](https://g
-00001400: 6974 6875 622e 636f 6d2f 546f 6d65 7246  ithub.com/TomerF
-00001410: 692f 6169 6f73 7769 7463 6865 722f 626c  i/aioswitcher/bl
-00001420: 6f62 2f64 6576 2f73 6372 6970 7473 2f64  ob/dev/scripts/d
-00001430: 6973 636f 7665 725f 6465 7669 6365 732e  iscover_devices.
-00001440: 7079 2920 6361 6e20 6469 7363 6f76 6572  py) can discover
-00001450: 2064 6576 6963 6573 2061 6e64 2074 6865   devices and the
-00001460: 6972 5c6e 2020 7374 6174 6573 2e5c 6e2d  ir\n  states.\n-
-00001470: 205b 636f 6e74 726f 6c5f 6465 7669 6365   [control_device
-00001480: 2e70 795d 2868 7474 7073 3a2f 2f67 6974  .py](https://git
-00001490: 6875 622e 636f 6d2f 546f 6d65 7246 692f  hub.com/TomerFi/
-000014a0: 6169 6f73 7769 7463 6865 722f 626c 6f62  aioswitcher/blob
-000014b0: 2f64 6576 2f73 6372 6970 7473 2f63 6f6e  /dev/scripts/con
-000014c0: 7472 6f6c 5f64 6576 6963 652e 7079 2920  trol_device.py) 
-000014d0: 6361 6e20 636f 6e74 726f 6c20 6120 6465  can control a de
-000014e0: 7669 6365 2e5c 6e5c 6e23 2320 4469 7363  vice.\n\n## Disc
-000014f0: 6c61 696d 6572 5c6e 5c6e 5468 6973 2069  laimer\n\nThis i
-00001500: 7320 2a2a 4e4f 542a 2a20 616e 206f 6666  s **NOT** an off
-00001510: 6963 6961 6c20 6d6f 6475 6c65 2061 6e64  icial module and
-00001520: 2069 7420 6973 202a 2a4e 4f54 2a2a 206f   it is **NOT** o
-00001530: 6666 6963 6961 6c6c 7920 7375 7070 6f72  fficially suppor
-00001540: 7465 6420 6279 2074 6865 2076 656e 646f  ted by the vendo
-00001550: 722e 3c2f 6272 3e5c 6e54 6861 7420 7361  r.</br>\nThat sa
-00001560: 6964 2c20 7468 616e 6b73 2061 7265 2069  id, thanks are i
-00001570: 6e20 6f72 6465 7220 746f 2061 6c6c 2074  n order to all t
-00001580: 6865 2070 656f 706c 6520 6174 205b 5377  he people at [Sw
-00001590: 6974 6368 6572 5d5b 3132 5d20 666f 7220  itcher][12] for 
-000015a0: 7468 6569 7220 636f 6f70 6572 6174 696f  their cooperatio
-000015b0: 6e20 616e 6420 6765 6e65 7261 6c20 7375  n and general su
-000015c0: 7070 6f72 742e 5c6e 5c6e 2323 2043 6f6e  pport.\n\n## Con
-000015d0: 7472 6962 7574 6f72 735c 6e5c 6e54 6861  tributors\n\nTha
-000015e0: 6e6b 7320 676f 6573 2074 6f20 7468 6573  nks goes to thes
-000015f0: 6520 776f 6e64 6572 6675 6c20 7065 6f70  e wonderful peop
-00001600: 6c65 2028 5b65 6d6f 6a69 206b 6579 5d5b  le ([emoji key][
-00001610: 315d 293a 5c6e 5c6e 3c21 2d2d 2041 4c4c  1]):\n\n<!-- ALL
-00001620: 2d43 4f4e 5452 4942 5554 4f52 532d 4c49  -CONTRIBUTORS-LI
-00001630: 5354 3a53 5441 5254 202d 2044 6f20 6e6f  ST:START - Do no
-00001640: 7420 7265 6d6f 7665 206f 7220 6d6f 6469  t remove or modi
-00001650: 6679 2074 6869 7320 7365 6374 696f 6e20  fy this section 
-00001660: 2d2d 3e5c 6e3c 212d 2d20 7072 6574 7469  -->\n<!-- pretti
-00001670: 6572 2d69 676e 6f72 652d 7374 6172 7420  er-ignore-start 
-00001680: 2d2d 3e5c 6e3c 212d 2d20 6d61 726b 646f  -->\n<!-- markdo
-00001690: 776e 6c69 6e74 2d64 6973 6162 6c65 202d  wnlint-disable -
-000016a0: 2d3e 5c6e 3c74 6162 6c65 3e5c 6e20 203c  ->\n<table>\n  <
-000016b0: 7462 6f64 793e 5c6e 2020 2020 3c74 723e  tbody>\n    <tr>
-000016c0: 5c6e 2020 2020 2020 3c74 6420 616c 6967  \n      <td alig
-000016d0: 6e3d 2263 656e 7465 7222 3e3c 6120 6872  n="center"><a hr
-000016e0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000016f0: 7562 2e63 6f6d 2f61 7669 6164 676f 6c61  ub.com/aviadgola
-00001700: 6e22 3e3c 696d 6720 7372 633d 2268 7474  n"><img src="htt
-00001710: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
-00001720: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00001730: 6f6d 2f75 2f31 3737 3432 3131 313f 763d  om/u/17742111?v=
-00001740: 343f 733d 3130 3022 2077 6964 7468 3d22  4?s=100" width="
-00001750: 3130 3070 783b 2220 616c 743d 2241 7669  100px;" alt="Avi
-00001760: 6164 2047 6f6c 616e 222f 3e3c 6272 202f  ad Golan"/><br /
-00001770: 3e3c 7375 623e 3c62 3e41 7669 6164 2047  ><sub><b>Aviad G
-00001780: 6f6c 616e 3c2f 623e 3c2f 7375 623e 3c2f  olan</b></sub></
-00001790: 613e 3c62 7220 2f3e 3c61 2068 7265 663d  a><br /><a href=
-000017a0: 2223 6461 7461 2d41 7669 6164 476f 6c61  "#data-AviadGola
-000017b0: 6e22 2074 6974 6c65 3d22 4461 7461 223e  n" title="Data">
-000017c0: f09f 94a3 3c2f 613e 3c2f 7464 3e5c 6e20  ....</a></td>\n 
-000017d0: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
-000017e0: 6365 6e74 6572 223e 3c61 2068 7265 663d  center"><a href=
-000017f0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001800: 636f 6d2f 646f 6c62 7933 3630 223e 3c69  com/dolby360"><i
-00001810: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001820: 6176 6174 6172 732e 6769 7468 7562 7573  avatars.githubus
-00001830: 6572 636f 6e74 656e 742e 636f 6d2f 752f  ercontent.com/u/
-00001840: 3232 3135 3133 3939 3f76 3d34 3f73 3d31  22151399?v=4?s=1
-00001850: 3030 2220 7769 6474 683d 2231 3030 7078  00" width="100px
-00001860: 3b22 2061 6c74 3d22 446f 6c65 7620 4265  ;" alt="Dolev Be
-00001870: 6e20 4168 6172 6f6e 222f 3e3c 6272 202f  n Aharon"/><br /
-00001880: 3e3c 7375 623e 3c62 3e44 6f6c 6576 2042  ><sub><b>Dolev B
-00001890: 656e 2041 6861 726f 6e3c 2f62 3e3c 2f73  en Aharon</b></s
-000018a0: 7562 3e3c 2f61 3e3c 6272 202f 3e3c 6120  ub></a><br /><a 
-000018b0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-000018c0: 7468 7562 2e63 6f6d 2f54 6f6d 6572 4669  thub.com/TomerFi
-000018d0: 2f61 696f 7377 6974 6368 6572 2f63 6f6d  /aioswitcher/com
-000018e0: 6d69 7473 3f61 7574 686f 723d 646f 6c62  mits?author=dolb
-000018f0: 7933 3630 2220 7469 746c 653d 2244 6f63  y360" title="Doc
-00001900: 756d 656e 7461 7469 6f6e 223e f09f 9396  umentation">....
-00001910: 3c2f 613e 3c2f 7464 3e5c 6e20 2020 2020  </a></td>\n     
-00001920: 203c 7464 2061 6c69 676e 3d22 6365 6e74   <td align="cent
-00001930: 6572 223e 3c61 2068 7265 663d 2268 7474  er"><a href="htt
-00001940: 703a 2f2f 6661 6269 616e 2d61 6666 6f6c  p://fabian-affol
-00001950: 7465 722e 6368 2f62 6c6f 672f 223e 3c69  ter.ch/blog/"><i
-00001960: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001970: 6176 6174 6172 732e 6769 7468 7562 7573  avatars.githubus
-00001980: 6572 636f 6e74 656e 742e 636f 6d2f 752f  ercontent.com/u/
-00001990: 3131 3631 3834 3f76 3d34 3f73 3d31 3030  116184?v=4?s=100
-000019a0: 2220 7769 6474 683d 2231 3030 7078 3b22  " width="100px;"
-000019b0: 2061 6c74 3d22 4661 6269 616e 2041 6666   alt="Fabian Aff
-000019c0: 6f6c 7465 7222 2f3e 3c62 7220 2f3e 3c73  olter"/><br /><s
-000019d0: 7562 3e3c 623e 4661 6269 616e 2041 6666  ub><b>Fabian Aff
-000019e0: 6f6c 7465 723c 2f62 3e3c 2f73 7562 3e3c  olter</b></sub><
-000019f0: 2f61 3e3c 6272 202f 3e3c 6120 6872 6566  /a><br /><a href
-00001a00: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00001a10: 2e63 6f6d 2f54 6f6d 6572 4669 2f61 696f  .com/TomerFi/aio
-00001a20: 7377 6974 6368 6572 2f63 6f6d 6d69 7473  switcher/commits
-00001a30: 3f61 7574 686f 723d 6661 6261 6666 2220  ?author=fabaff" 
-00001a40: 7469 746c 653d 2243 6f64 6522 3ef0 9f92  title="Code">...
-00001a50: bb3c 2f61 3e3c 2f74 643e 5c6e 2020 2020  .</a></td>\n    
-00001a60: 2020 3c74 6420 616c 6967 6e3d 2263 656e    <td align="cen
-00001a70: 7465 7222 3e3c 6120 6872 6566 3d22 6874  ter"><a href="ht
-00001a80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001a90: 2f6f 7261 6e6a 6122 3e3c 696d 6720 7372  /oranja"><img sr
-00001aa0: 633d 2268 7474 7073 3a2f 2f61 7661 7461  c="https://avata
-00001ab0: 7273 2e67 6974 6875 6275 7365 7263 6f6e  rs.githubusercon
-00001ac0: 7465 6e74 2e63 6f6d 2f75 2f36 3739 3138  tent.com/u/67918
-00001ad0: 343f 763d 343f 733d 3130 3022 2077 6964  4?v=4?s=100" wid
-00001ae0: 7468 3d22 3130 3070 783b 2220 616c 743d  th="100px;" alt=
-00001af0: 2249 747a 696b 2045 7068 7261 696d 222f  "Itzik Ephraim"/
-00001b00: 3e3c 6272 202f 3e3c 7375 623e 3c62 3e49  ><br /><sub><b>I
-00001b10: 747a 696b 2045 7068 7261 696d 3c2f 623e  tzik Ephraim</b>
-00001b20: 3c2f 7375 623e 3c2f 613e 3c62 7220 2f3e  </sub></a><br />
-00001b30: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001b40: 2f67 6974 6875 622e 636f 6d2f 546f 6d65  /github.com/Tome
-00001b50: 7246 692f 6169 6f73 7769 7463 6865 722f  rFi/aioswitcher/
-00001b60: 636f 6d6d 6974 733f 6175 7468 6f72 3d6f  commits?author=o
-00001b70: 7261 6e6a 6122 2074 6974 6c65 3d22 436f  ranja" title="Co
-00001b80: 6465 223e f09f 92bb 3c2f 613e 3c2f 7464  de">....</a></td
-00001b90: 3e5c 6e20 2020 2020 203c 7464 2061 6c69  >\n      <td ali
-00001ba0: 676e 3d22 6365 6e74 6572 223e 3c61 2068  gn="center"><a h
-00001bb0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00001bc0: 6875 622e 636f 6d2f 4b65 7361 7638 3930  hub.com/Kesav890
-00001bd0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-00001be0: 733a 2f2f 6176 6174 6172 732e 6769 7468  s://avatars.gith
-00001bf0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00001c00: 6d2f 752f 3832 3535 3939 3531 3f76 3d34  m/u/82559951?v=4
-00001c10: 3f73 3d31 3030 2220 7769 6474 683d 2231  ?s=100" width="1
-00001c20: 3030 7078 3b22 2061 6c74 3d22 4b65 7361  00px;" alt="Kesa
-00001c30: 7638 3930 222f 3e3c 6272 202f 3e3c 7375  v890"/><br /><su
-00001c40: 623e 3c62 3e4b 6573 6176 3839 303c 2f62  b><b>Kesav890</b
-00001c50: 3e3c 2f73 7562 3e3c 2f61 3e3c 6272 202f  ></sub></a><br /
-00001c60: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00001c70: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f6d  //github.com/Tom
-00001c80: 6572 4669 2f61 696f 7377 6974 6368 6572  erFi/aioswitcher
-00001c90: 2f63 6f6d 6d69 7473 3f61 7574 686f 723d  /commits?author=
-00001ca0: 4b65 7361 7638 3930 2220 7469 746c 653d  Kesav890" title=
-00001cb0: 2244 6f63 756d 656e 7461 7469 6f6e 223e  "Documentation">
-00001cc0: f09f 9396 3c2f 613e 3c2f 7464 3e5c 6e20  ....</a></td>\n 
-00001cd0: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
-00001ce0: 6365 6e74 6572 223e 3c61 2068 7265 663d  center"><a href=
-00001cf0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001d00: 636f 6d2f 4f72 4269 6e22 3e3c 696d 6720  com/OrBin"><img 
-00001d10: 7372 633d 2268 7474 7073 3a2f 2f61 7661  src="https://ava
-00001d20: 7461 7273 2e67 6974 6875 6275 7365 7263  tars.githubuserc
-00001d30: 6f6e 7465 6e74 2e63 6f6d 2f75 2f36 3839  ontent.com/u/689
-00001d40: 3732 3334 3f76 3d34 3f73 3d31 3030 2220  7234?v=4?s=100" 
-00001d50: 7769 6474 683d 2231 3030 7078 3b22 2061  width="100px;" a
-00001d60: 6c74 3d22 4f72 2042 696e 222f 3e3c 6272  lt="Or Bin"/><br
-00001d70: 202f 3e3c 7375 623e 3c62 3e4f 7220 4269   /><sub><b>Or Bi
-00001d80: 6e3c 2f62 3e3c 2f73 7562 3e3c 2f61 3e3c  n</b></sub></a><
-00001d90: 6272 202f 3e3c 6120 6872 6566 3d22 6874  br /><a href="ht
-00001da0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001db0: 2f54 6f6d 6572 4669 2f61 696f 7377 6974  /TomerFi/aioswit
-00001dc0: 6368 6572 2f63 6f6d 6d69 7473 3f61 7574  cher/commits?aut
-00001dd0: 686f 723d 4f72 4269 6e22 2074 6974 6c65  hor=OrBin" title
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6169 6f73  : 2.1.Name: aios
+00000020: 7769 7463 6865 720a 5665 7273 696f 6e3a  witcher.Version:
+00000030: 2033 2e33 2e30 0a53 756d 6d61 7279 3a20   3.3.0.Summary: 
+00000040: 5377 6974 6368 6572 2050 7974 686f 6e20  Switcher Python 
+00000050: 496e 7465 6772 6174 696f 6e2e 0a48 6f6d  Integration..Hom
+00000060: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
+00000070: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000080: 2f61 696f 7377 6974 6368 6572 2f0a 4c69  /aioswitcher/.Li
+00000090: 6365 6e73 653a 2041 7061 6368 652d 322e  cense: Apache-2.
+000000a0: 300a 4b65 7977 6f72 6473 3a20 686f 6d65  0.Keywords: home
+000000b0: 2c61 7574 6f6d 6174 696f 6e2c 7377 6974  ,automation,swit
+000000c0: 6368 6572 2c73 6d61 7274 0a41 7574 686f  cher,smart.Autho
+000000d0: 723a 2054 6f6d 6572 2046 6967 656e 626c  r: Tomer Figenbl
+000000e0: 6174 0a41 7574 686f 722d 656d 6169 6c3a  at.Author-email:
+000000f0: 2074 6f6d 6572 4074 6f6d 6669 2e69 6e66   tomer@tomfi.inf
+00000100: 6f0a 4d61 696e 7461 696e 6572 3a20 5368  o.Maintainer: Sh
+00000110: 6179 204c 6576 790a 5265 7175 6972 6573  ay Levy.Requires
+00000120: 2d50 7974 686f 6e3a 203e 3d33 2e39 2e30  -Python: >=3.9.0
+00000130: 2c3c 342e 302e 300a 436c 6173 7369 6669  ,<4.0.0.Classifi
+00000140: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+00000150: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00000160: 6572 730a 436c 6173 7369 6669 6572 3a20  ers.Classifier: 
+00000170: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000180: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
+00000190: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
+000001a0: 7365 0a43 6c61 7373 6966 6965 723a 204f  se.Classifier: O
+000001b0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000001c0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000001d0: 740a 436c 6173 7369 6669 6572 3a20 5072  t.Classifier: Pr
+000001e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000200: 330a 436c 6173 7369 6669 6572 3a20 5072  3.Classifier: Pr
+00000210: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000220: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000230: 332e 390a 436c 6173 7369 6669 6572 3a20  3.9.Classifier: 
+00000240: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000250: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000260: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
+00000270: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000280: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000290: 6e20 3a3a 2033 2e31 310a 436c 6173 7369  n :: 3.11.Classi
+000002a0: 6669 6572 3a20 546f 7069 6320 3a3a 2048  fier: Topic :: H
+000002b0: 6f6d 6520 4175 746f 6d61 7469 6f6e 0a43  ome Automation.C
+000002c0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+000002d0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+000002e0: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
+000002f0: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
+00000300: 4d6f 6475 6c65 730a 436c 6173 7369 6669  Modules.Classifi
+00000310: 6572 3a20 5479 7069 6e67 203a 3a20 5479  er: Typing :: Ty
+00000320: 7065 640a 5072 6f6a 6563 742d 5552 4c3a  ped.Project-URL:
+00000330: 2044 6f63 756d 656e 7461 7469 6f6e 2c20   Documentation, 
+00000340: 6874 7470 733a 2f2f 6169 6f73 7769 7463  https://aioswitc
+00000350: 6865 722e 746f 6d66 692e 696e 666f 0a50  her.tomfi.info.P
+00000360: 726f 6a65 6374 2d55 524c 3a20 5265 706f  roject-URL: Repo
+00000370: 7369 746f 7279 2c20 6874 7470 733a 2f2f  sitory, https://
+00000380: 6769 7468 7562 2e63 6f6d 2f74 6f6d 6572  github.com/tomer
+00000390: 6669 2f61 696f 7377 6974 6368 6572 0a44  fi/aioswitcher.D
+000003a0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+000003b0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+000003c0: 726b 646f 776e 0a0a 2320 4865 6c70 2057  rkdown..# Help W
+000003d0: 616e 7465 640a 0a3c 7020 616c 6967 6e3d  anted..<p align=
+000003e0: 226c 6566 7422 3e0a 3c73 7472 6f6e 673e  "left">.<strong>
+000003f0: 0a41 696f 7377 6974 6368 6572 2070 726f  .Aioswitcher pro
+00000400: 6a65 6374 2069 7320 6c6f 6f6b 696e 6720  ject is looking 
+00000410: 666f 7220 6d61 696e 7461 696e 6572 7320  for maintainers 
+00000420: 616e 6420 636f 6e74 7269 6275 746f 7273  and contributors
+00000430: 213c 6272 2f3e 0a46 6f72 2076 6172 696f  !<br/>.For vario
+00000440: 7573 2072 6561 736f 6e73 2c20 4920 6361  us reasons, I ca
+00000450: 6e20 6f6e 6c79 206b 6565 7020 6d61 696e  n only keep main
+00000460: 7461 696e 696e 6720 7468 6973 2070 726f  taining this pro
+00000470: 6a65 6374 2061 7320 6661 7220 6173 2064  ject as far as d
+00000480: 6570 656e 6465 6e63 7920 6275 6d70 7320  ependency bumps 
+00000490: 616e 6420 7075 626c 6973 6869 6e67 2e3c  and publishing.<
+000004a0: 6272 2f3e 0a41 7320 666f 7220 6e65 7720  br/>.As for new 
+000004b0: 6665 6174 7572 6573 2061 6e64 2074 6865  features and the
+000004c0: 206f 6363 6173 696f 6e61 6c20 6275 6720   occasional bug 
+000004d0: 7375 7070 6f72 742c 2074 6865 7365 2077  support, these w
+000004e0: 696c 6c20 7265 7175 6972 6520 6f74 6865  ill require othe
+000004f0: 7220 6d61 696e 7461 696e 6572 732f 636f  r maintainers/co
+00000500: 6e74 7269 6275 746f 7273 2e3c 6272 2f3e  ntributors.<br/>
+00000510: 0a3c 6272 2f3e 0a49 6620 7468 6174 2773  .<br/>.If that's
+00000520: 2079 6f75 202d 2070 6c65 6173 6520 6665   you - please fe
+00000530: 656c 2066 7265 6520 746f 2070 696e 6720  el free to ping 
+00000540: 6d65 2061 6e64 2049 2077 696c 6c20 646f  me and I will do
+00000550: 2061 6c6c 2049 2063 616e 2074 6f20 6d61   all I can to ma
+00000560: 6b65 2074 6865 206f 6e62 6f61 7264 696e  ke the onboardin
+00000570: 6720 7072 6f63 6573 7320 6561 7379 2e0a  g process easy..
+00000580: 3c2f 7374 726f 6e67 3e0a 3c2f 703e 0a0a  </strong>.</p>..
+00000590: 2320 5377 6974 6368 6572 2050 7974 686f  # Switcher Pytho
+000005a0: 6e20 496e 7465 6772 6174 696f 6e3c 2f62  n Integration</b
+000005b0: 723e 5b21 5b70 7970 692d 7665 7273 696f  r>[![pypi-versio
+000005c0: 6e5d 5d5b 3131 5d20 5b21 5b70 7970 692d  n]][11] [![pypi-
+000005d0: 646f 776e 6c6f 6164 735d 5d5b 3131 5d20  downloads]][11] 
+000005e0: 5b21 5b6c 6963 656e 7365 2d62 6164 6765  [![license-badge
+000005f0: 5d5d 5b34 5d0a 0a5b 215b 6768 2d62 7569  ]][4]..[![gh-bui
+00000600: 6c64 2d73 7461 7475 735d 5d5b 375d 205b  ld-status]][7] [
+00000610: 215b 6768 2d70 6167 6573 2d73 7461 7475  ![gh-pages-statu
+00000620: 735d 5d5b 385d 205b 215b 636f 6465 636f  s]][8] [![codeco
+00000630: 765d 5d5b 335d 0a0a 5079 5069 206d 6f64  v]][3]..PyPi mod
+00000640: 756c 6520 696e 7465 6772 6174 696e 6720  ule integrating 
+00000650: 7769 7468 2076 6172 696f 7573 205b 5377  with various [Sw
+00000660: 6974 6368 6572 5d5b 3132 5d20 6465 7669  itcher][12] devi
+00000670: 6365 732e 3c2f 6272 3e0a 4368 6563 6b20  ces.</br>.Check 
+00000680: 6f75 7420 7468 6520 5b77 696b 6920 7061  out the [wiki pa
+00000690: 6765 735d 5b30 5d20 666f 7220 6120 6c69  ges][0] for a li
+000006a0: 7374 206f 6620 7375 7070 6f72 7465 6420  st of supported 
+000006b0: 6465 7669 6365 732e 0a0a 6060 6073 6865  devices...```she
+000006c0: 6c6c 0a70 6970 2069 6e73 7461 6c6c 2061  ll.pip install a
+000006d0: 696f 7377 6974 6368 6572 0a60 6060 0a0a  ioswitcher.```..
+000006e0: 3c74 6162 6c65 3e0a 2020 3c74 643e 3c61  <table>.  <td><a
+000006f0: 2068 7265 663d 2268 7474 7073 3a2f 2f61   href="https://a
+00000700: 696f 7377 6974 6368 6572 2e74 6f6d 6669  ioswitcher.tomfi
+00000710: 2e69 6e66 6f2f 223e 446f 6375 6d65 6e74  .info/">Document
+00000720: 6174 696f 6e3c 2f61 3e3c 2f74 643e 0a20  ation</a></td>. 
+00000730: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
+00000740: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000750: 2f54 6f6d 6572 4669 2f61 696f 7377 6974  /TomerFi/aioswit
+00000760: 6368 6572 2f77 696b 6922 3e57 696b 693c  cher/wiki">Wiki<
+00000770: 2f61 3e3c 2f74 643e 0a20 203c 7464 3e3c  /a></td>.  <td><
+00000780: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000790: 6769 7468 7562 2e63 6f6d 2f54 6f6d 6572  github.com/Tomer
+000007a0: 4669 2f61 696f 7377 6974 6368 6572 2f62  Fi/aioswitcher/b
+000007b0: 6c6f 622f 6465 762f 434f 4e54 5249 4255  lob/dev/CONTRIBU
+000007c0: 5449 4e47 2e6d 6422 3e43 6f6e 7472 6962  TING.md">Contrib
+000007d0: 7574 696e 673c 2f61 3e3c 2f74 643e 0a3c  uting</a></td>.<
+000007e0: 2f74 6162 6c65 3e0a 0a23 2320 4578 616d  /table>..## Exam
+000007f0: 706c 6520 5573 6167 650a 0a3c 6465 7461  ple Usage..<deta
+00000800: 696c 733e 0a20 203c 7375 6d6d 6172 793e  ils>.  <summary>
+00000810: 5374 6174 6520 4272 6964 6765 3c2f 7375  State Bridge</su
+00000820: 6d6d 6172 793e 0a0a 6060 6070 7974 686f  mmary>..```pytho
+00000830: 6e0a 6173 796e 6320 6465 6620 7072 696e  n.async def prin
+00000840: 745f 6465 7669 6365 7328 6465 6c61 7929  t_devices(delay)
+00000850: 3a0a 2020 2020 6465 6620 6f6e 5f64 6576  :.    def on_dev
+00000860: 6963 655f 666f 756e 645f 6361 6c6c 6261  ice_found_callba
+00000870: 636b 2864 6576 6963 6529 3a0a 2020 2020  ck(device):.    
+00000880: 2020 2020 2320 6120 7377 6974 6368 6572      # a switcher
+00000890: 2064 6576 6963 6520 7769 6c6c 2062 726f   device will bro
+000008a0: 6164 6361 7374 2061 2073 7461 7465 206d  adcast a state m
+000008b0: 6573 7361 6765 2061 7070 726f 7869 6d61  essage approxima
+000008c0: 7465 6c79 2065 7665 7279 2034 2073 6563  tely every 4 sec
+000008d0: 6f6e 6473 0a20 2020 2020 2020 2070 7269  onds.        pri
+000008e0: 6e74 2861 7364 6963 7428 6465 7669 6365  nt(asdict(device
+000008f0: 2929 0a0a 2020 2020 6173 796e 6320 7769  ))..    async wi
+00000900: 7468 2053 7769 7463 6865 7242 7269 6467  th SwitcherBridg
+00000910: 6528 6f6e 5f64 6576 6963 655f 666f 756e  e(on_device_foun
+00000920: 645f 6361 6c6c 6261 636b 293a 0a20 2020  d_callback):.   
+00000930: 2020 2020 2061 7761 6974 2061 7379 6e63       await async
+00000940: 696f 2e73 6c65 6570 2864 656c 6179 290a  io.sleep(delay).
+00000950: 0a23 2072 756e 2074 6865 2062 7269 6467  .# run the bridg
+00000960: 6520 666f 7220 3630 2073 6563 6f6e 6473  e for 60 seconds
+00000970: 0a61 7379 6e63 696f 2e72 756e 2870 7269  .asyncio.run(pri
+00000980: 6e74 5f64 6576 6963 6573 2836 3029 290a  nt_devices(60)).
+00000990: 6060 600a 0a3c 2f64 6574 6169 6c73 3e0a  ```..</details>.
+000009a0: 0a3c 6465 7461 696c 733e 0a20 203c 7375  .<details>.  <su
+000009b0: 6d6d 6172 793e 506f 7765 7220 506c 7567  mmary>Power Plug
+000009c0: 2041 5049 3c2f 7375 6d6d 6172 793e 0a0a   API</summary>..
+000009d0: 2020 6060 6070 7974 686f 6e0a 2020 6173    ```python.  as
+000009e0: 796e 6320 6465 6620 636f 6e74 726f 6c5f  ync def control_
+000009f0: 706f 7765 725f 706c 7567 2864 6576 6963  power_plug(devic
+00000a00: 655f 6970 2c20 6465 7669 6365 5f69 6429  e_ip, device_id)
+00000a10: 203a 0a20 2020 2020 2023 2066 6f72 2063   :.      # for c
+00000a20: 6f6e 6e65 6374 696e 6720 746f 2061 2064  onnecting to a d
+00000a30: 6576 6963 6520 7765 206e 6565 6420 6974  evice we need it
+00000a40: 7320 6964 2061 6e64 2069 7020 6164 6472  s id and ip addr
+00000a50: 6573 730a 2020 2020 2020 6173 796e 6320  ess.      async 
+00000a60: 7769 7468 2053 7769 7463 6865 7254 7970  with SwitcherTyp
+00000a70: 6531 4170 6928 6465 7669 6365 5f69 702c  e1Api(device_ip,
+00000a80: 2064 6576 6963 655f 6964 2920 6173 2061   device_id) as a
+00000a90: 7069 3a0a 2020 2020 2020 2020 2020 2320  pi:.          # 
+00000aa0: 6765 7420 7468 6520 6465 7669 6365 2063  get the device c
+00000ab0: 7572 7265 6e74 2073 7461 7465 0a20 2020  urrent state.   
+00000ac0: 2020 2020 2020 2061 7761 6974 2061 7069         await api
+00000ad0: 2e67 6574 5f73 7461 7465 2829 0a20 2020  .get_state().   
+00000ae0: 2020 2020 2020 2023 2074 7572 6e20 7468         # turn th
+00000af0: 6520 6465 7669 6365 206f 6e0a 2020 2020  e device on.    
+00000b00: 2020 2020 2020 6177 6169 7420 6170 692e        await api.
+00000b10: 636f 6e74 726f 6c5f 6465 7669 6365 2843  control_device(C
+00000b20: 6f6d 6d61 6e64 2e4f 4e29 0a20 2020 2020  ommand.ON).     
+00000b30: 2020 2020 2023 2074 7572 6e20 7468 6520       # turn the 
+00000b40: 6465 7669 6365 206f 6666 0a20 2020 2020  device off.     
+00000b50: 2020 2020 2061 7761 6974 2061 7069 2e63       await api.c
+00000b60: 6f6e 7472 6f6c 5f64 6576 6963 6528 436f  ontrol_device(Co
+00000b70: 6d6d 616e 642e 4f46 4629 0a20 2020 2020  mmand.OFF).     
+00000b80: 2020 2020 2023 2073 6574 2074 6865 2064       # set the d
+00000b90: 6576 6963 6520 6e61 6d65 2074 6f20 276d  evice name to 'm
+00000ba0: 7920 6e65 7720 6e61 6d65 270a 2020 2020  y new name'.    
+00000bb0: 2020 2020 2020 6177 6169 7420 6170 692e        await api.
+00000bc0: 7365 745f 6465 7669 6365 5f6e 616d 6528  set_device_name(
+00000bd0: 226d 7920 6e65 7720 6e61 6d65 2229 0a0a  "my new name")..
+00000be0: 2020 6173 796e 6369 6f2e 7275 6e28 636f    asyncio.run(co
+00000bf0: 6e74 726f 6c5f 706f 7765 725f 706c 7567  ntrol_power_plug
+00000c00: 2822 3131 312e 3232 322e 3131 2e32 3222  ("111.222.11.22"
+00000c10: 2c20 2261 6231 6332 6422 2929 0a20 2060  , "ab1c2d")).  `
+00000c20: 6060 0a0a 3c2f 6465 7461 696c 733e 0a0a  ``..</details>..
+00000c30: 3c64 6574 6169 6c73 3e0a 2020 3c73 756d  <details>.  <sum
+00000c40: 6d61 7279 3e57 6174 6572 2048 6561 7465  mary>Water Heate
+00000c50: 7220 4150 493c 2f73 756d 6d61 7279 3e0a  r API</summary>.
+00000c60: 0a20 2060 6060 7079 7468 6f6e 0a20 2061  .  ```python.  a
+00000c70: 7379 6e63 2064 6566 2063 6f6e 7472 6f6c  sync def control
+00000c80: 5f77 6174 6572 5f68 6561 7465 7228 6465  _water_heater(de
+00000c90: 7669 6365 5f69 702c 2064 6576 6963 655f  vice_ip, device_
+00000ca0: 6964 2920 3a0a 2020 2020 2020 2320 666f  id) :.      # fo
+00000cb0: 7220 636f 6e6e 6563 7469 6e67 2074 6f20  r connecting to 
+00000cc0: 6120 6465 7669 6365 2077 6520 6e65 6564  a device we need
+00000cd0: 2069 7473 2069 6420 616e 6420 6970 2061   its id and ip a
+00000ce0: 6464 7265 7373 0a20 2020 2020 2061 7379  ddress.      asy
+00000cf0: 6e63 2077 6974 6820 5377 6974 6368 6572  nc with Switcher
+00000d00: 5479 7065 3141 7069 2864 6576 6963 655f  Type1Api(device_
+00000d10: 6970 2c20 6465 7669 6365 5f69 6429 2061  ip, device_id) a
+00000d20: 7320 6170 693a 0a20 2020 2020 2020 2020  s api:.         
+00000d30: 2023 2067 6574 2074 6865 2064 6576 6963   # get the devic
+00000d40: 6520 6375 7272 656e 7420 7374 6174 650a  e current state.
+00000d50: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00000d60: 6170 692e 6765 745f 7374 6174 6528 290a  api.get_state().
+00000d70: 2020 2020 2020 2020 2020 2320 7475 726e            # turn
+00000d80: 2074 6865 2064 6576 6963 6520 6f6e 2066   the device on f
+00000d90: 6f72 2031 3520 6d69 6e75 7465 730a 2020  or 15 minutes.  
+00000da0: 2020 2020 2020 2020 6177 6169 7420 6170          await ap
+00000db0: 692e 636f 6e74 726f 6c5f 6465 7669 6365  i.control_device
+00000dc0: 2843 6f6d 6d61 6e64 2e4f 4e2c 2031 3529  (Command.ON, 15)
+00000dd0: 0a20 2020 2020 2020 2020 2023 2074 7572  .          # tur
+00000de0: 6e20 7468 6520 6465 7669 6365 206f 6666  n the device off
+00000df0: 0a20 2020 2020 2020 2020 2061 7761 6974  .          await
+00000e00: 2061 7069 2e63 6f6e 7472 6f6c 5f64 6576   api.control_dev
+00000e10: 6963 6528 436f 6d6d 616e 642e 4f46 4629  ice(Command.OFF)
+00000e20: 0a20 2020 2020 2020 2020 2023 2073 6574  .          # set
+00000e30: 2074 6865 2064 6576 6963 6520 6e61 6d65   the device name
+00000e40: 2074 6f20 276d 7920 6e65 7720 6e61 6d65   to 'my new name
+00000e50: 270a 2020 2020 2020 2020 2020 6177 6169  '.          awai
+00000e60: 7420 6170 692e 7365 745f 6465 7669 6365  t api.set_device
+00000e70: 5f6e 616d 6528 226d 7920 6e65 7720 6e61  _name("my new na
+00000e80: 6d65 2229 0a20 2020 2020 2020 2020 2023  me").          #
+00000e90: 2063 6f6e 6669 6775 7265 2074 6865 2064   configure the d
+00000ea0: 6576 6963 6520 666f 7220 3032 3a33 3020  evice for 02:30 
+00000eb0: 6175 746f 2073 6875 7464 6f77 6e0a 2020  auto shutdown.  
+00000ec0: 2020 2020 2020 2020 6177 6169 7420 6170          await ap
+00000ed0: 692e 7365 745f 6175 746f 5f73 6875 7464  i.set_auto_shutd
+00000ee0: 6f77 6e28 7469 6d65 6465 6c74 6128 686f  own(timedelta(ho
+00000ef0: 7572 733d 322c 206d 696e 7574 6573 3d33  urs=2, minutes=3
+00000f00: 3029 290a 2020 2020 2020 2020 2020 2320  0)).          # 
+00000f10: 6765 7420 7468 6520 7363 6865 6475 6c65  get the schedule
+00000f20: 7320 6672 6f6d 2074 6865 2064 6576 6963  s from the devic
+00000f30: 650a 2020 2020 2020 2020 2020 6177 6169  e.          awai
+00000f40: 7420 6170 692e 6765 745f 7363 6865 6475  t api.get_schedu
+00000f50: 6c65 7328 290a 2020 2020 2020 2020 2020  les().          
+00000f60: 2320 6465 6c65 7465 2061 6e64 2065 7869  # delete and exi
+00000f70: 7374 696e 6720 7363 6865 6475 6c65 2077  sting schedule w
+00000f80: 6974 6820 6964 2031 0a20 2020 2020 2020  ith id 1.       
+00000f90: 2020 2061 7761 6974 2061 7069 2e64 656c     await api.del
+00000fa0: 6574 655f 7363 6865 6475 6c65 2822 3122  ete_schedule("1"
+00000fb0: 290a 2020 2020 2020 2020 2020 2320 6372  ).          # cr
+00000fc0: 6561 7465 2061 206e 6577 2072 6563 7572  eate a new recur
+00000fd0: 7269 6e67 2073 6368 6564 756c 6520 666f  ring schedule fo
+00000fe0: 7220 3133 3a30 302d 3134 3a33 300a 2020  r 13:00-14:30.  
+00000ff0: 2020 2020 2020 2020 2320 6578 6563 7574          # execut
+00001000: 696e 6720 6f6e 2073 756e 6461 7920 616e  ing on sunday an
+00001010: 6420 6672 6964 6179 0a20 2020 2020 2020  d friday.       
+00001020: 2020 2061 7761 6974 2061 7069 2e63 7265     await api.cre
+00001030: 6174 655f 7363 6865 6475 6c65 2822 3133  ate_schedule("13
+00001040: 3a30 3022 2c20 2231 343a 3330 222c 207b  :00", "14:30", {
+00001050: 4461 7973 2e53 554e 4441 592c 2044 6179  Days.SUNDAY, Day
+00001060: 732e 4652 4944 4159 7d29 0a0a 2020 6173  s.FRIDAY})..  as
+00001070: 796e 6369 6f2e 7275 6e28 636f 6e74 726f  yncio.run(contro
+00001080: 6c5f 7761 7465 725f 6865 6174 6572 2822  l_water_heater("
+00001090: 3131 312e 3232 322e 3131 2e32 3222 2c20  111.222.11.22", 
+000010a0: 2261 6231 6332 6422 2929 0a20 2060 6060  "ab1c2d")).  ```
+000010b0: 0a0a 3c2f 6465 7461 696c 733e 0a0a 3c64  ..</details>..<d
+000010c0: 6574 6169 6c73 3e0a 2020 3c73 756d 6d61  etails>.  <summa
+000010d0: 7279 3e52 756e 6e65 7220 4150 493c 2f73  ry>Runner API</s
+000010e0: 756d 6d61 7279 3e0a 0a20 2060 6060 7079  ummary>..  ```py
+000010f0: 7468 6f6e 0a20 2061 7379 6e63 2064 6566  thon.  async def
+00001100: 2063 6f6e 7472 6f6c 5f72 756e 6e65 7228   control_runner(
+00001110: 6465 7669 6365 5f69 702c 2064 6576 6963  device_ip, devic
+00001120: 655f 6964 2920 3a0a 2020 2020 2020 2320  e_id) :.      # 
+00001130: 666f 7220 636f 6e6e 6563 7469 6e67 2074  for connecting t
+00001140: 6f20 6120 6465 7669 6365 2077 6520 6e65  o a device we ne
+00001150: 6564 2069 7473 2069 6420 616e 6420 6970  ed its id and ip
+00001160: 2061 6464 7265 7373 0a20 2020 2020 2061   address.      a
+00001170: 7379 6e63 2077 6974 6820 5377 6974 6368  sync with Switch
+00001180: 6572 5479 7065 3241 7069 2864 6576 6963  erType2Api(devic
+00001190: 655f 6970 2c20 6465 7669 6365 5f69 6429  e_ip, device_id)
+000011a0: 2061 7320 6170 693a 0a20 2020 2020 2020   as api:.       
+000011b0: 2020 2023 2067 6574 2074 6865 2064 6576     # get the dev
+000011c0: 6963 6520 6375 7272 656e 7420 7374 6174  ice current stat
+000011d0: 650a 2020 2020 2020 2020 2020 6177 6169  e.          awai
+000011e0: 7420 6170 692e 6765 745f 7368 7574 7465  t api.get_shutte
+000011f0: 725f 7374 6174 6528 290a 2020 2020 2020  r_state().      
+00001200: 2020 2020 2320 6f70 656e 2074 6865 2073      # open the s
+00001210: 6875 7474 6572 2074 6f20 3330 250a 2020  hutter to 30%.  
+00001220: 2020 2020 2020 2020 6177 6169 7420 6170          await ap
+00001230: 692e 7365 745f 706f 7369 7469 6f6e 2833  i.set_position(3
+00001240: 3029 0a20 2020 2020 2020 2020 2023 2073  0).          # s
+00001250: 746f 7020 7468 6520 7368 7574 7465 7220  top the shutter 
+00001260: 6966 2063 7572 7265 6e74 6c79 2072 6f6c  if currently rol
+00001270: 6c69 6e67 0a20 2020 2020 2020 2020 2061  ling.          a
+00001280: 7761 6974 2061 7069 2e73 746f 7028 290a  wait api.stop().
+00001290: 0a20 2061 7379 6e63 696f 2e72 756e 2863  .  asyncio.run(c
+000012a0: 6f6e 7472 6f6c 5f72 756e 6e65 7228 2231  ontrol_runner("1
+000012b0: 3131 2e32 3232 2e31 312e 3232 222c 2022  11.222.11.22", "
+000012c0: 6162 3163 3264 2229 290a 2020 6060 600a  ab1c2d")).  ```.
+000012d0: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
+000012e0: 7461 696c 733e 0a20 203c 7375 6d6d 6172  tails>.  <summar
+000012f0: 793e 4272 6565 7a65 2041 5049 3c2f 7375  y>Breeze API</su
+00001300: 6d6d 6172 793e 0a0a 2020 6060 6070 7974  mmary>..  ```pyt
+00001310: 686f 6e0a 2020 6173 796e 6320 6465 6620  hon.  async def 
+00001320: 636f 6e74 726f 6c5f 6272 6565 7a65 2864  control_breeze(d
+00001330: 6576 6963 655f 6970 2c20 6465 7669 6365  evice_ip, device
+00001340: 5f69 642c 2072 656d 6f74 655f 6d61 6e61  _id, remote_mana
+00001350: 6765 722c 2072 656d 6f74 655f 6964 2920  ger, remote_id) 
+00001360: 3a0a 2020 2020 2020 2320 666f 7220 636f  :.      # for co
+00001370: 6e6e 6563 7469 6e67 2074 6f20 6120 6465  nnecting to a de
+00001380: 7669 6365 2077 6520 6e65 6564 2069 7473  vice we need its
+00001390: 2069 6420 616e 6420 6970 2061 6464 7265   id and ip addre
+000013a0: 7373 0a20 2020 2020 2061 7379 6e63 2077  ss.      async w
+000013b0: 6974 6820 5377 6974 6368 6572 5479 7065  ith SwitcherType
+000013c0: 3241 7069 2864 6576 6963 655f 6970 2c20  2Api(device_ip, 
+000013d0: 6465 7669 6365 5f69 6429 2061 7320 6170  device_id) as ap
+000013e0: 693a 0a20 2020 2020 2020 2020 2023 2067  i:.          # g
+000013f0: 6574 2074 6865 2064 6576 6963 6520 6375  et the device cu
+00001400: 7272 656e 7420 7374 6174 650a 2020 2020  rrent state.    
+00001410: 2020 2020 2020 6177 6169 7420 6170 692e        await api.
+00001420: 6765 745f 6272 6565 7a65 5f73 7461 7465  get_breeze_state
+00001430: 2829 0a20 2020 2020 2020 2020 2023 2069  ().          # i
+00001440: 6e69 7469 616c 697a 6520 7468 6520 4272  nitialize the Br
+00001450: 6565 7a65 2052 656d 6f74 654d 616e 6167  eeze RemoteManag
+00001460: 6572 2061 6e64 2067 6574 2074 6865 2072  er and get the r
+00001470: 656d 6f74 650a 2020 2020 2020 2020 2020  emote.          
+00001480: 7265 6d6f 7465 203d 2072 656d 6f74 655f  remote = remote_
+00001490: 6d61 6e61 6765 722e 6765 745f 7265 6d6f  manager.get_remo
+000014a0: 7465 2872 656d 6f74 655f 6964 290a 2020  te(remote_id).  
+000014b0: 2020 2020 2020 2020 2320 7072 6570 6172          # prepar
+000014c0: 6520 6120 636f 6e74 726f 6c20 636f 6d6d  e a control comm
+000014d0: 616e 6420 7468 6174 2074 7572 6e73 206f  and that turns o
+000014e0: 6e20 7468 6520 4272 6565 7a65 0a20 2020  n the Breeze.   
+000014f0: 2020 2020 2020 2023 2073 6574 2074 6f20         # set to 
+00001500: 3234 2064 6567 7265 6520 2843 656c 7369  24 degree (Celsi
+00001510: 7573 2920 636f 6f6c 696e 6720 7769 7468  us) cooling with
+00001520: 2076 6572 7469 6361 6c20 7377 696e 670a   vertical swing.
+00001530: 2020 2020 2020 2020 2020 2320 7365 6e64            # send
+00001540: 2063 6f6d 6d61 6e64 2074 6f20 7468 6520   command to the 
+00001550: 6465 7669 6365 0a20 2020 2020 2020 2020  device.         
+00001560: 2061 7761 6974 2061 7069 2e63 6f6e 7472   await api.contr
+00001570: 6f6c 5f62 7265 657a 655f 6465 7669 6365  ol_breeze_device
+00001580: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00001590: 7265 6d6f 7465 2c0a 2020 2020 2020 2020  remote,.        
+000015a0: 2020 2020 2020 4465 7669 6365 5374 6174        DeviceStat
+000015b0: 652e 4f4e 2c0a 2020 2020 2020 2020 2020  e.ON,.          
+000015c0: 2020 2020 5468 6572 6d6f 7374 6174 4d6f      ThermostatMo
+000015d0: 6465 2e43 4f4f 4c2c 0a20 2020 2020 2020  de.COOL,.       
+000015e0: 2020 2020 2020 2032 342c 0a20 2020 2020         24,.     
+000015f0: 2020 2020 2020 2020 2054 6865 726d 6f73           Thermos
+00001600: 7461 7446 616e 4c65 7665 6c2e 4d45 4449  tatFanLevel.MEDI
+00001610: 554d 2c0a 2020 2020 2020 2020 2020 2020  UM,.            
+00001620: 2020 5468 6572 6d6f 7374 6174 5377 696e    ThermostatSwin
+00001630: 672e 4f4e 2c0a 2020 2020 2020 2020 2020  g.ON,.          
+00001640: 290a 0a20 2023 2063 7265 6174 6520 7468  )..  # create th
+00001650: 6520 7265 6d6f 7465 206d 616e 6167 6572  e remote manager
+00001660: 206f 7574 7369 6465 2074 6865 2063 6f6e   outside the con
+00001670: 7465 7874 2066 6f72 2072 652d 7573 696e  text for re-usin
+00001680: 670a 2020 7265 6d6f 7465 5f6d 616e 6167  g.  remote_manag
+00001690: 6572 203d 2053 7769 7463 6865 7242 7265  er = SwitcherBre
+000016a0: 657a 6552 656d 6f74 654d 616e 6167 6572  ezeRemoteManager
+000016b0: 2829 0a20 2061 7379 6e63 696f 2e72 756e  ().  asyncio.run
+000016c0: 2863 6f6e 7472 6f6c 5f62 7265 657a 6528  (control_breeze(
+000016d0: 2231 3131 2e32 3232 2e31 312e 3232 222c  "111.222.11.22",
+000016e0: 2022 6162 3163 3264 222c 2072 656d 6f74   "ab1c2d", remot
+000016f0: 655f 6d61 6e61 6765 722c 2022 444c 4b36  e_manager, "DLK6
+00001700: 3538 3633 2229 290a 2020 6060 600a 0a3c  5863")).  ```..<
+00001710: 2f64 6574 6169 6c73 3e0a 0a23 2320 436f  /details>..## Co
+00001720: 6d6d 616e 6420 4c69 6e65 2048 656c 7065  mmand Line Helpe
+00001730: 7220 5363 7269 7074 730a 0a2d 205b 6469  r Scripts..- [di
+00001740: 7363 6f76 6572 5f64 6576 6963 6573 2e70  scover_devices.p
+00001750: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
+00001760: 622e 636f 6d2f 546f 6d65 7246 692f 6169  b.com/TomerFi/ai
+00001770: 6f73 7769 7463 6865 722f 626c 6f62 2f64  oswitcher/blob/d
+00001780: 6576 2f73 6372 6970 7473 2f64 6973 636f  ev/scripts/disco
+00001790: 7665 725f 6465 7669 6365 732e 7079 2920  ver_devices.py) 
+000017a0: 6361 6e20 6469 7363 6f76 6572 2064 6576  can discover dev
+000017b0: 6963 6573 2061 6e64 2074 6865 6972 0a20  ices and their. 
+000017c0: 2073 7461 7465 732e 0a2d 205b 636f 6e74   states..- [cont
+000017d0: 726f 6c5f 6465 7669 6365 2e70 795d 2868  rol_device.py](h
+000017e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000017f0: 6d2f 546f 6d65 7246 692f 6169 6f73 7769  m/TomerFi/aioswi
+00001800: 7463 6865 722f 626c 6f62 2f64 6576 2f73  tcher/blob/dev/s
+00001810: 6372 6970 7473 2f63 6f6e 7472 6f6c 5f64  cripts/control_d
+00001820: 6576 6963 652e 7079 2920 6361 6e20 636f  evice.py) can co
+00001830: 6e74 726f 6c20 6120 6465 7669 6365 2e0a  ntrol a device..
+00001840: 0a23 2320 4469 7363 6c61 696d 6572 0a0a  .## Disclaimer..
+00001850: 5468 6973 2069 7320 2a2a 4e4f 542a 2a20  This is **NOT** 
+00001860: 616e 206f 6666 6963 6961 6c20 6d6f 6475  an official modu
+00001870: 6c65 2061 6e64 2069 7420 6973 202a 2a4e  le and it is **N
+00001880: 4f54 2a2a 206f 6666 6963 6961 6c6c 7920  OT** officially 
+00001890: 7375 7070 6f72 7465 6420 6279 2074 6865  supported by the
+000018a0: 2076 656e 646f 722e 3c2f 6272 3e0a 5468   vendor.</br>.Th
+000018b0: 6174 2073 6169 642c 2074 6861 6e6b 7320  at said, thanks 
+000018c0: 6172 6520 696e 206f 7264 6572 2074 6f20  are in order to 
+000018d0: 616c 6c20 7468 6520 7065 6f70 6c65 2061  all the people a
+000018e0: 7420 5b53 7769 7463 6865 725d 5b31 325d  t [Switcher][12]
+000018f0: 2066 6f72 2074 6865 6972 2063 6f6f 7065   for their coope
+00001900: 7261 7469 6f6e 2061 6e64 2067 656e 6572  ration and gener
+00001910: 616c 2073 7570 706f 7274 2e0a 0a23 2320  al support...## 
+00001920: 436f 6e74 7269 6275 746f 7273 0a0a 5468  Contributors..Th
+00001930: 616e 6b73 2067 6f65 7320 746f 2074 6865  anks goes to the
+00001940: 7365 2077 6f6e 6465 7266 756c 2070 656f  se wonderful peo
+00001950: 706c 6520 285b 656d 6f6a 6920 6b65 795d  ple ([emoji key]
+00001960: 5b31 5d29 3a0a 0a3c 212d 2d20 414c 4c2d  [1]):..<!-- ALL-
+00001970: 434f 4e54 5249 4255 544f 5253 2d4c 4953  CONTRIBUTORS-LIS
+00001980: 543a 5354 4152 5420 2d20 446f 206e 6f74  T:START - Do not
+00001990: 2072 656d 6f76 6520 6f72 206d 6f64 6966   remove or modif
+000019a0: 7920 7468 6973 2073 6563 7469 6f6e 202d  y this section -
+000019b0: 2d3e 0a3c 212d 2d20 7072 6574 7469 6572  ->.<!-- prettier
+000019c0: 2d69 676e 6f72 652d 7374 6172 7420 2d2d  -ignore-start --
+000019d0: 3e0a 3c21 2d2d 206d 6172 6b64 6f77 6e6c  >.<!-- markdownl
+000019e0: 696e 742d 6469 7361 626c 6520 2d2d 3e0a  int-disable -->.
+000019f0: 3c74 6162 6c65 3e0a 2020 3c74 626f 6479  <table>.  <tbody
+00001a00: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00001a10: 203c 7464 2061 6c69 676e 3d22 6365 6e74   <td align="cent
+00001a20: 6572 2220 7661 6c69 676e 3d22 746f 7022  er" valign="top"
+00001a30: 2077 6964 7468 3d22 3134 2e32 3825 223e   width="14.28%">
+00001a40: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001a50: 2f67 6974 6875 622e 636f 6d2f 6176 6961  /github.com/avia
+00001a60: 6467 6f6c 616e 223e 3c69 6d67 2073 7263  dgolan"><img src
+00001a70: 3d22 6874 7470 733a 2f2f 6176 6174 6172  ="https://avatar
+00001a80: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
+00001a90: 656e 742e 636f 6d2f 752f 3137 3734 3231  ent.com/u/177421
+00001aa0: 3131 3f76 3d34 3f73 3d31 3030 2220 7769  11?v=4?s=100" wi
+00001ab0: 6474 683d 2231 3030 7078 3b22 2061 6c74  dth="100px;" alt
+00001ac0: 3d22 4176 6961 6420 476f 6c61 6e22 2f3e  ="Aviad Golan"/>
+00001ad0: 3c62 7220 2f3e 3c73 7562 3e3c 623e 4176  <br /><sub><b>Av
+00001ae0: 6961 6420 476f 6c61 6e3c 2f62 3e3c 2f73  iad Golan</b></s
+00001af0: 7562 3e3c 2f61 3e3c 6272 202f 3e3c 6120  ub></a><br /><a 
+00001b00: 6872 6566 3d22 2364 6174 612d 4176 6961  href="#data-Avia
+00001b10: 6447 6f6c 616e 2220 7469 746c 653d 2244  dGolan" title="D
+00001b20: 6174 6122 3ef0 9f94 a33c 2f61 3e3c 2f74  ata">....</a></t
+00001b30: 643e 0a20 2020 2020 203c 7464 2061 6c69  d>.      <td ali
+00001b40: 676e 3d22 6365 6e74 6572 2220 7661 6c69  gn="center" vali
+00001b50: 676e 3d22 746f 7022 2077 6964 7468 3d22  gn="top" width="
+00001b60: 3134 2e32 3825 223e 3c61 2068 7265 663d  14.28%"><a href=
+00001b70: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00001b80: 636f 6d2f 646f 6c62 7933 3630 223e 3c69  com/dolby360"><i
+00001b90: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00001ba0: 6176 6174 6172 732e 6769 7468 7562 7573  avatars.githubus
+00001bb0: 6572 636f 6e74 656e 742e 636f 6d2f 752f  ercontent.com/u/
+00001bc0: 3232 3135 3133 3939 3f76 3d34 3f73 3d31  22151399?v=4?s=1
+00001bd0: 3030 2220 7769 6474 683d 2231 3030 7078  00" width="100px
+00001be0: 3b22 2061 6c74 3d22 446f 6c65 7620 4265  ;" alt="Dolev Be
+00001bf0: 6e20 4168 6172 6f6e 222f 3e3c 6272 202f  n Aharon"/><br /
+00001c00: 3e3c 7375 623e 3c62 3e44 6f6c 6576 2042  ><sub><b>Dolev B
+00001c10: 656e 2041 6861 726f 6e3c 2f62 3e3c 2f73  en Aharon</b></s
+00001c20: 7562 3e3c 2f61 3e3c 6272 202f 3e3c 6120  ub></a><br /><a 
+00001c30: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001c40: 7468 7562 2e63 6f6d 2f54 6f6d 6572 4669  thub.com/TomerFi
+00001c50: 2f61 696f 7377 6974 6368 6572 2f63 6f6d  /aioswitcher/com
+00001c60: 6d69 7473 3f61 7574 686f 723d 646f 6c62  mits?author=dolb
+00001c70: 7933 3630 2220 7469 746c 653d 2244 6f63  y360" title="Doc
+00001c80: 756d 656e 7461 7469 6f6e 223e f09f 9396  umentation">....
+00001c90: 3c2f 613e 3c2f 7464 3e0a 2020 2020 2020  </a></td>.      
+00001ca0: 3c74 6420 616c 6967 6e3d 2263 656e 7465  <td align="cente
+00001cb0: 7222 2076 616c 6967 6e3d 2274 6f70 2220  r" valign="top" 
+00001cc0: 7769 6474 683d 2231 342e 3238 2522 3e3c  width="14.28%"><
+00001cd0: 6120 6872 6566 3d22 6874 7470 3a2f 2f66  a href="http://f
+00001ce0: 6162 6961 6e2d 6166 666f 6c74 6572 2e63  abian-affolter.c
+00001cf0: 682f 626c 6f67 2f22 3e3c 696d 6720 7372  h/blog/"><img sr
+00001d00: 633d 2268 7474 7073 3a2f 2f61 7661 7461  c="https://avata
+00001d10: 7273 2e67 6974 6875 6275 7365 7263 6f6e  rs.githubusercon
+00001d20: 7465 6e74 2e63 6f6d 2f75 2f31 3136 3138  tent.com/u/11618
+00001d30: 343f 763d 343f 733d 3130 3022 2077 6964  4?v=4?s=100" wid
+00001d40: 7468 3d22 3130 3070 783b 2220 616c 743d  th="100px;" alt=
+00001d50: 2246 6162 6961 6e20 4166 666f 6c74 6572  "Fabian Affolter
+00001d60: 222f 3e3c 6272 202f 3e3c 7375 623e 3c62  "/><br /><sub><b
+00001d70: 3e46 6162 6961 6e20 4166 666f 6c74 6572  >Fabian Affolter
+00001d80: 3c2f 623e 3c2f 7375 623e 3c2f 613e 3c62  </b></sub></a><b
+00001d90: 7220 2f3e 3c61 2068 7265 663d 2268 7474  r /><a href="htt
+00001da0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001db0: 546f 6d65 7246 692f 6169 6f73 7769 7463  TomerFi/aioswitc
+00001dc0: 6865 722f 636f 6d6d 6974 733f 6175 7468  her/commits?auth
+00001dd0: 6f72 3d66 6162 6166 6622 2074 6974 6c65  or=fabaff" title
 00001de0: 3d22 436f 6465 223e f09f 92bb 3c2f 613e  ="Code">....</a>
-00001df0: 3c2f 7464 3e5c 6e20 2020 2020 203c 7464  </td>\n      <td
-00001e00: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00001e10: 3c61 2068 7265 663d 2268 7474 703a 2f2f  <a href="http://
-00001e20: 6578 706c 6f69 742e 636f 2e69 6c22 3e3c  exploit.co.il"><
-00001e30: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00001e40: 2f61 7661 7461 7273 2e67 6974 6875 6275  /avatars.githubu
-00001e50: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f75  sercontent.com/u
-00001e60: 2f31 3736 3839 3135 3f76 3d34 3f73 3d31  /1768915?v=4?s=1
-00001e70: 3030 2220 7769 6474 683d 2231 3030 7078  00" width="100px
-00001e80: 3b22 2061 6c74 3d22 5368 6169 2072 6f64  ;" alt="Shai rod
-00001e90: 222f 3e3c 6272 202f 3e3c 7375 623e 3c62  "/><br /><sub><b
-00001ea0: 3e53 6861 6920 726f 643c 2f62 3e3c 2f73  >Shai rod</b></s
-00001eb0: 7562 3e3c 2f61 3e3c 6272 202f 3e3c 6120  ub></a><br /><a 
-00001ec0: 6872 6566 3d22 2364 6174 612d 6e69 6768  href="#data-nigh
-00001ed0: 7472 616e 6733 7222 2074 6974 6c65 3d22  trang3r" title="
-00001ee0: 4461 7461 223e f09f 94a3 3c2f 613e 3c2f  Data">....</a></
-00001ef0: 7464 3e5c 6e20 2020 203c 2f74 723e 5c6e  td>\n    </tr>\n
-00001f00: 2020 2020 3c74 723e 5c6e 2020 2020 2020      <tr>\n      
-00001f10: 3c74 6420 616c 6967 6e3d 2263 656e 7465  <td align="cente
-00001f20: 7222 3e3c 6120 6872 6566 3d22 6874 7470  r"><a href="http
-00001f30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00001f40: 6865 636f 6465 223e 3c69 6d67 2073 7263  hecode"><img src
-00001f50: 3d22 6874 7470 733a 2f2f 6176 6174 6172  ="https://avatar
-00001f60: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
-00001f70: 656e 742e 636f 6d2f 752f 3138 3538 3932  ent.com/u/185892
-00001f80: 353f 763d 343f 733d 3130 3022 2077 6964  5?v=4?s=100" wid
-00001f90: 7468 3d22 3130 3070 783b 2220 616c 743d  th="100px;" alt=
-00001fa0: 2253 6861 7920 4c65 7679 222f 3e3c 6272  "Shay Levy"/><br
-00001fb0: 202f 3e3c 7375 623e 3c62 3e53 6861 7920   /><sub><b>Shay 
-00001fc0: 4c65 7679 3c2f 623e 3c2f 7375 623e 3c2f  Levy</b></sub></
-00001fd0: 613e 3c62 7220 2f3e 3c61 2068 7265 663d  a><br /><a href=
-00001fe0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001ff0: 636f 6d2f 546f 6d65 7246 692f 6169 6f73  com/TomerFi/aios
-00002000: 7769 7463 6865 722f 636f 6d6d 6974 733f  witcher/commits?
-00002010: 6175 7468 6f72 3d74 6865 636f 6465 2220  author=thecode" 
-00002020: 7469 746c 653d 2243 6f64 6522 3ef0 9f92  title="Code">...
-00002030: bb3c 2f61 3e20 3c61 2068 7265 663d 2223  .</a> <a href="#
-00002040: 6964 6561 732d 7468 6563 6f64 6522 2074  ideas-thecode" t
-00002050: 6974 6c65 3d22 4964 6561 732c 2050 6c61  itle="Ideas, Pla
-00002060: 6e6e 696e 672c 2026 2046 6565 6462 6163  nning, & Feedbac
-00002070: 6b22 3ef0 9fa4 943c 2f61 3e20 3c61 2068  k">....</a> <a h
-00002080: 7265 663d 2223 6d61 696e 7465 6e61 6e63  ref="#maintenanc
-00002090: 652d 7468 6563 6f64 6522 2074 6974 6c65  e-thecode" title
-000020a0: 3d22 4d61 696e 7465 6e61 6e63 6522 3ef0  ="Maintenance">.
-000020b0: 9f9a a73c 2f61 3e3c 2f74 643e 5c6e 2020  ...</a></td>\n  
-000020c0: 2020 2020 3c74 6420 616c 6967 6e3d 2263      <td align="c
-000020d0: 656e 7465 7222 3e3c 6120 6872 6566 3d22  enter"><a href="
-000020e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000020f0: 6f6d 2f64 6d61 7469 6b22 3e3c 696d 6720  om/dmatik"><img 
-00002100: 7372 633d 2268 7474 7073 3a2f 2f61 7661  src="https://ava
-00002110: 7461 7273 2e67 6974 6875 6275 7365 7263  tars.githubuserc
-00002120: 6f6e 7465 6e74 2e63 6f6d 2f75 2f35 3537  ontent.com/u/557
-00002130: 3733 3836 3f76 3d34 3f73 3d31 3030 2220  7386?v=4?s=100" 
-00002140: 7769 6474 683d 2231 3030 7078 3b22 2061  width="100px;" a
-00002150: 6c74 3d22 646d 6174 696b 222f 3e3c 6272  lt="dmatik"/><br
-00002160: 202f 3e3c 7375 623e 3c62 3e64 6d61 7469   /><sub><b>dmati
-00002170: 6b3c 2f62 3e3c 2f73 7562 3e3c 2f61 3e3c  k</b></sub></a><
-00002180: 6272 202f 3e3c 6120 6872 6566 3d22 2362  br /><a href="#b
-00002190: 6c6f 672d 646d 6174 696b 2220 7469 746c  log-dmatik" titl
-000021a0: 653d 2242 6c6f 6770 6f73 7473 223e f09f  e="Blogposts">..
-000021b0: 939d 3c2f 613e 203c 6120 6872 6566 3d22  ..</a> <a href="
-000021c0: 2369 6465 6173 2d64 6d61 7469 6b22 2074  #ideas-dmatik" t
-000021d0: 6974 6c65 3d22 4964 6561 732c 2050 6c61  itle="Ideas, Pla
-000021e0: 6e6e 696e 672c 2026 2046 6565 6462 6163  nning, & Feedbac
-000021f0: 6b22 3ef0 9fa4 943c 2f61 3e20 3c61 2068  k">....</a> <a h
-00002200: 7265 663d 2223 7573 6572 5465 7374 696e  ref="#userTestin
-00002210: 672d 646d 6174 696b 2220 7469 746c 653d  g-dmatik" title=
-00002220: 2255 7365 7220 5465 7374 696e 6722 3ef0  "User Testing">.
-00002230: 9f93 933c 2f61 3e3c 2f74 643e 5c6e 2020  ...</a></td>\n  
-00002240: 2020 2020 3c74 6420 616c 6967 6e3d 2263      <td align="c
-00002250: 656e 7465 7222 3e3c 6120 6872 6566 3d22  enter"><a href="
-00002260: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002270: 6f6d 2f6a 6166 6172 2d61 7469 6c69 223e  om/jafar-atili">
-00002280: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00002290: 2f2f 6176 6174 6172 732e 6769 7468 7562  //avatars.github
-000022a0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-000022b0: 752f 3139 3530 3837 3837 3f76 3d34 3f73  u/19508787?v=4?s
-000022c0: 3d31 3030 2220 7769 6474 683d 2231 3030  =100" width="100
-000022d0: 7078 3b22 2061 6c74 3d22 6a61 6661 722d  px;" alt="jafar-
-000022e0: 6174 696c 6922 2f3e 3c62 7220 2f3e 3c73  atili"/><br /><s
-000022f0: 7562 3e3c 623e 6a61 6661 722d 6174 696c  ub><b>jafar-atil
-00002300: 693c 2f62 3e3c 2f73 7562 3e3c 2f61 3e3c  i</b></sub></a><
-00002310: 6272 202f 3e3c 6120 6872 6566 3d22 6874  br /><a href="ht
-00002320: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002330: 2f54 6f6d 6572 4669 2f61 696f 7377 6974  /TomerFi/aioswit
-00002340: 6368 6572 2f63 6f6d 6d69 7473 3f61 7574  cher/commits?aut
-00002350: 686f 723d 6a61 6661 722d 6174 696c 6922  hor=jafar-atili"
-00002360: 2074 6974 6c65 3d22 436f 6465 223e f09f   title="Code">..
-00002370: 92bb 3c2f 613e 203c 6120 6872 6566 3d22  ..</a> <a href="
-00002380: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002390: 6f6d 2f54 6f6d 6572 4669 2f61 696f 7377  om/TomerFi/aiosw
-000023a0: 6974 6368 6572 2f63 6f6d 6d69 7473 3f61  itcher/commits?a
-000023b0: 7574 686f 723d 6a61 6661 722d 6174 696c  uthor=jafar-atil
-000023c0: 6922 2074 6974 6c65 3d22 446f 6375 6d65  i" title="Docume
-000023d0: 6e74 6174 696f 6e22 3ef0 9f93 963c 2f61  ntation">....</a
-000023e0: 3e3c 2f74 643e 5c6e 2020 2020 3c2f 7472  ></td>\n    </tr
-000023f0: 3e5c 6e20 203c 2f74 626f 6479 3e5c 6e3c  >\n  </tbody>\n<
-00002400: 2f74 6162 6c65 3e5c 6e5c 6e3c 212d 2d20  /table>\n\n<!-- 
-00002410: 6d61 726b 646f 776e 6c69 6e74 2d72 6573  markdownlint-res
-00002420: 746f 7265 202d 2d3e 5c6e 3c21 2d2d 2070  tore -->\n<!-- p
-00002430: 7265 7474 6965 722d 6967 6e6f 7265 2d65  rettier-ignore-e
-00002440: 6e64 202d 2d3e 5c6e 5c6e 3c21 2d2d 2041  nd -->\n\n<!-- A
-00002450: 4c4c 2d43 4f4e 5452 4942 5554 4f52 532d  LL-CONTRIBUTORS-
-00002460: 4c49 5354 3a45 4e44 202d 2d3e 5c6e 5c6e  LIST:END -->\n\n
-00002470: 3c21 2d2d 2052 6561 6c20 4c69 6e6b 7320  <!-- Real Links 
-00002480: 2d2d 3e5c 6e5b 305d 3a20 6874 7470 733a  -->\n[0]: https:
-00002490: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f6d  //github.com/Tom
-000024a0: 6572 4669 2f61 696f 7377 6974 6368 6572  erFi/aioswitcher
-000024b0: 2f77 696b 695c 6e5b 315d 3a20 6874 7470  /wiki\n[1]: http
-000024c0: 733a 2f2f 616c 6c63 6f6e 7472 6962 7574  s://allcontribut
-000024d0: 6f72 732e 6f72 672f 646f 6373 2f65 6e2f  ors.org/docs/en/
-000024e0: 656d 6f6a 692d 6b65 795c 6e5b 335d 3a20  emoji-key\n[3]: 
-000024f0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
-00002500: 696f 2f67 682f 546f 6d65 7246 692f 6169  io/gh/TomerFi/ai
-00002510: 6f73 7769 7463 6865 725c 6e5b 345d 3a20  oswitcher\n[4]: 
-00002520: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002530: 6f6d 2f54 6f6d 6572 4669 2f61 696f 7377  om/TomerFi/aiosw
-00002540: 6974 6368 6572 5c6e 5b37 5d3a 2068 7474  itcher\n[7]: htt
+00001df0: 3c2f 7464 3e0a 2020 2020 2020 3c74 6420  </td>.      <td 
+00001e00: 616c 6967 6e3d 2263 656e 7465 7222 2076  align="center" v
+00001e10: 616c 6967 6e3d 2274 6f70 2220 7769 6474  align="top" widt
+00001e20: 683d 2231 342e 3238 2522 3e3c 6120 6872  h="14.28%"><a hr
+00001e30: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00001e40: 7562 2e63 6f6d 2f6f 7261 6e6a 6122 3e3c  ub.com/oranja"><
+00001e50: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001e60: 2f61 7661 7461 7273 2e67 6974 6875 6275  /avatars.githubu
+00001e70: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f75  sercontent.com/u
+00001e80: 2f36 3739 3138 343f 763d 343f 733d 3130  /679184?v=4?s=10
+00001e90: 3022 2077 6964 7468 3d22 3130 3070 783b  0" width="100px;
+00001ea0: 2220 616c 743d 2249 747a 696b 2045 7068  " alt="Itzik Eph
+00001eb0: 7261 696d 222f 3e3c 6272 202f 3e3c 7375  raim"/><br /><su
+00001ec0: 623e 3c62 3e49 747a 696b 2045 7068 7261  b><b>Itzik Ephra
+00001ed0: 696d 3c2f 623e 3c2f 7375 623e 3c2f 613e  im</b></sub></a>
+00001ee0: 3c62 7220 2f3e 3c61 2068 7265 663d 2268  <br /><a href="h
+00001ef0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001f00: 6d2f 546f 6d65 7246 692f 6169 6f73 7769  m/TomerFi/aioswi
+00001f10: 7463 6865 722f 636f 6d6d 6974 733f 6175  tcher/commits?au
+00001f20: 7468 6f72 3d6f 7261 6e6a 6122 2074 6974  thor=oranja" tit
+00001f30: 6c65 3d22 436f 6465 223e f09f 92bb 3c2f  le="Code">....</
+00001f40: 613e 3c2f 7464 3e0a 2020 2020 2020 3c74  a></td>.      <t
+00001f50: 6420 616c 6967 6e3d 2263 656e 7465 7222  d align="center"
+00001f60: 2076 616c 6967 6e3d 2274 6f70 2220 7769   valign="top" wi
+00001f70: 6474 683d 2231 342e 3238 2522 3e3c 6120  dth="14.28%"><a 
+00001f80: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001f90: 7468 7562 2e63 6f6d 2f4b 6573 6176 3839  thub.com/Kesav89
+00001fa0: 3022 3e3c 696d 6720 7372 633d 2268 7474  0"><img src="htt
+00001fb0: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
+00001fc0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00001fd0: 6f6d 2f75 2f38 3235 3539 3935 313f 763d  om/u/82559951?v=
+00001fe0: 343f 733d 3130 3022 2077 6964 7468 3d22  4?s=100" width="
+00001ff0: 3130 3070 783b 2220 616c 743d 224b 6573  100px;" alt="Kes
+00002000: 6176 3839 3022 2f3e 3c62 7220 2f3e 3c73  av890"/><br /><s
+00002010: 7562 3e3c 623e 4b65 7361 7638 3930 3c2f  ub><b>Kesav890</
+00002020: 623e 3c2f 7375 623e 3c2f 613e 3c62 7220  b></sub></a><br 
+00002030: 2f3e 3c61 2068 7265 663d 2268 7474 7073  /><a href="https
+00002040: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
+00002050: 6d65 7246 692f 6169 6f73 7769 7463 6865  merFi/aioswitche
+00002060: 722f 636f 6d6d 6974 733f 6175 7468 6f72  r/commits?author
+00002070: 3d4b 6573 6176 3839 3022 2074 6974 6c65  =Kesav890" title
+00002080: 3d22 446f 6375 6d65 6e74 6174 696f 6e22  ="Documentation"
+00002090: 3ef0 9f93 963c 2f61 3e3c 2f74 643e 0a20  >....</a></td>. 
+000020a0: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
+000020b0: 6365 6e74 6572 2220 7661 6c69 676e 3d22  center" valign="
+000020c0: 746f 7022 2077 6964 7468 3d22 3134 2e32  top" width="14.2
+000020d0: 3825 223e 3c61 2068 7265 663d 2268 7474  8%"><a href="htt
+000020e0: 703a 2f2f 6c69 6164 2e61 7672 6168 2e61  p://liad.avrah.a
+000020f0: 6d22 3e3c 696d 6720 7372 633d 2268 7474  m"><img src="htt
+00002100: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
+00002110: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00002120: 6f6d 2f75 2f37 3236 3332 3233 3f76 3d34  om/u/7263223?v=4
+00002130: 3f73 3d31 3030 2220 7769 6474 683d 2231  ?s=100" width="1
+00002140: 3030 7078 3b22 2061 6c74 3d22 4c69 6164  00px;" alt="Liad
+00002150: 2041 7672 6168 616d 222f 3e3c 6272 202f   Avraham"/><br /
+00002160: 3e3c 7375 623e 3c62 3e4c 6961 6420 4176  ><sub><b>Liad Av
+00002170: 7261 6861 6d3c 2f62 3e3c 2f73 7562 3e3c  raham</b></sub><
+00002180: 2f61 3e3c 6272 202f 3e3c 6120 6872 6566  /a><br /><a href
+00002190: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000021a0: 2e63 6f6d 2f54 6f6d 6572 4669 2f61 696f  .com/TomerFi/aio
+000021b0: 7377 6974 6368 6572 2f63 6f6d 6d69 7473  switcher/commits
+000021c0: 3f61 7574 686f 723d 6c69 6164 6176 2220  ?author=liadav" 
+000021d0: 7469 746c 653d 2243 6f64 6522 3ef0 9f92  title="Code">...
+000021e0: bb3c 2f61 3e3c 2f74 643e 0a20 2020 2020  .</a></td>.     
+000021f0: 203c 7464 2061 6c69 676e 3d22 6365 6e74   <td align="cent
+00002200: 6572 2220 7661 6c69 676e 3d22 746f 7022  er" valign="top"
+00002210: 2077 6964 7468 3d22 3134 2e32 3825 223e   width="14.28%">
+00002220: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00002230: 2f67 6974 6875 622e 636f 6d2f 4f72 4269  /github.com/OrBi
+00002240: 6e22 3e3c 696d 6720 7372 633d 2268 7474  n"><img src="htt
+00002250: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
+00002260: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00002270: 6f6d 2f75 2f36 3839 3732 3334 3f76 3d34  om/u/6897234?v=4
+00002280: 3f73 3d31 3030 2220 7769 6474 683d 2231  ?s=100" width="1
+00002290: 3030 7078 3b22 2061 6c74 3d22 4f72 2042  00px;" alt="Or B
+000022a0: 696e 222f 3e3c 6272 202f 3e3c 7375 623e  in"/><br /><sub>
+000022b0: 3c62 3e4f 7220 4269 6e3c 2f62 3e3c 2f73  <b>Or Bin</b></s
+000022c0: 7562 3e3c 2f61 3e3c 6272 202f 3e3c 6120  ub></a><br /><a 
+000022d0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000022e0: 7468 7562 2e63 6f6d 2f54 6f6d 6572 4669  thub.com/TomerFi
+000022f0: 2f61 696f 7377 6974 6368 6572 2f63 6f6d  /aioswitcher/com
+00002300: 6d69 7473 3f61 7574 686f 723d 4f72 4269  mits?author=OrBi
+00002310: 6e22 2074 6974 6c65 3d22 436f 6465 223e  n" title="Code">
+00002320: f09f 92bb 3c2f 613e 3c2f 7464 3e0a 2020  ....</a></td>.  
+00002330: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+00002340: 0a20 2020 2020 203c 7464 2061 6c69 676e  .      <td align
+00002350: 3d22 6365 6e74 6572 2220 7661 6c69 676e  ="center" valign
+00002360: 3d22 746f 7022 2077 6964 7468 3d22 3134  ="top" width="14
+00002370: 2e32 3825 223e 3c61 2068 7265 663d 2268  .28%"><a href="h
+00002380: 7474 703a 2f2f 6578 706c 6f69 742e 636f  ttp://exploit.co
+00002390: 2e69 6c22 3e3c 696d 6720 7372 633d 2268  .il"><img src="h
+000023a0: 7474 7073 3a2f 2f61 7661 7461 7273 2e67  ttps://avatars.g
+000023b0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000023c0: 2e63 6f6d 2f75 2f31 3736 3839 3135 3f76  .com/u/1768915?v
+000023d0: 3d34 3f73 3d31 3030 2220 7769 6474 683d  =4?s=100" width=
+000023e0: 2231 3030 7078 3b22 2061 6c74 3d22 5368  "100px;" alt="Sh
+000023f0: 6169 2072 6f64 222f 3e3c 6272 202f 3e3c  ai rod"/><br /><
+00002400: 7375 623e 3c62 3e53 6861 6920 726f 643c  sub><b>Shai rod<
+00002410: 2f62 3e3c 2f73 7562 3e3c 2f61 3e3c 6272  /b></sub></a><br
+00002420: 202f 3e3c 6120 6872 6566 3d22 2364 6174   /><a href="#dat
+00002430: 612d 6e69 6768 7472 616e 6733 7222 2074  a-nightrang3r" t
+00002440: 6974 6c65 3d22 4461 7461 223e f09f 94a3  itle="Data">....
+00002450: 3c2f 613e 3c2f 7464 3e0a 2020 2020 2020  </a></td>.      
+00002460: 3c74 6420 616c 6967 6e3d 2263 656e 7465  <td align="cente
+00002470: 7222 2076 616c 6967 6e3d 2274 6f70 2220  r" valign="top" 
+00002480: 7769 6474 683d 2231 342e 3238 2522 3e3c  width="14.28%"><
+00002490: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000024a0: 6769 7468 7562 2e63 6f6d 2f74 6865 636f  github.com/theco
+000024b0: 6465 223e 3c69 6d67 2073 7263 3d22 6874  de"><img src="ht
+000024c0: 7470 733a 2f2f 6176 6174 6172 732e 6769  tps://avatars.gi
+000024d0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+000024e0: 636f 6d2f 752f 3138 3538 3932 353f 763d  com/u/1858925?v=
+000024f0: 343f 733d 3130 3022 2077 6964 7468 3d22  4?s=100" width="
+00002500: 3130 3070 783b 2220 616c 743d 2253 6861  100px;" alt="Sha
+00002510: 7920 4c65 7679 222f 3e3c 6272 202f 3e3c  y Levy"/><br /><
+00002520: 7375 623e 3c62 3e53 6861 7920 4c65 7679  sub><b>Shay Levy
+00002530: 3c2f 623e 3c2f 7375 623e 3c2f 613e 3c62  </b></sub></a><b
+00002540: 7220 2f3e 3c61 2068 7265 663d 2268 7474  r /><a href="htt
 00002550: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00002560: 546f 6d65 7246 692f 6169 6f73 7769 7463  TomerFi/aioswitc
-00002570: 6865 722f 6163 7469 6f6e 732f 776f 726b  her/actions/work
-00002580: 666c 6f77 732f 7374 6167 652e 796d 6c5c  flows/stage.yml\
-00002590: 6e5b 385d 3a20 6874 7470 733a 2f2f 6169  n[8]: https://ai
-000025a0: 6f73 7769 7463 6865 722e 746f 6d66 692e  oswitcher.tomfi.
-000025b0: 696e 666f 2f5c 6e5b 3131 5d3a 2068 7474  info/\n[11]: htt
-000025c0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000025d0: 6f6a 6563 742f 6169 6f73 7769 7463 6865  oject/aioswitche
-000025e0: 725c 6e5b 3132 5d3a 2068 7474 7073 3a2f  r\n[12]: https:/
-000025f0: 2f77 7777 2e73 7769 7463 6865 722e 636f  /www.switcher.co
-00002600: 2e69 6c2f 5c6e 3c21 2d2d 2042 6164 6765  .il/\n<!-- Badge
-00002610: 7320 4c69 6e6b 7320 2d2d 3e5c 6e5b 636f  s Links -->\n[co
-00002620: 6465 636f 765d 3a20 6874 7470 733a 2f2f  decov]: https://
-00002630: 636f 6465 636f 762e 696f 2f67 682f 546f  codecov.io/gh/To
-00002640: 6d65 7246 692f 6169 6f73 7769 7463 6865  merFi/aioswitche
-00002650: 722f 6772 6170 682f 6261 6467 652e 7376  r/graph/badge.sv
-00002660: 675c 6e5b 6768 2d62 7569 6c64 2d73 7461  g\n[gh-build-sta
-00002670: 7475 735d 3a20 6874 7470 733a 2f2f 6769  tus]: https://gi
-00002680: 7468 7562 2e63 6f6d 2f54 6f6d 6572 4669  thub.com/TomerFi
-00002690: 2f61 696f 7377 6974 6368 6572 2f61 6374  /aioswitcher/act
-000026a0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f73  ions/workflows/s
-000026b0: 7461 6765 2e79 6d6c 2f62 6164 6765 2e73  tage.yml/badge.s
-000026c0: 7667 5c6e 5b67 682d 7061 6765 732d 7374  vg\n[gh-pages-st
-000026d0: 6174 7573 5d3a 2068 7474 7073 3a2f 2f67  atus]: https://g
-000026e0: 6974 6875 622e 636f 6d2f 546f 6d65 7246  ithub.com/TomerF
-000026f0: 692f 6169 6f73 7769 7463 6865 722f 6163  i/aioswitcher/ac
-00002700: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00002710: 7061 6765 732e 796d 6c2f 6261 6467 652e  pages.yml/badge.
-00002720: 7376 675c 6e5b 6c69 6365 6e73 652d 6261  svg\n[license-ba
-00002730: 6467 655d 3a20 6874 7470 733a 2f2f 696d  dge]: https://im
-00002740: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00002750: 6875 622f 6c69 6365 6e73 652f 746f 6d65  hub/license/tome
-00002760: 7266 692f 6169 6f73 7769 7463 6865 725c  rfi/aioswitcher\
-00002770: 6e5b 7079 7069 2d64 6f77 6e6c 6f61 6473  n[pypi-downloads
-00002780: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-00002790: 6869 656c 6473 2e69 6f2f 7079 7069 2f64  hields.io/pypi/d
-000027a0: 6d2f 6169 6f73 7769 7463 6865 722e 7376  m/aioswitcher.sv
-000027b0: 673f 6c6f 676f 3d70 7970 6926 636f 6c6f  g?logo=pypi&colo
-000027c0: 723d 3130 3832 4332 5c6e 5b70 7970 692d  r=1082C2\n[pypi-
-000027d0: 7665 7273 696f 6e5d 3a20 6874 7470 733a  version]: https:
-000027e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000027f0: 2f70 7970 692f 762f 6169 6f73 7769 7463  /pypi/v/aioswitc
-00002800: 6865 723f 6c6f 676f 3d70 7970 695c 6e27  her?logo=pypi\n'
-00002810: 2c0a 2020 2020 2761 7574 686f 7227 3a20  ,.    'author': 
-00002820: 2754 6f6d 6572 2046 6967 656e 626c 6174  'Tomer Figenblat
-00002830: 272c 0a20 2020 2027 6175 7468 6f72 5f65  ',.    'author_e
-00002840: 6d61 696c 273a 2027 746f 6d65 7240 746f  mail': 'tomer@to
-00002850: 6d66 692e 696e 666f 272c 0a20 2020 2027  mfi.info',.    '
-00002860: 6d61 696e 7461 696e 6572 273a 2027 5368  maintainer': 'Sh
-00002870: 6179 204c 6576 7927 2c0a 2020 2020 276d  ay Levy',.    'm
-00002880: 6169 6e74 6169 6e65 725f 656d 6169 6c27  aintainer_email'
-00002890: 3a20 274e 6f6e 6527 2c0a 2020 2020 2775  : 'None',.    'u
-000028a0: 726c 273a 2027 6874 7470 733a 2f2f 7079  rl': 'https://py
-000028b0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f61  pi.org/project/a
-000028c0: 696f 7377 6974 6368 6572 2f27 2c0a 2020  ioswitcher/',.  
-000028d0: 2020 2770 6163 6b61 6765 5f64 6972 273a    'package_dir':
-000028e0: 2070 6163 6b61 6765 5f64 6972 2c0a 2020   package_dir,.  
-000028f0: 2020 2770 6163 6b61 6765 7327 3a20 7061    'packages': pa
-00002900: 636b 6167 6573 2c0a 2020 2020 2770 6163  ckages,.    'pac
-00002910: 6b61 6765 5f64 6174 6127 3a20 7061 636b  kage_data': pack
-00002920: 6167 655f 6461 7461 2c0a 2020 2020 2770  age_data,.    'p
-00002930: 7974 686f 6e5f 7265 7175 6972 6573 273a  ython_requires':
-00002940: 2027 3e3d 332e 392e 302c 3c34 2e30 2e30   '>=3.9.0,<4.0.0
-00002950: 272c 0a7d 0a0a 0a73 6574 7570 282a 2a73  ',.}...setup(**s
-00002960: 6574 7570 5f6b 7761 7267 7329 0a         etup_kwargs).
+00002570: 6865 722f 636f 6d6d 6974 733f 6175 7468  her/commits?auth
+00002580: 6f72 3d74 6865 636f 6465 2220 7469 746c  or=thecode" titl
+00002590: 653d 2243 6f64 6522 3ef0 9f92 bb3c 2f61  e="Code">....</a
+000025a0: 3e20 3c61 2068 7265 663d 2223 6964 6561  > <a href="#idea
+000025b0: 732d 7468 6563 6f64 6522 2074 6974 6c65  s-thecode" title
+000025c0: 3d22 4964 6561 732c 2050 6c61 6e6e 696e  ="Ideas, Plannin
+000025d0: 672c 2026 2046 6565 6462 6163 6b22 3ef0  g, & Feedback">.
+000025e0: 9fa4 943c 2f61 3e20 3c61 2068 7265 663d  ...</a> <a href=
+000025f0: 2223 6d61 696e 7465 6e61 6e63 652d 7468  "#maintenance-th
+00002600: 6563 6f64 6522 2074 6974 6c65 3d22 4d61  ecode" title="Ma
+00002610: 696e 7465 6e61 6e63 6522 3ef0 9f9a a73c  intenance">....<
+00002620: 2f61 3e3c 2f74 643e 0a20 2020 2020 203c  /a></td>.      <
+00002630: 7464 2061 6c69 676e 3d22 6365 6e74 6572  td align="center
+00002640: 2220 7661 6c69 676e 3d22 746f 7022 2077  " valign="top" w
+00002650: 6964 7468 3d22 3134 2e32 3825 223e 3c61  idth="14.28%"><a
+00002660: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00002670: 6974 6875 622e 636f 6d2f 646d 6174 696b  ithub.com/dmatik
+00002680: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00002690: 733a 2f2f 6176 6174 6172 732e 6769 7468  s://avatars.gith
+000026a0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000026b0: 6d2f 752f 3535 3737 3338 363f 763d 343f  m/u/5577386?v=4?
+000026c0: 733d 3130 3022 2077 6964 7468 3d22 3130  s=100" width="10
+000026d0: 3070 783b 2220 616c 743d 2264 6d61 7469  0px;" alt="dmati
+000026e0: 6b22 2f3e 3c62 7220 2f3e 3c73 7562 3e3c  k"/><br /><sub><
+000026f0: 623e 646d 6174 696b 3c2f 623e 3c2f 7375  b>dmatik</b></su
+00002700: 623e 3c2f 613e 3c62 7220 2f3e 3c61 2068  b></a><br /><a h
+00002710: 7265 663d 2223 626c 6f67 2d64 6d61 7469  ref="#blog-dmati
+00002720: 6b22 2074 6974 6c65 3d22 426c 6f67 706f  k" title="Blogpo
+00002730: 7374 7322 3ef0 9f93 9d3c 2f61 3e20 3c61  sts">....</a> <a
+00002740: 2068 7265 663d 2223 6964 6561 732d 646d   href="#ideas-dm
+00002750: 6174 696b 2220 7469 746c 653d 2249 6465  atik" title="Ide
+00002760: 6173 2c20 506c 616e 6e69 6e67 2c20 2620  as, Planning, & 
+00002770: 4665 6564 6261 636b 223e f09f a494 3c2f  Feedback">....</
+00002780: 613e 203c 6120 6872 6566 3d22 2375 7365  a> <a href="#use
+00002790: 7254 6573 7469 6e67 2d64 6d61 7469 6b22  rTesting-dmatik"
+000027a0: 2074 6974 6c65 3d22 5573 6572 2054 6573   title="User Tes
+000027b0: 7469 6e67 223e f09f 9393 3c2f 613e 3c2f  ting">....</a></
+000027c0: 7464 3e0a 2020 2020 2020 3c74 6420 616c  td>.      <td al
+000027d0: 6967 6e3d 2263 656e 7465 7222 2076 616c  ign="center" val
+000027e0: 6967 6e3d 2274 6f70 2220 7769 6474 683d  ign="top" width=
+000027f0: 2231 342e 3238 2522 3e3c 6120 6872 6566  "14.28%"><a href
+00002800: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00002810: 2e63 6f6d 2f6a 6166 6172 2d61 7469 6c69  .com/jafar-atili
+00002820: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00002830: 733a 2f2f 6176 6174 6172 732e 6769 7468  s://avatars.gith
+00002840: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00002850: 6d2f 752f 3139 3530 3837 3837 3f76 3d34  m/u/19508787?v=4
+00002860: 3f73 3d31 3030 2220 7769 6474 683d 2231  ?s=100" width="1
+00002870: 3030 7078 3b22 2061 6c74 3d22 6a61 6661  00px;" alt="jafa
+00002880: 722d 6174 696c 6922 2f3e 3c62 7220 2f3e  r-atili"/><br />
+00002890: 3c73 7562 3e3c 623e 6a61 6661 722d 6174  <sub><b>jafar-at
+000028a0: 696c 693c 2f62 3e3c 2f73 7562 3e3c 2f61  ili</b></sub></a
+000028b0: 3e3c 6272 202f 3e3c 6120 6872 6566 3d22  ><br /><a href="
+000028c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000028d0: 6f6d 2f54 6f6d 6572 4669 2f61 696f 7377  om/TomerFi/aiosw
+000028e0: 6974 6368 6572 2f63 6f6d 6d69 7473 3f61  itcher/commits?a
+000028f0: 7574 686f 723d 6a61 6661 722d 6174 696c  uthor=jafar-atil
+00002900: 6922 2074 6974 6c65 3d22 436f 6465 223e  i" title="Code">
+00002910: f09f 92bb 3c2f 613e 203c 6120 6872 6566  ....</a> <a href
+00002920: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00002930: 2e63 6f6d 2f54 6f6d 6572 4669 2f61 696f  .com/TomerFi/aio
+00002940: 7377 6974 6368 6572 2f63 6f6d 6d69 7473  switcher/commits
+00002950: 3f61 7574 686f 723d 6a61 6661 722d 6174  ?author=jafar-at
+00002960: 696c 6922 2074 6974 6c65 3d22 446f 6375  ili" title="Docu
+00002970: 6d65 6e74 6174 696f 6e22 3ef0 9f93 963c  mentation">....<
+00002980: 2f61 3e3c 2f74 643e 0a20 2020 203c 2f74  /a></td>.    </t
+00002990: 723e 0a20 203c 2f74 626f 6479 3e0a 3c2f  r>.  </tbody>.</
+000029a0: 7461 626c 653e 0a0a 3c21 2d2d 206d 6172  table>..<!-- mar
+000029b0: 6b64 6f77 6e6c 696e 742d 7265 7374 6f72  kdownlint-restor
+000029c0: 6520 2d2d 3e0a 3c21 2d2d 2070 7265 7474  e -->.<!-- prett
+000029d0: 6965 722d 6967 6e6f 7265 2d65 6e64 202d  ier-ignore-end -
+000029e0: 2d3e 0a0a 3c21 2d2d 2041 4c4c 2d43 4f4e  ->..<!-- ALL-CON
+000029f0: 5452 4942 5554 4f52 532d 4c49 5354 3a45  TRIBUTORS-LIST:E
+00002a00: 4e44 202d 2d3e 0a0a 3c21 2d2d 2052 6561  ND -->..<!-- Rea
+00002a10: 6c20 4c69 6e6b 7320 2d2d 3e0a 5b30 5d3a  l Links -->.[0]:
+00002a20: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00002a30: 636f 6d2f 546f 6d65 7246 692f 6169 6f73  com/TomerFi/aios
+00002a40: 7769 7463 6865 722f 7769 6b69 0a5b 315d  witcher/wiki.[1]
+00002a50: 3a20 6874 7470 733a 2f2f 616c 6c63 6f6e  : https://allcon
+00002a60: 7472 6962 7574 6f72 732e 6f72 672f 646f  tributors.org/do
+00002a70: 6373 2f65 6e2f 656d 6f6a 692d 6b65 790a  cs/en/emoji-key.
+00002a80: 5b33 5d3a 2068 7474 7073 3a2f 2f63 6f64  [3]: https://cod
+00002a90: 6563 6f76 2e69 6f2f 6768 2f54 6f6d 6572  ecov.io/gh/Tomer
+00002aa0: 4669 2f61 696f 7377 6974 6368 6572 0a5b  Fi/aioswitcher.[
+00002ab0: 345d 3a20 6874 7470 733a 2f2f 6769 7468  4]: https://gith
+00002ac0: 7562 2e63 6f6d 2f54 6f6d 6572 4669 2f61  ub.com/TomerFi/a
+00002ad0: 696f 7377 6974 6368 6572 0a5b 375d 3a20  ioswitcher.[7]: 
+00002ae0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002af0: 6f6d 2f54 6f6d 6572 4669 2f61 696f 7377  om/TomerFi/aiosw
+00002b00: 6974 6368 6572 2f61 6374 696f 6e73 2f77  itcher/actions/w
+00002b10: 6f72 6b66 6c6f 7773 2f73 7461 6765 2e79  orkflows/stage.y
+00002b20: 6d6c 0a5b 385d 3a20 6874 7470 733a 2f2f  ml.[8]: https://
+00002b30: 6169 6f73 7769 7463 6865 722e 746f 6d66  aioswitcher.tomf
+00002b40: 692e 696e 666f 2f0a 5b31 315d 3a20 6874  i.info/.[11]: ht
+00002b50: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00002b60: 726f 6a65 6374 2f61 696f 7377 6974 6368  roject/aioswitch
+00002b70: 6572 0a5b 3132 5d3a 2068 7474 7073 3a2f  er.[12]: https:/
+00002b80: 2f77 7777 2e73 7769 7463 6865 722e 636f  /www.switcher.co
+00002b90: 2e69 6c2f 0a3c 212d 2d20 4261 6467 6573  .il/.<!-- Badges
+00002ba0: 204c 696e 6b73 202d 2d3e 0a5b 636f 6465   Links -->.[code
+00002bb0: 636f 765d 3a20 6874 7470 733a 2f2f 636f  cov]: https://co
+00002bc0: 6465 636f 762e 696f 2f67 682f 546f 6d65  decov.io/gh/Tome
+00002bd0: 7246 692f 6169 6f73 7769 7463 6865 722f  rFi/aioswitcher/
+00002be0: 6772 6170 682f 6261 6467 652e 7376 670a  graph/badge.svg.
+00002bf0: 5b67 682d 6275 696c 642d 7374 6174 7573  [gh-build-status
+00002c00: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
+00002c10: 622e 636f 6d2f 546f 6d65 7246 692f 6169  b.com/TomerFi/ai
+00002c20: 6f73 7769 7463 6865 722f 6163 7469 6f6e  oswitcher/action
+00002c30: 732f 776f 726b 666c 6f77 732f 7374 6167  s/workflows/stag
+00002c40: 652e 796d 6c2f 6261 6467 652e 7376 670a  e.yml/badge.svg.
+00002c50: 5b67 682d 7061 6765 732d 7374 6174 7573  [gh-pages-status
+00002c60: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
+00002c70: 622e 636f 6d2f 546f 6d65 7246 692f 6169  b.com/TomerFi/ai
+00002c80: 6f73 7769 7463 6865 722f 6163 7469 6f6e  oswitcher/action
+00002c90: 732f 776f 726b 666c 6f77 732f 7061 6765  s/workflows/page
+00002ca0: 732e 796d 6c2f 6261 6467 652e 7376 670a  s.yml/badge.svg.
+00002cb0: 5b6c 6963 656e 7365 2d62 6164 6765 5d3a  [license-badge]:
+00002cc0: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+00002cd0: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+00002ce0: 6963 656e 7365 2f74 6f6d 6572 6669 2f61  icense/tomerfi/a
+00002cf0: 696f 7377 6974 6368 6572 0a5b 7079 7069  ioswitcher.[pypi
+00002d00: 2d64 6f77 6e6c 6f61 6473 5d3a 2068 7474  -downloads]: htt
+00002d10: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00002d20: 2e69 6f2f 7079 7069 2f64 6d2f 6169 6f73  .io/pypi/dm/aios
+00002d30: 7769 7463 6865 722e 7376 673f 6c6f 676f  witcher.svg?logo
+00002d40: 3d70 7970 6926 636f 6c6f 723d 3130 3832  =pypi&color=1082
+00002d50: 4332 0a5b 7079 7069 2d76 6572 7369 6f6e  C2.[pypi-version
+00002d60: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
+00002d70: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00002d80: 2f61 696f 7377 6974 6368 6572 3f6c 6f67  /aioswitcher?log
+00002d90: 6f3d 7079 7069 0a0a                      o=pypi..
```


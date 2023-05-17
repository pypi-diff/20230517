# Comparing `tmp/aioswitcher-3.3.0.tar.gz` & `tmp/aioswitcher-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioswitcher-3.3.0.tar", max compression
+gzip compressed data, was "aioswitcher-3.4.0.tar", max compression
```

## Comparing `aioswitcher-3.3.0.tar` & `aioswitcher-3.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-04-10 18:44:09.095507 aioswitcher-3.3.0/LICENSE
--rw-r--r--   0        0        0    10703 2023-04-10 18:44:09.095507 aioswitcher-3.3.0/README.md
--rw-r--r--   0        0        0        0 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/py.typed
--rw-r--r--   0        0        0     3198 2023-04-10 18:44:34.064273 aioswitcher-3.3.0/pyproject.toml
--rwxr-xr-x   0        0        0      818 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/__init__.py
--rw-r--r--   0        0        0    27808 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/api/__init__.py
--rw-r--r--   0        0        0     9461 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/api/messages.py
--rw-r--r--   0        0        0     3924 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/api/packets.py
--rw-r--r--   0        0        0    15903 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/api/remotes.py
--rw-r--r--   0        0        0    16048 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/bridge.py
--rw-r--r--   0        0        0    11461 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/device/__init__.py
--rw-r--r--   0        0        0     4320 2023-04-10 18:44:09.099507 aioswitcher-3.3.0/src/aioswitcher/device/tools.py
--rw-r--r--   0        0        0 12418831 2023-04-10 18:44:09.131508 aioswitcher-3.3.0/src/aioswitcher/resources/irset_db.json
--rw-r--r--   0        0        0     2054 2023-04-10 18:44:09.131508 aioswitcher-3.3.0/src/aioswitcher/schedule/__init__.py
--rw-r--r--   0        0        0     4047 2023-04-10 18:44:09.131508 aioswitcher-3.3.0/src/aioswitcher/schedule/parser.py
--rw-r--r--   0        0        0     5683 2023-04-10 18:44:09.131508 aioswitcher-3.3.0/src/aioswitcher/schedule/tools.py
--rw-r--r--   0        0        0    11672 1970-01-01 00:00:00.000000 aioswitcher-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 13:27:59.720365 aioswitcher-3.4.0/LICENSE
+-rw-r--r--   0        0        0    10993 2023-05-17 13:27:59.720365 aioswitcher-3.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 13:27:59.720365 aioswitcher-3.4.0/py.typed
+-rw-r--r--   0        0        0     3177 2023-05-17 13:28:16.216476 aioswitcher-3.4.0/pyproject.toml
+-rwxr-xr-x   0        0        0      818 2023-05-17 13:27:59.724365 aioswitcher-3.4.0/src/aioswitcher/__init__.py
+-rw-r--r--   0        0        0    27808 2023-05-17 13:27:59.724365 aioswitcher-3.4.0/src/aioswitcher/api/__init__.py
+-rw-r--r--   0        0        0     9461 2023-05-17 13:27:59.724365 aioswitcher-3.4.0/src/aioswitcher/api/messages.py
+-rw-r--r--   0        0        0     3924 2023-05-17 13:27:59.724365 aioswitcher-3.4.0/src/aioswitcher/api/packets.py
+-rw-r--r--   0        0        0    15903 2023-05-17 13:27:59.724365 aioswitcher-3.4.0/src/aioswitcher/api/remotes.py
+-rw-r--r--   0        0        0    16199 2023-05-17 13:27:59.724365 aioswitcher-3.4.0/src/aioswitcher/bridge.py
+-rw-r--r--   0        0        0    11461 2023-05-17 13:27:59.724365 aioswitcher-3.4.0/src/aioswitcher/device/__init__.py
+-rw-r--r--   0        0        0     4320 2023-05-17 13:27:59.724365 aioswitcher-3.4.0/src/aioswitcher/device/tools.py
+-rw-r--r--   0        0        0 12418831 2023-05-17 13:27:59.752365 aioswitcher-3.4.0/src/aioswitcher/resources/irset_db.json
+-rw-r--r--   0        0        0     2054 2023-05-17 13:27:59.752365 aioswitcher-3.4.0/src/aioswitcher/schedule/__init__.py
+-rw-r--r--   0        0        0     4047 2023-05-17 13:27:59.752365 aioswitcher-3.4.0/src/aioswitcher/schedule/parser.py
+-rw-r--r--   0        0        0     5683 2023-05-17 13:27:59.752365 aioswitcher-3.4.0/src/aioswitcher/schedule/tools.py
+-rw-r--r--   0        0        0    11962 1970-01-01 00:00:00.000000 aioswitcher-3.4.0/PKG-INFO
```

### Comparing `aioswitcher-3.3.0/LICENSE` & `aioswitcher-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/README.md` & `aioswitcher-3.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/oranja"><img src="https://avatars.githubusercontent.com/u/679184?v=4?s=100" width="100px;" alt="Itzik Ephraim"/><br /><sub><b>Itzik Ephraim</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=oranja" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Kesav890"><img src="https://avatars.githubusercontent.com/u/82559951?v=4?s=100" width="100px;" alt="Kesav890"/><br /><sub><b>Kesav890</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=Kesav890" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://liad.avrah.am"><img src="https://avatars.githubusercontent.com/u/7263223?v=4?s=100" width="100px;" alt="Liad Avraham"/><br /><sub><b>Liad Avraham</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=liadav" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/OrBin"><img src="https://avatars.githubusercontent.com/u/6897234?v=4?s=100" width="100px;" alt="Or Bin"/><br /><sub><b>Or Bin</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=OrBin" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://exploit.co.il"><img src="https://avatars.githubusercontent.com/u/1768915?v=4?s=100" width="100px;" alt="Shai rod"/><br /><sub><b>Shai rod</b></sub></a><br /><a href="#data-nightrang3r" title="Data">🔣</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/thecode"><img src="https://avatars.githubusercontent.com/u/1858925?v=4?s=100" width="100px;" alt="Shay Levy"/><br /><sub><b>Shay Levy</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=thecode" title="Code">💻</a> <a href="#ideas-thecode" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-thecode" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/thecode"><img src="https://avatars.githubusercontent.com/u/1858925?v=4?s=100" width="100px;" alt="Shay Levy"/><br /><sub><b>Shay Levy</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=thecode" title="Code">💻</a> <a href="#ideas-thecode" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/YogevBokobza"><img src="https://avatars.githubusercontent.com/u/22839127?v=4?s=100" width="100px;" alt="YogevBokobza"/><br /><sub><b>YogevBokobza</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=YogevBokobza" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dmatik"><img src="https://avatars.githubusercontent.com/u/5577386?v=4?s=100" width="100px;" alt="dmatik"/><br /><sub><b>dmatik</b></sub></a><br /><a href="#blog-dmatik" title="Blogposts">📝</a> <a href="#ideas-dmatik" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-dmatik" title="User Testing">📓</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jafar-atili"><img src="https://avatars.githubusercontent.com/u/19508787?v=4?s=100" width="100px;" alt="jafar-atili"/><br /><sub><b>jafar-atili</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Code">💻</a> <a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
```

### Comparing `aioswitcher-3.3.0/pyproject.toml` & `aioswitcher-3.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioswitcher"
-version = "3.3.0"
+version = "3.4.0"
 description = "Switcher Python Integration."
 license = "Apache-2.0"
 authors = [ "Tomer Figenblat <tomer@tomfi.info>" ]
 maintainers = [ "Shay Levy" ]
 readme = "README.md"
 homepage = "https://pypi.org/project/aioswitcher/"
 repository = "https://github.com/tomerfi/aioswitcher"
@@ -22,37 +22,36 @@
 
   [tool.poetry.dependencies]
   python = "^3.9.0"
 
 [tool.poetry.group.dev.dependencies]
 assertpy = "^1.1"
 black = ">=22.8,<24.0"
-codecov = "^2.1.12"
 flake8 = ">=5.0.4,<7.0.0"
 flake8-docstrings = "^1.6.0"
 Flake8-pyproject = "^1.1.0.post0"
 isort = "^5.10.1"
-mypy = ">=0.971,<1.3"
-poethepoet = ">=0.16.1,<0.20.0"
+mypy = ">=0.971,<1.4"
+poethepoet = ">=0.16.1,<0.21.0"
 pytest = "^7.1.2"
 pytest-asyncio = ">=0.19,<0.22"
 pytest-cov = ">=3,<5"
 pytest-resource-path = "^1.3.0"
 pytest-mockservers = "^0.6.0"
 pytest-sugar = "^0.9.4"
 time-machine = "^2.7.0"
 yamllint = "^1.26.3"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.3.0"
 mkdocs-git-revision-date-plugin = "^0.3.2"
 mkdocs-material = ">=8.3.8,<10.0.0"
 mkdocstrings = ">=0.19,<0.22"
-mkdocstrings-python = ">=0.7.1,<0.10.0"
-poethepoet = ">=0.16.1,<0.20.0"
+mkdocstrings-python = ">=0.7.1,<1.1.0"
+poethepoet = ">=0.16.1,<0.21.0"
 
 [tool.poe.tasks]
 install = "poetry install --no-interaction"
 test = "poetry run pytest -v"
 test_cov = "poetry run pytest -v --cov --cov-report=term"
 test_rep = "poetry run pytest -v --cov --cov-report=xml:coverage.xml --junit-xml junit.xml"
 test_pub = "poetry publish --build --repository testpypi"
```

### Comparing `aioswitcher-3.3.0/src/aioswitcher/__init__.py` & `aioswitcher-3.4.0/src/aioswitcher/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/src/aioswitcher/api/__init__.py` & `aioswitcher-3.4.0/src/aioswitcher/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/src/aioswitcher/api/messages.py` & `aioswitcher-3.4.0/src/aioswitcher/api/messages.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/src/aioswitcher/api/packets.py` & `aioswitcher-3.4.0/src/aioswitcher/api/packets.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/src/aioswitcher/api/remotes.py` & `aioswitcher-3.4.0/src/aioswitcher/api/remotes.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/src/aioswitcher/bridge.py` & `aioswitcher-3.4.0/src/aioswitcher/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 
 # Protocol type 1 devices: V2, Touch, V4, Mini, Power Plug
 SWITCHER_UDP_PORT_TYPE1 = 20002
 SWITCHER_UDP_PORT_TYPE1_NEW_VERSION = 10002
 # Protocol type 2 devices: Breeze, Runner, Runner Mini
 SWITCHER_UDP_PORT_TYPE2 = 20003
+SWITCHER_UDP_PORT_TYPE2_NEW_VERSION = 10003
 
 SWITCHER_DEVICE_TO_UDP_PORT = {
     DeviceCategory.WATER_HEATER: SWITCHER_UDP_PORT_TYPE1,
     DeviceCategory.POWER_PLUG: SWITCHER_UDP_PORT_TYPE1,
     DeviceCategory.THERMOSTAT: SWITCHER_UDP_PORT_TYPE2,
     DeviceCategory.SHUTTER: SWITCHER_UDP_PORT_TYPE2,
 }
@@ -165,24 +166,26 @@
     """Use for running a UDP client for bridging Switcher devices broadcast messages.
 
     Args:
         on_device: a callable to which every new SwitcherBase device found will be send.
         broadcast_ports: broadcast ports list, default for type 1 devices is 20002,
             default for type 2 devices is 20003.
             On newer type1 devices, the port is 10002.
+            On newer type2 devices, the port is 10003.
 
     """
 
     def __init__(
         self,
         on_device: Callable[[SwitcherBase], Any],
         broadcast_ports: List[int] = [
             SWITCHER_UDP_PORT_TYPE1,
             SWITCHER_UDP_PORT_TYPE1_NEW_VERSION,
             SWITCHER_UDP_PORT_TYPE2,
+            SWITCHER_UDP_PORT_TYPE2_NEW_VERSION,
         ],
     ) -> None:
         """Initialize the switcher bridge."""
         self._on_device = on_device
         self._broadcast_ports = broadcast_ports
         self._is_running = False
         self._transports: Dict[int, Optional[BaseTransport]] = {}
```

### Comparing `aioswitcher-3.3.0/src/aioswitcher/device/__init__.py` & `aioswitcher-3.4.0/src/aioswitcher/device/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/src/aioswitcher/device/tools.py` & `aioswitcher-3.4.0/src/aioswitcher/device/tools.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/src/aioswitcher/resources/irset_db.json` & `aioswitcher-3.4.0/src/aioswitcher/resources/irset_db.json`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/src/aioswitcher/schedule/__init__.py` & `aioswitcher-3.4.0/src/aioswitcher/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/src/aioswitcher/schedule/parser.py` & `aioswitcher-3.4.0/src/aioswitcher/schedule/parser.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/src/aioswitcher/schedule/tools.py` & `aioswitcher-3.4.0/src/aioswitcher/schedule/tools.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.3.0/PKG-INFO` & `aioswitcher-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioswitcher
-Version: 3.3.0
+Version: 3.4.0
 Summary: Switcher Python Integration.
 Home-page: https://pypi.org/project/aioswitcher/
 License: Apache-2.0
 Keywords: home,automation,switcher,smart
 Author: Tomer Figenblat
 Author-email: tomer@tomfi.info
 Maintainer: Shay Levy
@@ -199,15 +199,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/oranja"><img src="https://avatars.githubusercontent.com/u/679184?v=4?s=100" width="100px;" alt="Itzik Ephraim"/><br /><sub><b>Itzik Ephraim</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=oranja" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Kesav890"><img src="https://avatars.githubusercontent.com/u/82559951?v=4?s=100" width="100px;" alt="Kesav890"/><br /><sub><b>Kesav890</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=Kesav890" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://liad.avrah.am"><img src="https://avatars.githubusercontent.com/u/7263223?v=4?s=100" width="100px;" alt="Liad Avraham"/><br /><sub><b>Liad Avraham</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=liadav" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/OrBin"><img src="https://avatars.githubusercontent.com/u/6897234?v=4?s=100" width="100px;" alt="Or Bin"/><br /><sub><b>Or Bin</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=OrBin" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://exploit.co.il"><img src="https://avatars.githubusercontent.com/u/1768915?v=4?s=100" width="100px;" alt="Shai rod"/><br /><sub><b>Shai rod</b></sub></a><br /><a href="#data-nightrang3r" title="Data">🔣</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/thecode"><img src="https://avatars.githubusercontent.com/u/1858925?v=4?s=100" width="100px;" alt="Shay Levy"/><br /><sub><b>Shay Levy</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=thecode" title="Code">💻</a> <a href="#ideas-thecode" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-thecode" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/thecode"><img src="https://avatars.githubusercontent.com/u/1858925?v=4?s=100" width="100px;" alt="Shay Levy"/><br /><sub><b>Shay Levy</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=thecode" title="Code">💻</a> <a href="#ideas-thecode" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/YogevBokobza"><img src="https://avatars.githubusercontent.com/u/22839127?v=4?s=100" width="100px;" alt="YogevBokobza"/><br /><sub><b>YogevBokobza</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=YogevBokobza" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dmatik"><img src="https://avatars.githubusercontent.com/u/5577386?v=4?s=100" width="100px;" alt="dmatik"/><br /><sub><b>dmatik</b></sub></a><br /><a href="#blog-dmatik" title="Blogposts">📝</a> <a href="#ideas-dmatik" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-dmatik" title="User Testing">📓</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jafar-atili"><img src="https://avatars.githubusercontent.com/u/19508787?v=4?s=100" width="100px;" alt="jafar-atili"/><br /><sub><b>jafar-atili</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Code">💻</a> <a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
```


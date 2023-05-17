# Comparing `tmp/benqprojector-0.0.8.tar.gz` & `tmp/benqprojector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benqprojector-0.0.8.tar", last modified: Mon Dec 12 17:22:54 2022, max compression
+gzip compressed data, was "benqprojector-0.0.9.tar", last modified: Sat Dec 24 17:53:31 2022, max compression
```

## Comparing `benqprojector-0.0.8.tar` & `benqprojector-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rogier     (502) staff       (20)        0 2022-12-12 17:22:54.685165 benqprojector-0.0.8/
--rw-r--r--   0 rogier     (502) staff       (20)    11357 2022-09-21 13:43:38.000000 benqprojector-0.0.8/LICENSE
--rw-r--r--   0 rogier     (502) staff       (20)     2962 2022-12-12 17:22:54.684979 benqprojector-0.0.8/PKG-INFO
--rw-r--r--   0 rogier     (502) staff       (20)     2370 2022-12-07 13:09:31.000000 benqprojector-0.0.8/README.md
-drwxr-xr-x   0 rogier     (502) staff       (20)        0 2022-12-12 17:22:54.682994 benqprojector-0.0.8/benqprojector/
--rw-r--r--   0 rogier     (502) staff       (20)      235 2022-12-12 17:15:55.000000 benqprojector-0.0.8/benqprojector/__init__.py
--rw-r--r--   0 rogier     (502) staff       (20)     5418 2022-12-04 16:41:09.000000 benqprojector-0.0.8/benqprojector/__main__.py
--rw-r--r--   0 rogier     (502) staff       (20)    29689 2022-12-12 17:18:09.000000 benqprojector-0.0.8/benqprojector/benqprojector.py
--rw-r--r--   0 rogier     (502) staff       (20)     6818 2022-12-12 17:18:09.000000 benqprojector-0.0.8/benqprojector/config.py
-drwxr-xr-x   0 rogier     (502) staff       (20)        0 2022-12-12 17:22:54.684055 benqprojector-0.0.8/benqprojector.egg-info/
--rw-r--r--   0 rogier     (502) staff       (20)     2962 2022-12-12 17:22:54.000000 benqprojector-0.0.8/benqprojector.egg-info/PKG-INFO
--rw-r--r--   0 rogier     (502) staff       (20)      381 2022-12-12 17:22:54.000000 benqprojector-0.0.8/benqprojector.egg-info/SOURCES.txt
--rw-r--r--   0 rogier     (502) staff       (20)        1 2022-12-12 17:22:54.000000 benqprojector-0.0.8/benqprojector.egg-info/dependency_links.txt
--rw-r--r--   0 rogier     (502) staff       (20)       14 2022-12-12 17:22:54.000000 benqprojector-0.0.8/benqprojector.egg-info/requires.txt
--rw-r--r--   0 rogier     (502) staff       (20)       14 2022-12-12 17:22:54.000000 benqprojector-0.0.8/benqprojector.egg-info/top_level.txt
--rw-r--r--   0 rogier     (502) staff       (20)      869 2022-12-12 17:17:08.000000 benqprojector-0.0.8/pyproject.toml
--rw-r--r--   0 rogier     (502) staff       (20)       38 2022-12-12 17:22:54.685218 benqprojector-0.0.8/setup.cfg
-drwxr-xr-x   0 rogier     (502) staff       (20)        0 2022-12-12 17:22:54.684584 benqprojector-0.0.8/test/
--rw-r--r--   0 rogier     (502) staff       (20)     3007 2022-11-29 01:02:36.000000 benqprojector-0.0.8/test/testBenQProjector.py
--rw-r--r--   0 rogier     (502) staff       (20)      814 2022-12-05 10:59:02.000000 benqprojector-0.0.8/test/testBenQProjectorErrors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 17:53:31.240824 benqprojector-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-24 17:53:21.000000 benqprojector-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2022-12-24 17:53:31.240824 benqprojector-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2022-12-24 17:53:21.000000 benqprojector-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 17:53:31.240824 benqprojector-0.0.9/benqprojector/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-24 17:53:21.000000 benqprojector-0.0.9/benqprojector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2022-12-24 17:53:21.000000 benqprojector-0.0.9/benqprojector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29690 2022-12-24 17:53:21.000000 benqprojector-0.0.9/benqprojector/benqprojector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2022-12-24 17:53:21.000000 benqprojector-0.0.9/benqprojector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 17:53:31.240824 benqprojector-0.0.9/benqprojector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2022-12-24 17:53:31.000000 benqprojector-0.0.9/benqprojector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2022-12-24 17:53:31.000000 benqprojector-0.0.9/benqprojector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-24 17:53:31.000000 benqprojector-0.0.9/benqprojector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-24 17:53:31.000000 benqprojector-0.0.9/benqprojector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-24 17:53:31.000000 benqprojector-0.0.9/benqprojector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-24 17:53:21.000000 benqprojector-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-24 17:53:31.240824 benqprojector-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 17:53:31.240824 benqprojector-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2022-12-24 17:53:21.000000 benqprojector-0.0.9/test/testBenQProjector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2022-12-24 17:53:21.000000 benqprojector-0.0.9/test/testBenQProjectorErrors.py
```

### Comparing `benqprojector-0.0.8/LICENSE` & `benqprojector-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `benqprojector-0.0.8/PKG-INFO` & `benqprojector-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benqprojector
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library to control BenQ projectors.
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/benqprojector.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/benqprojector.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -22,16 +22,14 @@
 projector and have not implemented any network functionality. Contact me if
 you have a network connected BenQ projector and like this to work.
 
 BenQ projectors and flat pannels with a serial port can support one of three
 protocols. This plugin supports projectors which are of the L, P, T, W and X
 series but probably also others.
 
-[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >](https://www.buymeacoffee.com/rrooggiieerr)  
-
 ## Protocol
 
 This are the protocol details:
 
 2400 baud 8N1
 
 ```
@@ -89,7 +87,10 @@
 Python library please run this command and create an issue on Github with the
 output attached.
 
 To examine your projector capabilities: `python3 -m benqprojector <serial port> <baud> examine`
 
 Your projector needs to be on to be able to detact all your projector
 capabilities.
+
+Do you enjoy using this Python library? Then consider supporting my work:\
+[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >](https://www.buymeacoffee.com/rrooggiieerr)
```

### Comparing `benqprojector-0.0.8/README.md` & `benqprojector-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 projector and have not implemented any network functionality. Contact me if
 you have a network connected BenQ projector and like this to work.
 
 BenQ projectors and flat pannels with a serial port can support one of three
 protocols. This plugin supports projectors which are of the L, P, T, W and X
 series but probably also others.
 
-[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >](https://www.buymeacoffee.com/rrooggiieerr)  
-
 ## Protocol
 
 This are the protocol details:
 
 2400 baud 8N1
 
 ```
@@ -73,7 +71,10 @@
 Python library please run this command and create an issue on Github with the
 output attached.
 
 To examine your projector capabilities: `python3 -m benqprojector <serial port> <baud> examine`
 
 Your projector needs to be on to be able to detact all your projector
 capabilities.
+
+Do you enjoy using this Python library? Then consider supporting my work:\
+[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >](https://www.buymeacoffee.com/rrooggiieerr)
```

### Comparing `benqprojector-0.0.8/benqprojector/__main__.py` & `benqprojector-0.0.9/benqprojector/__main__.py`

 * *Files identical despite different names*

### Comparing `benqprojector-0.0.8/benqprojector/benqprojector.py` & `benqprojector-0.0.9/benqprojector/benqprojector.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
             return None
 
         if self._connect() is False:
             logger.error("Connection not available")
             return None
 
         while self._busy is True:
-            logger.info("to busy for %s=%s", command, action)
+            logger.info("Too busy for %s=%s", command, action)
             self._sleep(0.1)
         self._busy = True
 
         response = None
 
         try:
             self._connection.reset_input_buffer()
```

### Comparing `benqprojector-0.0.8/benqprojector/config.py` & `benqprojector-0.0.9/benqprojector/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,42 +234,21 @@
             "sour",
             "sysfwversion",
             "vkeystone",
             "vol",
         ],
         "sources": ["hdmi", "hdmi2", "smartsystem"],
         "audio_sources": [],
-        "picture_modes": [
-            "bright",
-            "livingroom",
-            "game",
-            "cine",
-            "sport",
-            "user1",
-            "threed",
-        ],
-        "color_temperatures": [
-            "warm",
-            "normal",
-            "cool",
-        ],  # manual says native is supported, but apparently not
+        "picture_modes": ["bright", "livingroom", "game", "cine", "sport", "user1", "threed"],
+        "color_temperatures": ["warm", "normal", "cool"], # manual says native is supported, but apparently not
         "aspect_ratios": ["4:3", "16:9", "2.4:1", "auto"],
         "projector_positions": ["ft", "re", "rc", "fc"],
         "menu_positions": ["center", "tl", "tr", "br", "bl"],
         "lamp_modes": ["lnor", "eco", "seco", "custom"],
-        "3d_modes": [
-            "off",
-            "auto",
-            "tb",
-            "fs",
-            "fp",
-            "sbs",
-            "da",
-            "iv",
-        ],  # sbs, tb, and fp were enabled with a firmware update but undocumented
+        "3d_modes": ["off", "auto", "tb", "fs", "fp", "sbs", "da", "iv"], # sbs, tb, and fp were enabled with a firmware update but undocumented
         "poweron_time": 100,
         "poweroff_time": 100,
     },
 }
 
 BAUD_RATES = [2400, 4800, 9600, 14400, 19200, 38400, 57600, 115200]
```

### Comparing `benqprojector-0.0.8/benqprojector.egg-info/PKG-INFO` & `benqprojector-0.0.9/benqprojector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benqprojector
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library to control BenQ projectors.
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/benqprojector.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/benqprojector.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -22,16 +22,14 @@
 projector and have not implemented any network functionality. Contact me if
 you have a network connected BenQ projector and like this to work.
 
 BenQ projectors and flat pannels with a serial port can support one of three
 protocols. This plugin supports projectors which are of the L, P, T, W and X
 series but probably also others.
 
-[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >](https://www.buymeacoffee.com/rrooggiieerr)  
-
 ## Protocol
 
 This are the protocol details:
 
 2400 baud 8N1
 
 ```
@@ -89,7 +87,10 @@
 Python library please run this command and create an issue on Github with the
 output attached.
 
 To examine your projector capabilities: `python3 -m benqprojector <serial port> <baud> examine`
 
 Your projector needs to be on to be able to detact all your projector
 capabilities.
+
+Do you enjoy using this Python library? Then consider supporting my work:\
+[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >](https://www.buymeacoffee.com/rrooggiieerr)
```

### Comparing `benqprojector-0.0.8/pyproject.toml` & `benqprojector-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "benqprojector"
-version = "0.0.8"
+version = "0.0.9"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Library to control BenQ projectors."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `benqprojector-0.0.8/test/testBenQProjector.py` & `benqprojector-0.0.9/test/testBenQProjector.py`

 * *Files identical despite different names*

### Comparing `benqprojector-0.0.8/test/testBenQProjectorErrors.py` & `benqprojector-0.0.9/test/testBenQProjectorErrors.py`

 * *Files identical despite different names*


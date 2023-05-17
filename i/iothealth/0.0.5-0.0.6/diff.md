# Comparing `tmp/iothealth-0.0.5.tar.gz` & `tmp/iothealth-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iothealth-0.0.5.tar", last modified: Sun Apr 30 06:18:23 2023, max compression
+gzip compressed data, was "iothealth-0.0.6.tar", last modified: Wed May 17 06:07:00 2023, max compression
```

## Comparing `iothealth-0.0.5.tar` & `iothealth-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1070 2023-01-03 00:32:11.000000 iothealth-0.0.5/LICENSE
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2752 2023-04-30 06:18:23.071322 iothealth-0.0.5/PKG-INFO
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2345 2023-01-03 00:32:11.000000 iothealth-0.0.5/README.rst
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.061322 iothealth-0.0.5/docs/
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/docs/source/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1990 2023-01-03 00:32:11.000000 iothealth-0.0.5/docs/source/conf.py
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/iothealth/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/__init__.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      162 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/__main__.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1925 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/_base_health.py
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/iothealth/bin/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/bin/__init__.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1706 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/bin/cli.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2545 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/device_health.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     5120 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/linux.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1697 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/raspberry_pi.py
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/iothealth.egg-info/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2752 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/PKG-INFO
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      490 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/SOURCES.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        1 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/dependency_links.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       58 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/entry_points.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       13 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/requires.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       26 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/top_level.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      633 2023-04-30 06:17:46.000000 iothealth-0.0.5/pyproject.toml
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       38 2023-04-30 06:18:23.071322 iothealth-0.0.5/setup.cfg
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/tests/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      162 2023-01-03 00:32:11.000000 iothealth-0.0.5/tests/test_device_health.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      131 2023-01-03 00:32:11.000000 iothealth-0.0.5/tests/test_linux.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-05-17 06:07:00.625760 iothealth-0.0.6/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1070 2023-01-03 00:32:11.000000 iothealth-0.0.6/LICENSE
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2752 2023-05-17 06:07:00.625760 iothealth-0.0.6/PKG-INFO
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2345 2023-01-03 00:32:11.000000 iothealth-0.0.6/README.rst
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-05-17 06:07:00.625760 iothealth-0.0.6/docs/
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-05-17 06:07:00.625760 iothealth-0.0.6/docs/source/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1990 2023-01-03 00:32:11.000000 iothealth-0.0.6/docs/source/conf.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-05-17 06:07:00.625760 iothealth-0.0.6/iothealth/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-01-03 00:32:11.000000 iothealth-0.0.6/iothealth/__init__.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      162 2023-01-03 00:32:11.000000 iothealth-0.0.6/iothealth/__main__.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1925 2023-01-03 00:32:11.000000 iothealth-0.0.6/iothealth/_base_health.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-05-17 06:07:00.625760 iothealth-0.0.6/iothealth/bin/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-01-03 00:32:11.000000 iothealth-0.0.6/iothealth/bin/__init__.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1706 2023-01-03 00:32:11.000000 iothealth-0.0.6/iothealth/bin/cli.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2545 2023-01-03 00:32:11.000000 iothealth-0.0.6/iothealth/device_health.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     5120 2023-01-03 00:32:11.000000 iothealth-0.0.6/iothealth/linux.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1874 2023-05-17 06:05:50.000000 iothealth-0.0.6/iothealth/raspberry_pi.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-05-17 06:07:00.625760 iothealth-0.0.6/iothealth.egg-info/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2752 2023-05-17 06:07:00.000000 iothealth-0.0.6/iothealth.egg-info/PKG-INFO
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      490 2023-05-17 06:07:00.000000 iothealth-0.0.6/iothealth.egg-info/SOURCES.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        1 2023-05-17 06:07:00.000000 iothealth-0.0.6/iothealth.egg-info/dependency_links.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       58 2023-05-17 06:07:00.000000 iothealth-0.0.6/iothealth.egg-info/entry_points.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       13 2023-05-17 06:07:00.000000 iothealth-0.0.6/iothealth.egg-info/requires.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       26 2023-05-17 06:07:00.000000 iothealth-0.0.6/iothealth.egg-info/top_level.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      633 2023-05-17 06:05:50.000000 iothealth-0.0.6/pyproject.toml
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       38 2023-05-17 06:07:00.636594 iothealth-0.0.6/setup.cfg
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-05-17 06:07:00.625760 iothealth-0.0.6/tests/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      162 2023-01-03 00:32:11.000000 iothealth-0.0.6/tests/test_device_health.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      131 2023-01-03 00:32:11.000000 iothealth-0.0.6/tests/test_linux.py
```

### Comparing `iothealth-0.0.5/LICENSE` & `iothealth-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iothealth-0.0.5/PKG-INFO` & `iothealth-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iothealth
-Version: 0.0.5
+Version: 0.0.6
 Summary: Health and Status Library for IoT Devices
 Author: IoT Spectator
 License: MIT License
 Project-URL: repository, https://github.com/iot-spectator/iot-health
 Keywords: IoT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `iothealth-0.0.5/README.rst` & `iothealth-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `iothealth-0.0.5/docs/source/conf.py` & `iothealth-0.0.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `iothealth-0.0.5/iothealth/_base_health.py` & `iothealth-0.0.6/iothealth/_base_health.py`

 * *Files identical despite different names*

### Comparing `iothealth-0.0.5/iothealth/bin/cli.py` & `iothealth-0.0.6/iothealth/bin/cli.py`

 * *Files identical despite different names*

### Comparing `iothealth-0.0.5/iothealth/device_health.py` & `iothealth-0.0.6/iothealth/device_health.py`

 * *Files identical despite different names*

### Comparing `iothealth-0.0.5/iothealth/linux.py` & `iothealth-0.0.6/iothealth/linux.py`

 * *Files identical despite different names*

### Comparing `iothealth-0.0.5/iothealth/raspberry_pi.py` & `iothealth-0.0.6/iothealth/raspberry_pi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © 2020 by IoT Spectator. All rights reserved.
 
 """Raspberry Pi health information."""
 
 import re
+import shutil
 import subprocess
 
 from iothealth import linux
 
 
 class RaspberryPi(linux.Linux):
     """Check Raspberry Pi health and status."""
@@ -41,19 +42,25 @@
         -------
         float
             The device temperature, e.g., 54.8.
             The temperature unit is Celsius.
 
         Raises
         ------
-        `TemperatureError`
+        `RuntimeError`
             Raised if the temperature info is not available.
         """
+        VCGENGCMD = "vcgencmd"
+        vcgencmd_path = shutil.which(VCGENGCMD)
+
+        if not vcgencmd_path:
+            raise RuntimeError(f"No {VCGENGCMD} command found.")
+
         result = subprocess.run(
-            ["/opt/vc/bin/vcgencmd", "measure_temp"],
+            [vcgencmd_path, "measure_temp"],
             capture_output=True,
             text=True,
         )
         if not result.stderr:
             temp = re.search("\\d+\\.\\d+", result.stdout)
             if temp:
                 return {"chip": temp.group(0)}
```

### Comparing `iothealth-0.0.5/iothealth.egg-info/PKG-INFO` & `iothealth-0.0.6/iothealth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iothealth
-Version: 0.0.5
+Version: 0.0.6
 Summary: Health and Status Library for IoT Devices
 Author: IoT Spectator
 License: MIT License
 Project-URL: repository, https://github.com/iot-spectator/iot-health
 Keywords: IoT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `iothealth-0.0.5/pyproject.toml` & `iothealth-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iothealth"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="IoT Spectator" }
 ]
 description = "Health and Status Library for IoT Devices"
 readme = {file = "README.rst", content-type = "text/x-rst"}
 requires-python = ">=3.9"
 license = {text = "MIT License"}
```


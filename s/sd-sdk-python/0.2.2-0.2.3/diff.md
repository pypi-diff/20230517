# Comparing `tmp/sd_sdk_python-0.2.2.tar.gz` & `tmp/sd_sdk_python-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_sdk_python-0.2.2.tar", max compression
+gzip compressed data, was "sd_sdk_python-0.2.3.tar", max compression
```

## Comparing `sd_sdk_python-0.2.2.tar` & `sd_sdk_python-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-05-15 21:02:02.654724 sd_sdk_python-0.2.2/LICENSE
--rw-r--r--   0        0        0      636 2023-05-15 21:02:02.654724 sd_sdk_python-0.2.2/README.md
--rw-r--r--   0        0        0     1080 2023-05-15 21:02:02.654724 sd_sdk_python-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2783 2023-05-15 21:02:02.654724 sd_sdk_python-0.2.2/sd_sdk_python/__init__.py
--rw-r--r--   0        0        0    12568 2023-05-15 21:02:02.658723 sd_sdk_python-0.2.2/sd_sdk_python/sd_sdk.py
--rw-r--r--   0        0        0    13130 2023-05-15 21:02:02.658723 sd_sdk_python-0.2.2/sd_sdk_python/sd_sdk_wireless.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 sd_sdk_python-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-17 19:27:23.599773 sd_sdk_python-0.2.3/LICENSE
+-rw-r--r--   0        0        0      636 2023-05-17 19:27:23.599773 sd_sdk_python-0.2.3/README.md
+-rw-r--r--   0        0        0     1080 2023-05-17 19:27:23.603773 sd_sdk_python-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2783 2023-05-17 19:27:23.603773 sd_sdk_python-0.2.3/sd_sdk_python/__init__.py
+-rw-r--r--   0        0        0    12824 2023-05-17 19:27:23.603773 sd_sdk_python-0.2.3/sd_sdk_python/sd_sdk.py
+-rw-r--r--   0        0        0    13130 2023-05-17 19:27:23.603773 sd_sdk_python-0.2.3/sd_sdk_python/sd_sdk_wireless.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 sd_sdk_python-0.2.3/PKG-INFO
```

### Comparing `sd_sdk_python-0.2.2/LICENSE` & `sd_sdk_python-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.2/README.md` & `sd_sdk_python-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.2/pyproject.toml` & `sd_sdk_python-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sd-sdk-python"
 homepage = "https://github.com/markmelvin-onsemi/sd-sdk-python"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python helper module for the Sound Designer SDK"
 authors = ["Mark Melvin <mark.melvin@onsemi.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `sd_sdk_python-0.2.2/sd_sdk_python/__init__.py` & `sd_sdk_python-0.2.3/sd_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.2/sd_sdk_python/sd_sdk.py` & `sd_sdk_python-0.2.3/sd_sdk_python/sd_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,25 +268,31 @@
         for param in list_of_parameters:
             name += param.to_bytes(3, 'big')
         return name.decode('utf-8').strip('\x00')
 
     @staticmethod
     def device_name_to_parameters(name):
         params = [0]*8
-        # Clip length to 24 bytes (eight 24-bit parameters)
-        name = name.encode('utf-8')[:7*3]
-        for i in range(0, len(name), 3):
+        encoded_bytes = []
+        for character in name:
+            enc = character.encode('utf-8')
+            # Clip length to 24 bytes (eight 24-bit parameters)
+            if (len(encoded_bytes) + len(enc)) > 8*3:
+                break
+            encoded_bytes += [int(w) for w in enc]
+
+        # Pack encoded_bytes into 24-bit parameters
+        for i in range(0, len(encoded_bytes), 3):
             value = 0
-            substr = name[i:i+3]
+            substr = encoded_bytes[i:i+3]
             for j, char in enumerate(substr):
-                value |= (int(char) << (16 - j*8))
+                value |= (char << (16 - j*8))
             params[i // 3] = value
         return params
 
-
 def wait_for_async(_async, timeout_seconds=1.0, sleep_time_seconds=0.01):
     """Waits for an AsyncResult to finish"""
     while not _async.IsFinished and timeout > 0:
         time.sleep(sleep_time_seconds)
         timeout -= sleep_time_seconds
 
     if timeout <= 0:
```

### Comparing `sd_sdk_python-0.2.2/sd_sdk_python/sd_sdk_wireless.py` & `sd_sdk_python-0.2.3/sd_sdk_python/sd_sdk_wireless.py`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.2/PKG-INFO` & `sd_sdk_python-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-sdk-python
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python helper module for the Sound Designer SDK
 Home-page: https://github.com/markmelvin-onsemi/sd-sdk-python
 License: MIT
 Author: Mark Melvin
 Author-email: mark.melvin@onsemi.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```


# Comparing `tmp/hspylib-firebase-0.9.97.tar.gz` & `tmp/hspylib-firebase-0.9.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-firebase-0.9.97.tar", last modified: Tue Apr 25 19:08:15 2023, max compression
+gzip compressed data, was "hspylib-firebase-0.9.98.tar", last modified: Wed May 17 17:34:27 2023, max compression
```

## Comparing `hspylib-firebase-0.9.97.tar` & `hspylib-firebase-0.9.98.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.760093 hspylib-firebase-0.9.97/
--rw-r--r--   0 hjunior    (504) staff       (20)       95 2022-06-17 15:16:57.000000 hspylib-firebase-0.9.97/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-04-25 19:08:15.759235 hspylib-firebase-0.9.97/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      708 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.718462 hspylib-firebase-0.9.97/firebase/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/firebase/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      722 2023-04-19 22:01:55.000000 hspylib-firebase-0.9.97/firebase/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      186 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/firebase/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4427 2023-04-19 22:13:48.000000 hspylib-firebase-0.9.97/firebase/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.730540 hspylib-firebase-0.9.97/firebase/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      226 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/firebase/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6370 2023-04-25 19:05:44.000000 hspylib-firebase-0.9.97/firebase/core/agent_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4926 2023-04-19 22:17:54.000000 hspylib-firebase-0.9.97/firebase/core/file_processor.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2923 2023-04-19 22:17:54.000000 hspylib-firebase-0.9.97/firebase/core/firebase.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2644 2023-04-25 19:05:08.000000 hspylib-firebase-0.9.97/firebase/core/firebase_auth.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.736912 hspylib-firebase-0.9.97/firebase/domain/
--rw-r--r--   0 hjunior    (504) staff       (20)      172 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/firebase/domain/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3171 2023-04-19 22:17:54.000000 hspylib-firebase-0.9.97/firebase/domain/firebase_dto.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.742195 hspylib-firebase-0.9.97/firebase/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      173 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/firebase/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      765 2023-04-19 22:01:55.000000 hspylib-firebase-0.9.97/firebase/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.744469 hspylib-firebase-0.9.97/firebase/resources/
--rw-r--r--   0 hjunior    (504) staff       (20)      130 2022-11-12 19:14:41.000000 hspylib-firebase-0.9.97/firebase/resources/application.properties
--rw-r--r--   0 hjunior    (504) staff       (20)      237 2022-02-18 20:00:37.000000 hspylib-firebase-0.9.97/firebase/welcome.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.757868 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-04-25 19:08:15.000000 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      647 2023-04-25 19:08:15.000000 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-04-25 19:08:15.000000 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-04-25 19:08:15.000000 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        9 2023-04-25 19:08:15.000000 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-04-25 19:08:15.760277 hspylib-firebase-0.9.97/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1864 2023-04-19 22:13:48.000000 hspylib-firebase-0.9.97/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.710077 hspylib-firebase-0.9.98/
+-rw-r--r--   0 hjunior    (504) staff       (20)       95 2022-06-17 15:16:57.000000 hspylib-firebase-0.9.98/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-05-17 17:34:27.707313 hspylib-firebase-0.9.98/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      708 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.666035 hspylib-firebase-0.9.98/firebase/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/firebase/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      722 2023-04-19 22:01:55.000000 hspylib-firebase-0.9.98/firebase/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      186 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/firebase/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4427 2023-04-19 22:13:48.000000 hspylib-firebase-0.9.98/firebase/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.677038 hspylib-firebase-0.9.98/firebase/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      226 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/firebase/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6370 2023-04-25 19:05:44.000000 hspylib-firebase-0.9.98/firebase/core/agent_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4926 2023-04-19 22:17:54.000000 hspylib-firebase-0.9.98/firebase/core/file_processor.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2923 2023-04-19 22:17:54.000000 hspylib-firebase-0.9.98/firebase/core/firebase.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2644 2023-04-25 19:05:08.000000 hspylib-firebase-0.9.98/firebase/core/firebase_auth.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.682533 hspylib-firebase-0.9.98/firebase/domain/
+-rw-r--r--   0 hjunior    (504) staff       (20)      172 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/firebase/domain/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3136 2023-05-17 17:32:46.000000 hspylib-firebase-0.9.98/firebase/domain/firebase_dto.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.687370 hspylib-firebase-0.9.98/firebase/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      173 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/firebase/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      765 2023-04-19 22:01:55.000000 hspylib-firebase-0.9.98/firebase/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.689740 hspylib-firebase-0.9.98/firebase/resources/
+-rw-r--r--   0 hjunior    (504) staff       (20)      130 2022-11-12 19:14:41.000000 hspylib-firebase-0.9.98/firebase/resources/application.properties
+-rw-r--r--   0 hjunior    (504) staff       (20)      237 2022-02-18 20:00:37.000000 hspylib-firebase-0.9.98/firebase/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.704953 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-05-17 17:34:27.000000 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      647 2023-05-17 17:34:27.000000 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-05-17 17:34:27.000000 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-05-17 17:34:27.000000 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        9 2023-05-17 17:34:27.000000 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-05-17 17:34:27.710322 hspylib-firebase-0.9.98/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1864 2023-04-19 22:13:48.000000 hspylib-firebase-0.9.98/setup.py
```

### Comparing `hspylib-firebase-0.9.97/PKG-INFO` & `hspylib-firebase-0.9.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-firebase
-Version: 0.9.97
+Version: 0.9.98
 Summary: HsPyLib - Firebase integration
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-firebase/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.97/README.md` & `hspylib-firebase-0.9.98/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.97/firebase/__classpath__.py` & `hspylib-firebase-0.9.98/firebase/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.97/firebase/__main__.py` & `hspylib-firebase-0.9.98/firebase/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.97/firebase/core/agent_config.py` & `hspylib-firebase-0.9.98/firebase/core/agent_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.97/firebase/core/file_processor.py` & `hspylib-firebase-0.9.98/firebase/core/file_processor.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.97/firebase/core/firebase.py` & `hspylib-firebase-0.9.98/firebase/core/firebase.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.97/firebase/core/firebase_auth.py` & `hspylib-firebase-0.9.98/firebase/core/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.97/firebase/domain/firebase_dto.py` & `hspylib-firebase-0.9.98/firebase/domain/firebase_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,24 +60,24 @@
         if os.path.exists(self.path):
             with open(self.path, "r", encoding=Charset.UTF_8.val) as f_in:
                 self.data = f_in.read()
                 if (size := len(self.data)) == 0:
                     log.warning('Nothing to be loaded. File "%s" is empty', self.path)
                 self.size = size
                 return self
-        raise FileNotFoundError(f'The path "{self.path}" does represent an existing file!')
+        raise FileNotFoundError(f'File "{self.path}" could not be loaded because it does not exist!')
 
     def save(self) -> "FirebaseDto":
         """Saves current DTO content (overwrites current file content)."""
         if os.path.exists(self.path):
-            with open(self.path, "w+", encoding=Charset.UTF_8.val) as f_out:
-                f_out.write(self.data)
-                f_out.flush()
-                return self
-        raise FileNotFoundError(f'File could not be save because it\'s path: "{self.path}" was not found!')
+            log.warning('File "%s" exists and will be overwritten', self.path)
+        with open(self.path, "w+", encoding=Charset.UTF_8.val) as f_out:
+            f_out.write(self.data)
+            f_out.flush()
+            return self
 
     def encode(self) -> "FirebaseDto":
         """B64-Encode the entry contents."""
         self.data = b64_encode(self.data)
         return self
 
     def decode(self) -> "FirebaseDto":
```

### Comparing `hspylib-firebase-0.9.97/firebase/exception/exceptions.py` & `hspylib-firebase-0.9.98/firebase/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.97/hspylib_firebase.egg-info/PKG-INFO` & `hspylib-firebase-0.9.98/hspylib_firebase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-firebase
-Version: 0.9.97
+Version: 0.9.98
 Summary: HsPyLib - Firebase integration
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-firebase/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.97/hspylib_firebase.egg-info/SOURCES.txt` & `hspylib-firebase-0.9.98/hspylib_firebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.97/setup.py` & `hspylib-firebase-0.9.98/setup.py`

 * *Files identical despite different names*


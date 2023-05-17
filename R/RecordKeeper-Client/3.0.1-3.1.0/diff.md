# Comparing `tmp/RecordKeeper_Client-3.0.1.tar.gz` & `tmp/RecordKeeper_Client-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RecordKeeper_Client-3.0.1.tar", last modified: Thu Apr  6 16:40:08 2023, max compression
+gzip compressed data, was "RecordKeeper_Client-3.1.0.tar", last modified: Wed May 17 12:57:40 2023, max compression
```

## Comparing `RecordKeeper_Client-3.0.1.tar` & `RecordKeeper_Client-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-04-06 16:40:08.772000 RecordKeeper_Client-3.0.1/
--rw-r--r--   0 hubert    (1001) hubert    (1001)    35149 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.0.1/LICENSE
--rw-r--r--   0 hubert    (1001) hubert    (1001)       16 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.0.1/MANIFEST.in
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     6127 2023-04-06 16:40:08.772000 RecordKeeper_Client-3.0.1/PKG-INFO
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     4260 2023-04-06 16:39:47.000000 RecordKeeper_Client-3.0.1/README.md
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-04-06 16:40:08.772000 RecordKeeper_Client-3.0.1/RecordKeeper_Client.egg-info/
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     6127 2023-04-06 16:40:08.000000 RecordKeeper_Client-3.0.1/RecordKeeper_Client.egg-info/PKG-INFO
--rw-rw-r--   0 hubert    (1001) hubert    (1001)      416 2023-04-06 16:40:08.000000 RecordKeeper_Client-3.0.1/RecordKeeper_Client.egg-info/SOURCES.txt
--rw-rw-r--   0 hubert    (1001) hubert    (1001)        1 2023-04-06 16:40:08.000000 RecordKeeper_Client-3.0.1/RecordKeeper_Client.egg-info/dependency_links.txt
--rw-rw-r--   0 hubert    (1001) hubert    (1001)        9 2023-04-06 16:40:08.000000 RecordKeeper_Client-3.0.1/RecordKeeper_Client.egg-info/top_level.txt
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-04-06 16:40:08.772000 RecordKeeper_Client-3.0.1/rkclient/
--rw-rw-r--   0 hubert    (1001) hubert    (1001)      820 2023-04-06 16:26:10.000000 RecordKeeper_Client-3.0.1/rkclient/__init__.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)    14001 2023-04-06 16:26:10.000000 RecordKeeper_Client-3.0.1/rkclient/admin.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)       97 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.0.1/rkclient/auth.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     5540 2023-04-06 16:26:10.000000 RecordKeeper_Client-3.0.1/rkclient/client.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     3264 2023-03-29 19:51:20.000000 RecordKeeper_Client-3.0.1/rkclient/entities.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     2294 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.0.1/rkclient/factory.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     3456 2023-04-06 16:26:10.000000 RecordKeeper_Client-3.0.1/rkclient/request.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     4486 2023-04-06 16:26:10.000000 RecordKeeper_Client-3.0.1/rkclient/serialization.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)       38 2023-04-06 16:40:08.772000 RecordKeeper_Client-3.0.1/setup.cfg
--rw-rw-r--   0 hubert    (1001) hubert    (1001)      894 2023-03-15 09:31:37.000000 RecordKeeper_Client-3.0.1/setup.py
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-04-06 16:40:08.772000 RecordKeeper_Client-3.0.1/test/
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     2880 2023-04-06 16:26:10.000000 RecordKeeper_Client-3.0.1/test/test_api.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     6627 2023-04-06 16:26:10.000000 RecordKeeper_Client-3.0.1/test/test_serialization.py
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-17 12:57:40.003083 RecordKeeper_Client-3.1.0/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    35149 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.1.0/LICENSE
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       16 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.1.0/MANIFEST.in
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     6142 2023-05-17 12:57:40.003083 RecordKeeper_Client-3.1.0/PKG-INFO
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     4275 2023-05-17 12:49:18.000000 RecordKeeper_Client-3.1.0/README.md
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-17 12:57:39.999083 RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     6142 2023-05-17 12:57:39.000000 RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/PKG-INFO
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)      416 2023-05-17 12:57:39.000000 RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/SOURCES.txt
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)        1 2023-05-17 12:57:39.000000 RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/dependency_links.txt
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)        9 2023-05-17 12:57:39.000000 RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/top_level.txt
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-17 12:57:40.003083 RecordKeeper_Client-3.1.0/rkclient/
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)      820 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/rkclient/__init__.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)    14001 2023-05-12 12:37:06.000000 RecordKeeper_Client-3.1.0/rkclient/admin.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)       97 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.1.0/rkclient/auth.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     5540 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/rkclient/client.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     3264 2023-03-29 19:51:20.000000 RecordKeeper_Client-3.1.0/rkclient/entities.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     2294 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.1.0/rkclient/factory.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     3456 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/rkclient/request.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     4486 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/rkclient/serialization.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)       38 2023-05-17 12:57:40.003083 RecordKeeper_Client-3.1.0/setup.cfg
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)      894 2023-03-15 09:31:37.000000 RecordKeeper_Client-3.1.0/setup.py
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-17 12:57:40.003083 RecordKeeper_Client-3.1.0/test/
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     2880 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/test/test_api.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     6627 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/test/test_serialization.py
```

### Comparing `RecordKeeper_Client-3.0.1/LICENSE` & `RecordKeeper_Client-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.0.1/PKG-INFO` & `RecordKeeper_Client-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecordKeeper_Client
-Version: 3.0.1
+Version: 3.1.0
 Summary: Client library for accessing Record Keepers Receiver
 Home-page: UNKNOWN
 Author: ERST
 Author-email: noreply@example.ecom
 License: GPLv3+
 Description: 
         # Context
@@ -93,15 +93,15 @@
         >>> for pem in pems:
         >>>   print(pem)
         ```
         ## Changelog
         
         ### Unreleased
         
-        ## [3.0.1] - 2023-04-06
+        ## [3.1.0] - 2023-04-06 and 2023-05-17
         - Improved error logging, by creating less irrelevant logs. 
         - Add default User-Agent to requests to be equal to `recordkeeper-client-{version}`.
         - RKAdmin supports /info and /verify endpoints of GraphBuilder.
         
         ## [3.0.0] - 2023-02-06
         - Changed Artifact id field from uuid to string. This forces changes in many functions API.
         - Changed Emitter field from uuid to string.
```

### Comparing `RecordKeeper_Client-3.0.1/README.md` & `RecordKeeper_Client-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 >>> for pem in pems:
 >>>   print(pem)
 ```
 ## Changelog
 
 ### Unreleased
 
-## [3.0.1] - 2023-04-06
+## [3.1.0] - 2023-04-06 and 2023-05-17
 - Improved error logging, by creating less irrelevant logs. 
 - Add default User-Agent to requests to be equal to `recordkeeper-client-{version}`.
 - RKAdmin supports /info and /verify endpoints of GraphBuilder.
 
 ## [3.0.0] - 2023-02-06
 - Changed Artifact id field from uuid to string. This forces changes in many functions API.
 - Changed Emitter field from uuid to string.
```

### Comparing `RecordKeeper_Client-3.0.1/RecordKeeper_Client.egg-info/PKG-INFO` & `RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecordKeeper-Client
-Version: 3.0.1
+Version: 3.1.0
 Summary: Client library for accessing Record Keepers Receiver
 Home-page: UNKNOWN
 Author: ERST
 Author-email: noreply@example.ecom
 License: GPLv3+
 Description: 
         # Context
@@ -93,15 +93,15 @@
         >>> for pem in pems:
         >>>   print(pem)
         ```
         ## Changelog
         
         ### Unreleased
         
-        ## [3.0.1] - 2023-04-06
+        ## [3.1.0] - 2023-04-06 and 2023-05-17
         - Improved error logging, by creating less irrelevant logs. 
         - Add default User-Agent to requests to be equal to `recordkeeper-client-{version}`.
         - RKAdmin supports /info and /verify endpoints of GraphBuilder.
         
         ## [3.0.0] - 2023-02-06
         - Changed Artifact id field from uuid to string. This forces changes in many functions API.
         - Changed Emitter field from uuid to string.
```

### Comparing `RecordKeeper_Client-3.0.1/rkclient/__init__.py` & `RecordKeeper_Client-3.1.0/rkclient/__init__.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.0.1/rkclient/admin.py` & `RecordKeeper_Client-3.1.0/rkclient/admin.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.0.1/rkclient/client.py` & `RecordKeeper_Client-3.1.0/rkclient/client.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.0.1/rkclient/entities.py` & `RecordKeeper_Client-3.1.0/rkclient/entities.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.0.1/rkclient/factory.py` & `RecordKeeper_Client-3.1.0/rkclient/factory.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.0.1/rkclient/request.py` & `RecordKeeper_Client-3.1.0/rkclient/request.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.0.1/rkclient/serialization.py` & `RecordKeeper_Client-3.1.0/rkclient/serialization.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.0.1/setup.py` & `RecordKeeper_Client-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.0.1/test/test_api.py` & `RecordKeeper_Client-3.1.0/test/test_api.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.0.1/test/test_serialization.py` & `RecordKeeper_Client-3.1.0/test/test_serialization.py`

 * *Files identical despite different names*


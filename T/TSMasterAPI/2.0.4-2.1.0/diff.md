# Comparing `tmp/TSMasterAPI-2.0.4.tar.gz` & `tmp/TSMasterAPI-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-2.0.4.tar", last modified: Wed May 17 06:27:56 2023, max compression
+gzip compressed data, was "TSMasterAPI-2.1.0.tar", last modified: Wed May 17 07:00:06 2023, max compression
```

## Comparing `TSMasterAPI-2.0.4.tar` & `TSMasterAPI-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 06:27:56.161956 TSMasterAPI-2.0.4/
--rw-rw-rw-   0        0        0     1024 2023-05-17 06:27:56.160931 TSMasterAPI-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 06:27:56.151472 TSMasterAPI-2.0.4/TSMasterAPI/
--rw-rw-rw-   0        0        0    42782 2023-05-17 06:16:11.000000 TSMasterAPI-2.0.4/TSMasterAPI/TSBUSDriver.py
--rw-rw-rw-   0        0        0    70948 2023-05-17 06:16:04.000000 TSMasterAPI-2.0.4/TSMasterAPI/TSCommon.py
--rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.0.4/TSMasterAPI/TSDirver.py
--rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.0.4/TSMasterAPI/TSEnumdefine.py
--rw-rw-rw-   0        0        0    22804 2023-05-17 05:00:47.000000 TSMasterAPI-2.0.4/TSMasterAPI/TSFibex_parse.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.0.4/TSMasterAPI/TSFlexRayDriver.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.0.4/TSMasterAPI/TSLINDriver.py
--rw-rw-rw-   0        0        0   155849 2023-05-17 06:27:29.000000 TSMasterAPI-2.0.4/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0    27697 2023-05-17 06:26:49.000000 TSMasterAPI-2.0.4/TSMasterAPI/TSStructure.py
--rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.0.4/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 06:27:56.160135 TSMasterAPI-2.0.4/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-05-17 06:27:56.000000 TSMasterAPI-2.0.4/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-17 06:27:56.000000 TSMasterAPI-2.0.4/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 06:27:56.000000 TSMasterAPI-2.0.4/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-17 06:27:56.000000 TSMasterAPI-2.0.4/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.0.4/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 06:27:56.161956 TSMasterAPI-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-05-17 06:27:55.000000 TSMasterAPI-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:00:06.400349 TSMasterAPI-2.1.0/
+-rw-rw-rw-   0        0        0     1024 2023-05-17 07:00:06.398846 TSMasterAPI-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 07:00:06.390008 TSMasterAPI-2.1.0/TSMasterAPI/
+-rw-rw-rw-   0        0        0    42782 2023-05-17 06:16:11.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSBUSDriver.py
+-rw-rw-rw-   0        0        0    70944 2023-05-17 06:59:34.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSCommon.py
+-rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSDirver.py
+-rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSEnumdefine.py
+-rw-rw-rw-   0        0        0    22804 2023-05-17 05:00:47.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSFibex_parse.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSFlexRayDriver.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSLINDriver.py
+-rw-rw-rw-   0        0        0   155849 2023-05-17 06:27:29.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0    27697 2023-05-17 06:26:49.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSStructure.py
+-rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.1.0/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:00:06.398846 TSMasterAPI-2.1.0/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-05-17 07:00:06.000000 TSMasterAPI-2.1.0/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-17 07:00:06.000000 TSMasterAPI-2.1.0/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 07:00:06.000000 TSMasterAPI-2.1.0/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-17 07:00:06.000000 TSMasterAPI-2.1.0/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.1.0/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 07:00:06.400349 TSMasterAPI-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-05-17 06:59:52.000000 TSMasterAPI-2.1.0/setup.py
```

### Comparing `TSMasterAPI-2.0.4/PKG-INFO` & `TSMasterAPI-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.0.4
+Version: 2.1.0
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.0.4/TSMasterAPI/TSBUSDriver.py` & `TSMasterAPI-2.1.0/TSMasterAPI/TSBUSDriver.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.4/TSMasterAPI/TSCommon.py` & `TSMasterAPI-2.1.0/TSMasterAPI/TSCommon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:59:15
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-05-17 13:19:31
+LastEditTime: 2023-05-17 14:59:34
 '''
 from .TSDirver import *
 from .TSStructure import *  
 from .TSEnumdefine import *  
 from .TSFibex_parse import * 
 
 # Common Functions
@@ -789,15 +789,15 @@
 # 使能wakeup_pattern
 tsflexray_wakeup_pattern = dll.tsflexray_wakeup_pattern
 tsflexray_wakeup_pattern.argtypes = [s32,s32]  
 tsflexray_wakeup_pattern.restype = TS_ReturnType
 tsflexray_wakeup_pattern.errcheck = check_status_operation
 
 tsflexray_set_controller_frametrigger = dll.tsflexray_set_controller_frametrigger
-tsflexray_set_controller_frametrigger.argtypes = [s32,PLibFlexray_controller_config,c_char_p,s32,PLibTrigger_def,s32,s32]  
+tsflexray_set_controller_frametrigger.argtypes = [s32,PLibFlexray_controller_config,ps32,s32,PLibTrigger_def,s32,s32]  
 tsflexray_set_controller_frametrigger.restype = TS_ReturnType
 tsflexray_set_controller_frametrigger.errcheck = check_status_operation
 
 # flexray 发送
 # 异步单帧发送flexray报文
 tsapp_transmit_flexray_async = dll.tsapp_transmit_flexray_async
 tsapp_transmit_flexray_async.argtypes = [PFlexray]
```

### Comparing `TSMasterAPI-2.0.4/TSMasterAPI/TSDirver.py` & `TSMasterAPI-2.1.0/TSMasterAPI/TSDirver.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.4/TSMasterAPI/TSEnumdefine.py` & `TSMasterAPI-2.1.0/TSMasterAPI/TSEnumdefine.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.4/TSMasterAPI/TSFibex_parse.py` & `TSMasterAPI-2.1.0/TSMasterAPI/TSFibex_parse.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.4/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-2.1.0/TSMasterAPI/TSMasterAPI.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.4/TSMasterAPI/TSStructure.py` & `TSMasterAPI-2.1.0/TSMasterAPI/TSStructure.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.4/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-2.1.0/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.0.4
+Version: 2.1.0
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.0.4/license.txt` & `TSMasterAPI-2.1.0/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.4/setup.py` & `TSMasterAPI-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='2.0.4',  # 版本号
+      version='2.1.0',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```


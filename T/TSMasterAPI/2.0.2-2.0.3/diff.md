# Comparing `tmp/TSMasterAPI-2.0.2.tar.gz` & `tmp/TSMasterAPI-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-2.0.2.tar", last modified: Wed May 17 05:25:19 2023, max compression
+gzip compressed data, was "TSMasterAPI-2.0.3.tar", last modified: Wed May 17 06:17:11 2023, max compression
```

## Comparing `TSMasterAPI-2.0.2.tar` & `TSMasterAPI-2.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 05:25:19.904647 TSMasterAPI-2.0.2/
--rw-rw-rw-   0        0        0     1024 2023-05-17 05:25:19.904132 TSMasterAPI-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 05:25:19.894938 TSMasterAPI-2.0.2/TSMasterAPI/
--rw-rw-rw-   0        0        0    42781 2023-05-17 05:24:12.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSBUSDriver.py
--rw-rw-rw-   0        0        0    70944 2023-05-17 05:19:31.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSCommon.py
--rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSDirver.py
--rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSEnumdefine.py
--rw-rw-rw-   0        0        0    22804 2023-05-17 05:00:47.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSFibex_parse.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSFlexRayDriver.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSLINDriver.py
--rw-rw-rw-   0        0        0   151756 2023-04-23 03:00:28.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0    23604 2023-05-17 05:12:41.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSStructure.py
--rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.0.2/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:25:19.903107 TSMasterAPI-2.0.2/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-05-17 05:25:19.000000 TSMasterAPI-2.0.2/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-17 05:25:19.000000 TSMasterAPI-2.0.2/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 05:25:19.000000 TSMasterAPI-2.0.2/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-17 05:25:19.000000 TSMasterAPI-2.0.2/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.0.2/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 05:25:19.904647 TSMasterAPI-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-05-17 05:24:46.000000 TSMasterAPI-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:17:11.596140 TSMasterAPI-2.0.3/
+-rw-rw-rw-   0        0        0     1024 2023-05-17 06:17:11.595632 TSMasterAPI-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 06:17:11.579362 TSMasterAPI-2.0.3/TSMasterAPI/
+-rw-rw-rw-   0        0        0    42782 2023-05-17 06:16:11.000000 TSMasterAPI-2.0.3/TSMasterAPI/TSBUSDriver.py
+-rw-rw-rw-   0        0        0    70948 2023-05-17 06:16:04.000000 TSMasterAPI-2.0.3/TSMasterAPI/TSCommon.py
+-rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.0.3/TSMasterAPI/TSDirver.py
+-rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.0.3/TSMasterAPI/TSEnumdefine.py
+-rw-rw-rw-   0        0        0    22804 2023-05-17 05:00:47.000000 TSMasterAPI-2.0.3/TSMasterAPI/TSFibex_parse.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.0.3/TSMasterAPI/TSFlexRayDriver.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.0.3/TSMasterAPI/TSLINDriver.py
+-rw-rw-rw-   0        0        0   151756 2023-04-23 03:00:28.000000 TSMasterAPI-2.0.3/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0    23604 2023-05-17 05:12:41.000000 TSMasterAPI-2.0.3/TSMasterAPI/TSStructure.py
+-rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.0.3/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:17:11.594103 TSMasterAPI-2.0.3/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-05-17 06:17:11.000000 TSMasterAPI-2.0.3/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-17 06:17:11.000000 TSMasterAPI-2.0.3/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 06:17:11.000000 TSMasterAPI-2.0.3/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-17 06:17:11.000000 TSMasterAPI-2.0.3/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.0.3/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 06:17:11.596655 TSMasterAPI-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-05-17 06:17:11.000000 TSMasterAPI-2.0.3/setup.py
```

### Comparing `TSMasterAPI-2.0.2/PKG-INFO` & `TSMasterAPI-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.0.2
+Version: 2.0.3
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.0.2/TSMasterAPI/TSBUSDriver.py` & `TSMasterAPI-2.0.3/TSMasterAPI/TSBUSDriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:19:14
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-05-17 13:24:03
+LastEditTime: 2023-05-17 14:16:11
 github:https://github.com/sy950915/TSMasterAPI.git
 '''
 import time
-from TSCommon import *
+from .TSCommon import *
 
 Kbps_mapping = {
     "CAN":[[500,2000],[500,2000],[500,2000],[500,2000]],
     "LIN":[19.2,19.2,19.2,19.2],
 }
 
 mapping = {
```

### Comparing `TSMasterAPI-2.0.2/TSMasterAPI/TSCommon.py` & `TSMasterAPI-2.0.3/TSMasterAPI/TSCommon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:59:15
 LastEditors: seven 865762826@qq.com
 LastEditTime: 2023-05-17 13:19:31
 '''
-from TSDirver import *
-from TSStructure import *  
-from TSEnumdefine import *  
-from TSFibex_parse import * 
+from .TSDirver import *
+from .TSStructure import *  
+from .TSEnumdefine import *  
+from .TSFibex_parse import * 
 
 # Common Functions
```

### Comparing `TSMasterAPI-2.0.2/TSMasterAPI/TSDirver.py` & `TSMasterAPI-2.0.3/TSMasterAPI/TSDirver.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.2/TSMasterAPI/TSEnumdefine.py` & `TSMasterAPI-2.0.3/TSMasterAPI/TSEnumdefine.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.2/TSMasterAPI/TSFibex_parse.py` & `TSMasterAPI-2.0.3/TSMasterAPI/TSFibex_parse.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.2/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-2.0.3/TSMasterAPI/TSMasterAPI.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.2/TSMasterAPI/TSStructure.py` & `TSMasterAPI-2.0.3/TSMasterAPI/TSStructure.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.2/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-2.0.3/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.0.2
+Version: 2.0.3
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.0.2/license.txt` & `TSMasterAPI-2.0.3/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.2/setup.py` & `TSMasterAPI-2.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-24 09:26:29
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-05-17 13:24:46
+LastEditTime: 2023-05-17 14:17:11
 FilePath: \VSCode_Pro\Python_Pro\TSMasterApi\setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='2.0.2',  # 版本号
+      version='2.0.3',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```


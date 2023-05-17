# Comparing `tmp/TSMasterAPI-2.0.1.tar.gz` & `tmp/TSMasterAPI-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-2.0.1.tar", last modified: Fri May  5 03:10:44 2023, max compression
+gzip compressed data, was "TSMasterAPI-2.0.2.tar", last modified: Wed May 17 05:25:19 2023, max compression
```

## Comparing `TSMasterAPI-2.0.1.tar` & `TSMasterAPI-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 03:10:44.544637 TSMasterAPI-2.0.1/
--rw-rw-rw-   0        0        0     1024 2023-05-05 03:10:44.544637 TSMasterAPI-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 03:10:44.533488 TSMasterAPI-2.0.1/TSMasterAPI/
--rw-rw-rw-   0        0        0    32271 2023-05-05 03:07:38.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSBUSDriver.py
--rw-rw-rw-   0        0        0    70571 2023-05-05 03:07:30.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSCommon.py
--rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSDirver.py
--rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSEnumdefine.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSFlexRayDriver.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSLINDriver.py
--rw-rw-rw-   0        0        0   151756 2023-04-23 03:00:28.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0    23491 2023-05-05 03:08:22.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSStructure.py
--rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.0.1/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 03:10:44.543583 TSMasterAPI-2.0.1/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-05-05 03:10:44.000000 TSMasterAPI-2.0.1/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-05-05 03:10:44.000000 TSMasterAPI-2.0.1/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 03:10:44.000000 TSMasterAPI-2.0.1/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 03:10:44.000000 TSMasterAPI-2.0.1/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.0.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 03:10:44.544637 TSMasterAPI-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-05-05 03:10:11.000000 TSMasterAPI-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:25:19.904647 TSMasterAPI-2.0.2/
+-rw-rw-rw-   0        0        0     1024 2023-05-17 05:25:19.904132 TSMasterAPI-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 05:25:19.894938 TSMasterAPI-2.0.2/TSMasterAPI/
+-rw-rw-rw-   0        0        0    42781 2023-05-17 05:24:12.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSBUSDriver.py
+-rw-rw-rw-   0        0        0    70944 2023-05-17 05:19:31.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSCommon.py
+-rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSDirver.py
+-rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSEnumdefine.py
+-rw-rw-rw-   0        0        0    22804 2023-05-17 05:00:47.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSFibex_parse.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSFlexRayDriver.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSLINDriver.py
+-rw-rw-rw-   0        0        0   151756 2023-04-23 03:00:28.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0    23604 2023-05-17 05:12:41.000000 TSMasterAPI-2.0.2/TSMasterAPI/TSStructure.py
+-rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.0.2/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:25:19.903107 TSMasterAPI-2.0.2/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-05-17 05:25:19.000000 TSMasterAPI-2.0.2/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-17 05:25:19.000000 TSMasterAPI-2.0.2/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 05:25:19.000000 TSMasterAPI-2.0.2/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-17 05:25:19.000000 TSMasterAPI-2.0.2/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 05:25:19.904647 TSMasterAPI-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-05-17 05:24:46.000000 TSMasterAPI-2.0.2/setup.py
```

### Comparing `TSMasterAPI-2.0.1/PKG-INFO` & `TSMasterAPI-2.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.0.1
+Version: 2.0.2
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.0.1/TSMasterAPI/TSCommon.py` & `TSMasterAPI-2.0.2/TSMasterAPI/TSCommon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:59:15
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-04-23 13:36:50
+LastEditTime: 2023-05-17 13:19:31
 '''
-from .TSDirver import *
-from .TSStructure import *  
-from .TSEnumdefine import *  
-
+from TSDirver import *
+from TSStructure import *  
+from TSEnumdefine import *  
+from TSFibex_parse import * 
 
 # Common Functions
 
 
 
 
 
@@ -150,15 +150,15 @@
 tsapp_configure_canfd_regs.argtypes = [s32, c_float, s32,s32,s32,s32,c_float, s32,s32,s32,s32,s32,s32, c_bool]
 tsapp_configure_canfd_regs.restype = TS_ReturnType
 tsapp_configure_canfd_regs.errcheck = check_status_operation
 
 # LIN 通道参数配置
 tsapp_configure_baudrate_lin = dll.tsapp_configure_baudrate_lin
 # (AIdxChn: CHANNEL_INDEX, ABaudrateKbps: int, LIN_PROTOCOL: LIN_PROTOCOL)
-tsapp_configure_baudrate_lin.argtypes = [s32, s32, s32]
+tsapp_configure_baudrate_lin.argtypes = [s32, c_float, s32]
 tsapp_configure_baudrate_lin.restype = TS_ReturnType
 tsapp_configure_baudrate_lin.errcheck = check_status_operation
 
 # 设置LIN模式
 tslin_set_node_funtiontype = dll.tslin_set_node_funtiontype
 # (AIdxChn: CHANNEL_INDEX, TLINNodeType: T_LIN_NODE_FUNCTION)
 tslin_set_node_funtiontype.argtypes=[s32, s32]
@@ -788,14 +788,18 @@
 
 # 使能wakeup_pattern
 tsflexray_wakeup_pattern = dll.tsflexray_wakeup_pattern
 tsflexray_wakeup_pattern.argtypes = [s32,s32]  
 tsflexray_wakeup_pattern.restype = TS_ReturnType
 tsflexray_wakeup_pattern.errcheck = check_status_operation
 
+tsflexray_set_controller_frametrigger = dll.tsflexray_set_controller_frametrigger
+tsflexray_set_controller_frametrigger.argtypes = [s32,PLibFlexray_controller_config,c_char_p,s32,PLibTrigger_def,s32,s32]  
+tsflexray_set_controller_frametrigger.restype = TS_ReturnType
+tsflexray_set_controller_frametrigger.errcheck = check_status_operation
 
 # flexray 发送
 # 异步单帧发送flexray报文
 tsapp_transmit_flexray_async = dll.tsapp_transmit_flexray_async
 tsapp_transmit_flexray_async.argtypes = [PFlexray]  
 tsapp_transmit_flexray_async.restype = TS_ReturnType
 tsapp_transmit_flexray_async.errcheck = check_status_operation
```

### Comparing `TSMasterAPI-2.0.1/TSMasterAPI/TSDirver.py` & `TSMasterAPI-2.0.2/TSMasterAPI/TSDirver.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.1/TSMasterAPI/TSEnumdefine.py` & `TSMasterAPI-2.0.2/TSMasterAPI/TSEnumdefine.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.1/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-2.0.2/TSMasterAPI/TSMasterAPI.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.1/TSMasterAPI/TSStructure.py` & `TSMasterAPI-2.0.2/TSMasterAPI/TSStructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,15 +394,15 @@
                 ("config_byte", c_uint8),  # bit0: 1：启用cha上终端电阻 0：不启用
                 # bit1: 1：启用chb上终端电阻 0：不启用
                 # bit2: 1：启用接收FIFO     0：不启用
                 # bit4: 1：cha桥接使能    0：不使能
                 # bit5: 1：chb桥接使能    0：不使能
                 # bit6: 1:not ignore NULL Frame  0: ignore NULL Frame
                 ]
-
+PLibFlexray_controller_config = POINTER(TLibFlexray_controller_config) 
 class TLibTrigger_def(Structure):
     """
     Trigger 结构体
     作用:调度表,配置要下发的报文
     关联函数:tsflexray_set_controller_frametrigger
     """
     _pack_ = 1
@@ -415,15 +415,15 @@
                 # bit3: 传输模式，0 表示连续传输，1表示单次触发
                 # bit4: 是否为冷启动报文，只有缓冲区0可以置1
                 # bit5: 是否为同步报文，只有缓冲区0 / 1 可以置1
                 # bit6:
                 # bit7: 帧类型：0 - 静态，1 - 动态
                 ("recv", c_uint8),
                 ]
-
+PLibTrigger_def = POINTER(TLibTrigger_def)
 class TLIBHWInfo(Structure):
     """
     描述:TLib 的硬件信息结构体类型
     """
     _pack_ = 1
     _fields_ = [("FDeviceType", c_int32),
                 ("FDeviceIndex", c_int32),
```

### Comparing `TSMasterAPI-2.0.1/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-2.0.2/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.0.1
+Version: 2.0.2
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.0.1/license.txt` & `TSMasterAPI-2.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.1/setup.py` & `TSMasterAPI-2.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-24 09:26:29
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-05-05 11:10:11
+LastEditTime: 2023-05-17 13:24:46
 FilePath: \VSCode_Pro\Python_Pro\TSMasterApi\setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='2.0.1',  # 版本号
+      version='2.0.2',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```


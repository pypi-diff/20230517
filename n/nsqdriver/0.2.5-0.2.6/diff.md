# Comparing `tmp/nsqdriver-0.2.5.tar.gz` & `tmp/nsqdriver-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsqdriver-0.2.5.tar", last modified: Mon Mar 27 14:22:53 2023, max compression
+gzip compressed data, was "nsqdriver-0.2.6.tar", last modified: Wed May 17 07:10:58 2023, max compression
```

## Comparing `nsqdriver-0.2.5.tar` & `nsqdriver-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:22:53.212171 nsqdriver-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-27 14:22:53.212171 nsqdriver-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:22:53.208171 nsqdriver-0.2.5/nsqdriver/
--rw-r--r--   0 runner    (1001) docker     (123)    19233 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/nsqdriver/NS_MCI.py
--rw-r--r--   0 runner    (1001) docker     (123)    22747 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/nsqdriver/NS_QSYNC.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/nsqdriver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/nsqdriver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/nsqdriver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:22:53.212171 nsqdriver-0.2.5/nsqdriver/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/nsqdriver/wrapper/AWG_ADC.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/nsqdriver/wrapper/ND_NSMCI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/nsqdriver/wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:22:53.212171 nsqdriver-0.2.5/nsqdriver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-27 14:22:53.000000 nsqdriver-0.2.5/nsqdriver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-27 14:22:53.000000 nsqdriver-0.2.5/nsqdriver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:22:53.000000 nsqdriver-0.2.5/nsqdriver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 14:22:53.000000 nsqdriver-0.2.5/nsqdriver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-27 14:22:53.000000 nsqdriver-0.2.5/nsqdriver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:22:53.212171 nsqdriver-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:22:53.212171 nsqdriver-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/tests/test_cy_gen_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/tests/test_demod_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/tests/test_driver_info_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/tests/test_init_device.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/tests/test_mixer_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/tests/test_param_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/tests/test_rfskit_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-03-27 14:22:48.000000 nsqdriver-0.2.5/tests/test_rpc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:58.085828 nsqdriver-0.2.6/nsqdriver/
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/NS_CST.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/NS_MCI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22747 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/NS_QSYNC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/nsqdriver/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/wrapper/AWG_ADC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/wrapper/ND_NSMCI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/nsqdriver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-17 07:10:58.000000 nsqdriver-0.2.6/nsqdriver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-17 07:10:58.000000 nsqdriver-0.2.6/nsqdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:10:58.000000 nsqdriver-0.2.6/nsqdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 07:10:58.000000 nsqdriver-0.2.6/nsqdriver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 07:10:58.000000 nsqdriver-0.2.6/nsqdriver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_cy_gen_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_demod_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_driver_info_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_init_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_mixer_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_param_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_rfskit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_rpc_parser.py
```

### Comparing `nsqdriver-0.2.5/PKG-INFO` & `nsqdriver-0.2.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsqdriver
-Version: 0.2.5
+Version: 0.2.6
 Summary: Naishu Q series quantum measurement and control equipment driver interface
 Home-page: https://g2hoyqcmh4.feishu.cn/wiki/wikcnzvyMd82DLZUe2NsI6HxsFc
 Author: Naishu Technology
 Author-email: jilianyi@naishu.tech
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nsqdriver-0.2.5/README.md` & `nsqdriver-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.5/nsqdriver/NS_MCI.py` & `nsqdriver-0.2.6/nsqdriver/NS_MCI.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,21 +261,17 @@
         """
         查询设备属性，获取数据
 
         """
         if not self.device_online:
             return
         print_debug(f'Driver: get操作被调用{name}')
-        if name in {'TraceIQ', 'IQ', 'TraceData', 'IQData'}:
-            func = self.fast_rpc.rpc_get
-        else:
-            func = self.handle.rpc_get
-
         self.has_start_capture = False
 
+        func = self.fast_rpc.rpc_get
         tmp = func(name, channel, value)
         tmp = RPCValueParser.load(tmp)
         return tmp
 
     def update_firmware(self, file_path, target='all'):
         if not self.device_online:
             return
```

### Comparing `nsqdriver-0.2.5/nsqdriver/NS_QSYNC.py` & `nsqdriver-0.2.6/nsqdriver/NS_QSYNC.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.5/nsqdriver/wrapper/AWG_ADC.py` & `nsqdriver-0.2.6/nsqdriver/wrapper/AWG_ADC.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.5/nsqdriver/wrapper/ND_NSMCI.py` & `nsqdriver-0.2.6/nsqdriver/wrapper/ND_NSMCI.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.5/nsqdriver.egg-info/PKG-INFO` & `nsqdriver-0.2.6/nsqdriver.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsqdriver
-Version: 0.2.5
+Version: 0.2.6
 Summary: Naishu Q series quantum measurement and control equipment driver interface
 Home-page: https://g2hoyqcmh4.feishu.cn/wiki/wikcnzvyMd82DLZUe2NsI6HxsFc
 Author: Naishu Technology
 Author-email: jilianyi@naishu.tech
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nsqdriver-0.2.5/nsqdriver.egg-info/SOURCES.txt` & `nsqdriver-0.2.6/nsqdriver.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 README.md
 setup.py
+nsqdriver/NS_CST.py
 nsqdriver/NS_MCI.py
 nsqdriver/NS_QSYNC.py
 nsqdriver/__init__.py
 nsqdriver/common.py
 nsqdriver/setup.py
 nsqdriver.egg-info/PKG-INFO
 nsqdriver.egg-info/SOURCES.txt
```

### Comparing `nsqdriver-0.2.5/setup.py` & `nsqdriver-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.5/tests/test_cy_gen_wave.py` & `nsqdriver-0.2.6/tests/test_cy_gen_wave.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.5/tests/test_demod_speed.py` & `nsqdriver-0.2.6/tests/test_demod_speed.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.5/tests/test_driver_info_memory.py` & `nsqdriver-0.2.6/tests/test_driver_info_memory.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.5/tests/test_param_memory.py` & `nsqdriver-0.2.6/tests/test_param_memory.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.5/tests/test_rfskit_base.py` & `nsqdriver-0.2.6/tests/test_rfskit_base.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.5/tests/test_rpc_parser.py` & `nsqdriver-0.2.6/tests/test_rpc_parser.py`

 * *Files identical despite different names*


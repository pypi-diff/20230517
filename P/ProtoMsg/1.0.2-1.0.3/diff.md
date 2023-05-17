# Comparing `tmp/ProtoMsg-1.0.2.tar.gz` & `tmp/ProtoMsg-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProtoMsg-1.0.2.tar", last modified: Wed May 17 16:06:45 2023, max compression
+gzip compressed data, was "ProtoMsg-1.0.3.tar", last modified: Wed May 17 16:12:11 2023, max compression
```

## Comparing `ProtoMsg-1.0.2.tar` & `ProtoMsg-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 16:06:45.733543 ProtoMsg-1.0.2/
--rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 16:06:45.733428 ProtoMsg-1.0.2/PKG-INFO
-drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 16:06:45.732800 ProtoMsg-1.0.2/ProtoMsg/
--rw-r--r--   0 jove       (501) staff       (20)     1109 2023-05-16 18:58:01.000000 ProtoMsg-1.0.2/ProtoMsg/ControlIn_pb2.py
--rw-r--r--   0 jove       (501) staff       (20)     1196 2023-05-16 18:58:01.000000 ProtoMsg-1.0.2/ProtoMsg/ControlOut_pb2.py
--rw-r--r--   0 jove       (501) staff       (20)     1817 2023-05-16 18:58:01.000000 ProtoMsg-1.0.2/ProtoMsg/KafkaMessage_pb2.py
--rw-r--r--   0 jove       (501) staff       (20)     2061 2023-05-16 19:09:13.000000 ProtoMsg-1.0.2/ProtoMsg/SegmentCommon_pb2.py
--rw-r--r--   0 jove       (501) staff       (20)     1389 2023-05-16 18:58:01.000000 ProtoMsg-1.0.2/ProtoMsg/SegmentIn_pb2.py
--rw-r--r--   0 jove       (501) staff       (20)     1241 2023-05-16 19:12:45.000000 ProtoMsg-1.0.2/ProtoMsg/SegmentOut_pb2.py
--rw-r--r--   0 jove       (501) staff       (20)      345 2023-05-17 15:57:27.000000 ProtoMsg-1.0.2/ProtoMsg/__init__.py
--rw-r--r--   0 jove       (501) staff       (20)       22 2023-05-17 16:06:43.000000 ProtoMsg-1.0.2/ProtoMsg/version.py
-drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 16:06:45.733275 ProtoMsg-1.0.2/ProtoMsg.egg-info/
--rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 16:06:45.000000 ProtoMsg-1.0.2/ProtoMsg.egg-info/PKG-INFO
--rw-r--r--   0 jove       (501) staff       (20)      342 2023-05-17 16:06:45.000000 ProtoMsg-1.0.2/ProtoMsg.egg-info/SOURCES.txt
--rw-r--r--   0 jove       (501) staff       (20)        1 2023-05-17 16:06:45.000000 ProtoMsg-1.0.2/ProtoMsg.egg-info/dependency_links.txt
--rw-r--r--   0 jove       (501) staff       (20)        9 2023-05-17 16:06:45.000000 ProtoMsg-1.0.2/ProtoMsg.egg-info/top_level.txt
--rw-r--r--   0 jove       (501) staff       (20)       38 2023-05-17 16:06:45.733586 ProtoMsg-1.0.2/setup.cfg
--rw-r--r--   0 jove       (501) staff       (20)      555 2023-05-17 16:06:43.000000 ProtoMsg-1.0.2/setup.py
+drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 16:12:11.643058 ProtoMsg-1.0.3/
+-rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 16:12:11.642936 ProtoMsg-1.0.3/PKG-INFO
+drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 16:12:11.642296 ProtoMsg-1.0.3/ProtoMsg/
+-rw-r--r--   0 jove       (501) staff       (20)     1109 2023-05-16 18:58:01.000000 ProtoMsg-1.0.3/ProtoMsg/ControlIn_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)     1196 2023-05-16 18:58:01.000000 ProtoMsg-1.0.3/ProtoMsg/ControlOut_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)     1853 2023-05-17 16:10:59.000000 ProtoMsg-1.0.3/ProtoMsg/KafkaMessage_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)     2061 2023-05-16 19:09:13.000000 ProtoMsg-1.0.3/ProtoMsg/SegmentCommon_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)     1398 2023-05-17 16:11:07.000000 ProtoMsg-1.0.3/ProtoMsg/SegmentIn_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)     1241 2023-05-16 19:12:45.000000 ProtoMsg-1.0.3/ProtoMsg/SegmentOut_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)      369 2023-05-17 16:10:41.000000 ProtoMsg-1.0.3/ProtoMsg/__init__.py
+-rw-r--r--   0 jove       (501) staff       (20)       22 2023-05-17 16:06:43.000000 ProtoMsg-1.0.3/ProtoMsg/version.py
+drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 16:12:11.642774 ProtoMsg-1.0.3/ProtoMsg.egg-info/
+-rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 16:12:11.000000 ProtoMsg-1.0.3/ProtoMsg.egg-info/PKG-INFO
+-rw-r--r--   0 jove       (501) staff       (20)      342 2023-05-17 16:12:11.000000 ProtoMsg-1.0.3/ProtoMsg.egg-info/SOURCES.txt
+-rw-r--r--   0 jove       (501) staff       (20)        1 2023-05-17 16:12:11.000000 ProtoMsg-1.0.3/ProtoMsg.egg-info/dependency_links.txt
+-rw-r--r--   0 jove       (501) staff       (20)        9 2023-05-17 16:12:11.000000 ProtoMsg-1.0.3/ProtoMsg.egg-info/top_level.txt
+-rw-r--r--   0 jove       (501) staff       (20)       38 2023-05-17 16:12:11.643103 ProtoMsg-1.0.3/setup.cfg
+-rw-r--r--   0 jove       (501) staff       (20)      555 2023-05-17 16:12:05.000000 ProtoMsg-1.0.3/setup.py
```

### Comparing `ProtoMsg-1.0.2/ProtoMsg/ControlIn_pb2.py` & `ProtoMsg-1.0.3/ProtoMsg/ControlIn_pb2.py`

 * *Files identical despite different names*

### Comparing `ProtoMsg-1.0.2/ProtoMsg/ControlOut_pb2.py` & `ProtoMsg-1.0.3/ProtoMsg/ControlOut_pb2.py`

 * *Files identical despite different names*

### Comparing `ProtoMsg-1.0.2/ProtoMsg/KafkaMessage_pb2.py` & `ProtoMsg-1.0.3/ProtoMsg/KafkaMessage_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import SegmentIn_pb2 as SegmentIn__pb2
-import ControlIn_pb2 as ControlIn__pb2
-import ControlOut_pb2 as ControlOut__pb2
-import SegmentOut_pb2 as SegmentOut__pb2
+import ProtoMsg.SegmentIn_pb2 as SegmentIn__pb2
+import ProtoMsg.ControlIn_pb2 as ControlIn__pb2
+import ProtoMsg.ControlOut_pb2 as ControlOut__pb2
+import ProtoMsg.SegmentOut_pb2 as SegmentOut__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12KafkaMessage.proto\x12\x11\x63om.loorr.message\x1a\x0fSegmentIn.proto\x1a\x0f\x43ontrolIn.proto\x1a\x10\x43ontrolOut.proto\x1a\x10SegmentOut.proto\"\xac\x02\n\x0cKafkaMessage\x12\x0e\n\x06seqNum\x18\x01 \x01(\x03\x12\x0f\n\x07reqTime\x18\x02 \x01(\x03\x12\x11\n\terrorCode\x18\x04 \x01(\t\x12\x10\n\x08\x65rrorMsg\x18\x05 \x01(\t\x12\x33\n\nsegmentOut\x18\n \x01(\x0b\x32\x1d.com.loorr.message.SegmentOutH\x00\x12\x31\n\tsegmentIn\x18\x0b \x01(\x0b\x32\x1c.com.loorr.message.SegmentInH\x00\x12\x31\n\tcontrolIn\x18\x0c \x01(\x0b\x32\x1c.com.loorr.message.ControlInH\x00\x12\x33\n\ncontrolOut\x18\r \x01(\x0b\x32\x1d.com.loorr.message.ControlOutH\x00\x42\x06\n\x04\x62odyB\x15\x42\x11KafkaMessageProtoP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'KafkaMessage_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `ProtoMsg-1.0.2/ProtoMsg/SegmentCommon_pb2.py` & `ProtoMsg-1.0.3/ProtoMsg/SegmentCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `ProtoMsg-1.0.2/ProtoMsg/SegmentIn_pb2.py` & `ProtoMsg-1.0.3/ProtoMsg/SegmentIn_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import SegmentCommon_pb2 as SegmentCommon__pb2
+import ProtoMsg.SegmentCommon_pb2 as SegmentCommon__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fSegmentIn.proto\x12\x11\x63om.loorr.message\x1a\x13SegmentCommon.proto\"\xae\x01\n\tSegmentIn\x12\x0f\n\x07imageId\x18\x01 \x01(\x03\x12\x11\n\timagePath\x18\x02 \x01(\t\x12,\n\x04type\x18\x03 \x01(\x0e\x32\x1e.com.loorr.message.SegmentType\x12(\n\x06points\x18\x04 \x03(\x0b\x32\x18.com.loorr.message.Point\x12%\n\x05\x62oxes\x18\x05 \x03(\x0b\x32\x16.com.loorr.message.BoxB\x12\x42\x0eSegmentInProtoP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'SegmentIn_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `ProtoMsg-1.0.2/ProtoMsg/SegmentOut_pb2.py` & `ProtoMsg-1.0.3/ProtoMsg/SegmentOut_pb2.py`

 * *Files identical despite different names*

### Comparing `ProtoMsg-1.0.2/setup.py` & `ProtoMsg-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='ProtoMsg',
-      version='1.0.2',
+      version='1.0.3',
       description='scu-yang-proto-msg',
       author='loorr',
       author_email='zjianfa@foxmail.com',
       requires=['protobuf'],  # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       # packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```


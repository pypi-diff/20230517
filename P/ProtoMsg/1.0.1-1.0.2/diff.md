# Comparing `tmp/ProtoMsg-1.0.1.tar.gz` & `tmp/ProtoMsg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProtoMsg-1.0.1.tar", last modified: Wed May 17 15:59:14 2023, max compression
+gzip compressed data, was "ProtoMsg-1.0.2.tar", last modified: Wed May 17 16:06:45 2023, max compression
```

## Comparing `ProtoMsg-1.0.1.tar` & `ProtoMsg-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,18 @@
-drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 15:59:14.441460 ProtoMsg-1.0.1/
--rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 15:59:14.441347 ProtoMsg-1.0.1/PKG-INFO
-drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 15:59:14.441191 ProtoMsg-1.0.1/ProtoMsg.egg-info/
--rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 15:59:14.000000 ProtoMsg-1.0.1/ProtoMsg.egg-info/PKG-INFO
--rw-r--r--   0 jove       (501) staff       (20)      136 2023-05-17 15:59:14.000000 ProtoMsg-1.0.1/ProtoMsg.egg-info/SOURCES.txt
--rw-r--r--   0 jove       (501) staff       (20)        1 2023-05-17 15:59:14.000000 ProtoMsg-1.0.1/ProtoMsg.egg-info/dependency_links.txt
--rw-r--r--   0 jove       (501) staff       (20)        1 2023-05-17 15:59:14.000000 ProtoMsg-1.0.1/ProtoMsg.egg-info/top_level.txt
--rw-r--r--   0 jove       (501) staff       (20)       38 2023-05-17 15:59:14.441500 ProtoMsg-1.0.1/setup.cfg
--rw-r--r--   0 jove       (501) staff       (20)      555 2023-05-17 15:58:34.000000 ProtoMsg-1.0.1/setup.py
+drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 16:06:45.733543 ProtoMsg-1.0.2/
+-rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 16:06:45.733428 ProtoMsg-1.0.2/PKG-INFO
+drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 16:06:45.732800 ProtoMsg-1.0.2/ProtoMsg/
+-rw-r--r--   0 jove       (501) staff       (20)     1109 2023-05-16 18:58:01.000000 ProtoMsg-1.0.2/ProtoMsg/ControlIn_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)     1196 2023-05-16 18:58:01.000000 ProtoMsg-1.0.2/ProtoMsg/ControlOut_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)     1817 2023-05-16 18:58:01.000000 ProtoMsg-1.0.2/ProtoMsg/KafkaMessage_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)     2061 2023-05-16 19:09:13.000000 ProtoMsg-1.0.2/ProtoMsg/SegmentCommon_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)     1389 2023-05-16 18:58:01.000000 ProtoMsg-1.0.2/ProtoMsg/SegmentIn_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)     1241 2023-05-16 19:12:45.000000 ProtoMsg-1.0.2/ProtoMsg/SegmentOut_pb2.py
+-rw-r--r--   0 jove       (501) staff       (20)      345 2023-05-17 15:57:27.000000 ProtoMsg-1.0.2/ProtoMsg/__init__.py
+-rw-r--r--   0 jove       (501) staff       (20)       22 2023-05-17 16:06:43.000000 ProtoMsg-1.0.2/ProtoMsg/version.py
+drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 16:06:45.733275 ProtoMsg-1.0.2/ProtoMsg.egg-info/
+-rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 16:06:45.000000 ProtoMsg-1.0.2/ProtoMsg.egg-info/PKG-INFO
+-rw-r--r--   0 jove       (501) staff       (20)      342 2023-05-17 16:06:45.000000 ProtoMsg-1.0.2/ProtoMsg.egg-info/SOURCES.txt
+-rw-r--r--   0 jove       (501) staff       (20)        1 2023-05-17 16:06:45.000000 ProtoMsg-1.0.2/ProtoMsg.egg-info/dependency_links.txt
+-rw-r--r--   0 jove       (501) staff       (20)        9 2023-05-17 16:06:45.000000 ProtoMsg-1.0.2/ProtoMsg.egg-info/top_level.txt
+-rw-r--r--   0 jove       (501) staff       (20)       38 2023-05-17 16:06:45.733586 ProtoMsg-1.0.2/setup.cfg
+-rw-r--r--   0 jove       (501) staff       (20)      555 2023-05-17 16:06:43.000000 ProtoMsg-1.0.2/setup.py
```

### Comparing `ProtoMsg-1.0.1/setup.py` & `ProtoMsg-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='ProtoMsg',
-      version='1.0.1',
+      version='1.0.2',
       description='scu-yang-proto-msg',
       author='loorr',
       author_email='zjianfa@foxmail.com',
       requires=['protobuf'],  # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       # packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```


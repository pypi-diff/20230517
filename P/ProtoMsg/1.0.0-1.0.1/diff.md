# Comparing `tmp/ProtoMsg-1.0.0.tar.gz` & `tmp/ProtoMsg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProtoMsg-1.0.0.tar", last modified: Wed May 17 15:50:11 2023, max compression
+gzip compressed data, was "ProtoMsg-1.0.1.tar", last modified: Wed May 17 15:59:14 2023, max compression
```

## Comparing `ProtoMsg-1.0.0.tar` & `ProtoMsg-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 15:50:11.040064 ProtoMsg-1.0.0/
--rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 15:50:11.039948 ProtoMsg-1.0.0/PKG-INFO
-drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 15:50:11.039795 ProtoMsg-1.0.0/ProtoMsg.egg-info/
--rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 15:50:11.000000 ProtoMsg-1.0.0/ProtoMsg.egg-info/PKG-INFO
--rw-r--r--   0 jove       (501) staff       (20)      136 2023-05-17 15:50:11.000000 ProtoMsg-1.0.0/ProtoMsg.egg-info/SOURCES.txt
--rw-r--r--   0 jove       (501) staff       (20)        1 2023-05-17 15:50:11.000000 ProtoMsg-1.0.0/ProtoMsg.egg-info/dependency_links.txt
--rw-r--r--   0 jove       (501) staff       (20)        1 2023-05-17 15:50:11.000000 ProtoMsg-1.0.0/ProtoMsg.egg-info/top_level.txt
--rw-r--r--   0 jove       (501) staff       (20)       38 2023-05-17 15:50:11.040109 ProtoMsg-1.0.0/setup.cfg
--rw-r--r--   0 jove       (501) staff       (20)      555 2023-05-17 15:49:34.000000 ProtoMsg-1.0.0/setup.py
+drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 15:59:14.441460 ProtoMsg-1.0.1/
+-rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 15:59:14.441347 ProtoMsg-1.0.1/PKG-INFO
+drwxr-xr-x   0 jove       (501) staff       (20)        0 2023-05-17 15:59:14.441191 ProtoMsg-1.0.1/ProtoMsg.egg-info/
+-rw-r--r--   0 jove       (501) staff       (20)      167 2023-05-17 15:59:14.000000 ProtoMsg-1.0.1/ProtoMsg.egg-info/PKG-INFO
+-rw-r--r--   0 jove       (501) staff       (20)      136 2023-05-17 15:59:14.000000 ProtoMsg-1.0.1/ProtoMsg.egg-info/SOURCES.txt
+-rw-r--r--   0 jove       (501) staff       (20)        1 2023-05-17 15:59:14.000000 ProtoMsg-1.0.1/ProtoMsg.egg-info/dependency_links.txt
+-rw-r--r--   0 jove       (501) staff       (20)        1 2023-05-17 15:59:14.000000 ProtoMsg-1.0.1/ProtoMsg.egg-info/top_level.txt
+-rw-r--r--   0 jove       (501) staff       (20)       38 2023-05-17 15:59:14.441500 ProtoMsg-1.0.1/setup.cfg
+-rw-r--r--   0 jove       (501) staff       (20)      555 2023-05-17 15:58:34.000000 ProtoMsg-1.0.1/setup.py
```

### Comparing `ProtoMsg-1.0.0/setup.py` & `ProtoMsg-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='ProtoMsg',
-      version='1.0.0',
+      version='1.0.1',
       description='scu-yang-proto-msg',
       author='loorr',
       author_email='zjianfa@foxmail.com',
       requires=['protobuf'],  # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       # packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```


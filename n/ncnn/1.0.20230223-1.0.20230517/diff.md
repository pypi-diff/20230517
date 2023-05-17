# Comparing `tmp/ncnn-1.0.20230223.tar.gz` & `tmp/ncnn-1.0.20230517.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncnn-1.0.20230223.tar", last modified: Thu Feb 23 03:46:15 2023, max compression
+gzip compressed data, was "ncnn-1.0.20230517.tar", last modified: Wed May 17 06:52:08 2023, max compression
```

## Comparing `ncnn-1.0.20230223.tar` & `ncnn-1.0.20230517.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 03:46:15.013094 ncnn-1.0.20230223/
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26717 2023-02-23 03:46:15.013094 ncnn-1.0.20230223/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 03:46:15.009094 ncnn-1.0.20230223/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 03:46:15.009094 ncnn-1.0.20230223/python/ncnn/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 03:46:15.013094 ncnn-1.0.20230223/python/ncnn/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/fasterrcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/mobilenetssd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/mobilenetv2ssdlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/mobilenetv3ssdlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/model_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/model_zoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/nanodet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/peleenetssd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/rfcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/shufflenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/simplepose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/squeezenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/squeezenetssd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11162 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/yolact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/yolov2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/yolov3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/yolov4.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/model_zoo/yolov5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 03:46:15.013094 ncnn-1.0.20230223/python/ncnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/python/ncnn/utils/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 03:46:15.009094 ncnn-1.0.20230223/python/ncnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26717 2023-02-23 03:46:14.000000 ncnn-1.0.20230223/python/ncnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-23 03:46:15.000000 ncnn-1.0.20230223/python/ncnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 03:46:14.000000 ncnn-1.0.20230223/python/ncnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-23 03:46:14.000000 ncnn-1.0.20230223/python/ncnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-23 03:46:14.000000 ncnn-1.0.20230223/python/ncnn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 03:46:15.013094 ncnn-1.0.20230223/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-02-23 03:45:52.000000 ncnn-1.0.20230223/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:08.755735 ncnn-1.0.20230517/
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26798 2023-05-17 06:52:08.755735 ncnn-1.0.20230517/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25943 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:08.739735 ncnn-1.0.20230517/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:08.739735 ncnn-1.0.20230517/python/ncnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:08.751735 ncnn-1.0.20230517/python/ncnn/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/fasterrcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/mobilenetssd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/mobilenetv2ssdlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/mobilenetv3ssdlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/model_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/model_zoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/nanodet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/peleenetssd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/rfcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/shufflenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/simplepose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/squeezenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/squeezenetssd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11162 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/yolact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/yolov2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/yolov3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/yolov4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/yolov5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/yolov7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/model_zoo/yolov8.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:08.755735 ncnn-1.0.20230517/python/ncnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/python/ncnn/utils/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:08.743735 ncnn-1.0.20230517/python/ncnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26798 2023-05-17 06:52:08.000000 ncnn-1.0.20230517/python/ncnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-17 06:52:08.000000 ncnn-1.0.20230517/python/ncnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:52:08.000000 ncnn-1.0.20230517/python/ncnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-17 06:52:08.000000 ncnn-1.0.20230517/python/ncnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 06:52:08.000000 ncnn-1.0.20230517/python/ncnn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 06:52:08.755735 ncnn-1.0.20230517/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-17 06:51:44.000000 ncnn-1.0.20230517/setup.py
```

### Comparing `ncnn-1.0.20230223/LICENSE.txt` & `ncnn-1.0.20230517/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/PKG-INFO` & `ncnn-1.0.20230517/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncnn
-Version: 1.0.20230223
+Version: 1.0.20230517
 Summary: ncnn is a high-performance neural network inference framework optimized for the mobile platform
 Home-page: https://github.com/Tencent/ncnn
 Author: nihui
 Author-email: nihuini@tencent.com
 Maintainer: caishanli
 Maintainer-email: caishanli25@gmail.com
 License: BSD-3
@@ -74,15 +74,15 @@
 | Windows           | [![Build Status][pass-windows-x86-cpu]][ci-windows-x86-cpu]         | [![Build Status][pass-windows-x64-cpu]][ci-windows-x64-cpu]                     | —                                                               | [![Build Status][pass-windows-x64-gpu]][ci-windows-x64-gpu]         |
 | Windows (ARM)     | [![Build Status][pass-windows-arm-cpu]][ci-windows-arm-cpu]         | [![Build Status][pass-windows-arm64-cpu]][ci-windows-arm64-cpu]                 | —                                                               | —                                                                   |
 | macOS             | —                                                                   | [![Build Status][pass-macos-x64-cpu]][ci-macos-x64-cpu]                         | —                                                               | [![Build Status][pass-macos-x64-gpu]][ci-macos-x64-gpu]             |
 | macOS (ARM)       | —                                                                   | [![Build Status][pass-macos-arm64-cpu]][ci-macos-arm64-cpu]                     | —                                                               | [![Build Status][pass-macos-arm64-gpu]][ci-macos-arm64-gpu]         |
 | Android           | [![Build Status][pass-android-armv7-cpu]][ci-android-armv7-cpu]     | [![Build Status][pass-android-armv8-cpu]][ci-android-armv8-cpu]                 | [![Build Status][pass-android-armv7-gpu]][ci-android-armv7-gpu] | [![Build Status][pass-android-armv8-gpu]][ci-android-armv8-gpu]     |
 | Android-x86       | [![Build Status][pass-android-x86-cpu]][ci-android-x86-cpu]         | [![Build Status][pass-android-x64-cpu]][ci-android-x64-cpu]                     | [![Build Status][pass-android-x86-gpu]][ci-android-x86-gpu]     | [![Build Status][pass-android-x64-gpu]][ci-android-x64-gpu]         |
 | iOS               | [![Build Status][pass-ios-cpu]][ci-ios-cpu]                         | [![Build Status][pass-ios-cpu]][ci-ios-cpu]                                     | —                                                               | [![Build Status][pass-ios-arm64-gpu]][ci-ios-arm64-gpu]             |
-| iOS Simulator     | [![Build Status][pass-ios-simulator]][ci-ios-simulator]             | [![Build Status][pass-ios-simulator]][ci-ios-simulator]                         | —                                                               | —                                                                   |
+| iOS Simulator     | [![Build Status][pass-ios-simulator]][ci-ios-simulator]             | [![Build Status][pass-ios-simulator]][ci-ios-simulator]                         | —                                                               | [![Build Status][pass-ios-simulator-gpu]][ci-ios-simulator-gpu]     |
 | WebAssembly       | [![Build Status][pass-web-assembly]][ci-web-assembly]               | —                                                                               | —                                                               | —                                                                   |
 | RISC-V GCC/Newlib | [![Build Status][pass-elf-riscv32-cpu-gcc]][ci-elf-riscv32-cpu-gcc] | [![Build Status][pass-elf-riscv64-cpu-gcc]][ci-elf-riscv64-cpu-gcc]             | —                                                               | —                                                                   |
 
 [pass-android-armv7-cpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv7-cpu.yml?branch=master
 [pass-android-armv7-gpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv7-gpu.yml?branch=master
 [pass-android-armv8-cpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv8-cpu.yml?branch=master
 [pass-android-armv8-gpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv8-gpu.yml?branch=master
@@ -233,14 +233,15 @@
 - [Build for Hisilicon platform with cross-compiling](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-hisilicon-platform-with-cross-compiling)
 - [Build for Android](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-android)
 - [Build for iOS on macOS with xcode](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-ios-on-macos-with-xcode)
 - [Build for WebAssembly](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-webassembly)
 - [Build for AllWinner D1](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-allwinner-d1)
 - [Build for Loongson 2K1000](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-loongson-2k1000)
 - [Build for Termux on Android](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-termux-on-android)
+- [Build for QNX](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-qnx)
 
 **[download prebuild binary package for android and ios](https://github.com/Tencent/ncnn/releases)**
 
 **[use ncnn with alexnet](https://github.com/Tencent/ncnn/wiki/use-ncnn-with-alexnet) with detailed steps, recommended for beginners :)**
 
 **[ncnn 组件使用指北 alexnet](https://github.com/Tencent/ncnn/wiki/use-ncnn-with-alexnet.zh) 附带详细步骤，新人强烈推荐 :)**
```

### Comparing `ncnn-1.0.20230223/README.md` & `ncnn-1.0.20230517/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 | Windows           | [![Build Status][pass-windows-x86-cpu]][ci-windows-x86-cpu]         | [![Build Status][pass-windows-x64-cpu]][ci-windows-x64-cpu]                     | —                                                               | [![Build Status][pass-windows-x64-gpu]][ci-windows-x64-gpu]         |
 | Windows (ARM)     | [![Build Status][pass-windows-arm-cpu]][ci-windows-arm-cpu]         | [![Build Status][pass-windows-arm64-cpu]][ci-windows-arm64-cpu]                 | —                                                               | —                                                                   |
 | macOS             | —                                                                   | [![Build Status][pass-macos-x64-cpu]][ci-macos-x64-cpu]                         | —                                                               | [![Build Status][pass-macos-x64-gpu]][ci-macos-x64-gpu]             |
 | macOS (ARM)       | —                                                                   | [![Build Status][pass-macos-arm64-cpu]][ci-macos-arm64-cpu]                     | —                                                               | [![Build Status][pass-macos-arm64-gpu]][ci-macos-arm64-gpu]         |
 | Android           | [![Build Status][pass-android-armv7-cpu]][ci-android-armv7-cpu]     | [![Build Status][pass-android-armv8-cpu]][ci-android-armv8-cpu]                 | [![Build Status][pass-android-armv7-gpu]][ci-android-armv7-gpu] | [![Build Status][pass-android-armv8-gpu]][ci-android-armv8-gpu]     |
 | Android-x86       | [![Build Status][pass-android-x86-cpu]][ci-android-x86-cpu]         | [![Build Status][pass-android-x64-cpu]][ci-android-x64-cpu]                     | [![Build Status][pass-android-x86-gpu]][ci-android-x86-gpu]     | [![Build Status][pass-android-x64-gpu]][ci-android-x64-gpu]         |
 | iOS               | [![Build Status][pass-ios-cpu]][ci-ios-cpu]                         | [![Build Status][pass-ios-cpu]][ci-ios-cpu]                                     | —                                                               | [![Build Status][pass-ios-arm64-gpu]][ci-ios-arm64-gpu]             |
-| iOS Simulator     | [![Build Status][pass-ios-simulator]][ci-ios-simulator]             | [![Build Status][pass-ios-simulator]][ci-ios-simulator]                         | —                                                               | —                                                                   |
+| iOS Simulator     | [![Build Status][pass-ios-simulator]][ci-ios-simulator]             | [![Build Status][pass-ios-simulator]][ci-ios-simulator]                         | —                                                               | [![Build Status][pass-ios-simulator-gpu]][ci-ios-simulator-gpu]     |
 | WebAssembly       | [![Build Status][pass-web-assembly]][ci-web-assembly]               | —                                                                               | —                                                               | —                                                                   |
 | RISC-V GCC/Newlib | [![Build Status][pass-elf-riscv32-cpu-gcc]][ci-elf-riscv32-cpu-gcc] | [![Build Status][pass-elf-riscv64-cpu-gcc]][ci-elf-riscv64-cpu-gcc]             | —                                                               | —                                                                   |
 
 [pass-android-armv7-cpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv7-cpu.yml?branch=master
 [pass-android-armv7-gpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv7-gpu.yml?branch=master
 [pass-android-armv8-cpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv8-cpu.yml?branch=master
 [pass-android-armv8-gpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv8-gpu.yml?branch=master
@@ -210,14 +210,15 @@
 - [Build for Hisilicon platform with cross-compiling](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-hisilicon-platform-with-cross-compiling)
 - [Build for Android](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-android)
 - [Build for iOS on macOS with xcode](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-ios-on-macos-with-xcode)
 - [Build for WebAssembly](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-webassembly)
 - [Build for AllWinner D1](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-allwinner-d1)
 - [Build for Loongson 2K1000](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-loongson-2k1000)
 - [Build for Termux on Android](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-termux-on-android)
+- [Build for QNX](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-qnx)
 
 **[download prebuild binary package for android and ios](https://github.com/Tencent/ncnn/releases)**
 
 **[use ncnn with alexnet](https://github.com/Tencent/ncnn/wiki/use-ncnn-with-alexnet) with detailed steps, recommended for beginners :)**
 
 **[ncnn 组件使用指北 alexnet](https://github.com/Tencent/ncnn/wiki/use-ncnn-with-alexnet.zh) 附带详细步骤，新人强烈推荐 :)**
```

### Comparing `ncnn-1.0.20230223/python/ncnn/__init__.py` & `ncnn-1.0.20230517/python/ncnn/__init__.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/__init__.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/fasterrcnn.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/fasterrcnn.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/mobilenetssd.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/mobilenetssd.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/mobilenetv2ssdlite.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/mobilenetv2ssdlite.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/mobilenetv3ssdlite.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/mobilenetv3ssdlite.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/model_store.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/model_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         ("0705b0f8fe5a77718561b9b7d6ed4f33fcd3d455", "mobilenetv2_yolov3.bin"),
         ("de59186323ebad5650631e12a6cc66b526ec7df4", "yolov4-tiny-opt.param"),
         ("1765c3b251c041dd6ac59d2ec3ddf7b983fe9ee9", "yolov4-tiny-opt.bin"),
         ("e92d3a3a8ac5e6a6c08c433aa2252b0680124328", "yolov4-opt.param"),
         ("69d128b42b70fb790e9d3ccabcf1b6e8cc2859fe", "yolov4-opt.bin"),
         ("6fa8ccc8cabc0f5633ab3c6ffa268e6042b8888f", "yolov5s.param"),
         ("0cbab3664deb090480ea748c1305f6fe850b9ac4", "yolov5s.bin"),
+        ("35ab0c1ce2864e0759d5794aa818df2de3013ab3", "yolov7-tiny.param"),
+        ("c0454f072b41997aa230c3fe1c1d504566574b6c", "yolov7-tiny.bin"),
+        ("e9de3c929d1c93f7dc94ed0f125795ac16ecc120", "yolov8s.param"),
+        ("90f4eb9e90086e2ec3af4c7837f00757e710b9c6", "yolov8s.bin"),
         ("e65bae7052d9e9b9d45e1214a8d1b5fe6f64e8af", "yolact.param"),
         ("9bda99f50b1c14c98c5c6bbc08d4f782eed66548", "yolact.bin"),
         ("3723ce3e312db6a102cff1a5c39dae80e1de658e", "mobilenet_ssd_voc_ncnn.param"),
         ("8e2d2139550dcbee1ce5e200b7697b25aab29656", "mobilenet_ssd_voc_ncnn.bin"),
         ("52c669821dc32ef5b7ab30749fa71a3bc27786b8", "squeezenet_ssd_voc.param"),
         ("347e31d1cbe469259fa8305860a7c24a95039202", "squeezenet_ssd_voc.bin"),
         ("52dab628ecac8137e61ce3aea1a912f9c5a0a638", "mobilenetv2_ssdlite_voc.param"),
```

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/model_zoo.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/model_zoo.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from .yolov2 import MobileNet_YoloV2
 from .yolov3 import MobileNetV2_YoloV3
 from .yolov4 import YoloV4_Tiny, YoloV4
 from .yolov5 import YoloV5s
+from .yolov7 import YoloV7_Tiny
+from .yolov8 import YoloV8s
 from .yolact import Yolact
 from .mobilenetssd import MobileNet_SSD
 from .squeezenetssd import SqueezeNet_SSD
 from .mobilenetv2ssdlite import MobileNetV2_SSDLite
 from .mobilenetv3ssdlite import MobileNetV3_SSDLite
 from .squeezenet import SqueezeNet
 from .fasterrcnn import Faster_RCNN
@@ -34,14 +36,16 @@
 
 _models = {
     "mobilenet_yolov2": MobileNet_YoloV2,
     "mobilenetv2_yolov3": MobileNetV2_YoloV3,
     "yolov4_tiny": YoloV4_Tiny,
     "yolov4": YoloV4,
     "yolov5s": YoloV5s,
+    "yolov7_tiny": YoloV7_Tiny,
+    "yolov8s": YoloV8s,
     "yolact": Yolact,
     "mobilenet_ssd": MobileNet_SSD,
     "squeezenet_ssd": SqueezeNet_SSD,
     "mobilenetv2_ssdlite": MobileNetV2_SSDLite,
     "mobilenetv3_ssdlite": MobileNetV3_SSDLite,
     "squeezenet": SqueezeNet,
     "faster_rcnn": Faster_RCNN,
```

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/nanodet.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/nanodet.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/peleenetssd.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/peleenetssd.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/retinaface.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/retinaface.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/rfcn.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/rfcn.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/shufflenetv2.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/simplepose.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/simplepose.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/squeezenet.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/squeezenet.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/squeezenetssd.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/squeezenetssd.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/yolact.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/yolact.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/yolov2.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/yolov2.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/yolov3.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/yolov3.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/yolov4.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/yolov4.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/model_zoo/yolov5.py` & `ncnn-1.0.20230517/python/ncnn/model_zoo/yolov5.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/utils/__init__.py` & `ncnn-1.0.20230517/python/ncnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/utils/download.py` & `ncnn-1.0.20230517/python/ncnn/utils/download.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/utils/functional.py` & `ncnn-1.0.20230517/python/ncnn/utils/functional.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/utils/objects.py` & `ncnn-1.0.20230517/python/ncnn/utils/objects.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn/utils/visual.py` & `ncnn-1.0.20230517/python/ncnn/utils/visual.py`

 * *Files identical despite different names*

### Comparing `ncnn-1.0.20230223/python/ncnn.egg-info/PKG-INFO` & `ncnn-1.0.20230517/python/ncnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncnn
-Version: 1.0.20230223
+Version: 1.0.20230517
 Summary: ncnn is a high-performance neural network inference framework optimized for the mobile platform
 Home-page: https://github.com/Tencent/ncnn
 Author: nihui
 Author-email: nihuini@tencent.com
 Maintainer: caishanli
 Maintainer-email: caishanli25@gmail.com
 License: BSD-3
@@ -74,15 +74,15 @@
 | Windows           | [![Build Status][pass-windows-x86-cpu]][ci-windows-x86-cpu]         | [![Build Status][pass-windows-x64-cpu]][ci-windows-x64-cpu]                     | —                                                               | [![Build Status][pass-windows-x64-gpu]][ci-windows-x64-gpu]         |
 | Windows (ARM)     | [![Build Status][pass-windows-arm-cpu]][ci-windows-arm-cpu]         | [![Build Status][pass-windows-arm64-cpu]][ci-windows-arm64-cpu]                 | —                                                               | —                                                                   |
 | macOS             | —                                                                   | [![Build Status][pass-macos-x64-cpu]][ci-macos-x64-cpu]                         | —                                                               | [![Build Status][pass-macos-x64-gpu]][ci-macos-x64-gpu]             |
 | macOS (ARM)       | —                                                                   | [![Build Status][pass-macos-arm64-cpu]][ci-macos-arm64-cpu]                     | —                                                               | [![Build Status][pass-macos-arm64-gpu]][ci-macos-arm64-gpu]         |
 | Android           | [![Build Status][pass-android-armv7-cpu]][ci-android-armv7-cpu]     | [![Build Status][pass-android-armv8-cpu]][ci-android-armv8-cpu]                 | [![Build Status][pass-android-armv7-gpu]][ci-android-armv7-gpu] | [![Build Status][pass-android-armv8-gpu]][ci-android-armv8-gpu]     |
 | Android-x86       | [![Build Status][pass-android-x86-cpu]][ci-android-x86-cpu]         | [![Build Status][pass-android-x64-cpu]][ci-android-x64-cpu]                     | [![Build Status][pass-android-x86-gpu]][ci-android-x86-gpu]     | [![Build Status][pass-android-x64-gpu]][ci-android-x64-gpu]         |
 | iOS               | [![Build Status][pass-ios-cpu]][ci-ios-cpu]                         | [![Build Status][pass-ios-cpu]][ci-ios-cpu]                                     | —                                                               | [![Build Status][pass-ios-arm64-gpu]][ci-ios-arm64-gpu]             |
-| iOS Simulator     | [![Build Status][pass-ios-simulator]][ci-ios-simulator]             | [![Build Status][pass-ios-simulator]][ci-ios-simulator]                         | —                                                               | —                                                                   |
+| iOS Simulator     | [![Build Status][pass-ios-simulator]][ci-ios-simulator]             | [![Build Status][pass-ios-simulator]][ci-ios-simulator]                         | —                                                               | [![Build Status][pass-ios-simulator-gpu]][ci-ios-simulator-gpu]     |
 | WebAssembly       | [![Build Status][pass-web-assembly]][ci-web-assembly]               | —                                                                               | —                                                               | —                                                                   |
 | RISC-V GCC/Newlib | [![Build Status][pass-elf-riscv32-cpu-gcc]][ci-elf-riscv32-cpu-gcc] | [![Build Status][pass-elf-riscv64-cpu-gcc]][ci-elf-riscv64-cpu-gcc]             | —                                                               | —                                                                   |
 
 [pass-android-armv7-cpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv7-cpu.yml?branch=master
 [pass-android-armv7-gpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv7-gpu.yml?branch=master
 [pass-android-armv8-cpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv8-cpu.yml?branch=master
 [pass-android-armv8-gpu]: https://img.shields.io/github/actions/workflow/status/Tencent/ncnn/android-armv8-gpu.yml?branch=master
@@ -233,14 +233,15 @@
 - [Build for Hisilicon platform with cross-compiling](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-hisilicon-platform-with-cross-compiling)
 - [Build for Android](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-android)
 - [Build for iOS on macOS with xcode](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-ios-on-macos-with-xcode)
 - [Build for WebAssembly](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-webassembly)
 - [Build for AllWinner D1](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-allwinner-d1)
 - [Build for Loongson 2K1000](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-loongson-2k1000)
 - [Build for Termux on Android](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-termux-on-android)
+- [Build for QNX](https://github.com/Tencent/ncnn/wiki/how-to-build#build-for-qnx)
 
 **[download prebuild binary package for android and ios](https://github.com/Tencent/ncnn/releases)**
 
 **[use ncnn with alexnet](https://github.com/Tencent/ncnn/wiki/use-ncnn-with-alexnet) with detailed steps, recommended for beginners :)**
 
 **[ncnn 组件使用指北 alexnet](https://github.com/Tencent/ncnn/wiki/use-ncnn-with-alexnet.zh) 附带详细步骤，新人强烈推荐 :)**
```

### Comparing `ncnn-1.0.20230223/python/ncnn.egg-info/SOURCES.txt` & `ncnn-1.0.20230517/python/ncnn.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -24,12 +24,14 @@
 python/ncnn/model_zoo/squeezenet.py
 python/ncnn/model_zoo/squeezenetssd.py
 python/ncnn/model_zoo/yolact.py
 python/ncnn/model_zoo/yolov2.py
 python/ncnn/model_zoo/yolov3.py
 python/ncnn/model_zoo/yolov4.py
 python/ncnn/model_zoo/yolov5.py
+python/ncnn/model_zoo/yolov7.py
+python/ncnn/model_zoo/yolov8.py
 python/ncnn/utils/__init__.py
 python/ncnn/utils/download.py
 python/ncnn/utils/functional.py
 python/ncnn/utils/objects.py
 python/ncnn/utils/visual.py
```

### Comparing `ncnn-1.0.20230223/setup.py` & `ncnn-1.0.20230517/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,15 @@
     with io.open("CMakeLists.txt", encoding="utf8") as f:
         version_file = f.read()
 
     version_major = re.findall(r"NCNN_VERSION_MAJOR (.+?)", version_file)
     version_minor = re.findall(r"NCNN_VERSION_MINOR (.+?)", version_file)
 
     if version_major and version_minor:
-        if sys.platform == "darwin":
-            ncnn_version = time.strftime("%Y.%m.%d", time.localtime())
-        else:
-            ncnn_version = time.strftime("%Y%m%d", time.localtime())
+        ncnn_version = time.strftime("%Y%m%d", time.localtime())
 
         return version_major[0] + "." + version_minor[0] + "." + ncnn_version
     raise RuntimeError("Unable to find version string.")
 
 
 # Convert distutils Windows platform specifiers to CMake -A arguments
 PLAT_TO_CMAKE = {
```


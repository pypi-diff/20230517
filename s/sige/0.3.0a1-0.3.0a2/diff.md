# Comparing `tmp/sige-0.3.0a1.tar.gz` & `tmp/sige-0.3.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sige-0.3.0a1.tar", last modified: Tue May 16 20:00:45 2023, max compression
+gzip compressed data, was "sige-0.3.0a2.tar", last modified: Tue May 16 20:39:59 2023, max compression
```

## Comparing `sige-0.3.0a1.tar` & `sige-0.3.0a2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:00:45.729567 sige-0.3.0a1/
--rw-r--r--   0 lmxyy      (501) staff       (20)     2847 2023-05-16 19:02:20.000000 sige-0.3.0a1/LICENSE
--rw-r--r--   0 lmxyy      (501) staff       (20)      159 2023-05-16 19:17:09.000000 sige-0.3.0a1/MANIFEST.in
--rw-r--r--   0 lmxyy      (501) staff       (20)     8598 2023-05-16 20:00:45.729320 sige-0.3.0a1/PKG-INFO
--rw-r--r--   0 lmxyy      (501) staff       (20)     8241 2023-05-16 19:02:20.000000 sige-0.3.0a1/README.md
--rw-r--r--   0 lmxyy      (501) staff       (20)       38 2023-05-16 20:00:45.729629 sige-0.3.0a1/setup.cfg
--rw-r--r--   0 lmxyy      (501) staff       (20)     8173 2023-05-16 19:55:38.000000 sige-0.3.0a1/setup.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:00:45.722115 sige-0.3.0a1/sige/
--rw-r--r--   0 lmxyy      (501) staff       (20)       56 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)       24 2023-05-16 19:48:39.000000 sige-0.3.0a1/sige/__version__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)      791 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/common.cpp
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:00:45.724208 sige-0.3.0a1/sige/cpu/
--rw-r--r--   0 lmxyy      (501) staff       (20)      862 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cpu/common_cpu.cpp
--rw-r--r--   0 lmxyy      (501) staff       (20)     4581 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cpu/gather.cpp
--rw-r--r--   0 lmxyy      (501) staff       (20)      392 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cpu/gather.h
--rw-r--r--   0 lmxyy      (501) staff       (20)      543 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cpu/pybind_cpu.cpp
--rw-r--r--   0 lmxyy      (501) staff       (20)     5128 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cpu/scatter.cpp
--rw-r--r--   0 lmxyy      (501) staff       (20)      669 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cpu/scatter.h
--rw-r--r--   0 lmxyy      (501) staff       (20)     6832 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cpu/scatter_gather.cpp
--rw-r--r--   0 lmxyy      (501) staff       (20)      762 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cpu/scatter_gather.h
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:00:45.725392 sige-0.3.0a1/sige/cuda/
--rw-r--r--   0 lmxyy      (501) staff       (20)      984 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cuda/common_cuda.cu
--rw-r--r--   0 lmxyy      (501) staff       (20)      379 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cuda/gather.cpp
--rw-r--r--   0 lmxyy      (501) staff       (20)     4113 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cuda/gather_kernel.cu
--rw-r--r--   0 lmxyy      (501) staff       (20)      558 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cuda/pybind_cuda.cpp
--rw-r--r--   0 lmxyy      (501) staff       (20)      658 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cuda/scatter.cpp
--rw-r--r--   0 lmxyy      (501) staff       (20)      749 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cuda/scatter_gather.cpp
--rw-r--r--   0 lmxyy      (501) staff       (20)     6572 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cuda/scatter_gather_kernel.cu
--rw-r--r--   0 lmxyy      (501) staff       (20)     4807 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/cuda/scatter_kernel.cu
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:00:45.727810 sige-0.3.0a1/sige/mps/
--rw-r--r--   0 lmxyy      (501) staff       (20)     2152 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/MPSDevice.h
--rw-r--r--   0 lmxyy      (501) staff       (20)     1633 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/MPSLibrary.h
--rw-r--r--   0 lmxyy      (501) staff       (20)     3514 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/MPSLibrary.mm
--rw-r--r--   0 lmxyy      (501) staff       (20)     4813 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/MPSStream.h
--rw-r--r--   0 lmxyy      (501) staff       (20)     1780 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/MPSUtils.h
--rw-r--r--   0 lmxyy      (501) staff       (20)      990 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/common_mps.metal
--rw-r--r--   0 lmxyy      (501) staff       (20)      380 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/gather.h
--rw-r--r--   0 lmxyy      (501) staff       (20)     2077 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/gather.metal
--rw-r--r--   0 lmxyy      (501) staff       (20)     2875 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/gather.mm
--rw-r--r--   0 lmxyy      (501) staff       (20)      543 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/pybind_mps.cpp
--rw-r--r--   0 lmxyy      (501) staff       (20)      656 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/scatter.h
--rw-r--r--   0 lmxyy      (501) staff       (20)     2278 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/scatter.metal
--rw-r--r--   0 lmxyy      (501) staff       (20)     4120 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/scatter.mm
--rw-r--r--   0 lmxyy      (501) staff       (20)      747 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/scatter_gather.h
--rw-r--r--   0 lmxyy      (501) staff       (20)     3261 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/scatter_gather.metal
--rw-r--r--   0 lmxyy      (501) staff       (20)     4966 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/mps/scatter_gather.mm
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:00:45.729013 sige-0.3.0a1/sige/nn/
--rw-r--r--   0 lmxyy      (501) staff       (20)      176 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/nn/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     4192 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/nn/base.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     4122 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/nn/gather.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     5353 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/nn/scatter.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     4722 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/nn/scatter_gather.py
--rw-r--r--   0 lmxyy      (501) staff       (20)      483 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/nn/utils.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     4066 2023-05-16 19:02:20.000000 sige-0.3.0a1/sige/utils.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:00:45.722773 sige-0.3.0a1/sige.egg-info/
--rw-r--r--   0 lmxyy      (501) staff       (20)     8598 2023-05-16 20:00:45.000000 sige-0.3.0a1/sige.egg-info/PKG-INFO
--rw-r--r--   0 lmxyy      (501) staff       (20)     1114 2023-05-16 20:00:45.000000 sige-0.3.0a1/sige.egg-info/SOURCES.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)        1 2023-05-16 20:00:45.000000 sige-0.3.0a1/sige.egg-info/dependency_links.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)       11 2023-05-16 20:00:45.000000 sige-0.3.0a1/sige.egg-info/requires.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)        5 2023-05-16 20:00:45.000000 sige-0.3.0a1/sige.egg-info/top_level.txt
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:39:59.128196 sige-0.3.0a2/
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2847 2023-05-16 19:02:20.000000 sige-0.3.0a2/LICENSE
+-rw-r--r--   0 lmxyy      (501) staff       (20)      159 2023-05-16 19:17:09.000000 sige-0.3.0a2/MANIFEST.in
+-rw-r--r--   0 lmxyy      (501) staff       (20)     8598 2023-05-16 20:39:59.126988 sige-0.3.0a2/PKG-INFO
+-rw-r--r--   0 lmxyy      (501) staff       (20)     8241 2023-05-16 19:02:20.000000 sige-0.3.0a2/README.md
+-rw-r--r--   0 lmxyy      (501) staff       (20)       38 2023-05-16 20:39:59.128290 sige-0.3.0a2/setup.cfg
+-rw-r--r--   0 lmxyy      (501) staff       (20)     8148 2023-05-16 20:36:26.000000 sige-0.3.0a2/setup.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:39:59.119135 sige-0.3.0a2/sige/
+-rw-r--r--   0 lmxyy      (501) staff       (20)       56 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)       24 2023-05-16 20:38:55.000000 sige-0.3.0a2/sige/__version__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)      791 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/common.cpp
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:39:59.121433 sige-0.3.0a2/sige/cpu/
+-rw-r--r--   0 lmxyy      (501) staff       (20)      862 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cpu/common_cpu.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4581 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cpu/gather.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      392 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cpu/gather.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)      543 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cpu/pybind_cpu.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)     5128 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cpu/scatter.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      669 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cpu/scatter.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     6832 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cpu/scatter_gather.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      762 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cpu/scatter_gather.h
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:39:59.122970 sige-0.3.0a2/sige/cuda/
+-rw-r--r--   0 lmxyy      (501) staff       (20)      984 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cuda/common_cuda.cu
+-rw-r--r--   0 lmxyy      (501) staff       (20)      379 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cuda/gather.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4113 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cuda/gather_kernel.cu
+-rw-r--r--   0 lmxyy      (501) staff       (20)      558 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cuda/pybind_cuda.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      658 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cuda/scatter.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      749 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cuda/scatter_gather.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)     6572 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cuda/scatter_gather_kernel.cu
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4807 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/cuda/scatter_kernel.cu
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:39:59.125383 sige-0.3.0a2/sige/mps/
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2152 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/MPSDevice.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1633 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/MPSLibrary.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     3514 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/MPSLibrary.mm
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4813 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/MPSStream.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1780 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/MPSUtils.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)      990 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/common_mps.metal
+-rw-r--r--   0 lmxyy      (501) staff       (20)      380 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/gather.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2077 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/gather.metal
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2875 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/gather.mm
+-rw-r--r--   0 lmxyy      (501) staff       (20)      543 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/pybind_mps.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      656 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/scatter.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2278 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/scatter.metal
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4120 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/scatter.mm
+-rw-r--r--   0 lmxyy      (501) staff       (20)      747 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/scatter_gather.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     3261 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/scatter_gather.metal
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4966 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/mps/scatter_gather.mm
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:39:59.126575 sige-0.3.0a2/sige/nn/
+-rw-r--r--   0 lmxyy      (501) staff       (20)      176 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/nn/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4488 2023-05-16 20:38:12.000000 sige-0.3.0a2/sige/nn/base.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4122 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/nn/gather.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     5353 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/nn/scatter.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4722 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/nn/scatter_gather.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)      483 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/nn/utils.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4066 2023-05-16 20:31:08.000000 sige-0.3.0a2/sige/utils.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 20:39:59.119887 sige-0.3.0a2/sige.egg-info/
+-rw-r--r--   0 lmxyy      (501) staff       (20)     8598 2023-05-16 20:39:59.000000 sige-0.3.0a2/sige.egg-info/PKG-INFO
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1114 2023-05-16 20:39:59.000000 sige-0.3.0a2/sige.egg-info/SOURCES.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)        1 2023-05-16 20:39:59.000000 sige-0.3.0a2/sige.egg-info/dependency_links.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       11 2023-05-16 20:39:59.000000 sige-0.3.0a2/sige.egg-info/requires.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)        5 2023-05-16 20:39:59.000000 sige-0.3.0a2/sige.egg-info/top_level.txt
```

### Comparing `sige-0.3.0a1/LICENSE` & `sige-0.3.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/PKG-INFO` & `sige-0.3.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sige
-Version: 0.3.0a1
+Version: 0.3.0a2
 Summary: Spatially Incremental Generative Engine (SIGE)
 Home-page: https://github.com/lmxyy/sige
 Author: Muyang Li
 Author-email: muyangli@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `sige-0.3.0a1/README.md` & `sige-0.3.0a2/README.md`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/setup.py` & `sige-0.3.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import glob
 import os
 import platform
 
 import torch
-from setuptools import Extension, find_packages, setup
+from setuptools import find_packages, setup
 from torch.utils.cpp_extension import build_ext, BuildExtension, CppExtension, CUDAExtension, IS_WINDOWS
 
 
 def get_mps_extension(name, sources, *args, **kwargs):
     from torch.utils.cpp_extension import CppExtension
 
     extra_compile_args = {}
@@ -18,14 +18,16 @@
 
     kwargs["extra_compile_args"] = kwargs.get("extra_compile_args", {})
     kwargs["extra_compile_args"].update(extra_compile_args)
     return CppExtension(name, sources, *args, **kwargs)
 
 
 def get_metal_extension(name, sources, *args, **kwargs):
+    from setuptools import Extension
+
     for src in sources:
         assert os.path.splitext(src)[1] == ".metal", f"Expect .metal file, but get {src}."
 
     kwargs["language"] = "metal"
     return Extension(name, sources, *args, **kwargs)
 
 
@@ -70,27 +72,27 @@
                     cflags = cflags["cxx"]
 
                 original_compile(obj, src, ext, cc_args, cflags, pp_opts)
             finally:
                 self.compiler.set_executable("compiler_so", original_compiler)
 
         def darwin_wrap_single_link(
-                target_desc,
-                objects,
-                output_filename,
-                output_dir=None,
-                libraries=None,
-                library_dirs=None,
-                runtime_library_dirs=None,
-                export_symbols=None,
-                debug=0,
-                extra_preargs=None,
-                extra_postargs=None,
-                build_temp=None,
-                target_lang=None,
+            target_desc,
+            objects,
+            output_filename,
+            output_dir=None,
+            libraries=None,
+            library_dirs=None,
+            runtime_library_dirs=None,
+            export_symbols=None,
+            debug=0,
+            extra_preargs=None,
+            extra_postargs=None,
+            build_temp=None,
+            target_lang=None,
         ):
             if os.path.splitext(objects[0])[1].lower() == ".air":
                 for obj in objects:
                     assert os.path.splitext(obj)[1].lower() == ".air", f"Expect .air file, but get {obj}."
 
                 linker = ["xcrun", "metallib"]
                 self.compiler.spawn(linker + objects + ["-o", output_filename])
```

### Comparing `sige-0.3.0a1/sige/common.cpp` & `sige-0.3.0a2/sige/common.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cpu/common_cpu.cpp` & `sige-0.3.0a2/sige/cpu/common_cpu.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cpu/gather.cpp` & `sige-0.3.0a2/sige/cpu/gather.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cpu/pybind_cpu.cpp` & `sige-0.3.0a2/sige/cpu/pybind_cpu.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cpu/scatter.cpp` & `sige-0.3.0a2/sige/cpu/scatter.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cpu/scatter.h` & `sige-0.3.0a2/sige/cpu/scatter.h`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cpu/scatter_gather.cpp` & `sige-0.3.0a2/sige/cpu/scatter_gather.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cpu/scatter_gather.h` & `sige-0.3.0a2/sige/cpu/scatter_gather.h`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cuda/common_cuda.cu` & `sige-0.3.0a2/sige/cuda/common_cuda.cu`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cuda/gather_kernel.cu` & `sige-0.3.0a2/sige/cuda/gather_kernel.cu`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cuda/pybind_cuda.cpp` & `sige-0.3.0a2/sige/cuda/pybind_cuda.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cuda/scatter.cpp` & `sige-0.3.0a2/sige/cuda/scatter.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cuda/scatter_gather.cpp` & `sige-0.3.0a2/sige/cuda/scatter_gather.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cuda/scatter_gather_kernel.cu` & `sige-0.3.0a2/sige/cuda/scatter_gather_kernel.cu`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/cuda/scatter_kernel.cu` & `sige-0.3.0a2/sige/cuda/scatter_kernel.cu`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/MPSDevice.h` & `sige-0.3.0a2/sige/mps/MPSDevice.h`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/MPSLibrary.h` & `sige-0.3.0a2/sige/mps/MPSLibrary.h`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/MPSLibrary.mm` & `sige-0.3.0a2/sige/mps/MPSLibrary.mm`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/MPSStream.h` & `sige-0.3.0a2/sige/mps/MPSStream.h`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/MPSUtils.h` & `sige-0.3.0a2/sige/mps/MPSUtils.h`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/common_mps.metal` & `sige-0.3.0a2/sige/mps/common_mps.metal`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/gather.metal` & `sige-0.3.0a2/sige/mps/gather.metal`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/gather.mm` & `sige-0.3.0a2/sige/mps/gather.mm`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/pybind_mps.cpp` & `sige-0.3.0a2/sige/mps/pybind_mps.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/scatter.h` & `sige-0.3.0a2/sige/mps/scatter.h`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/scatter.metal` & `sige-0.3.0a2/sige/mps/scatter.metal`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/scatter.mm` & `sige-0.3.0a2/sige/mps/scatter.mm`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/scatter_gather.h` & `sige-0.3.0a2/sige/mps/scatter_gather.h`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/scatter_gather.metal` & `sige-0.3.0a2/sige/mps/scatter_gather.metal`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/mps/scatter_gather.mm` & `sige-0.3.0a2/sige/mps/scatter_gather.mm`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/nn/base.py` & `sige-0.3.0a2/sige/nn/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import importlib
+import os
 from typing import Dict, List, Optional, Tuple
 
 import torch
 from torch import nn
 from torch.nn import functional as F
 
 
@@ -36,14 +37,19 @@
             runtime_dict = self.runtime
         for device in self.devices:
             name = "sige.%s" % device
             try:
                 module = importlib.import_module(name)
                 runtime = getattr(module, function_name)
                 runtime_dict[device] = runtime
+                if device == "mps":
+                    os.environ["SIGE_METAL_LIB_PATH"] = os.path.abspath(
+                        os.path.join(os.path.dirname(module.__file__), "..", "sige.metallib")
+                    )
+                    print(os.environ["SIGE_METAL_LIB_PATH"])
             except (ModuleNotFoundError, AttributeError):
                 runtime_dict[device] = None
         return runtime_dict
 
     def set_mode(self, mode: str):
         self.mode = mode
```

### Comparing `sige-0.3.0a1/sige/nn/gather.py` & `sige-0.3.0a2/sige/nn/gather.py`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/nn/scatter.py` & `sige-0.3.0a2/sige/nn/scatter.py`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/nn/scatter_gather.py` & `sige-0.3.0a2/sige/nn/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige/utils.py` & `sige-0.3.0a2/sige/utils.py`

 * *Files identical despite different names*

### Comparing `sige-0.3.0a1/sige.egg-info/PKG-INFO` & `sige-0.3.0a2/sige.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sige
-Version: 0.3.0a1
+Version: 0.3.0a2
 Summary: Spatially Incremental Generative Engine (SIGE)
 Home-page: https://github.com/lmxyy/sige
 Author: Muyang Li
 Author-email: muyangli@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `sige-0.3.0a1/sige.egg-info/SOURCES.txt` & `sige-0.3.0a2/sige.egg-info/SOURCES.txt`

 * *Files identical despite different names*


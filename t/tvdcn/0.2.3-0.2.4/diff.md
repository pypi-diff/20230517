# Comparing `tmp/tvdcn-0.2.3.tar.gz` & `tmp/tvdcn-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.2.3.tar", last modified: Tue May 16 06:40:25 2023, max compression
+gzip compressed data, was "tvdcn-0.2.4.tar", last modified: Tue May 16 20:06:41 2023, max compression
```

## Comparing `tvdcn-0.2.3.tar` & `tvdcn-0.2.4.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.966572 tvdcn-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 06:38:08.000000 tvdcn-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-16 06:40:25.966572 tvdcn-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-16 06:38:08.000000 tvdcn-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-16 06:38:08.000000 tvdcn-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-16 06:40:25.966572 tvdcn-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-16 06:38:08.000000 tvdcn-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.938572 tvdcn-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tests/test_compatibility_with_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.942572 tvdcn-0.2.3/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.946572 tvdcn-0.2.3/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.954572 tvdcn-0.2.3/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.958572 tvdcn-0.2.3/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26828 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27086 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.958572 tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.962572 tvdcn-0.2.3/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35710 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    38546 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/ops/mask_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.946572 tvdcn-0.2.3/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:06:41.600417 tvdcn-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 20:04:14.000000 tvdcn-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-05-16 20:06:41.600417 tvdcn-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-16 20:04:14.000000 tvdcn-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-16 20:04:14.000000 tvdcn-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-16 20:06:41.600417 tvdcn-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-16 20:04:14.000000 tvdcn-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:06:41.576417 tvdcn-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:06:41.580417 tvdcn-0.2.4/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:06:41.584417 tvdcn-0.2.4/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:06:41.588417 tvdcn-0.2.4/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:06:41.592417 tvdcn-0.2.4/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26828 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27086 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:06:41.592417 tvdcn-0.2.4/tvdcn/csrc/ops/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:06:41.596417 tvdcn-0.2.4/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:06:41.600417 tvdcn-0.2.4/tvdcn/ops/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/ops/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/ops/activations/mask_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/ops/activations/mask_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35727 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38668 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-16 20:04:14.000000 tvdcn-0.2.4/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:06:41.584417 tvdcn-0.2.4/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-05-16 20:06:41.000000 tvdcn-0.2.4/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-16 20:06:41.000000 tvdcn-0.2.4/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:06:41.000000 tvdcn-0.2.4/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:06:41.000000 tvdcn-0.2.4/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 20:06:41.000000 tvdcn-0.2.4/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 20:06:41.000000 tvdcn-0.2.4/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.2.3/LICENSE.txt` & `tvdcn-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/PKG-INFO` & `tvdcn-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.3
+Version: 0.2.4
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
@@ -57,46 +57,45 @@
   - `tvdcn.ops.deform_conv_transpose3d`
 
 - And the following **supplementary operations** (for activating `mask`):
   - `tvdcn.ops.mask_softmax1d`
   - `tvdcn.ops.mask_softmax2d`
   - `tvdcn.ops.mask_softmax3d`
 
-- Both `offset` and `mask` can turned off, and can be applied in separate groups
-  ([Deformable Convolution v3](https://arxiv.org/abs/2211.05778)).
+- Both `offset` and `mask` can be turned off, and can be applied in separate groups.
 
 - All the `nn.Module` wrappers for these operations are implemented,
   everything is `@torch.jit.script`-able! Please check [Usage](#usage).
 
 **Note:** We don't care much about `onnx` exportation, but if you do, you can check this repo:
 https://github.com/masamitsu-murase/deform_conv2d_onnx_exporter.
 
 ## Requirements
 
-- `torch>=1.8`
+- `torch>=1.9.0`
 
 ## Installation
 
 #### From PyPI:
 
 [tvdcn](https://pypi.org/project/tvdcn) provides some prebuilt wheels on **PyPI**.
 Run this command to install:
 
 ```terminal
 pip install tvdcn
 ```
 
-The Linux and Windows wheels are built with **Cuda 11.8**, which is compatible with `torch==2.0.0`.
+The Linux and Windows wheels are built with **Cuda 11.8**.
 If you cannot find a wheel for your Arch/Python/Cuda, or there is any problem with library linking when importing,
 please proceed to [instructions to build from source](#from-source), all steps are super easy.
 
 |                  |     Linux/Windows     |     MacOS      |
 |------------------|:---------------------:|:--------------:|
 | Python version:  |       3.8-3.11        |    3.8-3.11    |
-| PyTorch version: |    `torch==2.0.0`     | `torch==2.0.0` |
+| PyTorch version: |    `torch==2.0.1`     | `torch==2.0.1` |
 | Cuda version:    |         11.8          |       -        |
 | GPU CCs:         | `6.1,7.5,8.6,8.9+PTX` |       -        |
 
 #### From Source:
 
 For installing from source, you need a C++ compiler (`gcc`/`msvc`) and a Cuda compiler (`nvcc`).
 Clone this repo and execute the following command:
@@ -208,22 +207,28 @@
 
 These are easy-to-use classes that contain ordinary convolution layers with appropriate hyperparameters to generate
 `offset` (and `mask` if initialized with `modulated=True`);
 but that means less customization.
 The only tunable hyperparameters that effect these supplementary conv layers are `offset_groups` and `mask_groups`,
 which have been decoupled from and behave somewhat similar to `groups`.
 
+To use the softmax activation for mask proposed in [Deformable Convolution v3](https://arxiv.org/abs/2211.05778),
+set `mask_activation='softmax'`. `offset_activation` and `mask_activation` also accept any `nn.Module`.
+
 ```python
 import torch
 
 from tvdcn import PackedDeformConv1d
 
 input = torch.rand(2, 3, 128)
 
-conv = PackedDeformConv1d(3, 16, kernel_size=5, modulated=True)
+conv = PackedDeformConv1d(3, 16,
+                          kernel_size=5,
+                          modulated=True,
+                          mask_activation='softmax')
 # jit scripting
 scripted_conv = torch.jit.script(conv)
 print(scripted_conv)
 
 output = scripted_conv(input)
 print(output.shape)
 ```
```

### Comparing `tvdcn-0.2.3/README.md` & `tvdcn-0.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,46 +25,45 @@
   - `tvdcn.ops.deform_conv_transpose3d`
 
 - And the following **supplementary operations** (for activating `mask`):
   - `tvdcn.ops.mask_softmax1d`
   - `tvdcn.ops.mask_softmax2d`
   - `tvdcn.ops.mask_softmax3d`
 
-- Both `offset` and `mask` can turned off, and can be applied in separate groups
-  ([Deformable Convolution v3](https://arxiv.org/abs/2211.05778)).
+- Both `offset` and `mask` can be turned off, and can be applied in separate groups.
 
 - All the `nn.Module` wrappers for these operations are implemented,
   everything is `@torch.jit.script`-able! Please check [Usage](#usage).
 
 **Note:** We don't care much about `onnx` exportation, but if you do, you can check this repo:
 https://github.com/masamitsu-murase/deform_conv2d_onnx_exporter.
 
 ## Requirements
 
-- `torch>=1.8`
+- `torch>=1.9.0`
 
 ## Installation
 
 #### From PyPI:
 
 [tvdcn](https://pypi.org/project/tvdcn) provides some prebuilt wheels on **PyPI**.
 Run this command to install:
 
 ```terminal
 pip install tvdcn
 ```
 
-The Linux and Windows wheels are built with **Cuda 11.8**, which is compatible with `torch==2.0.0`.
+The Linux and Windows wheels are built with **Cuda 11.8**.
 If you cannot find a wheel for your Arch/Python/Cuda, or there is any problem with library linking when importing,
 please proceed to [instructions to build from source](#from-source), all steps are super easy.
 
 |                  |     Linux/Windows     |     MacOS      |
 |------------------|:---------------------:|:--------------:|
 | Python version:  |       3.8-3.11        |    3.8-3.11    |
-| PyTorch version: |    `torch==2.0.0`     | `torch==2.0.0` |
+| PyTorch version: |    `torch==2.0.1`     | `torch==2.0.1` |
 | Cuda version:    |         11.8          |       -        |
 | GPU CCs:         | `6.1,7.5,8.6,8.9+PTX` |       -        |
 
 #### From Source:
 
 For installing from source, you need a C++ compiler (`gcc`/`msvc`) and a Cuda compiler (`nvcc`).
 Clone this repo and execute the following command:
@@ -176,22 +175,28 @@
 
 These are easy-to-use classes that contain ordinary convolution layers with appropriate hyperparameters to generate
 `offset` (and `mask` if initialized with `modulated=True`);
 but that means less customization.
 The only tunable hyperparameters that effect these supplementary conv layers are `offset_groups` and `mask_groups`,
 which have been decoupled from and behave somewhat similar to `groups`.
 
+To use the softmax activation for mask proposed in [Deformable Convolution v3](https://arxiv.org/abs/2211.05778),
+set `mask_activation='softmax'`. `offset_activation` and `mask_activation` also accept any `nn.Module`.
+
 ```python
 import torch
 
 from tvdcn import PackedDeformConv1d
 
 input = torch.rand(2, 3, 128)
 
-conv = PackedDeformConv1d(3, 16, kernel_size=5, modulated=True)
+conv = PackedDeformConv1d(3, 16,
+                          kernel_size=5,
+                          modulated=True,
+                          mask_activation='softmax')
 # jit scripting
 scripted_conv = torch.jit.script(conv)
 print(scripted_conv)
 
 output = scripted_conv(input)
 print(output.shape)
 ```
```

### Comparing `tvdcn-0.2.3/pyproject.toml` & `tvdcn-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel",
 #    "--find-links https://download.pytorch.org/whl/cu118; sys_platform == \"linux\" or sys_platform == \"win32\"",
-    "torch>=1.8",
+    "torch>=1.9.0",
 ]
 
 [tool.cibuildwheel]
 build = ["cp38-*", "cp39-*", "cp310-*", "cp311-*"]
 archs = ["auto64"]
 skip = ["*-musllinux_*", "*-win32", "*-manylinux_i686"]
 
@@ -17,14 +17,14 @@
 repair-wheel-command = [
     "pip install auditwheel patchelf",
     "python tools/packaging/audit_torch_extension.py repair -w {dest_dir} {wheel}"
 ]
 
 [tool.cibuildwheel.windows]
 before-all = "bash tools/packaging/prepare_build_environment_windows.sh"
-before-build = "pip install torch>=1.8 --index-url https://download.pytorch.org/whl/cu118"
+before-build = "pip install torch>=1.9.0 --index-url https://download.pytorch.org/whl/cu118"
 environment = "FORCE_CUDA='1' PIP_NO_BUILD_ISOLATION='0' TORCH_CUDA_ARCH_LIST='6.1 7.5 8.6 8.9+PTX'"
 repair-wheel-command = ""
 
 [tool.cibuildwheel.macos]
 before-all = "tools/packaging/prepare_build_environment_macos.sh"
 repair-wheel-command = ""
```

### Comparing `tvdcn-0.2.3/setup.cfg` & `tvdcn-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/setup.py` & `tvdcn-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tests/test_compatibility_with_torchvision.py` & `tvdcn-0.2.4/tests/test_compatibility_with_torchvision.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tests/test_grad.py` & `tvdcn-0.2.4/tests/test_grad.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import torch
 from torch.autograd.gradcheck import gradcheck
 
 import tvdcn
 from utils.deform_conv_test_args import DeformConvTestArgs
 
 
-def test_deform_conv_grad(dim=2,
+def test_deform_conv_grad(dim=1,
                           transposed=False,
                           dtype=torch.float64,
                           device='cuda'):
     torch.manual_seed(12)
     conv_func = getattr(tvdcn, f'deform_conv{"_transpose" if transposed else ""}{dim}d')
     args = DeformConvTestArgs(dim=dim, transposed=transposed, dtype=dtype, device=device)
     print(args)
 
-    c_res = conv_func(args.input,
-                      args.weight,
-                      args.offset,
-                      args.mask,
-                      args.bias,
-                      args.stride,
-                      args.padding,
-                      args.dilation,
-                      args.groups)
-    c_res.sum().backward()
+    c_output = conv_func(args.input,
+                         args.weight,
+                         args.offset,
+                         args.mask,
+                         args.bias,
+                         args.stride,
+                         args.padding,
+                         args.dilation,
+                         args.groups)
+    c_output.sum().backward()
     c_input_grad = args.input.grad.clone()
     c_weight_grad = args.weight.grad.clone()
     c_offset_grad = args.offset.grad.clone()
     c_mask_grad = args.mask.grad.clone()
     c_bias_grad = args.bias.grad.clone()
     args.zero_grad()
-    print(c_res)
+    print(c_output)
 
     grad_ok = gradcheck(
         lambda inp, wei, off, msk, bi: conv_func(inp, wei, off, msk, bi,
                                                  args.stride,
                                                  args.padding,
                                                  args.dilation,
                                                  args.groups),
```

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv3d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp` & `tvdcn-0.2.4/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.2.4/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/extension.py` & `tvdcn-0.2.4/tvdcn/extension.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn/ops/deform_conv.py` & `tvdcn-0.2.4/tvdcn/ops/deform_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from typing import Union, Optional, Tuple
+
 import torch
 import torch.nn.functional as F
 from torch import nn, Tensor
-from torch.jit.annotations import Optional, Tuple, Union
 from torch.nn import init
 from torch.nn.common_types import _size_1_t, _size_2_t, _size_3_t
 from torch.nn.modules.conv import _ConvNd
 from torch.nn.modules.utils import _single, _pair, _triple
 
-from .mask_activation import MaskSoftmax1d, MaskSoftmax2d, MaskSoftmax3d
+from .activations import (
+    MaskSigmoid, MaskSoftmax1d, MaskSoftmax2d, MaskSoftmax3d,
+)
 from .._types import _IntTuple, _Activation
 from ..extension import _assert_has_ops
 from ..utils import _log_api_usage_once
 
 __all__ = [
     'deform_conv1d',
     'deform_conv2d',
@@ -69,49 +72,49 @@
         >>> print(out.shape)
         Output:
         >>>  torch.Size([4, 5, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv1d)
     _assert_has_ops()
-    out_channels = weight.shape[0]
+    out_channels = weight.size(0)
 
     deformable = offset is not None
     modulated = mask is not None
 
     if offset is None:
-        offset = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if mask is None:
-        mask = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if bias is None:
         bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
 
     stride = _single(stride)
     pad = _single(padding)
     dil = _single(dilation)
 
-    weight_w = weight.shape[-1]
-    _, n_in_channels, in_w = input.shape
+    weight_w = weight.size(-1)
+    _, n_in_channels, in_w = input.size()
 
-    assert groups == n_in_channels // weight.shape[1]
-    offset_groups = offset.shape[1] // weight_w
-    mask_groups = mask.shape[1] // weight_w
+    assert groups == n_in_channels // weight.size(1)
+    offset_groups = offset.size(1) // weight_w
+    mask_groups = mask.size(1) // weight_w
 
     if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size[2].\n"
-            "Got offset.shape[1]={}, while weight.size[2]={}".format(
-                offset.shape[1], weight_w))
+            "be a multiple of weight.size(2).\n"
+            "Got offset.size(1)={}, while weight.size(2)={}".format(
+                offset.size(1), weight_w))
     if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size[2].\n"
-            "Got mask.shape[1]={}, while weight.size[2]={}".format(
-                mask.shape[1], weight_w))
+            "be a multiple of weight.size(2).\n"
+            "Got mask.size(1)={}, while weight.size(2)={}".format(
+                mask.size(1), weight_w))
 
     return torch.ops.tvdcn.deform_conv1d(
         input,
         weight,
         offset,
         mask,
         bias,
@@ -176,48 +179,48 @@
         >>> print(out.shape)
         Output:
         >>>  torch.Size([4, 5, 8, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv2d)
     _assert_has_ops()
-    out_channels = weight.shape[0]
+    out_channels = weight.size(0)
 
     deformable = offset is not None
     modulated = mask is not None
 
     if offset is None:
-        offset = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if mask is None:
-        mask = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if bias is None:
         bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
 
     stride_h, stride_w = _pair(stride)
     pad_h, pad_w = _pair(padding)
     dil_h, dil_w = _pair(dilation)
-    weight_h, weight_w = weight.shape[-2:]
-    _, n_in_channels, in_h, in_w = input.shape
+    weight_h, weight_w = weight.size()[-2:]
+    _, n_in_channels, in_h, in_w = input.size()
 
-    assert groups == n_in_channels // weight.shape[1]
-    offset_groups = offset.shape[1] // (2 * weight_h * weight_w)
-    mask_groups = mask.shape[1] // (weight_h * weight_w)
+    assert groups == n_in_channels // weight.size(1)
+    offset_groups = offset.size(1) // (2 * weight_h * weight_w)
+    mask_groups = mask.size(1) // (weight_h * weight_w)
 
     if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of 2 * weight.size[2] * weight.size[3].\n"
-            "Got offset.shape[1]={}, while 2 * weight.size[2] * weight.size[3]={}".format(
-                offset.shape[1], 2 * weight_h * weight_w))
+            "be a multiple of 2 * weight.size(2) * weight.size(3).\n"
+            "Got offset.size(1)={}, while 2 * weight.size(2) * weight.size(3)={}".format(
+                offset.size(1), 2 * weight_h * weight_w))
     if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size[2] * weight.size[3].\n"
-            "Got mask.shape[1]={}, while weight.size[2] * weight.size[3]={}".format(
-                mask.shape[1], weight_h * weight_w))
+            "be a multiple of weight.size(2) * weight.size(3).\n"
+            "Got mask.size(1)={}, while weight.size(2) * weight.size(3)={}".format(
+                mask.size(1), weight_h * weight_w))
 
     return torch.ops.tvdcn.deform_conv2d(
         input,
         weight,
         offset,
         mask,
         bias,
@@ -278,48 +281,48 @@
         >>> print(out.shape)
         Output:
         >>> torch.Size([4, 5, 8, 8, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv3d)
     _assert_has_ops()
-    out_channels = weight.shape[0]
+    out_channels = weight.size(0)
 
     deformable = offset is not None
     modulated = mask is not None
 
     if offset is None:
-        offset = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if mask is None:
-        mask = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if bias is None:
         bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
 
     stride_d, stride_h, stride_w = _triple(stride)
     pad_d, pad_h, pad_w = _triple(padding)
     dil_d, dil_h, dil_w = _triple(dilation)
-    weight_d, weight_h, weight_w = weight.shape[-3:]
-    _, n_in_channels, in_d, in_h, in_w = input.shape
+    weight_d, weight_h, weight_w = weight.size()[-3:]
+    _, n_in_channels, in_d, in_h, in_w = input.size()
 
-    assert groups == n_in_channels // weight.shape[1]
-    offset_groups = offset.shape[1] // (3 * weight_d * weight_h * weight_w)
-    mask_groups = mask.shape[1] // (weight_d * weight_h * weight_w)
+    assert groups == n_in_channels // weight.size(1)
+    offset_groups = offset.size(1) // (3 * weight_d * weight_h * weight_w)
+    mask_groups = mask.size(1) // (weight_d * weight_h * weight_w)
 
     if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of 3 * weight.size[2] * weight.size[3] * weight.size[4].\n"
-            "Got offset.shape[1]={}, while 3 * weight.size[2] * weight.size[3] * weight.size[4]={}".format(
-                offset.shape[1], 3 * weight_d * weight_h * weight_w))
+            "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\n"
+            "Got offset.size(1)={}, while 3 * weight.size(2) * weight.size(3) * weight.size(4)={}".format(
+                offset.size(1), 3 * weight_d * weight_h * weight_w))
     if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size[2] * weight.size[3] * weight.size[4].\n"
-            "Got mask.shape[1]={}, while weight.size[2] * weight.size[3] * weight.size[4]={}".format(
-                mask.shape[1], weight_d * weight_h * weight_w))
+            "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\n"
+            "Got mask.size(1)={}, while weight.size(2) * weight.size(3) * weight.size(4)={}".format(
+                mask.size(1), weight_d * weight_h * weight_w))
 
     return torch.ops.tvdcn.deform_conv3d(
         input,
         weight,
         offset,
         mask,
         bias,
@@ -397,15 +400,15 @@
         if self.padding_mode != 'zeros':
             s += ', padding_mode={padding_mode}'
         return s.format(**self.__dict__)
 
 
 class DeformConv1d(_DeformConvNd):
     """
-    See :func:`deform_conv1d`
+    See :func:`deform_conv1d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_1_t,
                  stride: _size_1_t = 1,
@@ -437,15 +440,15 @@
                                  (0,), self.dilation, self.groups)
         return deform_conv1d(input, weight, offset, mask, bias,
                              self.stride, self.padding, self.dilation, self.groups)
 
 
 class DeformConv2d(_DeformConvNd):
     """
-    See :func:`deform_conv2d`
+    See :func:`deform_conv2d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_2_t,
                  stride: _size_2_t = 1,
@@ -477,15 +480,15 @@
                                  (0, 0), self.dilation, self.groups)  # type: ignore[arg-type]
         return deform_conv2d(input, weight, offset, mask, bias,
                              self.stride, self.padding, self.dilation, self.groups)  # type: ignore[arg-type]
 
 
 class DeformConv3d(_DeformConvNd):
     """
-    See :func:`deform_conv3d`
+    See :func:`deform_conv3d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_3_t,
                  stride: _size_3_t = 1,
@@ -521,15 +524,15 @@
 
 ################################################################################
 # Packed Modules
 ################################################################################
 # noinspection PyMethodOverriding
 class PackedDeformConv1d(DeformConv1d):
     """
-    Packed version of :class:`DeformConv1d`
+    Packed version of :class:`DeformConv1d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_1_t,
                  stride: _size_1_t = 1,
@@ -538,15 +541,15 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'softmax',
+                 mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             groups, bias, padding_mode, device, dtype)
 
@@ -560,15 +563,15 @@
         if out_channels % mask_groups != 0:
             raise ValueError('out_channels must be divisible by mask_groups')
 
         if isinstance(offset_activation, str):
             raise ValueError('currently, no activation is supported for offset')
         if isinstance(mask_activation, str):
             if mask_activation == 'sigmoid':
-                mask_activation = nn.Sigmoid()
+                mask_activation = MaskSigmoid(scale=2.)
             elif mask_activation == 'softmax':
                 mask_activation = MaskSoftmax1d(self.kernel_size)  # type: ignore[arg-type]
             else:
                 raise ValueError('only \"sigmoid\" and \"softmax\" activations are supported for mask')
 
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
@@ -586,15 +589,14 @@
                 dilation=self.dilation,
                 groups=self.groups,
                 bias=self.bias is not None,
                 device=device,
                 dtype=dtype)
         else:
             self.register_module('conv_offset', None)
-        self.offset_activation = offset_activation
 
         if self.modulated:
             self.conv_mask = nn.Conv1d(
                 self.in_channels,
                 self.kernel_size[0] * self.mask_groups,
                 kernel_size=self.kernel_size,
                 stride=self.stride,
@@ -602,28 +604,30 @@
                 dilation=self.dilation,
                 groups=self.groups,
                 bias=self.bias is not None,
                 device=device,
                 dtype=dtype)
         else:
             self.register_module('conv_mask', None)
+
+        self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.ones_(self.conv_mask.weight)
+            init.zeros_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
@@ -640,15 +644,15 @@
 
         return self._conv_forward(input, self.weight, offset, mask, self.bias)
 
 
 # noinspection PyMethodOverriding
 class PackedDeformConv2d(DeformConv2d):
     """
-    Packed version of :class:`DeformConv2d`
+    Packed version of :class:`DeformConv2d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_2_t,
                  stride: _size_2_t = 1,
@@ -657,15 +661,15 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'softmax',
+                 mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             groups, bias, padding_mode, device, dtype)
 
@@ -679,15 +683,15 @@
         if out_channels % mask_groups != 0:
             raise ValueError('out_channels must be divisible by mask_groups')
 
         if isinstance(offset_activation, str):
             raise ValueError('currently, no activation is supported for offset')
         if isinstance(mask_activation, str):
             if mask_activation == 'sigmoid':
-                mask_activation = nn.Sigmoid()
+                mask_activation = MaskSigmoid(scale=2.)
             elif mask_activation == 'softmax':
                 mask_activation = MaskSoftmax2d(self.kernel_size)  # type: ignore[arg-type]
             else:
                 raise ValueError('only \"sigmoid\" and \"softmax\" activations are supported for mask')
 
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
@@ -705,15 +709,14 @@
                 dilation=self.dilation,  # type: ignore[arg-type]
                 groups=self.groups,
                 bias=self.bias is not None,
                 device=device,
                 dtype=dtype)
         else:
             self.register_module('conv_offset', None)
-        self.offset_activation = offset_activation
 
         if self.modulated:
             self.conv_mask = nn.Conv2d(
                 self.in_channels,
                 self.kernel_size[0] * self.kernel_size[1] * self.mask_groups,
                 kernel_size=self.kernel_size,  # type: ignore[arg-type]
                 stride=self.stride,  # type: ignore[arg-type]
@@ -721,28 +724,30 @@
                 dilation=self.dilation,  # type: ignore[arg-type]
                 groups=self.groups,
                 bias=self.bias is not None,
                 device=device,
                 dtype=dtype)
         else:
             self.register_module('conv_mask', None)
+
+        self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.ones_(self.conv_mask.weight)
+            init.zeros_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
@@ -759,15 +764,15 @@
 
         return self._conv_forward(input, self.weight, offset, mask, self.bias)
 
 
 # noinspection PyMethodOverriding
 class PackedDeformConv3d(DeformConv3d):
     """
-    Packed version of :class:`DeformConv3d`
+    Packed version of :class:`DeformConv3d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_3_t,
                  stride: _size_3_t = 1,
@@ -776,15 +781,15 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'softmax',
+                 mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             groups, bias, padding_mode, device, dtype)
 
@@ -798,15 +803,15 @@
         if out_channels % mask_groups != 0:
             raise ValueError('out_channels must be divisible by mask_groups')
 
         if isinstance(offset_activation, str):
             raise ValueError('currently, no activation is supported for offset')
         if isinstance(mask_activation, str):
             if mask_activation == 'sigmoid':
-                mask_activation = nn.Sigmoid()
+                mask_activation = MaskSigmoid(scale=2.)
             elif mask_activation == 'softmax':
                 mask_activation = MaskSoftmax3d(self.kernel_size)  # type: ignore[arg-type]
             else:
                 raise ValueError('only \"sigmoid\" and \"softmax\" activations are supported for mask')
 
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
@@ -824,15 +829,14 @@
                 dilation=self.dilation,  # type: ignore[arg-type]
                 groups=self.groups,
                 bias=self.bias is not None,
                 device=dtype,
                 dtype=device)
         else:
             self.register_module('conv_offset', None)
-        self.offset_activation = offset_activation
 
         if self.modulated:
             self.conv_mask = nn.Conv3d(
                 self.in_channels,
                 self.kernel_size[0] * self.kernel_size[1] * self.kernel_size[2] * self.mask_groups,
                 kernel_size=self.kernel_size,  # type: ignore[arg-type]
                 stride=self.stride,  # type: ignore[arg-type]
@@ -840,28 +844,30 @@
                 dilation=self.dilation,  # type: ignore[arg-type]
                 groups=self.groups,
                 bias=self.bias is not None,
                 device=dtype,
                 dtype=device)
         else:
             self.register_module('conv_mask', None)
+
+        self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.ones_(self.conv_mask.weight)
+            init.zeros_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
```

### Comparing `tvdcn-0.2.3/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.2.4/tvdcn/ops/deform_conv_transpose.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from typing import List, Tuple, Optional, Union
+
 import torch
 from torch import nn, Tensor
-from torch.jit.annotations import List, Optional, Tuple, Union
 from torch.nn import init
 from torch.nn.common_types import _size_1_t, _size_2_t, _size_3_t
 from torch.nn.modules.utils import _single, _pair, _triple
 
-from .deform_conv import _DeformConvNd
 # noinspection PyUnresolvedReferences
-from .mask_activation import MaskSoftmax1d, MaskSoftmax2d, MaskSoftmax3d
+from .activations import (
+    MaskSigmoid, MaskSoftmax1d, MaskSoftmax2d, MaskSoftmax3d,
+)
+from .deform_conv import _DeformConvNd
 from .._types import _IntTuple, _Activation
 from ..extension import _assert_has_ops
 from ..utils import _log_api_usage_once
 
 __all__ = [
     'deform_conv_transpose1d',
     'deform_conv_transpose2d',
@@ -70,49 +73,49 @@
         >>> print(out.shape)
         Output:
         >>>  torch.Size([4, 5, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose1d)
     _assert_has_ops()
-    out_channels = weight.shape[1] // groups
+    out_channels = weight.size(1) // groups
 
     deformable = offset is not None
     modulated = mask is not None
 
     if offset is None:
-        offset = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if mask is None:
-        mask = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if bias is None:
         bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
 
     stride = _single(stride)
     pad = _single(padding)
     out_pad = _single(output_padding)
     dil = _single(dilation)
 
-    weight_w = weight.shape[-1]
-    _, _, in_w = input.shape
+    weight_w = weight.size(-1)
+    _, _, in_w = input.size()
 
-    offset_groups = offset.shape[1] // weight_w
-    mask_groups = mask.shape[1] // weight_w
+    offset_groups = offset.size(1) // weight_w
+    mask_groups = mask.size(1) // weight_w
 
     if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size[2].\n"
-            "Got offset.shape[1]={}, while weight.size[2]={}".format(
-                offset.shape[1], weight_w))
+            "be a multiple of weight.size(2).\n"
+            "Got offset.size(1)={}, while weight.size(2)={}".format(
+                offset.size(1), weight_w))
     if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size[2].\n"
-            "Got mask.shape[1]={}, while weight.size[2]={}".format(
-                mask.shape[1], weight_w))
+            "be a multiple of weight.size(2).\n"
+            "Got mask.size(1)={}, while weight.size(2)={}".format(
+                mask.size(1), weight_w))
 
     return torch.ops.tvdcn.deform_conv_transpose1d(
         input,
         weight,
         offset,
         mask,
         bias,
@@ -174,48 +177,48 @@
         >>> print(out.shape)
         Output:
         >>>  torch.Size([4, 5, 10, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose2d)
     _assert_has_ops()
-    out_channels = weight.shape[1] // groups
+    out_channels = weight.size(1) // groups
 
     deformable = offset is not None
     modulated = mask is not None
 
     if offset is None:
-        offset = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if mask is None:
-        mask = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if bias is None:
         bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
 
     stride_h, stride_w = _pair(stride)
     pad_h, pad_w = _pair(padding)
     out_pad_h, out_pad_w = _pair(output_padding)
     dil_h, dil_w = _pair(dilation)
-    weight_h, weight_w = weight.shape[-2:]
-    _, _, in_h, in_w = input.shape
+    weight_h, weight_w = weight.size()[-2:]
+    _, _, in_h, in_w = input.size()
 
-    offset_groups = offset.shape[1] // (2 * weight_h * weight_w)
-    mask_groups = mask.shape[1] // (weight_h * weight_w)
+    offset_groups = offset.size(1) // (2 * weight_h * weight_w)
+    mask_groups = mask.size(1) // (weight_h * weight_w)
 
     if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of 2 * weight.size[2] * weight.size[3].\n"
-            "Got offset.shape[1]={}, while 2 * weight.size[2] * weight.size[3]={}".format(
-                offset.shape[1], 2 * weight_h * weight_w))
+            "be a multiple of 2 * weight.size(2) * weight.size(3).\n"
+            "Got offset.size(1)={}, while 2 * weight.size(2) * weight.size(3)={}".format(
+                offset.size(1), 2 * weight_h * weight_w))
     if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size[2] * weight.size[3].\n"
-            "Got mask.shape[1]={}, while weight.size[2] * weight.size[3]={}".format(
-                mask.shape[1], weight_h * weight_w))
+            "be a multiple of weight.size(2) * weight.size(3).\n"
+            "Got mask.size(1)={}, while weight.size(2) * weight.size(3)={}".format(
+                mask.size(1), weight_h * weight_w))
 
     return torch.ops.tvdcn.deform_conv_transpose2d(
         input,
         weight,
         offset,
         mask,
         bias,
@@ -278,48 +281,48 @@
         >>> print(out.shape)
         Output:
         >>> torch.Size([4, 5, 10, 10, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose3d)
     _assert_has_ops()
-    out_channels = weight.shape[1] // groups
+    out_channels = weight.size(1) // groups
 
     deformable = offset is not None
     modulated = mask is not None
 
     if offset is None:
-        offset = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if mask is None:
-        mask = torch.zeros((input.shape[0], 0), device=input.device, dtype=input.dtype)
+        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
     if bias is None:
         bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
 
     stride_d, stride_h, stride_w = _triple(stride)
     pad_d, pad_h, pad_w = _triple(padding)
     out_pad_d, out_pad_h, out_pad_w = _triple(output_padding)
     dil_d, dil_h, dil_w = _triple(dilation)
-    weight_d, weight_h, weight_w = weight.shape[-3:]
-    _, _, in_d, in_h, in_w = input.shape
+    weight_d, weight_h, weight_w = weight.size()[-3:]
+    _, _, in_d, in_h, in_w = input.size()
 
-    offset_groups = offset.shape[1] // (3 * weight_d * weight_h * weight_w)
-    mask_groups = mask.shape[1] // (weight_d * weight_h * weight_w)
+    offset_groups = offset.size(1) // (3 * weight_d * weight_h * weight_w)
+    mask_groups = mask.size(1) // (weight_d * weight_h * weight_w)
 
     if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of 3 * weight.size[2] * weight.size[3] * weight.size[4].\n"
-            "Got offset.shape[1]={}, while 3 * weight.size[2] * weight.size[3] * weight.size[4]={}".format(
-                offset.shape[1], 3 * weight_d * weight_h * weight_w))
+            "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\n"
+            "Got offset.size(1)={}, while 3 * weight.size(2) * weight.size(3) * weight.size(4)={}".format(
+                offset.size(1), 3 * weight_d * weight_h * weight_w))
     if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size[2] * weight.size[3] * weight.size[4].\n"
-            "Got mask.shape[1]={}, while weight.size[2] * weight.size[3] * weight.size[4]={}".format(
-                mask.shape[1], weight_d * weight_h * weight_w))
+            "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\n"
+            "Got mask.size(1)={}, while weight.size(2) * weight.size(3) * weight.size(4)={}".format(
+                mask.size(1), weight_d * weight_h * weight_w))
 
     return torch.ops.tvdcn.deform_conv_transpose3d(
         input,
         weight,
         offset,
         mask,
         bias,
@@ -420,15 +423,15 @@
                 mask: Optional[Tensor] = None,
                 output_size: Optional[List[int]] = None) -> Tensor:
         return self._conv_transpose_forward(input, self.weight, offset, mask, self.bias, output_size)
 
 
 class DeformConvTranspose1d(_DeformConvTransposeNd):
     """
-    See :func:`deform_conv_transpose1d`
+    See :func:`deform_conv_transpose1d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_1_t,
                  stride: _size_1_t = 1,
@@ -471,15 +474,15 @@
                                        self.stride, self.padding,
                                        (output_padding[0],),
                                        self.dilation, self.groups)
 
 
 class DeformConvTranspose2d(_DeformConvTransposeNd):
     """
-    See :func:`deform_conv_transpose2d`
+    See :func:`deform_conv_transpose2d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_2_t,
                  stride: _size_2_t = 1,
@@ -523,15 +526,15 @@
                                        self.stride, self.padding,  # type: ignore[arg-type]
                                        (output_padding[0], output_padding[1]),
                                        self.dilation, self.groups)  # type: ignore[arg-type]
 
 
 class DeformConvTranspose3d(_DeformConvTransposeNd):
     """
-    See :func:`deform_conv_transpose3d`
+    See :func:`deform_conv_transpose3d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_3_t,
                  stride: _size_3_t = 1,
@@ -579,15 +582,15 @@
 
 ################################################################################
 # Packed Modules
 ################################################################################
 # noinspection PyMethodOverriding
 class PackedDeformConvTranspose1d(DeformConvTranspose1d):
     """
-    Packed version of :class:`DeformConvTranspose1d`
+    Packed version of :class:`DeformConvTranspose1d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_1_t,
                  stride: _size_1_t = 1,
@@ -597,15 +600,15 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'softmax',
+                 mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             output_padding, groups, bias, padding_mode, device, dtype)
 
@@ -619,15 +622,15 @@
         if out_channels % mask_groups != 0:
             raise ValueError('out_channels must be divisible by mask_groups')
 
         if isinstance(offset_activation, str):
             raise ValueError('currently, no activation is supported for offset')
         if isinstance(mask_activation, str):
             if mask_activation == 'sigmoid':
-                mask_activation = nn.Sigmoid()
+                mask_activation = MaskSigmoid(scale=2.)
             elif mask_activation == 'softmax':
                 mask_activation = MaskSoftmax1d(self.kernel_size)  # type: ignore[arg-type]
             else:
                 raise ValueError('only \"sigmoid\" and \"softmax\" activations are supported for mask')
 
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
@@ -641,40 +644,41 @@
                 self.kernel_size[0] * self.offset_groups,
                 kernel_size=1,
                 bias=self.bias is not None,
                 device=dtype,
                 dtype=device)
         else:
             self.register_module('conv_offset', None)
-        self.offset_activation = offset_activation
 
         if self.modulated:
             self.conv_mask = nn.Conv1d(
                 self.in_channels,
                 self.kernel_size[0] * self.mask_groups,
                 kernel_size=1,
                 bias=self.bias is not None,
                 device=dtype,
                 dtype=device)
         else:
             self.register_module('conv_mask', None)
+
+        self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.ones_(self.conv_mask.weight)
+            init.zeros_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor, output_size: Optional[List[int]] = None) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
@@ -691,15 +695,15 @@
 
         return self._conv_transpose_forward(input, self.weight, offset, mask, self.bias, output_size)
 
 
 # noinspection PyMethodOverriding
 class PackedDeformConvTranspose2d(DeformConvTranspose2d):
     """
-    Packed version of :class:`DeformConvTranspose2d`
+    Packed version of :class:`DeformConvTranspose2d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_2_t,
                  stride: _size_2_t = 1,
@@ -709,15 +713,15 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'softmax',
+                 mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             output_padding, groups, bias, padding_mode, device, dtype)
 
@@ -731,15 +735,15 @@
         if out_channels % mask_groups != 0:
             raise ValueError('out_channels must be divisible by mask_groups')
 
         if isinstance(offset_activation, str):
             raise ValueError('currently, no activation is supported for offset')
         if isinstance(mask_activation, str):
             if mask_activation == 'sigmoid':
-                mask_activation = nn.Sigmoid()
+                mask_activation = MaskSigmoid(scale=2.)
             elif mask_activation == 'softmax':
                 mask_activation = MaskSoftmax2d(self.kernel_size)  # type: ignore[arg-type]
             else:
                 raise ValueError('only \"sigmoid\" and \"softmax\" activations are supported for mask')
 
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
@@ -765,28 +769,30 @@
                 self.kernel_size[0] * self.kernel_size[1] * self.mask_groups,
                 kernel_size=1,
                 bias=self.bias is not None,
                 device=dtype,
                 dtype=device)
         else:
             self.register_module('conv_mask', None)
+
+        self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.ones_(self.conv_mask.weight)
+            init.zeros_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor, output_size: Optional[List[int]] = None) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
@@ -803,15 +809,15 @@
 
         return self._conv_transpose_forward(input, self.weight, offset, mask, self.bias, output_size)
 
 
 # noinspection PyMethodOverriding
 class PackedDeformConvTranspose3d(DeformConvTranspose3d):
     """
-    Packed version of :class:`DeformConvTranspose3d`
+    Packed version of :class:`DeformConvTranspose3d`.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_3_t,
                  stride: _size_3_t = 1,
@@ -821,15 +827,15 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'softmax',
+                 mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             output_padding, groups, bias, padding_mode, device, dtype)
 
@@ -843,15 +849,15 @@
         if out_channels % mask_groups != 0:
             raise ValueError('out_channels must be divisible by mask_groups')
 
         if isinstance(offset_activation, str):
             raise ValueError('currently, no activation is supported for offset')
         if isinstance(mask_activation, str):
             if mask_activation == 'sigmoid':
-                mask_activation = nn.Sigmoid()
+                mask_activation = MaskSigmoid(scale=2.)
             elif mask_activation == 'softmax':
                 mask_activation = MaskSoftmax3d(self.kernel_size)  # type: ignore[arg-type]
             else:
                 raise ValueError('only \"sigmoid\" and \"softmax\" activations are supported for mask')
 
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
@@ -877,28 +883,30 @@
                 self.kernel_size[0] * self.kernel_size[1] * self.kernel_size[2] * self.mask_groups,
                 kernel_size=1,
                 bias=self.bias is not None,
                 device=dtype,
                 dtype=device)
         else:
             self.register_module('conv_mask', None)
+
+        self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.ones_(self.conv_mask.weight)
+            init.zeros_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor, output_size: Optional[List[int]] = None) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
```

### Comparing `tvdcn-0.2.3/tvdcn/ops/mask_activation.py` & `tvdcn-0.2.4/tvdcn/ops/activations/mask_softmax.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from typing import Tuple, Optional
+
 import torch
 import torch.nn as nn
 from torch import Tensor
-from torch.jit.annotations import Tuple, Optional
 from torch.nn.common_types import _size_1_t, _size_2_t, _size_3_t
 from torch.nn.modules.utils import _single, _pair, _triple
 
-from .._types import _IntTuple
+from tvdcn._types import _IntTuple
 
 __all__ = [
     'mask_softmax1d',
     'mask_softmax2d',
     'mask_softmax3d',
     'MaskSoftmax1d',
     'MaskSoftmax2d',
@@ -32,16 +33,16 @@
     weight_w, = _single(kernel_size)
     mask_groups = mask.size(1) // weight_w
 
     if mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
             "be a multiple of kernel_size[0].\n"
-            "Got mask.shape[1]={}, while kernel_size[0]={}".format(
-                mask.shape[1], weight_w))
+            "Got mask.size(1)={}, while kernel_size[0]={}".format(
+                mask.size(1), weight_w))
 
     mask = mask.view(batch_size,
                      mask_groups,
                      weight_w,
                      out_width)
     mask = torch.softmax(mask, dim=2)
     mask = mask.view(batch_size,
@@ -69,16 +70,16 @@
     weight_h, weight_w = _pair(kernel_size)
     mask_groups = mask.size(1) // (weight_h * weight_w)
 
     if mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
             "be a multiple of kernel_size[0] * kernel_size[1].\n"
-            "Got mask.shape[1]={}, while kernel_size[0] * kernel_size[1]={}".format(
-                mask.shape[1], weight_h * weight_w))
+            "Got mask.size(1)={}, while kernel_size[0] * kernel_size[1]={}".format(
+                mask.size(1), weight_h * weight_w))
 
     mask = mask.view(batch_size,
                      mask_groups,
                      weight_h * weight_w,
                      out_height,
                      out_width)
     mask = torch.softmax(mask, dim=2)
@@ -105,16 +106,16 @@
     weight_d, weight_h, weight_w = _triple(kernel_size)
     mask_groups = mask.size(1) // (weight_d * weight_h * weight_w)
 
     if mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
             "be a multiple of kernel_size[0] * kernel_size[1] * kernel_size[2].\n"
-            "Got mask.shape[1]={}, while kernel_size[0] * kernel_size[1] * kernel_size[2]={}".format(
-                mask.shape[1], weight_d * weight_h * weight_w))
+            "Got mask.size(1)={}, while kernel_size[0] * kernel_size[1] * kernel_size[2]={}".format(
+                mask.size(1), weight_d * weight_h * weight_w))
 
     mask = mask.view(batch_size,
                      mask_groups,
                      weight_d * weight_h * weight_w,
                      out_depth,
                      out_height,
                      out_width)
```

### Comparing `tvdcn-0.2.3/tvdcn/utils.py` & `tvdcn-0.2.4/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.3/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.2.4/tvdcn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.3
+Version: 0.2.4
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
@@ -57,46 +57,45 @@
   - `tvdcn.ops.deform_conv_transpose3d`
 
 - And the following **supplementary operations** (for activating `mask`):
   - `tvdcn.ops.mask_softmax1d`
   - `tvdcn.ops.mask_softmax2d`
   - `tvdcn.ops.mask_softmax3d`
 
-- Both `offset` and `mask` can turned off, and can be applied in separate groups
-  ([Deformable Convolution v3](https://arxiv.org/abs/2211.05778)).
+- Both `offset` and `mask` can be turned off, and can be applied in separate groups.
 
 - All the `nn.Module` wrappers for these operations are implemented,
   everything is `@torch.jit.script`-able! Please check [Usage](#usage).
 
 **Note:** We don't care much about `onnx` exportation, but if you do, you can check this repo:
 https://github.com/masamitsu-murase/deform_conv2d_onnx_exporter.
 
 ## Requirements
 
-- `torch>=1.8`
+- `torch>=1.9.0`
 
 ## Installation
 
 #### From PyPI:
 
 [tvdcn](https://pypi.org/project/tvdcn) provides some prebuilt wheels on **PyPI**.
 Run this command to install:
 
 ```terminal
 pip install tvdcn
 ```
 
-The Linux and Windows wheels are built with **Cuda 11.8**, which is compatible with `torch==2.0.0`.
+The Linux and Windows wheels are built with **Cuda 11.8**.
 If you cannot find a wheel for your Arch/Python/Cuda, or there is any problem with library linking when importing,
 please proceed to [instructions to build from source](#from-source), all steps are super easy.
 
 |                  |     Linux/Windows     |     MacOS      |
 |------------------|:---------------------:|:--------------:|
 | Python version:  |       3.8-3.11        |    3.8-3.11    |
-| PyTorch version: |    `torch==2.0.0`     | `torch==2.0.0` |
+| PyTorch version: |    `torch==2.0.1`     | `torch==2.0.1` |
 | Cuda version:    |         11.8          |       -        |
 | GPU CCs:         | `6.1,7.5,8.6,8.9+PTX` |       -        |
 
 #### From Source:
 
 For installing from source, you need a C++ compiler (`gcc`/`msvc`) and a Cuda compiler (`nvcc`).
 Clone this repo and execute the following command:
@@ -208,22 +207,28 @@
 
 These are easy-to-use classes that contain ordinary convolution layers with appropriate hyperparameters to generate
 `offset` (and `mask` if initialized with `modulated=True`);
 but that means less customization.
 The only tunable hyperparameters that effect these supplementary conv layers are `offset_groups` and `mask_groups`,
 which have been decoupled from and behave somewhat similar to `groups`.
 
+To use the softmax activation for mask proposed in [Deformable Convolution v3](https://arxiv.org/abs/2211.05778),
+set `mask_activation='softmax'`. `offset_activation` and `mask_activation` also accept any `nn.Module`.
+
 ```python
 import torch
 
 from tvdcn import PackedDeformConv1d
 
 input = torch.rand(2, 3, 128)
 
-conv = PackedDeformConv1d(3, 16, kernel_size=5, modulated=True)
+conv = PackedDeformConv1d(3, 16,
+                          kernel_size=5,
+                          modulated=True,
+                          mask_activation='softmax')
 # jit scripting
 scripted_conv = torch.jit.script(conv)
 print(scripted_conv)
 
 output = scripted_conv(input)
 print(output.shape)
 ```
```

### Comparing `tvdcn-0.2.3/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.2.4/tvdcn.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -28,8 +28,10 @@
 tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
 tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
 tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
 tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
 tvdcn/ops/__init__.py
 tvdcn/ops/deform_conv.py
 tvdcn/ops/deform_conv_transpose.py
-tvdcn/ops/mask_activation.py
+tvdcn/ops/activations/__init__.py
+tvdcn/ops/activations/mask_sigmoid.py
+tvdcn/ops/activations/mask_softmax.py
```


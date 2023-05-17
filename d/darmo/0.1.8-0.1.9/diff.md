# Comparing `tmp/darmo-0.1.8.tar.gz` & `tmp/darmo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/darmo-0.1.8.tar", last modified: Mon Sep 20 15:59:46 2021, max compression
+gzip compressed data, was "dist/darmo-0.1.9.tar", last modified: Mon Sep 20 16:10:41 2021, max compression
```

## Comparing `darmo-0.1.8.tar` & `darmo-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 15:59:46.000000 darmo-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-09-20 15:59:34.000000 darmo-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo/
--rw-r--r--   0 runner    (1001) docker     (121)    10139 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/nsga.py
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/resnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     6489 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/network.py
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo/config/
--rw-r--r--   0 runner    (1001) docker     (121)    10520 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/config/eeea_c1.config
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/config/eeea_c2.subnet
--rw-r--r--   0 runner    (1001) docker     (121)    15486 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/config/eeea_c2.config
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/config/eeea_c1.subnet
--rw-r--r--   0 runner    (1001) docker     (121)    16318 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/config/ofa595.config
--rw-r--r--   0 runner    (1001) docker     (121)     4949 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo/layers/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo/layers/tresnetv1/
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/layers/tresnetv1/anti_aliasing.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/layers/tresnetv1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2963 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/layers/tresnetv1/general_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/layers/tresnetv1/inplace_abn.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/layers/tresnetv1/avg_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo/layers/tresnetv2/
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/layers/tresnetv2/anti_aliasing.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/layers/tresnetv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/layers/tresnetv2/squeeze_and_excite.py
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/layers/tresnetv2/space_to_depth.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/layers/tresnetv2/avg_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)    31577 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    10476 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/tresnetv2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9679 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/tresnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3966 2021-09-20 15:59:34.000000 darmo-0.1.8/darmo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      890 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      273 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-09-20 15:59:46.000000 darmo-0.1.8/darmo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      273 2021-09-20 15:59:46.000000 darmo-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-09-20 15:59:34.000000 darmo-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-20 15:59:46.000000 darmo-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 16:10:41.000000 darmo-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2021-09-20 16:10:27.000000 darmo-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 16:10:41.000000 darmo-0.1.9/darmo/
+-rw-r--r--   0 runner    (1001) docker     (121)    10139 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/nsga.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1657 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1555 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1131 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6489 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 16:10:41.000000 darmo-0.1.9/darmo/config/
+-rw-r--r--   0 runner    (1001) docker     (121)    10520 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/config/eeea_c1.config
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/config/eeea_c2.subnet
+-rw-r--r--   0 runner    (1001) docker     (121)    15486 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/config/eeea_c2.config
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/config/eeea_c1.subnet
+-rw-r--r--   0 runner    (1001) docker     (121)    16318 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/config/ofa595.config
+-rw-r--r--   0 runner    (1001) docker     (121)     4924 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 16:10:41.000000 darmo-0.1.9/darmo/layers/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 16:10:41.000000 darmo-0.1.9/darmo/layers/tresnetv1/
+-rw-r--r--   0 runner    (1001) docker     (121)     2016 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/layers/tresnetv1/anti_aliasing.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/layers/tresnetv1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2963 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/layers/tresnetv1/general_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3352 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/layers/tresnetv1/inplace_abn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/layers/tresnetv1/avg_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31577 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9679 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/tresnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3966 2021-09-20 16:10:27.000000 darmo-0.1.9/darmo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 16:10:41.000000 darmo-0.1.9/darmo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2021-09-20 16:10:40.000000 darmo-0.1.9/darmo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-20 16:10:40.000000 darmo-0.1.9/darmo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-20 16:10:40.000000 darmo-0.1.9/darmo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2021-09-20 16:10:40.000000 darmo-0.1.9/darmo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-09-20 16:10:40.000000 darmo-0.1.9/darmo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2021-09-20 16:10:41.000000 darmo-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2795 2021-09-20 16:10:27.000000 darmo-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-20 16:10:41.000000 darmo-0.1.9/setup.cfg
```

### Comparing `darmo-0.1.8/darmo/nsga.py` & `darmo-0.1.9/darmo/nsga.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/resnet.py` & `darmo-0.1.9/darmo/resnet.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/utils.py` & `darmo-0.1.9/darmo/utils.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/factory.py` & `darmo-0.1.9/darmo/factory.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/network.py` & `darmo-0.1.9/darmo/network.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/operations.py` & `darmo-0.1.9/darmo/operations.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/config/eeea_c1.config` & `darmo-0.1.9/darmo/config/eeea_c1.config`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/config/eeea_c2.config` & `darmo-0.1.9/darmo/config/eeea_c2.config`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/config/ofa595.config` & `darmo-0.1.9/darmo/config/ofa595.config`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/__init__.py` & `darmo-0.1.9/darmo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from collections import namedtuple
 import torch.utils.model_zoo as model_zoo
 import json
 import pkg_resources
 
 from .resnet import *
 from .tresnet import *
-from .tresnetv2 import *
 from .nasnet import NASNetAMobile
 from .nsga import *
 
 Genotype = namedtuple('Genotype', 'normal normal_concat reduce reduce_concat')
 
 url_cfgs = {
     'dartsv2': 'https://github.com/jitdee-ai/darts-models/releases/download/0.0.1/dartv2.pt',
```

### Comparing `darmo-0.1.8/darmo/layers/tresnetv1/anti_aliasing.py` & `darmo-0.1.9/darmo/layers/tresnetv1/anti_aliasing.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/layers/tresnetv1/general_layers.py` & `darmo-0.1.9/darmo/layers/tresnetv1/general_layers.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/layers/tresnetv1/inplace_abn.py` & `darmo-0.1.9/darmo/layers/tresnetv1/inplace_abn.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/nasnet.py` & `darmo-0.1.9/darmo/nasnet.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo/tresnetv2.py` & `darmo-0.1.9/darmo/tresnet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,81 +1,60 @@
-from collections import OrderedDict
-from functools import partial
-import torch.nn as nn
 import torch
+import torch.nn as nn
 from torch.nn import Module as Module
-from .layers.tresnetv2.anti_aliasing import AntiAliasDownsampleLayer
-from .layers.tresnetv2.avg_pool import FastGlobalAvgPool2d
-from .layers.tresnetv2.space_to_depth import SpaceToDepthModule
-from .layers.tresnetv2.squeeze_and_excite import SEModule
-
-try:
-    from inplace_abn import InPlaceABN
-    from inplace_abn import ABN
-except ImportError:
-    raise ImportError(
-            "We supported only Linux system, Please install InplaceABN:'pip install inplace-abn'")
+from collections import OrderedDict
+from .layers.tresnetv1.anti_aliasing import AntiAliasDownsampleLayer
+from .layers.tresnetv1.avg_pool import FastAvgPool2d
+from .layers.tresnetv1.general_layers import SEModule, SpaceToDepthModule
+from .layers.tresnetv1.inplace_abn import InplaceAbn
 
 from .registry import register_model
 from .utils import _set_config, _load
 
 url_cfgs = {
-    'tresnetv2_l_21k' : 'https://github.com/jitdee-ai/darmo/releases/download/0.0.1/tresnet_l_v2_miil_21k.pth',
+    'tresnet_m_21k' : 'https://github.com/jitdee-ai/darmo/releases/download/0.0.1/tresnet_m_miil_21k.pth',
 }
 
 @register_model
-def tresnetv2_l_21k(pretrained=True, num_classes=11221, auxiliary=False):
+def tresnet_m_21k(pretrained=True, num_classes=11221, auxiliary=False):
     model_params = {'num_classes': 11221}
 
-    config = _set_config(_config={}, name= 'tresnetv2_l_21k', first_channels=46, layers=14, auxiliary=auxiliary, 
+    config = _set_config(_config={}, name= 'tresnet_m_21k', first_channels=46, layers=14, auxiliary=auxiliary, 
                         genotype=None, last_bn=False, pretrained=pretrained, num_classes=11221)
 
-    base_net = TResnetL_V2(model_params)
+    base_net = TResnetM(model_params)
     _load(config, base_net, url_cfgs, True)
     return base_net
 
-def InplacABN_to_ABN(module: nn.Module) -> nn.Module:
-    # convert all InplaceABN layer to bit-accurate ABN layers.
-    if isinstance(module, InPlaceABN):
-        module_new = ABN(module.num_features, activation=module.activation,
-                         activation_param=module.activation_param)
-        for key in module.state_dict():
-            module_new.state_dict()[key].copy_(module.state_dict()[key])
-        module_new.training = module.training
-        module_new.weight.data = module_new.weight.abs() + module_new.eps
-        return module_new
-    for name, child in reversed(module._modules.items()):
-        new_child = InplacABN_to_ABN(child)
-        if new_child != child:
-            module._modules[name] = new_child
-    return module
-
+class bottleneck_head(nn.Module):
+    def __init__(self, num_features, num_classes, bottleneck_features=200):
+        super(bottleneck_head, self).__init__()
+        self.embedding_generator = nn.ModuleList()
+        self.embedding_generator.append(nn.Linear(num_features, bottleneck_features))
+        self.embedding_generator = nn.Sequential(*self.embedding_generator)
+        self.FC = nn.Linear(bottleneck_features, num_classes)
 
-def conv3x3(in_planes, out_planes, stride=1):
-    return nn.Conv2d(in_planes, out_planes, kernel_size=3, stride=stride, padding=1, bias=False)
-
-
-def conv3x3_depth(planes, stride=1):
-    return nn.Conv2d(planes, planes, groups=planes, kernel_size=3, stride=stride, padding=1, bias=False)
+    def forward(self, x):
+        self.embedding = self.embedding_generator(x)
+        logits = self.FC(self.embedding)
+        return logits
 
 
 def conv2d(ni, nf, stride):
     return nn.Sequential(
         nn.Conv2d(ni, nf, kernel_size=3, stride=stride, padding=1, bias=False),
         nn.BatchNorm2d(nf),
         nn.ReLU(inplace=True)
     )
 
 
 def conv2d_ABN(ni, nf, stride, activation="leaky_relu", kernel_size=3, activation_param=1e-2, groups=1):
-    activation_param = 1e-6
     return nn.Sequential(
-        nn.Conv2d(ni, nf, kernel_size=kernel_size, stride=stride, padding=kernel_size // 2, groups=groups,
-                  bias=False),
-        InPlaceABN(num_features=nf, activation=activation, activation_param=activation_param)
+        nn.Conv2d(ni, nf, kernel_size=kernel_size, stride=stride, padding=kernel_size // 2, groups=groups, bias=False), 
+        InplaceAbn(num_features=nf, act_layer=activation, act_param=activation_param)
     )
 
 
 class BasicBlock(Module):
     expansion = 1
 
     def __init__(self, inplanes, planes, stride=1, downsample=None, use_se=True, anti_alias_layer=None):
@@ -90,16 +69,15 @@
                                            anti_alias_layer(channels=planes, filt_size=3, stride=2))
 
         self.conv2 = conv2d_ABN(planes, planes, stride=1, activation="identity")
         self.relu = nn.ReLU(inplace=True)
         self.downsample = downsample
         self.stride = stride
         reduce_layer_planes = max(planes * self.expansion // 4, 64)
-        self.se = SEModule(channels=planes * self.expansion, reduction_channels=reduce_layer_planes) if \
-            use_se else None
+        self.se = SEModule(planes * self.expansion, reduce_layer_planes) if use_se else None
 
     def forward(self, x):
         if self.downsample is not None:
             residual = self.downsample(x)
         else:
             residual = x
 
@@ -157,101 +135,101 @@
         out = self.conv3(out)
         out = out + residual  # no inplace
         out = self.relu(out)
 
         return out
 
 
-class TResNetV2(Module):
+class TResNet(Module):
 
-    def __init__(self, layers, in_chans=3, num_classes=1000, width_factor=1.0, remove_model_jit=False):
-        super(TResNetV2, self).__init__()
-        ## body
-        self.inplanes = int(int(64 * width_factor + 4) / 8) * 8
-        self.planes = int(int(64 * width_factor + 4) / 8) * 8
-        SpaceToDepth = SpaceToDepthModule(remove_model_jit=remove_model_jit)
+    def __init__(self, layers, in_chans=3, num_classes=1000, width_factor=1.0,
+                 do_bottleneck_head=False, bottleneck_features=512, first_two_layers=BasicBlock):
+        super(TResNet, self).__init__()
+
+        # JIT layers
+        space_to_depth = SpaceToDepthModule()
+        anti_alias_layer = AntiAliasDownsampleLayer
+        global_pool_layer = FastAvgPool2d(flatten=True)
+
+        # TResnet stages
+        self.inplanes = int(64 * width_factor)
+        self.planes = int(64 * width_factor)
         conv1 = conv2d_ABN(in_chans * 16, self.planes, stride=1, kernel_size=3)
-
-        anti_alias_layer = partial(AntiAliasDownsampleLayer, remove_aa_jit=remove_model_jit)
-        global_pool_layer = FastGlobalAvgPool2d(flatten=True)
-        layer1 = self._make_layer(Bottleneck, self.planes, layers[0], stride=1, use_se=True,
+        layer1 = self._make_layer(first_two_layers, self.planes, layers[0], stride=1, use_se=True,
                                   anti_alias_layer=anti_alias_layer)  # 56x56
-        layer2 = self._make_layer(Bottleneck, self.planes * 2, layers[1], stride=2, use_se=True,
+        layer2 = self._make_layer(first_two_layers, self.planes * 2, layers[1], stride=2, use_se=True,
                                   anti_alias_layer=anti_alias_layer)  # 28x28
         layer3 = self._make_layer(Bottleneck, self.planes * 4, layers[2], stride=2, use_se=True,
                                   anti_alias_layer=anti_alias_layer)  # 14x14
         layer4 = self._make_layer(Bottleneck, self.planes * 8, layers[3], stride=2, use_se=False,
                                   anti_alias_layer=anti_alias_layer)  # 7x7
 
+        # body
         self.body = nn.Sequential(OrderedDict([
-            ('SpaceToDepth', SpaceToDepth),
+            ('SpaceToDepth', space_to_depth),
             ('conv1', conv1),
             ('layer1', layer1),
             ('layer2', layer2),
             ('layer3', layer3),
             ('layer4', layer4)]))
 
-        # default head
-        self.num_features = (self.planes * 8) * Bottleneck.expansion
-
-        fc = nn.Linear(self.num_features , num_classes)
-
+        # head
+        self.embeddings = []
         self.global_pool = nn.Sequential(OrderedDict([('global_pool_layer', global_pool_layer)]))
+        self.num_features = (self.planes * 8) * Bottleneck.expansion
+        if do_bottleneck_head:
+            fc = bottleneck_head(self.num_features, num_classes,
+                                 bottleneck_features=bottleneck_features)
+        else:
+            fc = nn.Linear(self.num_features, num_classes)
 
         self.head = nn.Sequential(OrderedDict([('fc', fc)]))
 
-        self.embeddings = []
-
+        # model initilization
         for m in self.modules():
             if isinstance(m, nn.Conv2d):
                 nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='leaky_relu')
-            elif isinstance(m, nn.BatchNorm2d) or isinstance(m, InPlaceABN):
+            elif isinstance(m, nn.BatchNorm2d) or isinstance(m, InplaceAbn):
                 nn.init.constant_(m.weight, 1)
                 nn.init.constant_(m.bias, 0)
 
-        # initilize resnet in a magic way
+        # residual connections special initialization
         for m in self.modules():
             if isinstance(m, BasicBlock):
                 m.conv2[1].weight = nn.Parameter(torch.zeros_like(m.conv2[1].weight))  # BN to zero
             if isinstance(m, Bottleneck):
                 m.conv3[1].weight = nn.Parameter(torch.zeros_like(m.conv3[1].weight))  # BN to zero
             if isinstance(m, nn.Linear): m.weight.data.normal_(0, 0.01)
 
     def _make_layer(self, block, planes, blocks, stride=1, use_se=True, anti_alias_layer=None):
         downsample = None
         if stride != 1 or self.inplanes != planes * block.expansion:
             layers = []
             if stride == 2:
                 # avg pooling before 1x1 conv
-                layers.append(
-                    nn.AvgPool2d(kernel_size=2, stride=2, ceil_mode=True, count_include_pad=False))
-            layers += [
-                conv2d_ABN(self.inplanes, planes * block.expansion, kernel_size=1, stride=1,
-                           activation="identity")]
+                layers.append(nn.AvgPool2d(kernel_size=2, stride=2, ceil_mode=True, count_include_pad=False))
+            layers += [conv2d_ABN(self.inplanes, planes * block.expansion, kernel_size=1, stride=1,
+                                  activation="identity")]
             downsample = nn.Sequential(*layers)
 
         layers = []
         layers.append(block(self.inplanes, planes, stride, downsample, use_se=use_se,
                             anti_alias_layer=anti_alias_layer))
         self.inplanes = planes * block.expansion
         for i in range(1, blocks): layers.append(
             block(self.inplanes, planes, use_se=use_se, anti_alias_layer=anti_alias_layer))
         return nn.Sequential(*layers)
 
     def forward(self, x):
         x = self.body(x)
-        # self.embeddings = self.global_pool(x)
-        logits = self.head(self.global_pool(x))
+        self.embeddings = self.global_pool(x)
+        logits = self.head(self.embeddings)
         return logits
 
 
-def TResnetL_V2(model_params):
-    """Constructs a large TResnet model.
+def TResnetM(model_params):
+    """Constructs a medium TResnet model.
     """
     in_chans = 3
     num_classes = model_params['num_classes']
-    remove_model_jit = False
-    layers_list = [3, 4, 23, 3]
-    width_factor = 1.0
-    model = TResNetV2(layers=layers_list, num_classes=num_classes, in_chans=in_chans,
-                      width_factor=width_factor, remove_model_jit=remove_model_jit)
+    model = TResNet(layers=[3, 4, 11, 3], num_classes=num_classes, in_chans=in_chans)
     return model
```

### Comparing `darmo-0.1.8/darmo/registry.py` & `darmo-0.1.9/darmo/registry.py`

 * *Files identical despite different names*

### Comparing `darmo-0.1.8/darmo.egg-info/SOURCES.txt` & `darmo-0.1.9/darmo.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 darmo/nasnet.py
 darmo/network.py
 darmo/nsga.py
 darmo/operations.py
 darmo/registry.py
 darmo/resnet.py
 darmo/tresnet.py
-darmo/tresnetv2.py
 darmo/utils.py
 darmo/version.py
 darmo.egg-info/PKG-INFO
 darmo.egg-info/SOURCES.txt
 darmo.egg-info/dependency_links.txt
 darmo.egg-info/requires.txt
 darmo.egg-info/top_level.txt
@@ -22,13 +21,8 @@
 darmo/config/eeea_c2.config
 darmo/config/eeea_c2.subnet
 darmo/config/ofa595.config
 darmo/layers/tresnetv1/__init__.py
 darmo/layers/tresnetv1/anti_aliasing.py
 darmo/layers/tresnetv1/avg_pool.py
 darmo/layers/tresnetv1/general_layers.py
-darmo/layers/tresnetv1/inplace_abn.py
-darmo/layers/tresnetv2/__init__.py
-darmo/layers/tresnetv2/anti_aliasing.py
-darmo/layers/tresnetv2/avg_pool.py
-darmo/layers/tresnetv2/space_to_depth.py
-darmo/layers/tresnetv2/squeeze_and_excite.py
+darmo/layers/tresnetv1/inplace_abn.py
```

### Comparing `darmo-0.1.8/README.md` & `darmo-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ![PyPI Release](https://github.com/jitdee-ai/darts-models/workflows/PyPI%20Release/badge.svg)
 [![DOI](https://zenodo.org/badge/307382940.svg)](https://zenodo.org/badge/latestdoi/307382940)
 
 ## What's New
 
 Sep 20, 2021
  - Add OFA-595 ImageNet-1k and ImageNet-21k, Thank from [21k-weight](https://github.com/Alibaba-MIIL/ImageNet21K) 
- - Add TResNet-M and TResNetV2-L ImageNet-21k, Thank from [21k-weight](https://github.com/Alibaba-MIIL/ImageNet21K)
+ - Add TResNet-M ImageNet-21k, Thank from [21k-weight](https://github.com/Alibaba-MIIL/ImageNet21K)
 
 Sep 5, 2021
  - Add ResNet50 ImageNet-1k and ImageNet-21k, Thank from [21k-weight](https://github.com/Alibaba-MIIL/ImageNet21K)
 
 Aug 17, 2021
  - Add EEEA-Net-C1 model
 
@@ -38,15 +38,15 @@
  - [nasnet](https://arxiv.org/abs/1707.07012)
  - [dartsv2](https://github.com/quark0/darts)
  - [pdarts](https://github.com/chenxin061/pdarts)
  - [relative_nas](https://github.com/EMI-Group/RelativeNAS)
  - [eeea_c1, eeea_c2](https://github.com/chakkritte/EEEA-Net)
  - [resnet50_1k, resnet50_21k](https://arxiv.org/abs/1512.03385)
  - [ofa595_1k, ofa595_21k](https://github.com/mit-han-lab/once-for-all)
- - [tresnet_m_21k, tresnetv2_l_21k](https://github.com/Alibaba-MIIL/TResNet)
+ - [tresnet_m_21k](https://github.com/Alibaba-MIIL/TResNet)
   
 ## Install
 
 The library can be installed with pip:
 
     pip install darmo
```


# Comparing `tmp/conformer-0.2.5.tar.gz` & `tmp/conformer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conformer-0.2.5.tar", last modified: Wed Apr 28 14:30:41 2021, max compression
+gzip compressed data, was "conformer-0.3.0.tar", last modified: Wed May 17 18:17:59 2023, max compression
```

## Comparing `conformer-0.2.5.tar` & `conformer-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 14:30:41.872696 conformer-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (121)      586 2021-04-28 14:30:41.872696 conformer-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-04-28 14:30:34.000000 conformer-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 14:30:41.872696 conformer-0.2.5/conformer/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-04-28 14:30:34.000000 conformer-0.2.5/conformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6230 2021-04-28 14:30:34.000000 conformer-0.2.5/conformer/conformer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 14:30:41.872696 conformer-0.2.5/conformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      586 2021-04-28 14:30:41.000000 conformer-0.2.5/conformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-04-28 14:30:41.000000 conformer-0.2.5/conformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 14:30:41.000000 conformer-0.2.5/conformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-04-28 14:30:41.000000 conformer-0.2.5/conformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-04-28 14:30:41.000000 conformer-0.2.5/conformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-28 14:30:41.872696 conformer-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-04-28 14:30:34.000000 conformer-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:17:59.080335 conformer-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 18:17:49.000000 conformer-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-17 18:17:59.080335 conformer-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-17 18:17:49.000000 conformer-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:17:59.080335 conformer-0.3.0/conformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 18:17:49.000000 conformer-0.3.0/conformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-05-17 18:17:49.000000 conformer-0.3.0/conformer/conformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:17:59.080335 conformer-0.3.0/conformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-17 18:17:58.000000 conformer-0.3.0/conformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-17 18:17:59.000000 conformer-0.3.0/conformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:17:58.000000 conformer-0.3.0/conformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 18:17:58.000000 conformer-0.3.0/conformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 18:17:58.000000 conformer-0.3.0/conformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:17:59.080335 conformer-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-17 18:17:49.000000 conformer-0.3.0/setup.py
```

### Comparing `conformer-0.2.5/PKG-INFO` & `conformer-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: conformer
-Version: 0.2.5
+Version: 0.3.0
 Summary: The convolutional module from the Conformer paper
 Home-page: https://github.com/lucidrains/conformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
-Description: UNKNOWN
-Keywords: transformers,artificial intelligence,transformer
-Platform: UNKNOWN
+Keywords: artificial intelligence,deep learning,transformers,audio
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
```

### Comparing `conformer-0.2.5/README.md` & `conformer-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,47 @@
     conv_kernel_size = 31,
     attn_dropout = 0.,
     ff_dropout = 0.,
     conv_dropout = 0.
 )
 
 x = torch.randn(1, 1024, 512)
+
 block(x) # (1, 1024, 512)
 ```
+
+Conformer - just multiple `ConformerBlock` from above
+
+```python
+import torch
+from conformer import Conformer
+
+conformer = Conformer(
+    dim = 512,
+    depth = 12,          # 12 blocks
+    dim_head = 64,
+    heads = 8,
+    ff_mult = 4,
+    conv_expansion_factor = 2,
+    conv_kernel_size = 31,
+    attn_dropout = 0.,
+    ff_dropout = 0.,
+    conv_dropout = 0.
+)
+
+x = torch.randn(1, 1024, 512)
+
+conformer(x) # (1, 1024, 512)
+```
+
+## Todo
+
+- [ ] switch to a better relative positional encoding. shaw's is dated
+- [ ] flash attention with a better RPE
+
 ## Citations
 
 ```bibtex
 @misc{gulati2020conformer,
     title={Conformer: Convolution-augmented Transformer for Speech Recognition},
     author={Anmol Gulati and James Qin and Chung-Cheng Chiu and Niki Parmar and Yu Zhang and Jiahui Yu and Wei Han and Shibo Wang and Zhengdong Zhang and Yonghui Wu and Ruoming Pang},
     year={2020},
```

#### html2text {}

```diff
@@ -7,13 +7,20 @@
 causal with padding if so expansion_factor = 2, # what multiple of the
 dimension to expand for the depthwise convolution kernel_size = 31, # kernel
 size, 17 - 31 was said to be optimal dropout = 0. # dropout at the very end ) x
 = torch.randn(1, 1024, 512) x = layer(x) + x ``` 1 Conformer Block ```python
 import torch from conformer import ConformerBlock block = ConformerBlock( dim =
 512, dim_head = 64, heads = 8, ff_mult = 4, conv_expansion_factor = 2,
 conv_kernel_size = 31, attn_dropout = 0., ff_dropout = 0., conv_dropout = 0. )
-x = torch.randn(1, 1024, 512) block(x) # (1, 1024, 512) ``` ## Citations
-```bibtex @misc{gulati2020conformer, title={Conformer: Convolution-augmented
-Transformer for Speech Recognition}, author={Anmol Gulati and James Qin and
-Chung-Cheng Chiu and Niki Parmar and Yu Zhang and Jiahui Yu and Wei Han and
-Shibo Wang and Zhengdong Zhang and Yonghui Wu and Ruoming Pang}, year={2020},
-eprint={2005.08100}, archivePrefix={arXiv}, primaryClass={eess.AS} } ```
+x = torch.randn(1, 1024, 512) block(x) # (1, 1024, 512) ``` Conformer - just
+multiple `ConformerBlock` from above ```python import torch from conformer
+import Conformer conformer = Conformer( dim = 512, depth = 12, # 12 blocks
+dim_head = 64, heads = 8, ff_mult = 4, conv_expansion_factor = 2,
+conv_kernel_size = 31, attn_dropout = 0., ff_dropout = 0., conv_dropout = 0. )
+x = torch.randn(1, 1024, 512) conformer(x) # (1, 1024, 512) ``` ## Todo - [ ]
+switch to a better relative positional encoding. shaw's is dated - [ ] flash
+attention with a better RPE ## Citations ```bibtex @misc{gulati2020conformer,
+title={Conformer: Convolution-augmented Transformer for Speech Recognition},
+author={Anmol Gulati and James Qin and Chung-Cheng Chiu and Niki Parmar and Yu
+Zhang and Jiahui Yu and Wei Han and Shibo Wang and Zhengdong Zhang and Yonghui
+Wu and Ruoming Pang}, year={2020}, eprint={2005.08100}, archivePrefix={arXiv},
+primaryClass={eess.AS} } ```
```

### Comparing `conformer-0.2.5/conformer/conformer.py` & `conformer-0.3.0/conformer/conformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -81,24 +81,31 @@
         self.to_out = nn.Linear(inner_dim, dim)
 
         self.max_pos_emb = max_pos_emb
         self.rel_pos_emb = nn.Embedding(2 * max_pos_emb + 1, dim_head)
 
         self.dropout = nn.Dropout(dropout)
 
-    def forward(self, x, context = None, mask = None, context_mask = None):
+    def forward(
+        self,
+        x,
+        context = None,
+        mask = None,
+        context_mask = None
+    ):
         n, device, h, max_pos_emb, has_context = x.shape[-2], x.device, self.heads, self.max_pos_emb, exists(context)
         context = default(context, x)
 
         q, k, v = (self.to_q(x), *self.to_kv(context).chunk(2, dim = -1))
         q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = h), (q, k, v))
 
         dots = einsum('b h i d, b h j d -> b h i j', q, k) * self.scale
 
         # shaw's relative positional embedding
+
         seq = torch.arange(n, device = device)
         dist = rearrange(seq, 'i -> i ()') - rearrange(seq, 'j -> () j')
         dist = dist.clamp(-max_pos_emb, max_pos_emb) + max_pos_emb
         rel_pos_emb = self.rel_pos_emb(dist).to(q)
         pos_attn = einsum('b h n d, n r d -> b h n r', q, rel_pos_emb) * self.scale
         dots = dots + pos_attn
 
@@ -195,7 +202,45 @@
     def forward(self, x, mask = None):
         x = self.ff1(x) + x
         x = self.attn(x, mask = mask) + x
         x = self.conv(x) + x
         x = self.ff2(x) + x
         x = self.post_norm(x)
         return x
+
+# Conformer
+
+class Conformer(nn.Module):
+    def __init__(
+        self,
+        dim,
+        *,
+        depth,
+        dim_head = 64,
+        heads = 8,
+        ff_mult = 4,
+        conv_expansion_factor = 2,
+        conv_kernel_size = 31,
+        attn_dropout = 0.,
+        ff_dropout = 0.,
+        conv_dropout = 0.
+    ):
+        super().__init__()
+        self.layers = nn.ModuleList([])
+
+        for _ in range(depth):
+            self.layers.append(ConformerBlock(
+                dim = dim,
+                dim_head = dim_head,
+                heads = heads,
+                ff_mult = ff_mult,
+                conv_expansion_factor = conv_expansion_factor,
+                conv_kernel_size = conv_kernel_size,
+
+            ))
+
+    def forward(self, x):
+
+        for block in self.layers:
+            x = block(x)
+
+        return x
```

### Comparing `conformer-0.2.5/conformer.egg-info/PKG-INFO` & `conformer-0.3.0/conformer.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: conformer
-Version: 0.2.5
+Version: 0.3.0
 Summary: The convolutional module from the Conformer paper
 Home-page: https://github.com/lucidrains/conformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
-Description: UNKNOWN
-Keywords: transformers,artificial intelligence,transformer
-Platform: UNKNOWN
+Keywords: artificial intelligence,deep learning,transformers,audio
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
```

### Comparing `conformer-0.2.5/setup.py` & `conformer-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'conformer',
   packages = find_packages(),
-  version = '0.2.5',
+  version = '0.3.0',
   license='MIT',
   description = 'The convolutional module from the Conformer paper',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/conformer',
-  keywords = ['transformers', 'artificial intelligence', 'transformer'],
+  keywords = [
+      'artificial intelligence',
+      'deep learning',
+      'transformers',
+      'audio'
+  ],
   install_requires=[
-      'einops',
+      'einops>=0.6.1',
       'torch'
   ],
   classifiers=[
       'Development Status :: 4 - Beta',
       'Intended Audience :: Developers',
       'Topic :: Scientific/Engineering :: Artificial Intelligence',
       'License :: OSI Approved :: MIT License',
```


# Comparing `tmp/MEGABYTE-pytorch-0.0.6.tar.gz` & `tmp/MEGABYTE-pytorch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.0.6.tar", last modified: Tue May 16 15:32:17 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.0.7.tar", last modified: Wed May 17 14:15:21 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.0.6.tar` & `MEGABYTE-pytorch-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:32:17.693616 MEGABYTE-pytorch-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 15:32:04.000000 MEGABYTE-pytorch-0.0.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:32:17.693616 MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 15:32:04.000000 MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-16 15:32:04.000000 MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-05-16 15:32:04.000000 MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:32:17.693616 MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-16 15:32:17.000000 MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-16 15:32:17.000000 MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:32:17.000000 MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 15:32:17.000000 MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 15:32:17.000000 MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-16 15:32:17.693616 MEGABYTE-pytorch-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-16 15:32:04.000000 MEGABYTE-pytorch-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:32:17.693616 MEGABYTE-pytorch-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-16 15:32:04.000000 MEGABYTE-pytorch-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:21.091014 MEGABYTE-pytorch-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 14:15:07.000000 MEGABYTE-pytorch-0.0.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:21.091014 MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 14:15:07.000000 MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-17 14:15:07.000000 MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-05-17 14:15:07.000000 MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:21.091014 MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-17 14:15:21.000000 MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-17 14:15:21.000000 MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:15:21.000000 MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-17 14:15:21.000000 MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 14:15:21.000000 MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-17 14:15:21.091014 MEGABYTE-pytorch-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-17 14:15:07.000000 MEGABYTE-pytorch-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:15:21.091014 MEGABYTE-pytorch-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-17 14:15:07.000000 MEGABYTE-pytorch-0.0.7/setup.py
```

### Comparing `MEGABYTE-pytorch-0.0.6/LICENSE` & `MEGABYTE-pytorch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch/attend.py` & `MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch/megabyte.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,21 @@
     num_logits = logits.shape[-1]
     k = max(int((1 - thres) * num_logits), 1)
     val, ind = torch.topk(logits, k)
     probs = torch.full_like(logits, float('-inf'))
     probs.scatter_(1, ind, val)
     return probs
 
+# token shift, from Peng et al of RWKV
+
+def token_shift(t):
+    t, t_shift = t.chunk(2, dim = -1)
+    t_shift = F.pad(t_shift, (0, 0, 1, -1))
+    return torch.cat((t, t_shift), dim = -1)
+
 # positional bias
 
 class Alibi(nn.Module):
     def __init__(self, heads, **kwargs):
         super().__init__()
         self.heads = heads
         slopes = torch.Tensor(self._get_slopes(heads))
@@ -180,16 +187,16 @@
         self.norm = RMSNorm(dim)
 
     def forward(self, x):
         n = x.shape[-2]
         attn_bias = self.alibi(n, n, device = x.device) if exists(self.alibi) else None
 
         for attn, ff in self.layers:
-            x = attn(x, attn_bias = attn_bias) + x
-            x = ff(x) + x
+            x = attn(token_shift(x), attn_bias = attn_bias) + x
+            x = ff(token_shift(x)) + x
 
         return self.norm(x)
 
 # main class
 
 class MEGABYTE(nn.Module):
     def __init__(
```

### Comparing `MEGABYTE-pytorch-0.0.6/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.0.7/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.6/PKG-INFO` & `MEGABYTE-pytorch-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.6/README.md` & `MEGABYTE-pytorch-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <img src="./MEGABYTE.png" width="450px"></img>
 
 ## MEGABYTE - Pytorch
 
-Implementation of <a href="https://arxiv.org/abs/2305.07185">MEGABYTE</a>, Predicting Million-byte Sequences with Multiscale Transformers, in Pytorch
+Implementation of <a href="https://arxiv.org/abs/2305.07185">MEGABYTE</a>, Predicting Million-byte Sequences with Multiscale Transformers, in Pytorch. Took the liberty to generalize it even further so one can have multiple local models.
 
-<a href="https://github.com/lucidrains/simple-hierarchical-transformer">Similar independent research</a>
+<a href="https://github.com/lucidrains/simple-hierarchical-transformer">Similar independent research that is a further generalization</a>
 
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability</a> and <a href="https://huggingface.co/">🤗 Huggingface</a> for the generous sponsorship to work on and open source cutting edge artificial intelligence research
 
 ## Install
 
@@ -21,16 +21,16 @@
 ```python
 import torch
 from MEGABYTE_pytorch import MEGABYTE
 
 model = MEGABYTE(
     num_tokens = 16000,             # number of tokens
     dim = 512,                      # transformer model dimension
-    max_seq_len = (1024, 4),        # sequence length for global and then local
-    depth = (6, 4),                 # number of layers for global and then local
+    max_seq_len = (1024, 4),        # sequence length for global and then local. this can be more than 2
+    depth = (6, 4),                 # number of layers for global and then local. this can be more than 2, but length must match the max_seq_len's
     dim_head = 64,                  # dimension per head
     heads = 8,                      # number of attention heads
     flash_attn = True               # use flash attention
 )
 
 x = torch.randint(0, 16000, (1, 1024, 4))
 
@@ -93,7 +93,20 @@
 @misc{press2021ALiBi,
     title   = {Train Short, Test Long: Attention with Linear Biases Enable Input Length Extrapolation},
     author  = {Ofir Press and Noah A. Smith and Mike Lewis},
     year    = {2021},
     url     = {https://ofir.io/train_short_test_long.pdf}
 }
 ```
+
+```bibtex
+@software{peng_bo_2021_5196578,
+    author    = {PENG Bo},
+    title     = {BlinkDL/RWKV-LM: 0.01},
+    month     = {aug},
+    year      = {2021},
+    publisher = {Zenodo},
+    version   = {0.01},
+    doi       = {10.5281/zenodo.5196578},
+    url       = {https://doi.org/10.5281/zenodo.5196578}
+}
+```
```

#### html2text {}

```diff
@@ -1,32 +1,38 @@
 [./MEGABYTE.png] ## MEGABYTE - Pytorch Implementation of MEGABYTE, Predicting
-Million-byte Sequences with Multiscale Transformers, in Pytorch Similar
-independent_research ## Appreciation - Stability and ð¤_Huggingface for the
-generous sponsorship to work on and open source cutting edge artificial
-intelligence research ## Install ```bash $ pip install MEGABYTE-pytorch ``` ##
-Usage ```python import torch from MEGABYTE_pytorch import MEGABYTE model =
-MEGABYTE( num_tokens = 16000, # number of tokens dim = 512, # transformer model
-dimension max_seq_len = (1024, 4), # sequence length for global and then local
-depth = (6, 4), # number of layers for global and then local dim_head = 64, #
-dimension per head heads = 8, # number of attention heads flash_attn = True #
-use flash attention ) x = torch.randint(0, 16000, (1, 1024, 4)) loss = model(x,
-return_loss = True) loss.backward() # then after much training logits = model
-(x) # and sample from the logits accordingly # or you can use the generate
-function sampled = model.generate(temperature = 0.9, filter_thres = 0.9) # (1,
-1024, 4) ``` ## Test Train on character-level enwik8 with patches of size 4
-```bash $ python train.py ``` ## Citations ```bibtex @misc{yu2023megabyte,
-title = {MEGABYTE: Predicting Million-byte Sequences with Multiscale
-Transformers}, author = {Lili Yu and DÃ¡niel Simig and Colin Flaherty and Armen
-Aghajanyan and Luke Zettlemoyer and Mike Lewis}, year = {2023}, eprint =
-{2305.07185}, archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex
-@misc{https://doi.org/10.48550/arxiv.2302.01327, doi = {10.48550/
-ARXIV.2302.01327}, url = {https://arxiv.org/abs/2302.01327}, author = {Kumar,
-Manoj and Dehghani, Mostafa and Houlsby, Neil}, title = {Dual PatchNorm},
-publisher = {arXiv}, year = {2023}, copyright = {Creative Commons Attribution
-4.0 International} } ``` ```bibtex @inproceedings{dao2022flashattention, title
-= {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-
-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra,
-Atri and R{\'e}, Christopher}, booktitle = {Advances in Neural Information
-Processing Systems}, year = {2022} } ``` ```bibtex @misc{press2021ALiBi, title
-= {Train Short, Test Long: Attention with Linear Biases Enable Input Length
-Extrapolation}, author = {Ofir Press and Noah A. Smith and Mike Lewis}, year =
-{2021}, url = {https://ofir.io/train_short_test_long.pdf} } ```
+Million-byte Sequences with Multiscale Transformers, in Pytorch. Took the
+liberty to generalize it even further so one can have multiple local models.
+Similar_independent_research_that_is_a_further_generalization ## Appreciation -
+Stability and ð¤_Huggingface for the generous sponsorship to work on and open
+source cutting edge artificial intelligence research ## Install ```bash $ pip
+install MEGABYTE-pytorch ``` ## Usage ```python import torch from
+MEGABYTE_pytorch import MEGABYTE model = MEGABYTE( num_tokens = 16000, # number
+of tokens dim = 512, # transformer model dimension max_seq_len = (1024, 4), #
+sequence length for global and then local. this can be more than 2 depth = (6,
+4), # number of layers for global and then local. this can be more than 2, but
+length must match the max_seq_len's dim_head = 64, # dimension per head heads =
+8, # number of attention heads flash_attn = True # use flash attention ) x =
+torch.randint(0, 16000, (1, 1024, 4)) loss = model(x, return_loss = True)
+loss.backward() # then after much training logits = model(x) # and sample from
+the logits accordingly # or you can use the generate function sampled =
+model.generate(temperature = 0.9, filter_thres = 0.9) # (1, 1024, 4) ``` ##
+Test Train on character-level enwik8 with patches of size 4 ```bash $ python
+train.py ``` ## Citations ```bibtex @misc{yu2023megabyte, title = {MEGABYTE:
+Predicting Million-byte Sequences with Multiscale Transformers}, author = {Lili
+Yu and DÃ¡niel Simig and Colin Flaherty and Armen Aghajanyan and Luke
+Zettlemoyer and Mike Lewis}, year = {2023}, eprint = {2305.07185},
+archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex @misc{https://
+doi.org/10.48550/arxiv.2302.01327, doi = {10.48550/ARXIV.2302.01327}, url =
+{https://arxiv.org/abs/2302.01327}, author = {Kumar, Manoj and Dehghani,
+Mostafa and Houlsby, Neil}, title = {Dual PatchNorm}, publisher = {arXiv}, year
+= {2023}, copyright = {Creative Commons Attribution 4.0 International} } ```
+```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
+and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
+and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
+} ``` ```bibtex @misc{press2021ALiBi, title = {Train Short, Test Long:
+Attention with Linear Biases Enable Input Length Extrapolation}, author = {Ofir
+Press and Noah A. Smith and Mike Lewis}, year = {2021}, url = {https://ofir.io/
+train_short_test_long.pdf} } ``` ```bibtex @software{peng_bo_2021_5196578,
+author = {PENG Bo}, title = {BlinkDL/RWKV-LM: 0.01}, month = {aug}, year =
+{2021}, publisher = {Zenodo}, version = {0.01}, doi = {10.5281/zenodo.5196578},
+url = {https://doi.org/10.5281/zenodo.5196578} } ```
```

### Comparing `MEGABYTE-pytorch-0.0.6/setup.py` & `MEGABYTE-pytorch-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```


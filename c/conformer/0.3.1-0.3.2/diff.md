# Comparing `tmp/conformer-0.3.1.tar.gz` & `tmp/conformer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conformer-0.3.1.tar", last modified: Wed May 17 19:17:42 2023, max compression
+gzip compressed data, was "conformer-0.3.2.tar", last modified: Wed May 17 21:08:42 2023, max compression
```

## Comparing `conformer-0.3.1.tar` & `conformer-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:17:42.272460 conformer-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 19:17:27.000000 conformer-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-17 19:17:42.272460 conformer-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-17 19:17:27.000000 conformer-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:17:42.268460 conformer-0.3.1/conformer/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 19:17:27.000000 conformer-0.3.1/conformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-17 19:17:27.000000 conformer-0.3.1/conformer/conformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:17:42.272460 conformer-0.3.1/conformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-17 19:17:42.000000 conformer-0.3.1/conformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-17 19:17:42.000000 conformer-0.3.1/conformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:17:42.000000 conformer-0.3.1/conformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 19:17:42.000000 conformer-0.3.1/conformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 19:17:42.000000 conformer-0.3.1/conformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:17:42.272460 conformer-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-17 19:17:27.000000 conformer-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:42.174281 conformer-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 21:08:31.000000 conformer-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-17 21:08:42.174281 conformer-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-17 21:08:31.000000 conformer-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:42.174281 conformer-0.3.2/conformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 21:08:31.000000 conformer-0.3.2/conformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-17 21:08:31.000000 conformer-0.3.2/conformer/conformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:42.174281 conformer-0.3.2/conformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-17 21:08:42.000000 conformer-0.3.2/conformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-17 21:08:42.000000 conformer-0.3.2/conformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:08:42.000000 conformer-0.3.2/conformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 21:08:42.000000 conformer-0.3.2/conformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 21:08:42.000000 conformer-0.3.2/conformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:08:42.174281 conformer-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-17 21:08:31.000000 conformer-0.3.2/setup.py
```

### Comparing `conformer-0.3.1/LICENSE` & `conformer-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conformer-0.3.1/PKG-INFO` & `conformer-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conformer
-Version: 0.3.1
+Version: 0.3.2
 Summary: The convolutional module from the Conformer paper
 Home-page: https://github.com/lucidrains/conformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,audio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `conformer-0.3.1/README.md` & `conformer-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `conformer-0.3.1/conformer/conformer.py` & `conformer-0.3.2/conformer/conformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,15 +145,16 @@
 class ConformerConvModule(nn.Module):
     def __init__(
         self,
         dim,
         causal = False,
         expansion_factor = 2,
         kernel_size = 31,
-        dropout = 0.):
+        dropout = 0.
+    ):
         super().__init__()
 
         inner_dim = dim * expansion_factor
         padding = calc_same_padding(kernel_size) if not causal else (kernel_size - 1, 0)
 
         self.net = nn.Sequential(
             nn.LayerNorm(dim),
@@ -181,20 +182,21 @@
         dim_head = 64,
         heads = 8,
         ff_mult = 4,
         conv_expansion_factor = 2,
         conv_kernel_size = 31,
         attn_dropout = 0.,
         ff_dropout = 0.,
-        conv_dropout = 0.
+        conv_dropout = 0.,
+        conv_causal = False
     ):
         super().__init__()
         self.ff1 = FeedForward(dim = dim, mult = ff_mult, dropout = ff_dropout)
         self.attn = Attention(dim = dim, dim_head = dim_head, heads = heads, dropout = attn_dropout)
-        self.conv = ConformerConvModule(dim = dim, causal = False, expansion_factor = conv_expansion_factor, kernel_size = conv_kernel_size, dropout = conv_dropout)
+        self.conv = ConformerConvModule(dim = dim, causal = conv_causal, expansion_factor = conv_expansion_factor, kernel_size = conv_kernel_size, dropout = conv_dropout)
         self.ff2 = FeedForward(dim = dim, mult = ff_mult, dropout = ff_dropout)
 
         self.attn = PreNorm(dim, self.attn)
         self.ff1 = Scale(0.5, PreNorm(dim, self.ff1))
         self.ff2 = Scale(0.5, PreNorm(dim, self.ff2))
 
         self.post_norm = nn.LayerNorm(dim)
@@ -218,28 +220,30 @@
         dim_head = 64,
         heads = 8,
         ff_mult = 4,
         conv_expansion_factor = 2,
         conv_kernel_size = 31,
         attn_dropout = 0.,
         ff_dropout = 0.,
-        conv_dropout = 0.
+        conv_dropout = 0.,
+        conv_causal = False
     ):
         super().__init__()
         self.dim = dim
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(ConformerBlock(
                 dim = dim,
                 dim_head = dim_head,
                 heads = heads,
                 ff_mult = ff_mult,
                 conv_expansion_factor = conv_expansion_factor,
                 conv_kernel_size = conv_kernel_size,
+                conv_causal = conv_causal
 
             ))
 
     def forward(self, x):
 
         for block in self.layers:
             x = block(x)
```

### Comparing `conformer-0.3.1/conformer.egg-info/PKG-INFO` & `conformer-0.3.2/conformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conformer
-Version: 0.3.1
+Version: 0.3.2
 Summary: The convolutional module from the Conformer paper
 Home-page: https://github.com/lucidrains/conformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,audio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `conformer-0.3.1/setup.py` & `conformer-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'conformer',
   packages = find_packages(),
-  version = '0.3.1',
+  version = '0.3.2',
   license='MIT',
   description = 'The convolutional module from the Conformer paper',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/conformer',
   keywords = [
       'artificial intelligence',
```


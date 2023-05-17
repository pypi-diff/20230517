# Comparing `tmp/soundstorm-pytorch-0.0.2.tar.gz` & `tmp/soundstorm-pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundstorm-pytorch-0.0.2.tar", last modified: Wed May 17 20:10:07 2023, max compression
+gzip compressed data, was "soundstorm-pytorch-0.0.3.tar", last modified: Wed May 17 21:03:22 2023, max compression
```

## Comparing `soundstorm-pytorch-0.0.2.tar` & `soundstorm-pytorch-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:10:07.233034 soundstorm-pytorch-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 20:09:54.000000 soundstorm-pytorch-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 20:10:07.233034 soundstorm-pytorch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-17 20:09:54.000000 soundstorm-pytorch-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:10:07.233034 soundstorm-pytorch-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-17 20:09:54.000000 soundstorm-pytorch-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:10:07.233034 soundstorm-pytorch-0.0.2/soundstorm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 20:09:54.000000 soundstorm-pytorch-0.0.2/soundstorm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-17 20:09:54.000000 soundstorm-pytorch-0.0.2/soundstorm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-17 20:09:54.000000 soundstorm-pytorch-0.0.2/soundstorm_pytorch/soundstorm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:10:07.233034 soundstorm-pytorch-0.0.2/soundstorm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 20:10:07.000000 soundstorm-pytorch-0.0.2/soundstorm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-17 20:10:07.000000 soundstorm-pytorch-0.0.2/soundstorm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:10:07.000000 soundstorm-pytorch-0.0.2/soundstorm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 20:10:07.000000 soundstorm-pytorch-0.0.2/soundstorm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 20:10:07.000000 soundstorm-pytorch-0.0.2/soundstorm_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:22.319116 soundstorm-pytorch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 21:03:08.000000 soundstorm-pytorch-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 21:03:22.319116 soundstorm-pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-17 21:03:08.000000 soundstorm-pytorch-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:03:22.319116 soundstorm-pytorch-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-17 21:03:08.000000 soundstorm-pytorch-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:22.315116 soundstorm-pytorch-0.0.3/soundstorm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 21:03:08.000000 soundstorm-pytorch-0.0.3/soundstorm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-17 21:03:08.000000 soundstorm-pytorch-0.0.3/soundstorm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-17 21:03:08.000000 soundstorm-pytorch-0.0.3/soundstorm_pytorch/soundstorm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:22.319116 soundstorm-pytorch-0.0.3/soundstorm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 21:03:22.000000 soundstorm-pytorch-0.0.3/soundstorm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-17 21:03:22.000000 soundstorm-pytorch-0.0.3/soundstorm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:03:22.000000 soundstorm-pytorch-0.0.3/soundstorm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 21:03:22.000000 soundstorm-pytorch-0.0.3/soundstorm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 21:03:22.000000 soundstorm-pytorch-0.0.3/soundstorm_pytorch.egg-info/top_level.txt
```

### Comparing `soundstorm-pytorch-0.0.2/LICENSE` & `soundstorm-pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.0.2/PKG-INFO` & `soundstorm-pytorch-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/lucidrains/soundstorm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `soundstorm-pytorch-0.0.2/README.md` & `soundstorm-pytorch-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.0.2/setup.py` & `soundstorm-pytorch-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'soundstorm-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/soundstorm-pytorch',
   keywords = [
```

### Comparing `soundstorm-pytorch-0.0.2/soundstorm_pytorch/attend.py` & `soundstorm-pytorch-0.0.3/soundstorm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.0.2/soundstorm_pytorch/soundstorm.py` & `soundstorm-pytorch-0.0.3/soundstorm_pytorch/soundstorm.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,24 +34,41 @@
     ):
         super().__init__()
         self.conformer = conformer
 
         if isinstance(conformer, dict):
             self.conformer = Conformer(**self.conformer)
 
+        dim = self.conformer.dim
+
+        self.mask_tokens = nn.Parameter(torch.randn(num_tokens_reduce, dim))
+
         self.num_tokens_reduce = num_tokens_reduce
         self.num_tokens_per_head = default(num_tokens_per_head, num_tokens_reduce)
 
-        dim = self.conformer.dim
-
         self.heads = nn.Sequential(
             nn.Linear(dim, dim * self.num_tokens_per_head),
             Rearrange('b n (h d) -> b (n h) d', h = self.num_tokens_per_head)
         )
 
+    def add_mask_tokens(
+        self,
+        x,
+        mask
+    ):
+        h = self.num_tokens_reduce
+
+        x = torch.where(
+            rearrange(mask, 'b (n h) -> b n h 1', h = h),
+            rearrange(x, 'b (n h) d -> b n h d', h = h),
+            self.mask_tokens,
+        )
+
+        return rearrange(x, 'b n h d -> b (n h) d')
+
     def forward(
         self,
         x,
         cond = None
     ):
         x = reduce(x, 'b (n h) d -> b n d', h = self.num_tokens_reduce)
```

### Comparing `soundstorm-pytorch-0.0.2/soundstorm_pytorch.egg-info/PKG-INFO` & `soundstorm-pytorch-0.0.3/soundstorm_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/lucidrains/soundstorm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```


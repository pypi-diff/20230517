# Comparing `tmp/varwizard-0.1.1.tar.gz` & `tmp/varwizard-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varwizard-0.1.1.tar", max compression
+gzip compressed data, was "varwizard-0.2.tar", max compression
```

## Comparing `varwizard-0.1.1.tar` & `varwizard-0.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0      665 2023-05-13 18:28:14.765596 varwizard-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1516 2023-05-13 18:22:34.079807 varwizard-0.1.1/readme.md
--rw-r--r--   0        0        0       60 2023-05-11 10:13:41.438955 varwizard-0.1.1/varwizard/__init__.py
--rw-r--r--   0        0        0       51 2023-05-12 16:52:19.678029 varwizard-0.1.1/varwizard/config/__init__.py
--rw-r--r--   0        0        0      554 2023-05-11 10:13:41.198952 varwizard-0.1.1/varwizard/config/prefix_tuning.py
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.1.1/varwizard/data/__init__.py
--rw-r--r--   0        0        0     1843 2023-05-13 18:07:36.475838 varwizard-0.1.1/varwizard/data/input_preparation.py
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.1.1/varwizard/generation/__init__.py
--rw-r--r--   0        0        0      873 2023-05-13 17:41:18.298783 varwizard-0.1.1/varwizard/generation/gen.py
--rw-r--r--   0        0        0   401536 2023-05-11 10:13:40.998948 varwizard-0.1.1/varwizard/libs/tree-sitter/c.so
--rw-r--r--   0        0        0  4076856 2023-05-11 10:13:41.242952 varwizard-0.1.1/varwizard/libs/tree-sitter/c_sharp.so
--rw-r--r--   0        0        0  2300056 2023-05-11 10:13:41.446956 varwizard-0.1.1/varwizard/libs/tree-sitter/cpp.so
--rw-r--r--   0        0        0   246152 2023-05-11 10:13:41.190951 varwizard-0.1.1/varwizard/libs/tree-sitter/go.so
--rw-r--r--   0        0        0   401704 2023-05-11 10:13:41.494956 varwizard-0.1.1/varwizard/libs/tree-sitter/java.so
--rw-r--r--   0        0        0   354200 2023-05-11 10:13:41.458956 varwizard-0.1.1/varwizard/libs/tree-sitter/javascript.so
--rw-r--r--   0        0        0   785016 2023-05-11 10:13:41.490956 varwizard-0.1.1/varwizard/libs/tree-sitter/php.so
--rw-r--r--   0        0        0   494864 2023-05-11 10:13:41.470956 varwizard-0.1.1/varwizard/libs/tree-sitter/python.so
--rw-r--r--   0        0        0  2130104 2023-05-11 10:13:41.090950 varwizard-0.1.1/varwizard/libs/tree-sitter/ruby.so
--rw-r--r--   0        0        0   849608 2023-05-11 10:13:41.238952 varwizard-0.1.1/varwizard/libs/tree-sitter/rust.so
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.1.1/varwizard/models/__init__.py
--rw-r--r--   0        0        0      252 2023-05-11 10:13:41.090950 varwizard-0.1.1/varwizard/models/bloom.py
--rw-r--r--   0        0        0     1421 2023-05-13 18:00:37.514695 varwizard-0.1.1/varwizard/models/varwizard.py
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.1.1/varwizard/utils/__init__.py
--rw-r--r--   0        0        0    13556 2023-05-11 10:13:41.086950 varwizard-0.1.1/varwizard/utils/obfuscation.py
--rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 varwizard-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      746 2023-05-17 09:38:45.519137 varwizard-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2021 2023-05-17 09:39:36.088003 varwizard-0.2/readme.md
+-rw-r--r--   0        0        0       82 2023-05-17 09:38:58.503358 varwizard-0.2/varwizard/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-17 04:28:27.343893 varwizard-0.2/varwizard/__main__.py
+-rw-r--r--   0        0        0     1659 2023-05-17 06:43:28.374791 varwizard-0.2/varwizard/cli.py
+-rw-r--r--   0        0        0       51 2023-05-12 16:52:19.678029 varwizard-0.2/varwizard/config/__init__.py
+-rw-r--r--   0        0        0      554 2023-05-11 10:13:41.198952 varwizard-0.2/varwizard/config/prefix_tuning.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2/varwizard/data/__init__.py
+-rw-r--r--   0        0        0     2904 2023-05-17 09:17:31.229411 varwizard-0.2/varwizard/data/input_preparation.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2/varwizard/generation/__init__.py
+-rw-r--r--   0        0        0     1005 2023-05-17 08:15:49.110211 varwizard-0.2/varwizard/generation/gen.py
+-rw-r--r--   0        0        0   401536 2023-05-11 10:13:40.998948 varwizard-0.2/varwizard/libs/tree-sitter/c.so
+-rw-r--r--   0        0        0  4076856 2023-05-11 10:13:41.242952 varwizard-0.2/varwizard/libs/tree-sitter/c_sharp.so
+-rw-r--r--   0        0        0  2300056 2023-05-11 10:13:41.446956 varwizard-0.2/varwizard/libs/tree-sitter/cpp.so
+-rw-r--r--   0        0        0   246152 2023-05-11 10:13:41.190951 varwizard-0.2/varwizard/libs/tree-sitter/go.so
+-rw-r--r--   0        0        0   401704 2023-05-11 10:13:41.494956 varwizard-0.2/varwizard/libs/tree-sitter/java.so
+-rw-r--r--   0        0        0   354200 2023-05-11 10:13:41.458956 varwizard-0.2/varwizard/libs/tree-sitter/javascript.so
+-rw-r--r--   0        0        0   785016 2023-05-11 10:13:41.490956 varwizard-0.2/varwizard/libs/tree-sitter/php.so
+-rw-r--r--   0        0        0   494864 2023-05-11 10:13:41.470956 varwizard-0.2/varwizard/libs/tree-sitter/python.so
+-rw-r--r--   0        0        0  2130104 2023-05-11 10:13:41.090950 varwizard-0.2/varwizard/libs/tree-sitter/ruby.so
+-rw-r--r--   0        0        0   849608 2023-05-11 10:13:41.238952 varwizard-0.2/varwizard/libs/tree-sitter/rust.so
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2/varwizard/models/__init__.py
+-rw-r--r--   0        0        0      252 2023-05-11 10:13:41.090950 varwizard-0.2/varwizard/models/bloom.py
+-rw-r--r--   0        0        0     2178 2023-05-17 09:26:23.014501 varwizard-0.2/varwizard/models/varwizard.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2/varwizard/utils/__init__.py
+-rw-r--r--   0        0        0    13556 2023-05-11 10:13:41.086950 varwizard-0.2/varwizard/utils/obfuscation.py
+-rw-r--r--   0        0        0     3015 1970-01-01 00:00:00.000000 varwizard-0.2/PKG-INFO
```

### Comparing `varwizard-0.1.1/pyproject.toml` & `varwizard-0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 requires = [
     "setuptools>=60",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 [tool.poetry]
 name="varwizard"
-version="0.1.1"
+version="0.2"
 license = "Apache-2.0"
 description = "An Automated Tool for Improving Code Quality Through Variable Name Refinement with Language Models"
 readme = "readme.md"
 homepage = "https://github.com/FSoft-AI4Code/VarWizard"
 repository = "https://github.com/FSoft-AI4Code/VarWizard"
 keywords = ["variable renaming", "language models", "code quality"]
 authors = ["FSoft-AI4Code <support.aic@fpt.com>"]
 [tool.poetry.dependencies]
 python = ">=3.7"
 torch = ">=1.12.1"
 peft = "0.1.0"
 transformers = ">=4.28.0"
 tree-sitter = "*"
+codetext = "*"
+[tool.poetry.plugins."console_scripts"]
+varwizard = "varwizard:main"
```

### Comparing `varwizard-0.1.1/varwizard/config/prefix_tuning.py` & `varwizard-0.2/varwizard/config/prefix_tuning.py`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/generation/gen.py` & `varwizard-0.2/varwizard/generation/gen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-def generate(input_ids, tokenizer, model, max_length: int = 505, penalty_alpha: float = 0.6, top_k: int = 4):
+def generate(input_ids, vmap, tokenizer, model, max_new_tokens: int = 100, penalty_alpha: float = 0.6, top_k: int = 4):
     attention_mask = input_ids.ne(tokenizer.pad_token_id)
     predictions = model.generate(input_ids = input_ids,
                                   attention_mask =  attention_mask,
-                   max_length = max_length,
+                   max_new_tokens = max_new_tokens,
                    penalty_alpha = penalty_alpha,
                    top_k = top_k,
                    eos_token_id = tokenizer.eos_token_id)
     prediction = tokenizer.batch_decode(predictions.cpu().numpy())[0]
-    obfuscated_code, prediction = prediction.replace('<s>', '').replace('</s>','').split('Output')
+    obfuscated_code, prediction, *_ = prediction.replace('<s>', '').replace('</s>','').split('Output')
     pred_coms = prediction.split()
     new_code = obfuscated_code
+    new_vmap = {}
     for i in range(len(pred_coms) // 3):
         key, _, value = pred_coms[3 * i: 3 * i + 3]
+        new_vmap[key] = value
+    vmap.update(new_vmap)
+    for key, value in vmap.items():
         new_code = new_code.replace(key, value)
     return new_code
```

### Comparing `varwizard-0.1.1/varwizard/libs/tree-sitter/c.so` & `varwizard-0.2/varwizard/libs/tree-sitter/c.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/libs/tree-sitter/c_sharp.so` & `varwizard-0.2/varwizard/libs/tree-sitter/c_sharp.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/libs/tree-sitter/cpp.so` & `varwizard-0.2/varwizard/libs/tree-sitter/cpp.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/libs/tree-sitter/go.so` & `varwizard-0.2/varwizard/libs/tree-sitter/go.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/libs/tree-sitter/java.so` & `varwizard-0.2/varwizard/libs/tree-sitter/java.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/libs/tree-sitter/javascript.so` & `varwizard-0.2/varwizard/libs/tree-sitter/javascript.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/libs/tree-sitter/php.so` & `varwizard-0.2/varwizard/libs/tree-sitter/php.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/libs/tree-sitter/python.so` & `varwizard-0.2/varwizard/libs/tree-sitter/python.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/libs/tree-sitter/ruby.so` & `varwizard-0.2/varwizard/libs/tree-sitter/ruby.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/libs/tree-sitter/rust.so` & `varwizard-0.2/varwizard/libs/tree-sitter/rust.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/varwizard/utils/obfuscation.py` & `varwizard-0.2/varwizard/utils/obfuscation.py`

 * *Files identical despite different names*

### Comparing `varwizard-0.1.1/PKG-INFO` & `varwizard-0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: varwizard
-Version: 0.1.1
+Version: 0.2
 Summary: An Automated Tool for Improving Code Quality Through Variable Name Refinement with Language Models
 Home-page: https://github.com/FSoft-AI4Code/VarWizard
 License: Apache-2.0
 Keywords: variable renaming,language models,code quality
 Author: FSoft-AI4Code
 Author-email: support.aic@fpt.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: codetext
 Requires-Dist: peft (==0.1.0)
 Requires-Dist: torch (>=1.12.1)
 Requires-Dist: transformers (>=4.28.0)
 Requires-Dist: tree-sitter
 Project-URL: Repository, https://github.com/FSoft-AI4Code/VarWizard
 Description-Content-Type: text/markdown
 
@@ -30,22 +31,36 @@
 
 2. Installation
 
 You can easily install this package by the command
 ```
     pip install varwizard
 ```
-3. Tutorial
+3. Usage
+    * Command-line
+    
+    You can use VarWizard by running the command
+```
+varwizard [--model-name {bloom-560m}]
+            --input INPUT --lang {c,cpp,java,php,go,javascript,ruby,rust,python,c_sharp} 
+            [--output-path OUTPUT_PATH] [--max-input-len MAX_INPUT_LEN]
+            [--device DEVICE] [--penalty-alpha PENALTY_ALPHA] [--top-k TOP_K] [--max-new-tokens MAX_NEW_TOKENS]
+```
+Details for each argument can be found by 
+```varwizard --help```
+
 
+ * Python API
+Another way is to Python methods.
 Here is a simple example of VarWizard.
 ```
 from varwizard import VarWizard
 
 model = VarWizard()
 code = """
 static void lsp2poly ( int * var0, const int16_t * var1, int var2 ) { int var3, var4 ; var0 [ 0 ] = 0x400000 ; // 1.0 in (3.22) var0 [ 1 ] = - var1 [ 0 ] << 8 ; // *2 and (0.15) -> (3.22) for ( var3 = 2 ; var3 <= var2 ; var3 ++ ) { var0 [ var3 ] = var0 [ var3 - 2 ] ; for ( var4 = var3 ; var4 > 1 ; var4 -- ) var0 [ var4 ] -= MULL ( var0 [ var4 - 1 ], var1 [ 2 * var3 - 2 ], FRAC_BITS ) - var0 [ var4 - 2 ] ; var0 [ 1 ] -= var1 [ 2 * var3 - 2 ] << 8 ; } }"""
-print(model.make_new_code(code, 'cpp'), device = 'cuda:0')
+print(model.make_new_code(code, 'cpp', device = 'cuda:0'))
 ```
 VarWizard produces the output
 ```
 static void lsp2poly ( int * lsp, const int16_t * lsp2, int nbits ) { int index, count ; lsp [ 0 ] = 0x400000 ; // 1.0 in (3.22) lsp [ 1 ] = - lsp2 [ 0 ] << 8 ; // *2 and (0.15) -> (3.22) for ( index = 2 ; index <= nbits ; index ++ ) { lsp [ index ] = lsp [ index - 2 ] ; for ( count = index ; count > 1 ; count -- ) lsp [ count ] -= MULL ( lsp [ count - 1 ], lsp2 [ 2 * index - 2 ], FRAC_BITS ) - lsp [ count - 2 ] ; lsp [ 1 ] -= lsp2 [ 2 * index - 2 ] << 8 ; } }
 ```
```


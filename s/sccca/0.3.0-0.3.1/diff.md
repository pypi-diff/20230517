# Comparing `tmp/sccca-0.3.0.tar.gz` & `tmp/sccca-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sccca-0.3.0.tar", max compression
+gzip compressed data, was "sccca-0.3.1.tar", max compression
```

## Comparing `sccca-0.3.0.tar` & `sccca-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1002 2023-05-17 08:25:32.563562 sccca-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      149 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/__init__.py
--rw-r--r--   0        0        0     8325 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/cca.py
--rw-r--r--   0        0        0      108 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/logger.py
--rw-r--r--   0        0        0    22241 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/model.py
--rw-r--r--   0        0        0     9600 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/pca.py
--rw-r--r--   0        0        0      297 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/plots/__init__.py
--rw-r--r--   0        0        0     3308 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/plots/factor_embedding.py
--rw-r--r--   0        0        0     6052 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/plots/loadings_bar.py
--rw-r--r--   0        0        0     8995 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/plots/loadings_scatter.py
--rw-r--r--   0        0        0     8624 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/plots/qc.py
--rw-r--r--   0        0        0     2663 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/plots/utils.py
--rw-r--r--   0        0        0      154 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/train/__init__.py
--rw-r--r--   0        0        0     7299 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/train/handler.py
--rw-r--r--   0        0        0     3836 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/train/local_handler.py
--rw-r--r--   0        0        0      488 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/train/settings.py
--rw-r--r--   0        0        0      425 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/utils/__init__.py
--rw-r--r--   0        0        0     1589 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/utils/data.py
--rw-r--r--   0        0        0     4739 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/utils/design.py
--rw-r--r--   0        0        0      319 2023-05-17 08:25:32.563562 sccca-0.3.0/scCCA/utils/scanpy.py
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 sccca-0.3.0/setup.py
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 sccca-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-05-17 08:56:13.883142 sccca-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/__init__.py
+-rw-r--r--   0        0        0     8325 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/cca.py
+-rw-r--r--   0        0        0      108 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/logger.py
+-rw-r--r--   0        0        0    22241 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/model.py
+-rw-r--r--   0        0        0     9846 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/pca.py
+-rw-r--r--   0        0        0      297 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/plots/__init__.py
+-rw-r--r--   0        0        0     3308 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/plots/factor_embedding.py
+-rw-r--r--   0        0        0     6052 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/plots/loadings_bar.py
+-rw-r--r--   0        0        0     8995 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/plots/loadings_scatter.py
+-rw-r--r--   0        0        0     8624 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/plots/qc.py
+-rw-r--r--   0        0        0     2663 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/plots/utils.py
+-rw-r--r--   0        0        0      154 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/train/__init__.py
+-rw-r--r--   0        0        0     7299 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/train/handler.py
+-rw-r--r--   0        0        0     3836 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/train/local_handler.py
+-rw-r--r--   0        0        0      488 2023-05-17 08:56:13.883142 sccca-0.3.1/scCCA/train/settings.py
+-rw-r--r--   0        0        0      425 2023-05-17 08:56:13.887142 sccca-0.3.1/scCCA/utils/__init__.py
+-rw-r--r--   0        0        0     1589 2023-05-17 08:56:13.887142 sccca-0.3.1/scCCA/utils/data.py
+-rw-r--r--   0        0        0     4739 2023-05-17 08:56:13.887142 sccca-0.3.1/scCCA/utils/design.py
+-rw-r--r--   0        0        0      319 2023-05-17 08:56:13.887142 sccca-0.3.1/scCCA/utils/scanpy.py
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 sccca-0.3.1/setup.py
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 sccca-0.3.1/PKG-INFO
```

### Comparing `sccca-0.3.0/pyproject.toml` & `sccca-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "scCCA"
 packages = [
     { include = "scCCA" },
 ]
-version = "0.3.0"
+version = "0.3.1"
 description = "Single cell canonical correlation analysis."
 authors = ["Harald Vohringer"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 scanpy = ">=1.8.2"
 pyro-ppl = ">=1.8.0"
```

### Comparing `sccca-0.3.0/scCCA/cca.py` & `sccca-0.3.1/scCCA/cca.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/scCCA/model.py` & `sccca-0.3.1/scCCA/model.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/scCCA/pca.py` & `sccca-0.3.1/scCCA/pca.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,39 +219,47 @@
         if σ_rna.ndim == 2:
             σ_rna = np.expand_dims(σ_rna, 1)
 
         adata.varm[f"{model_key}_σ_rna"] = σ_rna.swapaxes(-1, -2)
 
         adata.obsm[f"X_{model_key}"] = self.handler.predict_local_variable("z", num_samples=num_samples).swapaxes(0, 1)
 
-    def mean_to_anndata(self, model_key=None, num_samples=25):
+    def mean_to_anndata(self, model_key=None, num_samples=25, num_split=2048):
         _ = self._meta_to_anndata(model_key, num_samples)
         adata = self.adata
 
-        adata.layers[f"{model_key}_μ_rna"] = self.handler.predict_local_variable("μ_rna", num_samples=num_samples).mean(
-            0
-        )
+        adata.layers[f"{model_key}_μ_rna"] = self.handler.predict_local_variable(
+            "μ_rna", num_samples=num_samples, num_split=num_split
+        ).mean(0)
         adata.layers[f"{model_key}_offset_rna"] = self.handler.predict_local_variable(
-            "offset_rna", num_samples=num_samples
+            "offset_rna", num_samples=num_samples, num_split=num_split
+        ).mean(0)
+        adata.obsm[f"X_{model_key}"] = self.handler.predict_local_variable(
+            "z", num_samples=num_samples, num_split=num_split
         ).mean(0)
-        adata.obsm[f"X_{model_key}"] = self.handler.predict_local_variable("z", num_samples=num_samples).mean(0)
         adata.varm[f"{model_key}_W_rna"] = (
             self.handler.predict_global_variable("W_lin", num_samples=num_samples).mean(0).T
         )
         adata.varm[f"{model_key}_V_rna"] = (
             self.handler.predict_global_variable("W_add", num_samples=num_samples).mean(0).T
         )
         adata.varm[f"{model_key}_α_rna"] = self.handler.predict_global_variable("α_rna").mean(0).T
         adata.varm[f"{model_key}_σ_rna"] = self.handler.predict_global_variable("σ_rna").mean(0).T
 
-    def to_anndata(self, model_key=None, num_samples=25):
+    def to_anndata(self, model_key=None, num_samples=25, num_split=2048):
         res = self._meta_to_anndata(model_key, num_samples)
         adata = self.adata
         res["α_rna"] = self.handler.predict_global_variable("α_rna", num_samples=num_samples).mean(0)
         res["W_fac"] = self.handler.predict_global_variable("W_fac", num_samples=num_samples).mean(0)
         res["W_vec"] = self.handler.predict_global_variable("W_vec", num_samples=num_samples).mean(0)
         res["W_lin"] = self.handler.predict_global_variable("W_lin", num_samples=num_samples).mean(0)
         res["W_add"] = self.handler.predict_global_variable("W_add", num_samples=num_samples).mean(0)
 
-        res["μ_rna"] = self.handler.predict_local_variable("μ_rna", num_samples=num_samples).mean(0)
-        adata.obsm[f"X_{model_key}"] = self.handler.predict_local_variable("z", num_samples=num_samples).mean(0)
-        adata.obsm[f"Z_{model_key}"] = self.handler.predict_local_variable("z_vec", num_samples=num_samples).mean(0)
+        res["μ_rna"] = self.handler.predict_local_variable("μ_rna", num_samples=num_samples, num_split=num_split).mean(
+            0
+        )
+        adata.obsm[f"X_{model_key}"] = self.handler.predict_local_variable(
+            "z", num_samples=num_samples, num_split=num_split
+        ).mean(0)
+        adata.obsm[f"Z_{model_key}"] = self.handler.predict_local_variable(
+            "z_vec", num_samples=num_samples, num_split=num_split
+        ).mean(0)
```

### Comparing `sccca-0.3.0/scCCA/plots/factor_embedding.py` & `sccca-0.3.1/scCCA/plots/factor_embedding.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/scCCA/plots/loadings_bar.py` & `sccca-0.3.1/scCCA/plots/loadings_bar.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/scCCA/plots/loadings_scatter.py` & `sccca-0.3.1/scCCA/plots/loadings_scatter.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/scCCA/plots/qc.py` & `sccca-0.3.1/scCCA/plots/qc.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/scCCA/plots/utils.py` & `sccca-0.3.1/scCCA/plots/utils.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/scCCA/train/handler.py` & `sccca-0.3.1/scCCA/train/handler.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/scCCA/train/local_handler.py` & `sccca-0.3.1/scCCA/train/local_handler.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/scCCA/utils/data.py` & `sccca-0.3.1/scCCA/utils/data.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/scCCA/utils/design.py` & `sccca-0.3.1/scCCA/utils/design.py`

 * *Files identical despite different names*

### Comparing `sccca-0.3.0/setup.py` & `sccca-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
           'sphinx-rtd-theme==1.0.0',
           'sphinxcontrib-napoleon==0.7',
           'nbsphinx==0.8.9'],
  'notebook': ['jupyter']}
 
 setup_kwargs = {
     'name': 'sccca',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Single cell canonical correlation analysis.',
     'long_description': 'None',
     'author': 'Harald Vohringer',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `sccca-0.3.0/PKG-INFO` & `sccca-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sccca
-Version: 0.3.0
+Version: 0.3.1
 Summary: Single cell canonical correlation analysis.
 Author: Harald Vohringer
 Requires-Python: >=3.8.1,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: docs
```


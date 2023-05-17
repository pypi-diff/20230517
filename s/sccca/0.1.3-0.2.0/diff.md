# Comparing `tmp/scCCA-0.1.3.tar.gz` & `tmp/sccca-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scCCA-0.1.3.tar", max compression
+gzip compressed data, was "sccca-0.2.0.tar", max compression
```

## Comparing `scCCA-0.1.3.tar` & `sccca-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0      979 2022-12-15 05:57:21.608314 scCCA-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      137 2022-12-15 05:57:21.608314 scCCA-0.1.3/scCCA/__init__.py
--rw-r--r--   0        0        0     5446 2022-12-15 05:57:21.608314 scCCA-0.1.3/scCCA/cca.py
--rw-r--r--   0        0        0      108 2022-12-15 05:57:21.608314 scCCA-0.1.3/scCCA/logger.py
--rw-r--r--   0        0        0    17294 2022-12-15 05:57:21.608314 scCCA-0.1.3/scCCA/model.py
--rw-r--r--   0        0        0     6818 2022-12-15 05:57:21.608314 scCCA-0.1.3/scCCA/pca.py
--rw-r--r--   0        0        0       72 2022-12-15 05:57:21.608314 scCCA-0.1.3/scCCA/plots/__init__.py
--rw-r--r--   0        0        0     5009 2022-12-15 05:57:21.608314 scCCA-0.1.3/scCCA/plots/qc.py
--rw-r--r--   0        0        0      154 2022-12-15 05:57:21.612314 scCCA-0.1.3/scCCA/train/__init__.py
--rw-r--r--   0        0        0     7296 2022-12-15 05:57:21.612314 scCCA-0.1.3/scCCA/train/handler.py
--rw-r--r--   0        0        0     3866 2022-12-15 05:57:21.612314 scCCA-0.1.3/scCCA/train/local_handler.py
--rw-r--r--   0        0        0      488 2022-12-15 05:57:21.612314 scCCA-0.1.3/scCCA/train/settings.py
--rw-r--r--   0        0        0      243 2022-12-15 05:57:21.612314 scCCA-0.1.3/scCCA/utils/__init__.py
--rw-r--r--   0        0        0     1352 2022-12-15 05:57:21.612314 scCCA-0.1.3/scCCA/utils/data.py
--rw-r--r--   0        0        0     3173 2022-12-15 05:57:21.612314 scCCA-0.1.3/scCCA/utils/design.py
--rw-r--r--   0        0        0      888 2022-12-15 05:57:31.602593 scCCA-0.1.3/setup.py
--rw-r--r--   0        0        0      685 2022-12-15 05:57:31.602903 scCCA-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-04-04 09:44:34.103988 sccca-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/__init__.py
+-rw-r--r--   0        0        0     8325 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/cca.py
+-rw-r--r--   0        0        0      108 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/logger.py
+-rw-r--r--   0        0        0    22241 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/model.py
+-rw-r--r--   0        0        0     9733 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/pca.py
+-rw-r--r--   0        0        0      297 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/plots/__init__.py
+-rw-r--r--   0        0        0     3308 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/plots/factor_embedding.py
+-rw-r--r--   0        0        0     6052 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/plots/loadings_bar.py
+-rw-r--r--   0        0        0     8587 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/plots/loadings_scatter.py
+-rw-r--r--   0        0        0     8624 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/plots/qc.py
+-rw-r--r--   0        0        0     2663 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/plots/utils.py
+-rw-r--r--   0        0        0      154 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/train/__init__.py
+-rw-r--r--   0        0        0     7299 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/train/handler.py
+-rw-r--r--   0        0        0     3836 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/train/local_handler.py
+-rw-r--r--   0        0        0      488 2023-04-04 09:44:34.103988 sccca-0.2.0/scCCA/train/settings.py
+-rw-r--r--   0        0        0      356 2023-04-04 09:44:34.107988 sccca-0.2.0/scCCA/utils/__init__.py
+-rw-r--r--   0        0        0     1589 2023-04-04 09:44:34.107988 sccca-0.2.0/scCCA/utils/data.py
+-rw-r--r--   0        0        0     3468 2023-04-04 09:44:34.107988 sccca-0.2.0/scCCA/utils/design.py
+-rw-r--r--   0        0        0      319 2023-04-04 09:44:34.107988 sccca-0.2.0/scCCA/utils/scanpy.py
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 sccca-0.2.0/setup.py
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 sccca-0.2.0/PKG-INFO
```

### Comparing `scCCA-0.1.3/pyproject.toml` & `sccca-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "scCCA"
 packages = [
     { include = "scCCA" },
 ]
-version = "0.1.3"
+version = "0.2.0"
 description = "Single cell canonical correlation analysis."
 authors = ["Harald Vohringer"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 scanpy = ">=1.8.2"
 pyro-ppl = ">=1.8.0"
 Sphinx = { version = "4.2.0", optional = true }
 sphinx-rtd-theme = { version = "1.0.0", optional = true }
 sphinxcontrib-napoleon = { version = "0.7", optional = true }
 nbsphinx = { version = "0.8.9", optional = true }
 jupyter = {version = "*", optional = true}
+adjusttext = "^0.7.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 black = "^22.12.0"
 isort = "^5.11.2"
 bandit = "^1.7.4"
@@ -31,11 +32,11 @@
 notebook = ["jupyter"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-line-length = 88
+line-length = 120
 force-exclude = """
 scCCA/model.py
 """
```

### Comparing `scCCA-0.1.3/scCCA/pca.py` & `sccca-0.2.0/scCCA/pca.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from functools import partial
 from typing import Union
 
 import numpy as np
 import torch
 from anndata import AnnData
-from patsy.design_info import DesignMatrix
 from torch.types import Device
 
 from .model import guide, model
 from .train import SUBSAMPLE, SVILocalHandler
-from .utils import get_formula, get_rna_counts, get_state_loadings, get_states
+from .utils import get_formula, get_rna_counts, get_states
 
 
 class scPCA(object):
     """
     scPCA model.
 
     Parameters
@@ -72,100 +71,100 @@
 
         self.subsampling = min([subsampling, adata.shape[0]])
         self.device = device
 
         # prepare design and batch matrix
         self.batch_matrix = get_formula(self.adata, self.batch_formula)
         self.design_matrix = get_formula(self.adata, self.design_formula)
+        self.batch_states = get_states(self.batch_matrix)
+        self.design_states = get_states(self.design_matrix)
 
         #
         self.model_kwargs = model_kwargs
         self.training_kwargs = training_kwargs
 
         # setup data
         self.data = self._setup_data()
         self.handler = self._setup_handler()
 
     def _to_torch(self, data):
         """
         Helper method to convert numpy arrays of a dict to torch tensors.
         """
-        return {
-            k: torch.tensor(v, device=self.device) if isinstance(v, np.ndarray) else v
-            for k, v in data.items()
-        }
+        return {k: torch.tensor(v, device=self.device) if isinstance(v, np.ndarray) else v for k, v in data.items()}
 
     def _setup_data(self):
         """
         Sets up the data.
         """
         X = get_rna_counts(self.adata, self.layers_key)
         X_size = np.log(X.sum(axis=1, keepdims=True))
-        batch = np.asarray(self.batch_matrix).astype(np.float32)
-        design = np.asarray(self.design_matrix).astype(np.float32)
+        batch = np.asarray(self.batch_states.encoding).astype(np.float32)
+        design = np.asarray(self.design_states.encoding).astype(np.float32)
+        batch_idx = self.batch_states.index
+        design_idx = self.design_states.index
 
         num_genes = X.shape[1]
         num_cells = X.shape[0]
         num_batches = batch.shape[1]
         idx = np.arange(num_cells)
 
         data = dict(
+            num_factors=self.num_factors,
             X=X,
             X_size=X_size,
             Y=None,
             Y_size=None,
+            design=design,
             batch=batch,
+            design_idx=design_idx,
+            batch_idx=batch_idx,
             idx=idx,
             num_genes=num_genes,
             num_proteins=None,
             num_batches=num_batches,
             num_cells=num_cells,
-            design=design,
         )
         return self._to_torch(data)
 
     def _setup_handler(self):
         """
         Sets up the handler for training the model.
         """
         train_model = partial(
             model,
-            num_factors=self.num_factors,
             subsampling=self.subsampling,
             minibatches=False,
             device=self.device,
             **self.data,
             **self.model_kwargs,
         )
 
         train_guide = partial(
             guide,
-            num_factors=self.num_factors,
             subsampling=self.subsampling,
             minibatches=False,
             device=self.device,
             **self.data,
             **self.model_kwargs,
         )
 
         idx = self.data.pop("idx")
 
         predict_model = partial(
             model,
-            num_factors=self.num_factors,
             subsampling=0,
             minibatches=True,
             device=self.device,
             **self.data,
             **self.model_kwargs,
         )
 
         predict_guide = partial(
             guide,
-            num_factors=self.num_factors,
             subsampling=0,
             minibatches=True,
             device=self.device,
             **self.data,
             **self.model_kwargs,
         )
 
@@ -177,35 +176,85 @@
             idx=idx,
             **self.training_kwargs,
         )
 
     def fit(self, *args, **kwargs):
         self.handler.fit(*args, **kwargs)
 
-    def to_anndata(self, adata=None, model_key=None, num_samples=25):
-        if model_key is None:
-            model_key = self.model_key
+    def _meta_to_anndata(self, model_key=None, num_samples=25):
+        model_key = self.model_key if model_key is None else model_key
+        adata = self.adata
+
+        adata.uns[f"{model_key}"] = {}
+        res = adata.uns[f"{model_key}"]
+        res["design"] = {
+            **{str(k): v for k, v in self.design_states.columns.items()},
+            **{str(k): v for k, v in self.design_states.states.items()},
+        }
+        res["intercept"] = {
+            **{str(k): v for k, v in self.batch_states.columns.items()},
+            **{str(k): v for k, v in self.batch_states.states.items()},
+        }
+        res["loss"] = self.handler.loss
+        res["model"] = {"num_factors": self.num_factors, **self.model_kwargs}
 
-        if adata is None:
-            adata = self.adata
+        return res
 
-        adata.obsm[f"X_{model_key}"] = self.handler.predict_local_variable(
-            "z", num_samples=num_samples
-        ).mean(0)
-        adata.layers[f"{model_key}_pred_rna"] = self.handler.predict_local_variable(
-            "μ_rna", num_samples=num_samples
-        ).mean(0)
+    def posterior_to_anndata(self, model_key=None, num_samples=25):
+        _ = self._meta_to_anndata(model_key, num_samples)
+        adata = self.adata
 
-        adata.varm[f"{model_key}"] = (
-            self.handler.predict_global_variable("W_fac", num_samples=num_samples)
-            .mean(0)
-            .T
+        adata.varm[f"{model_key}_W_rna"] = (
+            self.handler.predict_global_variable("W_lin", num_samples=num_samples).T.swapaxes(-1, -3).swapaxes(-1, -2)
         )
+        adata.varm[f"{model_key}_V_rna"] = self.handler.predict_global_variable(
+            "W_add", num_samples=num_samples
+        ).T.swapaxes(-1, -2)
 
-        if isinstance(self.design_matrix, DesignMatrix):
-            adata.uns[f"{model_key}"] = {"design": get_states(self.design_matrix)}
-
-        state_loadings = get_state_loadings(adata, model_key)
-        adata.uns[f"{model_key}"]["states"] = state_loadings
-        adata.uns[f"{model_key}"]["α_rna"] = self.handler.predict_global_variable(
-            "α_rna"
+        α_rna = self.handler.predict_global_variable("α_rna", num_samples=num_samples).T
+
+        if α_rna.ndim == 2:
+            α_rna = np.expand_dims(α_rna, 1)
+
+        adata.varm[f"{model_key}_α_rna"] = α_rna.swapaxes(-1, -2)
+
+        σ_rna = self.handler.predict_global_variable("σ_rna", num_samples=num_samples).T
+
+        if σ_rna.ndim == 2:
+            σ_rna = np.expand_dims(σ_rna, 1)
+
+        adata.varm[f"{model_key}_σ_rna"] = σ_rna.swapaxes(-1, -2)
+
+        adata.obsm[f"X_{model_key}"] = self.handler.predict_local_variable("z", num_samples=num_samples).swapaxes(0, 1)
+
+    def mean_to_anndata(self, model_key=None, num_samples=25):
+        _ = self._meta_to_anndata(model_key, num_samples)
+        adata = self.adata
+
+        adata.layers[f"{model_key}_μ_rna"] = self.handler.predict_local_variable("μ_rna", num_samples=num_samples).mean(
+            0
+        )
+        adata.layers[f"{model_key}_offset_rna"] = self.handler.predict_local_variable(
+            "offset_rna", num_samples=num_samples
         ).mean(0)
+        adata.obsm[f"X_{model_key}"] = self.handler.predict_local_variable("z", num_samples=num_samples).mean(0)
+        adata.varm[f"{model_key}_W_rna"] = (
+            self.handler.predict_global_variable("W_lin", num_samples=num_samples).mean(0).T
+        )
+        adata.varm[f"{model_key}_V_rna"] = (
+            self.handler.predict_global_variable("W_add", num_samples=num_samples).mean(0).T
+        )
+        adata.varm[f"{model_key}_α_rna"] = self.handler.predict_global_variable("α_rna").mean(0).T
+        adata.varm[f"{model_key}_σ_rna"] = self.handler.predict_global_variable("σ_rna").mean(0).T
+
+    def to_anndata(self, model_key=None, num_samples=25):
+        res = self._meta_to_anndata(model_key, num_samples)
+        adata = self.adata
+        res["α_rna"] = self.handler.predict_global_variable("α_rna", num_samples=num_samples).mean(0)
+        res["W_fac"] = self.handler.predict_global_variable("W_fac", num_samples=num_samples).mean(0)
+        res["W_vec"] = self.handler.predict_global_variable("W_vec", num_samples=num_samples).mean(0)
+        res["W_lin"] = self.handler.predict_global_variable("W_lin", num_samples=num_samples).mean(0)
+        res["W_add"] = self.handler.predict_global_variable("W_add", num_samples=num_samples).mean(0)
+
+        res["μ_rna"] = self.handler.predict_local_variable("μ_rna", num_samples=num_samples).mean(0)
+        adata.obsm[f"X_{model_key}"] = self.handler.predict_local_variable("z", num_samples=num_samples).mean(0)
+        adata.obsm[f"Z_{model_key}"] = self.handler.predict_local_variable("z_vec", num_samples=num_samples).mean(0)
```

### Comparing `scCCA-0.1.3/scCCA/train/handler.py` & `sccca-0.2.0/scCCA/train/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 
         self.loss = None
         self.to_numpy = to_numpy
         self.best_elbo = None
         self.steps = 0
 
     def _update_state(self, loss):
+        if isinstance(loss, list):
+            loss = np.asarray(loss)
         self.loss = loss if self.loss is None else np.concatenate([self.loss, loss])
 
     def _to_numpy(self, posterior):
         return {k: v.detach().cpu().numpy() for k, v in posterior.items()}
 
     def _init_svi(self):
         """
@@ -113,27 +115,23 @@
 
     def _track_learning_rate(self):
         """
         Tracks the learning rate during training.
         """
         for name, param in self.optimizer.get_state().items():
             if "optimizer" in param:
-                self.learning_rates[name].append(
-                    param["optimizer"]["param_groups"][0]["lr"]
-                )
+                self.learning_rates[name].append(param["optimizer"]["param_groups"][0]["lr"])
             else:
                 self.learning_rates[name].append(param["param_groups"][0]["lr"])
 
     def _track_gradient_norms(self):
         # Register hooks to monitor gradient norms.
 
         for name, value in pyro.get_param_store().named_parameters():
-            value.register_hook(
-                lambda g, name=name: self.gradient_norms[name].append(g.norm().item())
-            )
+            value.register_hook(lambda g, name=name: self.gradient_norms[name].append(g.norm().item()))
 
     def _fit(self, *args, **kwargs):
         losses = []
         pbar = tqdm(range(self.steps, self.steps + self.num_epochs))
         failure = False
 
         previous_elbo = 0
```

### Comparing `scCCA-0.1.3/scCCA/train/local_handler.py` & `sccca-0.2.0/scCCA/train/local_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,12 +114,10 @@
         pbar = tqdm(range(len(split_obs)))
 
         results = []
         for i in pbar:
             self.predict([var], num_samples=num_samples, idx=split_obs[i])
             results.append(self.posterior[var])
             # update status bar
-            pbar.set_description(
-                f"Predicting {var} for obs {torch.min(split_obs[i])}-{torch.max(split_obs[i])}."
-            )
+            pbar.set_description(f"Predicting {var} for obs {torch.min(split_obs[i])}-{torch.max(split_obs[i])}.")
 
         return np.concatenate(results, obs_dim)
```

### Comparing `scCCA-0.1.3/scCCA/utils/data.py` & `sccca-0.2.0/scCCA/utils/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from scipy.sparse import issparse
 
 
+def extract_counts(adata, layers_key, protein_obsm_key):
+    if protein_obsm_key is not None:
+        counts = get_protein_counts(adata, protein_obsm_key)
+    else:
+        counts = get_rna_counts(adata, layers_key)
+
+    return counts
+
+
 def get_rna_counts(adata: AnnData, layers_key: Union[str, None] = None) -> np.ndarray:
     """
     Extracts RNA counts from AnnData object.
 
     Parameters
     ----------
     adata: AnnData
```

### Comparing `scCCA-0.1.3/PKG-INFO` & `sccca-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: sccca
-Version: 0.1.3
+Version: 0.2.0
 Summary: Single cell canonical correlation analysis.
 Author: Harald Vohringer
 Requires-Python: >=3.8.1,<3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: docs
 Provides-Extra: notebook
-Requires-Dist: Sphinx (==4.2.0); extra == "docs"
-Requires-Dist: jupyter; extra == "notebook"
-Requires-Dist: nbsphinx (==0.8.9); extra == "docs"
+Requires-Dist: Sphinx (==4.2.0) ; extra == "docs"
+Requires-Dist: adjusttext (>=0.7.3,<0.8.0)
+Requires-Dist: jupyter ; extra == "notebook"
+Requires-Dist: nbsphinx (==0.8.9) ; extra == "docs"
 Requires-Dist: pyro-ppl (>=1.8.0)
 Requires-Dist: scanpy (>=1.8.2)
-Requires-Dist: sphinx-rtd-theme (==1.0.0); extra == "docs"
-Requires-Dist: sphinxcontrib-napoleon (==0.7); extra == "docs"
+Requires-Dist: sphinx-rtd-theme (==1.0.0) ; extra == "docs"
+Requires-Dist: sphinxcontrib-napoleon (==0.7) ; extra == "docs"
```


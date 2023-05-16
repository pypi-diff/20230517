# Comparing `tmp/causalforge-0.0.9.tar.gz` & `tmp/causalforge-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalforge-0.0.9.tar", last modified: Thu May 11 20:45:40 2023, max compression
+gzip compressed data, was "causalforge-0.1.0.tar", last modified: Tue May 16 22:12:40 2023, max compression
```

## Comparing `causalforge-0.0.9.tar` & `causalforge-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-11 20:45:40.512554 causalforge-0.0.9/
--rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.9/LICENSE
--rw-r--r--   0 AG62216    (501) staff       (20)     3032 2023-05-11 20:45:40.512770 causalforge-0.0.9/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)     2580 2023-05-04 08:14:33.000000 causalforge-0.0.9/README.md
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-11 20:45:40.500987 causalforge-0.0.9/causalforge/
--rw-r--r--   0 AG62216    (501) staff       (20)      146 2023-05-11 20:42:17.000000 causalforge-0.0.9/causalforge/__init__.py
--rw-r--r--   0 AG62216    (501) staff       (20)     3801 2023-05-03 23:40:50.000000 causalforge-0.0.9/causalforge/data_loader.py
--rw-r--r--   0 AG62216    (501) staff       (20)     3285 2023-05-05 22:52:33.000000 causalforge-0.0.9/causalforge/metrics.py
--rw-r--r--   0 AG62216    (501) staff       (20)     3381 2023-05-11 18:46:21.000000 causalforge-0.0.9/causalforge/model.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-11 20:45:40.511680 causalforge-0.0.9/causalforge/models/
--rw-r--r--   0 AG62216    (501) staff       (20)      159 2023-05-11 18:46:32.000000 causalforge-0.0.9/causalforge/models/__init__.py
--rw-r--r--   0 AG62216    (501) staff       (20)     8906 2023-05-11 20:21:07.000000 causalforge-0.0.9/causalforge/models/bcauss.py
--rw-r--r--   0 AG62216    (501) staff       (20)     6699 2023-05-11 19:38:39.000000 causalforge-0.0.9/causalforge/models/dragonnet.py
--rw-r--r--   0 AG62216    (501) staff       (20)    12960 2023-05-08 22:56:29.000000 causalforge-0.0.9/causalforge/models/ganite.py
--rw-r--r--   0 AG62216    (501) staff       (20)     6077 2023-05-11 19:12:08.000000 causalforge-0.0.9/causalforge/models/utils.py
--rw-r--r--   0 AG62216    (501) staff       (20)      519 2023-05-05 04:55:01.000000 causalforge-0.0.9/causalforge/utils.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-11 20:45:40.505539 causalforge-0.0.9/causalforge.egg-info/
--rw-r--r--   0 AG62216    (501) staff       (20)     3032 2023-05-11 20:45:40.000000 causalforge-0.0.9/causalforge.egg-info/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)      475 2023-05-11 20:45:40.000000 causalforge-0.0.9/causalforge.egg-info/SOURCES.txt
--rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-05-11 20:45:40.000000 causalforge-0.0.9/causalforge.egg-info/dependency_links.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      137 2023-05-11 20:45:40.000000 causalforge-0.0.9/causalforge.egg-info/requires.txt
--rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-05-11 20:45:40.000000 causalforge-0.0.9/causalforge.egg-info/top_level.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-05-11 20:45:40.514249 causalforge-0.0.9/setup.cfg
--rw-r--r--   0 AG62216    (501) staff       (20)     1660 2023-05-02 00:20:37.000000 causalforge-0.0.9/setup.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-16 22:12:40.176460 causalforge-0.1.0/
+-rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.1.0/LICENSE
+-rw-r--r--   0 AG62216    (501) staff       (20)     3032 2023-05-16 22:12:40.176656 causalforge-0.1.0/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)     2580 2023-05-04 08:14:33.000000 causalforge-0.1.0/README.md
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-16 22:12:40.161114 causalforge-0.1.0/causalforge/
+-rw-r--r--   0 AG62216    (501) staff       (20)      146 2023-05-16 22:12:11.000000 causalforge-0.1.0/causalforge/__init__.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     3801 2023-05-03 23:40:50.000000 causalforge-0.1.0/causalforge/data_loader.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     3285 2023-05-05 22:52:33.000000 causalforge-0.1.0/causalforge/metrics.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     4311 2023-05-16 20:49:16.000000 causalforge-0.1.0/causalforge/model.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-16 22:12:40.175238 causalforge-0.1.0/causalforge/models/
+-rw-r--r--   0 AG62216    (501) staff       (20)    17298 2023-05-16 00:10:26.000000 causalforge-0.1.0/causalforge/models/CFR.py
+-rw-r--r--   0 AG62216    (501) staff       (20)      262 2023-05-16 20:39:05.000000 causalforge-0.1.0/causalforge/models/__init__.py
+-rw-r--r--   0 AG62216    (501) staff       (20)    14062 2023-05-16 21:09:26.000000 causalforge-0.1.0/causalforge/models/bcaus.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     8894 2023-05-16 20:49:37.000000 causalforge-0.1.0/causalforge/models/bcauss.py
+-rw-r--r--   0 AG62216    (501) staff       (20)    15906 2023-05-16 00:37:35.000000 causalforge-0.1.0/causalforge/models/cfr_net.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     6743 2023-05-16 20:49:51.000000 causalforge-0.1.0/causalforge/models/dragonnet.py
+-rw-r--r--   0 AG62216    (501) staff       (20)    13108 2023-05-16 20:50:06.000000 causalforge-0.1.0/causalforge/models/ganite.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     6077 2023-05-11 19:12:08.000000 causalforge-0.1.0/causalforge/models/utils.py
+-rw-r--r--   0 AG62216    (501) staff       (20)      519 2023-05-05 04:55:01.000000 causalforge-0.1.0/causalforge/utils.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-16 22:12:40.165544 causalforge-0.1.0/causalforge.egg-info/
+-rw-r--r--   0 AG62216    (501) staff       (20)     3032 2023-05-16 22:12:40.000000 causalforge-0.1.0/causalforge.egg-info/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)      559 2023-05-16 22:12:40.000000 causalforge-0.1.0/causalforge.egg-info/SOURCES.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-05-16 22:12:40.000000 causalforge-0.1.0/causalforge.egg-info/dependency_links.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      137 2023-05-16 22:12:40.000000 causalforge-0.1.0/causalforge.egg-info/requires.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-05-16 22:12:40.000000 causalforge-0.1.0/causalforge.egg-info/top_level.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-05-16 22:12:40.177678 causalforge-0.1.0/setup.cfg
+-rw-r--r--   0 AG62216    (501) staff       (20)     1660 2023-05-02 00:20:37.000000 causalforge-0.1.0/setup.py
```

### Comparing `causalforge-0.0.9/LICENSE` & `causalforge-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.9/PKG-INFO` & `causalforge-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python Package for Causal Inference
 Home-page: https://github.com/anthem-ai/causalforge
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `causalforge-0.0.9/README.md` & `causalforge-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.9/causalforge/data_loader.py` & `causalforge-0.1.0/causalforge/data_loader.py`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.9/causalforge/metrics.py` & `causalforge-0.1.0/causalforge/metrics.py`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.9/causalforge/model.py` & `causalforge-0.1.0/causalforge/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,48 @@
     return mod
 
 
 class PROBLEM_TYPE(Enum):
     CAUSAL_TREATMENT_EFFECT_ESTIMATION = "causal_treatment_effect_estimation"
     PROPENSITY_ESTIMATION = "propensity_estimation"
     SYNTHETIC_DATA_GENERATION = "syntethic_data_generation"
+    
+
+class Propensity_Estimator(ABC):
+    def __init__(self):
+        pass
+    
+    @abstractmethod
+    def build(self,params):
+        pass 
+    
+    @abstractmethod
+    def fit(self, X, treatment):
+        """
+        Fits the model.
+
+        Args:
+            X (np.matrix or np.array or pd.Dataframe): a feature matrix
+            treatment (np.array or pd.Series): a treatment vector
+        """
+        pass 
+    
+    @abstractmethod
+    def predict(self, X):
+        """
+        Clones scikitlearn style. Check scickitlearn documentation for details.
+        """
+        pass 
+    
+    @abstractmethod
+    def predict_proba(self, X):
+        """
+        Clones scikitlearn style. Check scickitlearn documentation for details.
+        """
+        pass 
 
 
 class Model(ABC):
     
     def __init__(self):
         pass
 
@@ -29,33 +63,34 @@
                      multiple_treatments=False):
         if  problem_type==PROBLEM_TYPE.CAUSAL_TREATMENT_EFFECT_ESTIMATION:
             if multiple_treatments:
                 raise Exception("Multiple treatments not supported yet")
             else:
                 if name == 'bcauss':
                     klass = dynamic_import('causalforge.models.BCAUSS')
-                    net = klass()
-                    net.build(params)
-                    return net
                 elif name == 'dragonnet':
                     klass = dynamic_import('causalforge.models.DragonNet')
-                    net = klass()
-                    net.build(params)
-                    return net
                 elif name == 'ganite':
                     klass = dynamic_import('causalforge.models.Ganite')
-                    net = klass()
-                    net.build(params) 
-                    return net
-                elif name == 'bcauss':
-                    pass 
+                elif name == 'bcaus_dr':
+                    klass = dynamic_import('causalforge.models.BCAUS_DR') 
                 else:
                     raise Exception("Model not supported yet::"+str(name))
+                #
+                net = klass()
+                net.build(params)
+                return net
         elif problem_type==PROBLEM_TYPE.PROPENSITY_ESTIMATION:
-            raise Exception("problem_type not supported yet::"+str(problem_type))
+            if name == 'bcaus':
+                klass = dynamic_import('causalforge.models.BCAUS')
+            else:
+                raise Exception("Model not supported yet::"+str(name))
+            net = klass()
+            net.build(params)
+            return net
         elif problem_type==PROBLEM_TYPE.SYNTHETIC_DATA_GENERATION:
             raise Exception("problem_type not supported yet::"+str(problem_type))
         else:
             raise Exception("Invalid problem_type ::"+str(problem_type))
     
     @abstractmethod
     def build(self,params):
@@ -93,18 +128,20 @@
             X (np.matrix or np.array or pd.Dataframe): a feature matrix
         Returns:
             (np.array): treatment effect vector
         """
         pass 
     
     @abstractmethod
-    def predict_ate(self, X):
+    def predict_ate(self, X,treatment,y):
         """
         Predicts the average treatment effect ("ATE").
 
         Args:
             X (np.matrix or np.array or pd.Dataframe): a feature matrix
+            treatment (np.array or pd.Series): a treatment vector
+            y (np.array or pd.Series): an outcome vector
         Returns:
             (np.array): treatment effect vector
         """
         pass
```

### Comparing `causalforge-0.0.9/causalforge/models/bcauss.py` & `causalforge-0.1.0/causalforge/models/bcauss.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,22 +25,20 @@
             'neurons_per_layer': 200, 
             "act_fn": "relu",
             'reg_l2': 0.01, 
             'verbose': True, 
             'val_split': 0.22, 
             'ratio': 1.0, 
             'optim': "sgd",
-            'batch_size': 64,
             'epochs': 500,
             'learning_rate': 1e-5, 
             'momentum': 0.9,
             "use_bce": False, 
             "norm_bal_term": True, 
             "use_targ_term": False, 
-            "ratio": 1., 
             "b_ratio": 1.,
             "bs_ratio": 1.,
             "scale_preds": True
         }
         
         for k in params:
             params[k] = user_params.get(k,params[k])
@@ -138,22 +136,23 @@
         self.params = params
         
     
     def support_ite(self):
         return True 
     
     def predict_ite(self, X):
+        X = convert_pd_to_np(X)
         dummy = np.zeros((X.shape[0],))
         preds = self.model.predict([X,dummy,dummy])
         if self.params['scale_preds']:
             preds[:, 0] = np.squeeze(self.y_scaler.inverse_transform(preds[:, 0].reshape(-1,1).copy()),axis=-1)
             preds[:, 1] = np.squeeze(self.y_scaler.inverse_transform(preds[:, 1].reshape(-1,1).copy()),axis=-1)
         return (preds[:, 1] - preds[:, 0])
     
-    def predict_ate(self, X):
+    def predict_ate(self, X,treatment,y):
         return np.mean(self.predict_ite(X))
     
     def fit(self, X, treatment, y):
         X, treatment, y = convert_pd_to_np(X, treatment, y)
         
         treatment = treatment.reshape(-1, 1)
         y = y.reshape(-1, 1)
```

### Comparing `causalforge-0.0.9/causalforge/models/dragonnet.py` & `causalforge-0.1.0/causalforge/models/dragonnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,18 +126,19 @@
         self.model = keras_Model(inputs=inputs, outputs=concat_pred)
         self.params = params
     
     def support_ite(self):
         return True 
     
     def predict_ite(self, X):
+        X = convert_pd_to_np(X)
         preds = self.model.predict(X)
         return (preds[:, 1] - preds[:, 0])
     
-    def predict_ate(self, X):
+    def predict_ate(self, X,treatment,y):
         return np.mean(self.predict_ite(X))
     
     def fit(self, X, treatment, y):
         X, treatment, y = convert_pd_to_np(X, treatment, y)
         y = np.hstack((y.reshape(-1, 1), treatment.reshape(-1, 1)))
         metrics = [
             regression_loss,
```

### Comparing `causalforge-0.0.9/causalforge/models/ganite.py` & `causalforge-0.1.0/causalforge/models/ganite.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import random
 
 # third party
 import numpy as np
 import torch
 from torch import nn
 from causalforge.model import Model
+from .utils import (
+    convert_pd_to_np
+)
 
 
 DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 EPS = 1e-10
 
 #------------------------------------------------------------------------------
 
@@ -23,20 +26,22 @@
     def build(self,user_params):
         self.params = user_params
     
     def support_ite(self):
         return True 
     
     def predict_ite(self, X):
+        X = convert_pd_to_np(X)
         return self.model(X).numpy()
     
-    def predict_ate(self, X):
+    def predict_ate(self, X,treatment,y):
         return np.mean(self.predict_ite(X))
     
     def fit(self, X, treatment, y):
+        X, treatment, y = convert_pd_to_np(X, treatment, y)
         self.model = Ganite_Model(self,X, treatment, y)
         
 #------------------------------------------------------------------------------
 
 def enable_reproducible_results() -> None:
     np.random.seed(0)
     torch.manual_seed(0)
```

### Comparing `causalforge-0.0.9/causalforge/models/utils.py` & `causalforge-0.1.0/causalforge/models/utils.py`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.9/causalforge/utils.py` & `causalforge-0.1.0/causalforge/utils.py`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.9/causalforge.egg-info/PKG-INFO` & `causalforge-0.1.0/causalforge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python Package for Causal Inference
 Home-page: https://github.com/anthem-ai/causalforge
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `causalforge-0.0.9/setup.py` & `causalforge-0.1.0/setup.py`

 * *Files identical despite different names*


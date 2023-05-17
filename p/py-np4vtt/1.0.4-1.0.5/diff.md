# Comparing `tmp/py_np4vtt-1.0.4.tar.gz` & `tmp/py-np4vtt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_np4vtt-1.0.4.tar", max compression
+gzip compressed data, was "py-np4vtt-1.0.5.tar", max compression
```

## Comparing `py_np4vtt-1.0.4.tar` & `py-np4vtt-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     3162 2023-01-20 12:34:35.543166 py_np4vtt-1.0.4/README.md
--rw-r--r--   0        0        0      705 2023-01-20 12:34:18.579148 py_np4vtt-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1168 2022-11-18 15:58:31.871431 py_np4vtt-1.0.4/src/py_np4vtt/__init__.py
--rw-r--r--   0        0        0     2703 2022-11-18 15:58:31.871431 py_np4vtt-1.0.4/src/py_np4vtt/data_format.py
--rw-r--r--   0        0        0     7211 2022-11-18 15:58:31.871431 py_np4vtt-1.0.4/src/py_np4vtt/data_import.py
--rw-r--r--   0        0        0     9783 2023-01-20 12:31:19.638973 py_np4vtt-1.0.4/src/py_np4vtt/model_ann.py
--rw-r--r--   0        0        0     7402 2023-01-20 12:28:37.746849 py_np4vtt-1.0.4/src/py_np4vtt/model_ann_2.py
--rw-r--r--   0        0        0     6328 2023-01-20 12:20:35.194823 py_np4vtt-1.0.4/src/py_np4vtt/model_lconstant.py
--rw-r--r--   0        0        0     6804 2023-01-20 12:20:35.194823 py_np4vtt-1.0.4/src/py_np4vtt/model_loclogit.py
--rw-r--r--   0        0        0     6432 2023-01-20 12:20:35.198823 py_np4vtt-1.0.4/src/py_np4vtt/model_logistic.py
--rw-r--r--   0        0        0     8457 2022-11-18 15:58:31.875431 py_np4vtt-1.0.4/src/py_np4vtt/model_rouwendal.py
--rw-r--r--   0        0        0     5202 2022-11-18 15:58:31.875431 py_np4vtt-1.0.4/src/py_np4vtt/model_rv.py
--rw-r--r--   0        0        0     4909 2022-11-18 15:58:31.875431 py_np4vtt-1.0.4/src/py_np4vtt/plots.py
--rw-r--r--   0        0        0     1844 2023-01-20 12:20:35.198823 py_np4vtt-1.0.4/src/py_np4vtt/utils.py
--rw-r--r--   0        0        0     4104 1970-01-01 00:00:00.000000 py_np4vtt-1.0.4/setup.py
--rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 py_np4vtt-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3162 2023-05-15 18:15:40.174563 py-np4vtt-1.0.5/README.md
+-rw-r--r--   0        0        0      705 2023-05-17 06:21:35.582999 py-np4vtt-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1168 2023-05-15 18:15:40.190980 py-np4vtt-1.0.5/src/py_np4vtt/__init__.py
+-rw-r--r--   0        0        0     3579 2023-05-15 18:28:22.310516 py-np4vtt-1.0.5/src/py_np4vtt/data_format.py
+-rw-r--r--   0        0        0     7968 2023-05-15 18:28:22.311128 py-np4vtt-1.0.5/src/py_np4vtt/data_import.py
+-rw-r--r--   0        0        0    10354 2023-05-15 18:15:40.191804 py-np4vtt-1.0.5/src/py_np4vtt/model_ann.py
+-rw-r--r--   0        0        0     6590 2023-05-15 18:15:40.192356 py-np4vtt-1.0.5/src/py_np4vtt/model_lconstant.py
+-rw-r--r--   0        0        0     6952 2023-05-15 18:15:40.192592 py-np4vtt-1.0.5/src/py_np4vtt/model_loclogit.py
+-rw-r--r--   0        0        0     6819 2023-05-15 18:15:40.192800 py-np4vtt-1.0.5/src/py_np4vtt/model_logistic.py
+-rw-r--r--   0        0        0     9175 2023-05-15 18:15:40.192984 py-np4vtt-1.0.5/src/py_np4vtt/model_rouwendal.py
+-rw-r--r--   0        0        0     5385 2023-05-15 18:15:40.193225 py-np4vtt-1.0.5/src/py_np4vtt/model_rv.py
+-rw-r--r--   0        0        0     4909 2023-05-15 18:15:40.193377 py-np4vtt-1.0.5/src/py_np4vtt/plots.py
+-rw-r--r--   0        0        0     8211 2023-05-15 18:15:40.193577 py-np4vtt-1.0.5/src/py_np4vtt/utils.py
+-rw-r--r--   0        0        0     4103 2023-05-17 06:21:50.096403 py-np4vtt-1.0.5/setup.py
+-rw-r--r--   0        0        0     3981 2023-05-17 06:21:50.096883 py-np4vtt-1.0.5/PKG-INFO
```

### Comparing `py_np4vtt-1.0.4/README.md` & `py-np4vtt-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `py_np4vtt-1.0.4/pyproject.toml` & `py-np4vtt-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "py-np4vtt"
-version = "1.0.4"
+version = "1.0.5"
 description = "Python library providing NonParametric models for Value of Travel Time analysis"
-authors = ["João Paulo Pizani Flor <paulopizani@posteo.net>", "José Ignacio Hernández <J.I.Hernandez@tudelft.nl>"]
+authors = ["José Ignacio Hernández <J.I.Hernandez@tudelft.nl>", "João Paulo Pizani Flor <paulopizani@posteo.net>"]
 
 homepage = "https://gitlab.tudelft.nl/np4vtt/py-np4vtt"
 repository = "https://gitlab.tudelft.nl/np4vtt/py-np4vtt"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<=3.10"
```

### Comparing `py_np4vtt-1.0.4/src/py_np4vtt/__init__.py` & `py-np4vtt-1.0.5/src/py_np4vtt/__init__.py`

 * *Files identical despite different names*

### Comparing `py_np4vtt-1.0.4/src/py_np4vtt/data_format.py` & `py-np4vtt-1.0.5/src/py_np4vtt/data_format.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,35 +35,61 @@
 class ModelArrays:
     BVTT: npt.NDArray[np.float64]  # pd.Series[float]
     Choice: npt.NDArray[np.bool_]
     Accepts: npt.NDArray[np.int_]
     ID: npt.NDArray[np.int_]  # Unique participant IDs
     NP: int  # Number of participants
     T: int  # Number of choice situations per participant
+    is_balanced_panel: bool # Is the dataset a balanced panel?
 
 
 @dataclass
 class DescriptiveStatsBasic:
     NP: int  # Number of participants
+    N_BVTT: int # Number of unique BVTT points
+    ChosenBVTT_Mean: float  # Mean chosen BVTT
+    BVTT_min: float  # Minimum of BVTT
+    BVTT_max: float  # Maximum of BVTT
+
+    def __str__(self) -> str:
+        formatted_descriptives = cleandoc(f"""
+            Balanced panel: False
+            No. individuals: {self.NP}
+
+            BVTT statistics:
+            No. of unique BVTT points: {self.N_BVTT}
+            Mean chosen BVTT: {self.ChosenBVTT_Mean}
+            Minimum of BVTT: {self.BVTT_min}
+            Maximum of BVTT: {self.BVTT_max}
+        """)
+
+        return formatted_descriptives
+
+@dataclass
+class DescriptiveStatsPanel:
+    NP: int  # Number of participants
     T: int  # Number of choice situations per participant
+    N_BVTT: int # Number of unique BVTT points
     NT_FastExp: int  # Number of non-traders (fast-expensive alt.)
     NT_CheapSlow: int  # Number of non-traders (cheap-slow alt.)
     ChosenBVTT_Mean: float  # Mean chosen BVTT
     BVTT_min: float  # Minimum of BVTT
     BVTT_max: float  # Maximum of BVTT
 
     def __str__(self) -> str:
         formatted_descriptives = cleandoc(f"""
+            Balanced panel: True
             No. individuals: {self.NP}
             Sets per indiv.: {self.T}
 
             Number of non-traders:
             Fast-exp. alt.: {self.NT_FastExp}
             Slow-cheap alt.: {self.NT_CheapSlow}
 
             BVTT statistics:
+            No. of unique BVTT points: {self.N_BVTT}
             Mean chosen BVTT: {self.ChosenBVTT_Mean}
             Minimum of BVTT: {self.BVTT_min}
             Maximum of BVTT: {self.BVTT_max}
         """)
 
         return formatted_descriptives
```

### Comparing `py_np4vtt-1.0.4/src/py_np4vtt/data_import.py` & `py-np4vtt-1.0.5/src/py_np4vtt/data_import.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import math
 from typing import List
 
 import pandas as pd
 import numpy as np
 
-from py_np4vtt.data_format import Vars, VarsMapping, DescriptiveStatsBasic, ModelArrays, Arrays
+from py_np4vtt.data_format import Vars, VarsMapping, DescriptiveStatsBasic, DescriptiveStatsPanel, ModelArrays, Arrays
 
 
 class VarMappingException(Exception):
     def __init__(self, missingVar: Vars, colName: str):
         self.missingVar = missingVar
         self.colName = colName
 
@@ -42,16 +42,16 @@
 def validate_modeldata(id_all, t, cost1, cost2, time1, time2, slow_alt, cheap_alt, choice) -> List[str]:
     # Create errormessage list
     errorList = []
 
     if not np.isfinite(id_all).all():
         errorList.append('There are either NAs or (minus) infinite values in ID Variable')
 
-    if not (int(t) == t):
-        errorList.append('Number of choice situations must be equal for all individuals.')
+    # if not (int(t) == t):
+    #     errorList.append('Number of choice situations must be equal for all individuals.')
 
     if not np.isfinite(cost1).all():
         errorList.append('There are either NAs or (minus) infinite values in Cost of alternative 1.')
 
     if not np.isfinite(cost2).all():
         errorList.append('There are either NAs or (minus) infinite values in Cost of alternative 2.')
 
@@ -116,36 +116,47 @@
     # Identify expensive and slow alternative
     cheap_alt = np.c_[cost1,cost2].argmin(axis=1) + 1
     slow_alt = np.c_[time1,time2].argmax(axis=1) + 1
 
     # Create scalars and ID variables
     id_all = study_arrays[Vars.Id]
     id_uniq = pd.unique(id_all)
-    npar = id_uniq.size
     t = id_all.size / id_uniq.size
 
-    errorList = validate_modeldata(id_all, t, c1, c2, t1, t2, slow_alt, cheap_alt, choice)
-    t_int = math.floor(t)
+    # Determine if the panel is balanced
+    if int(t) == t:
+        is_balanced_panel = True
+        t_int = math.floor(t)
+        rows = id_uniq.size
+    else:
+        is_balanced_panel = False
+        t_int = 1
+        rows = id_all.size
+
+    npar = id_uniq.size
+
+    # errorList = validate_modeldata(id_all, t, c1, c2, t1, t2, slow_alt, cheap_alt, choice)
 
     # BVTT
-    bvtt = (- (c1-c2)/(t1-t2)).reshape((npar,t_int))
+    bvtt = (- (c1-c2)/(t1-t2)).reshape((rows,t_int))
 
     # FBE = "Fast But Expensive"
-    fbe_chosen = (choice != cheap_alt).reshape((npar, t_int))
+    fbe_chosen = (choice != cheap_alt).reshape((rows, t_int))
 
     # The number of times a DM accepted the 'FBE' alt. Sum accross columns
     accepts = np.sum(fbe_chosen.astype(int), 1)
 
     return ModelArrays(
         BVTT=bvtt,
         Choice=fbe_chosen,
         Accepts=accepts,
         ID=id_uniq,
         NP=npar,
         T=t_int,
+        is_balanced_panel=is_balanced_panel
     )
 
 
 def compute_descriptives(arrs: ModelArrays) -> DescriptiveStatsBasic:
     """Compute descriptive statistics
     
     It takes the object that contains the model arrays and returns a set of 
@@ -167,20 +178,36 @@
     fbe_units = arrs.Choice.astype(int)
 
     chosenBVTT = (fbe_units * arrs.BVTT)
 
     # noinspection PyTypeChecker
     chosenBVTT_mean: int = np.sum(chosenBVTT)/np.sum(fbe_units)
 
-    chosen_fastexp = np.sum(fbe_units, 1)
-    nt_cheapslow = np.count_nonzero(chosen_fastexp == 0)
-    nt_fastext = np.count_nonzero(chosen_fastexp == arrs.T)
-
-    return DescriptiveStatsBasic(
-        NP=arrs.NP,
-        T=arrs.T,
+    if arrs.is_balanced_panel:
+        n = arrs.NP
+        t = arrs.T
+        n_bvtt = len(np.unique(arrs.BVTT))
+        chosen_fastexp = np.sum(fbe_units, 1)
+        nt_cheapslow = np.count_nonzero(chosen_fastexp == 0)
+        nt_fastext = np.count_nonzero(chosen_fastexp == arrs.T)
+    
+        return DescriptiveStatsPanel(
+        NP=n,
+        T=t,
+        N_BVTT=n_bvtt,
         NT_FastExp=nt_fastext,
         NT_CheapSlow=nt_cheapslow,
         ChosenBVTT_Mean=np.round(chosenBVTT_mean,4),
         BVTT_min=np.round(np.amin(arrs.BVTT),4),
         BVTT_max=np.round(np.amax(arrs.BVTT),4),
-    )
+        )
+    else:
+        n = arrs.NP * arrs.T
+        n_bvtt = len(np.unique(arrs.BVTT))
+
+        return DescriptiveStatsBasic(
+        NP=n,
+        N_BVTT=n_bvtt,
+        ChosenBVTT_Mean=np.round(chosenBVTT_mean,4),
+        BVTT_min=np.round(np.amin(arrs.BVTT),4),
+        BVTT_max=np.round(np.amax(arrs.BVTT),4),
+        )
```

### Comparing `py_np4vtt-1.0.4/src/py_np4vtt/model_ann.py` & `py-np4vtt-1.0.5/src/py_np4vtt/model_ann.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import List, Optional
 
 from numpy import ndarray
 
 from py_np4vtt.data_format import ModelArrays
 
 import numpy as np
+import time
 
 from sklearn.neural_network import MLPClassifier
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import log_loss
 from sklearn.preprocessing import StandardScaler
 
 # TODO: Check with Joao how safe is to import os
@@ -103,14 +104,17 @@
     network based method to uncover the value-of-travel-time distribution." 
     Transportation 48.5 (2021): 2545-2583.
     """
     def __init__(self, cfg: ConfigANN, arrays: ModelArrays):
         self.cfg = cfg
         self.arrays = arrays
 
+        # Check if data is a balanced panel. Otherwise raise an error
+        assert arrays.is_balanced_panel, "Data is not a balanced panel. ModelANN is only compatible with balanced panel data"
+
         # Initialise arrays for randomisation
         shuffle_index = np.zeros((self.cfg.shufflesPerRepeat,self.arrays.T+1))
         full_data_array = np.zeros((self.arrays.NP,self.cfg.shufflesPerRepeat*(self.arrays.T+1),2))
 
         # Randomise data
         for n in range(self.arrays.NP):
             for m in range(self.cfg.shufflesPerRepeat):
@@ -153,20 +157,26 @@
         -------
         ll_list : np.ndarray
             The log-likelihood values per repetition.
         r2_list : np.ndarray
             The Rho-squared values per repetition.
         vtt_list : np.ndarray
             The estimated VTT per respondent and repetition.
+        est_time : float
+            The estimation time in seconds.
+        avg_time : float
+            Average estimation time per repetition.
         """
         ll_list = []
         rho_sq = []
         y_predict = []
         VTT_mid_list = []
 
+        # Start optimisation loop
+        t0 = time.time()
         for r in range(self.cfg.trainingRepeats):
             
             if verbose:
                 print('Rep ' + str(r+1) + ': ',end='',flush=True)
 
             clf = MLPClassifier(
                 hidden_layer_sizes=self.cfg.hiddenLayerNodes,
@@ -214,19 +224,24 @@
                     no_vtt = no_vtt+1
 
             VTT_mid_list.append(VTT_mid)
 
             if verbose:
                 print('(No VTT recovered for ' + str(no_vtt) + ' respondents)')
 
+        # Compute elapsed time
+        t1 = time.time()
+        est_time = t1 - t0
+        avg_time = est_time/self.cfg.trainingRepeats
+
         ll_list = np.array(ll_list)
         r2_list = np.array(rho_sq)
         vtt_list = np.array(VTT_mid_list)
 
-        return ll_list, r2_list, vtt_list
+        return ll_list, r2_list, vtt_list, est_time, avg_time
 
     @staticmethod
     def simulateNChoice(self,clf,y,vtt_grid,X,R):
 
         # Create arrays for random shufflings
         x_sim = np.zeros((y.shape[0]*vtt_grid.shape[1],2*self.arrays.T+1,R))
         y_sim = np.zeros((y.shape[0],vtt_grid.shape[1],R))
```

### Comparing `py_np4vtt-1.0.4/src/py_np4vtt/model_lconstant.py` & `py-np4vtt-1.0.5/src/py_np4vtt/model_lconstant.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """Modules to configure and estimate a Local constant model."""
 
 from dataclasses import dataclass
 import numpy as np
 from scipy.stats import norm
 from py_np4vtt.data_format import ModelArrays
 from py_np4vtt.utils import predicted_vtt, vtt_midpoints
+import time
 
 @dataclass
 class ConfigLConstant:
     """Configuration class of the local constant model.
     
     This class stores the configuration parameters of a local constant model 
     and performs integrity checks before being passed to the model object.
@@ -121,24 +122,34 @@
             The estimates of the cumulative choice probability (CDF), evaluated 
             at each mid point of the VTT grid. The first point is always zero 
             while the last point is always equal to the second last for 
             compatibility with plots.
         vtt : numpy.ndarray
             The estimated VTT per respondent, based in the estimated 
             CDF points (`p`) and the sample.
+        est_time : float
+            The estimation time in seconds.
         """
+
+        # Start estimation
+        t0 = time.time()
         p = ModelLConstant.nadaraya_watson(self.vtt_mid[1:-1],~self.arrays.Choice.flatten(),self.arrays.BVTT.flatten(),self.params.kernelWidth)
 
         # Create counts per point of the VTT mid points
         vtt = predicted_vtt(p,self.vtt_grid,self.arrays.NP)
 
+        # Compute elapsed time
+        t1 = time.time()
+        est_time = t1 - t0
+
         # Add point 0 in the estimated CDF and repeat last point to make coincide with point zero and last point in the VTT mid point
         p = np.concatenate((0,p,p[-1]),axis=None)
 
-        return p, vtt
+        # Return list of outcomes
+        return p, vtt, est_time
 
     # Nadaraya-Watson estimator with gaussian kernel
     @staticmethod
     def nadaraya_watson(x,Y,X,h):
         
         g = np.empty(shape=x.shape)
```

### Comparing `py_np4vtt-1.0.4/src/py_np4vtt/model_loclogit.py` & `py-np4vtt-1.0.5/src/py_np4vtt/model_loclogit.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #
 #  The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 #
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """Modules to configure and estimate a Local logit model."""
 from dataclasses import dataclass
 import numpy as np
-from scipy.optimize import minimize
 from py_np4vtt.data_format import ModelArrays
-from py_np4vtt.utils import vtt_midpoints, predicted_vtt
+from py_np4vtt.utils import vtt_midpoints, predicted_vtt, _bfgsmin
+import time
 
 @dataclass
 class ConfigLocLogit:
     """Configuration class of the local logit model.
     
     This class stores the configuration parameters of a local logit model 
     and performs integrity checks before being passed to the model object.
@@ -112,56 +112,63 @@
             while the last point is always equal to the second last for 
             compatibility with plots.
         vtt : numpy.ndarray
             The estimated VTT per respondent, based in the estimated 
             CDF points (`p`) and the sample.
         ll : float
             The log-likelihood function at the optimum of the estimation.
+        est_time : float
+            The estimation time in seconds.
         """
         # Compute the kernel width
         k = np.r_[self.vtt_grid, 0.] - np.r_[0., self.vtt_grid]
         k = k[:-2]
         k[0] = k[1].copy()
 
         YX = self.arrays.Choice.T.flatten()
 
         # Perform a weighted logit for each support point
+        t0 = time.time()
         p = []
         fval = 0.
         for n in range(len(self.vtt_grid)-1):
             x, fval_x = ModelLocLogit.initLocalLogit(n, k[n], self.arrays.BVTT, YX, self.vtt_grid)
             p.append(x[0])
             fval = fval + fval_x
-        
+
+        # Compute elapsed time
+        t1 = time.time()
+        est_time = t1 - t0
+
         # Return probability array and -ll
         p = np.array(p)
         ll = -fval
 
         # Compute the predicted VTT at the midpoints
         vtt = predicted_vtt(p,self.vtt_grid,self.arrays.NP)
 
         # Add point 0 in the estimated CDF and repeat last point to make coincide with point zero and last point in the VTT mid point
         p = np.concatenate((0,p,p[-1]),axis=None)
 
-        return p, vtt, ll
+        return p, vtt, ll, est_time
 
     @staticmethod
     def initLocalLogit(n, k, BVTT, YX, vtt_grid):
         # Get observations
         BVTT_flat = BVTT.T.flatten()
         xn = BVTT_flat[(BVTT_flat > (vtt_grid[n]-k)) & (BVTT_flat < (vtt_grid[n] + k))]
         x0 = vtt_grid[n]
         y_local = YX[(BVTT_flat > (vtt_grid[n]-k)) & (BVTT_flat < (vtt_grid[n] + k))]
         dist = np.abs(x0-xn)
         weight = (k-dist)/k
 
         # Search function
         coef_start = np.array([0., 0.])
         args = (y_local, xn, x0, weight)
-        results = minimize(ModelLocLogit.objectiveFunction, coef_start, args=args, method='L-BFGS-B',options={'gtol': 1e-6})
+        results = _bfgsmin(ModelLocLogit.objectiveFunction, coef_start, args=args, tol=1e-6,verbose=False)
 
         # Collect results
         x = results['x']
         fval = results['fun']
 
         # Convert to probabilities
         x = 1 - (np.exp(x)/(1+np.exp(x)))
```

### Comparing `py_np4vtt-1.0.4/src/py_np4vtt/model_logistic.py` & `py-np4vtt-1.0.5/src/py_np4vtt/model_logistic.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 #
 #  The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 #
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """Modules to configure and estimate a Logistic regression-based model."""
 from dataclasses import dataclass
 from typing import Optional, Tuple
-from scipy.optimize import minimize
 from numdifftools import Hessian
 import numpy as np
 import warnings
+import time
+from py_np4vtt.utils import _bfgsmin
 
 from py_np4vtt.data_format import ModelArrays
 
 warnings.filterwarnings('ignore')
 
 @dataclass
 class ConfigLogistic:
@@ -79,14 +80,17 @@
     ----------
     None.
     """
     def __init__(self, cfg: ConfigLogistic, arrays: ModelArrays):
         self.cfg = cfg
         self.arrays = arrays
 
+        # Check if data is a balanced panel. Otherwise raise an error
+        assert arrays.is_balanced_panel, "Data is not a balanced panel. ModelLogistic is only compatible with balanced panel data"
+
     def run(self):
         """Estimates the logistic regression model.
         
         Parameters
         ----------
         None.
 
@@ -102,14 +106,16 @@
         init_ll : float
             Log-likelihood at the starting values
         ll : float
             Log-likelihood in the optimum.
         exitflag : int
             Exit flag of the optimisation routine. If `exitflag=0`, the 
             optimisation succeeded. Otherwise, check the configuration parameters.
+        est_time : float
+            The estimation time in seconds.
         """
         # Use passed seed if desired
         if self.cfg.seed:
             np.random.seed(self.cfg.seed)
 
         # Prepare data
         i_obs_y = \
@@ -128,28 +134,33 @@
         # LL at the start values
         init_ll = -ModelLogistic.objectiveFunction(x0, sumYBVTT, BVTT, y_regress)
 
         # Starting arguments and values for minimizer
         argTuple = (sumYBVTT, BVTT, y_regress)
         
         # Start minimization routine
-        results = minimize(ModelLogistic.objectiveFunction, x0, args=argTuple, method='L-BFGS-B',options={'gtol': 1e-6,'maxiter': self.cfg.maxIterations})
+        t0 = time.time()
+        results = _bfgsmin(ModelLogistic.objectiveFunction, x0, args=argTuple,tol=1e-6, maxiter= self.cfg.maxIterations,verbose=True)
+
+        # Compute elapsed time
+        t1 = time.time()
+        est_time = t1 - t0
 
         # Collect results
         x = results['x']
         hess = Hessian(ModelLogistic.objectiveFunction,method='forward')(x,sumYBVTT, BVTT, y_regress)
         se = np.sqrt(np.diag(np.linalg.inv(hess)))
         ll = -results['fun']
-        exitflag = results['status']
+        exitflag = results['convergence']
 
         # Compute VTT
         vtt = x[1] + x[2]*((self.arrays.T-1)/self.arrays.T)*np.sum(self.arrays.Choice*self.arrays.BVTT,1)
         vtt = np.concatenate((0.,vtt),axis=None)
         
-        return x, se, vtt, init_ll ,ll, exitflag
+        return x, se, vtt, init_ll ,ll, exitflag, est_time
 
     @staticmethod
     def objectiveFunction(x: np.ndarray, sumYBVTT: np.ndarray, BVTT: np.ndarray, y_regress: np.ndarray):
         
         # Separate parameters: x is the estimated (multi-dimensional) parameter
         scale, intercept, parameter = x
```

### Comparing `py_np4vtt-1.0.4/src/py_np4vtt/model_rouwendal.py` & `py-np4vtt-1.0.5/src/py_np4vtt/model_rouwendal.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 #
 #  The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 #
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """Modules to configure and estimate a Rouwendal model."""
 from dataclasses import dataclass
 from typing import Tuple
-from scipy.optimize import minimize
 from numdifftools import Hessian
 import numpy as np
 import warnings
 from py_np4vtt.data_format import ModelArrays
-from py_np4vtt.utils import vtt_midpoints, predicted_vtt
+from py_np4vtt.utils import vtt_midpoints, predicted_vtt,_bfgsmin
+import time
 
 warnings.filterwarnings('ignore')
 
 @dataclass
 class ConfigRouwendal:
     """Configuration class of the Rouwendal model.
     
@@ -91,14 +91,17 @@
     statistical life." Transportation research part B: methodological 44.1 
     (2010): 136-151.
     """
     def __init__(self, cfg: ConfigRouwendal, arrays: ModelArrays):
         self.cfg = cfg
         self.arrays = arrays
 
+        # Check if data is a balanced panel. Otherwise raise an error
+        assert arrays.is_balanced_panel, "Data is not a balanced panel. ModelRouwendal is only compatible with balanced panel data"
+
         # Create grid of support points
         self.vtt_grid = np.linspace(self.cfg.minimum, self.cfg.maximum, self.cfg.supportPoints)
 
         # Compute the midpoints of the VTT grid
         self.vtt_mid = vtt_midpoints(self.vtt_grid)
 
         # Compute distance between points at each support point
@@ -141,37 +144,51 @@
             Value of log-likelihood function in the initial value of startQ. 
             Starting values of support point parameters are equal to zero.
         ll : float
             Value of the likelihood function in the optimum.
         exitflag : int
             Exit flag of the optimisation routine. If `exitflag=0`, the 
             optimisation succeeded. Otherwise, check the configuration parameters.
+        est_time : float
+            The estimation time in seconds.
         """
         # Set vector of starting values of xameters to estimate
         q0 = np.log(self.cfg.startQ/(1-self.cfg.startQ))
         x0 = np.hstack([q0, np.zeros(len(self.vtt_grid))])
 
+        # Get VTT grid shape
+        grid_shape = len(self.vtt_grid)
+
+        # Prepare arrays
+        BVTT_array = np.tile(self.arrays.BVTT,(grid_shape,1,1)).T
+        Choice_array = np.tile(self.arrays.Choice,(grid_shape,1,1)).T
+
         # Initial value of the log-likelihood function
-        init_ll = -ModelRouwendal.objectiveFunction(x0, self.arrays.NP, self.arrays.T, self.arrays.BVTT,
-                                                      self.arrays.Choice, self.vtt_grid)
+        init_ll = -ModelRouwendal.objectiveFunction(x0, self.arrays.NP, self.arrays.T, BVTT_array,
+                                                      Choice_array, self.vtt_grid)
 
         # TODO: add an integrity check: initialVal should be finite. Otherwise, rise an error.
 
         # Starting values
-        argTuple = (self.arrays.NP, self.arrays.T, self.arrays.BVTT, self.arrays.Choice, self.vtt_grid)
+        argTuple = (self.arrays.NP, self.arrays.T, BVTT_array, Choice_array, self.vtt_grid)
 
         # Start optimization
-        results = minimize(ModelRouwendal.objectiveFunction, x0, args=argTuple, method='L-BFGS-B',options={'gtol': 1e-6})
+        t0 = time.time()
+        results = _bfgsmin(ModelRouwendal.objectiveFunction, x0, args=argTuple,tol=1e-6,verbose=True)
+
+        # Compute elapsed time
+        t1 = time.time()
+        est_time = t1 - t0
 
         # Collect results
         x = results['x']
-        hess = Hessian(ModelRouwendal.objectiveFunction,method='forward')(x,self.arrays.NP, self.arrays.T, self.arrays.BVTT, self.arrays.Choice, self.vtt_grid)
+        hess = Hessian(ModelRouwendal.objectiveFunction,method='forward')(x,self.arrays.NP, self.arrays.T, BVTT_array, Choice_array, self.vtt_grid)
         se = np.sqrt(np.diag(np.linalg.inv(hess)))
         ll = -results['fun']
-        exitflag = results['status']
+        exitflag = results['convergence']
 
         # Get estimated probability of consistent choice
         q_prob = np.exp(x[0])/(1+np.exp(x[0]))
         q_est = x[0]
         q_se = np.sqrt((np.exp(q_est)/(1+np.exp(q_est)))**2)**2 * se[0]**2
 
         # Get estimated FVTT and xameters
@@ -183,28 +200,32 @@
         # Compute the predicted VTT at the midpoints
         vtt = predicted_vtt(p,self.vtt_mid,self.arrays.NP)
 
         # Add point 0 in the estimated CDF to make coincide with point zero in the VTT mid point
         p = np.concatenate((0,p),axis=None)
 
         # Return output
-        return q_est, q_se, q_prob, x, se, p, vtt, init_ll, ll, exitflag
+        return q_est, q_se, q_prob, x, se, p, vtt, init_ll, ll, exitflag, est_time
 
     @staticmethod
     def objectiveFunction(x, NP, T, BVTT, Choice, vtt_grid):
         
         # Re-scale Q and FVTT to fit between zero and one
         q = np.exp(x[0]) / (1 + np.exp(x[0]))
         fvtt = np.exp(x[1:]) / np.sum(np.exp(x[1:]))
 
+        # Compute conditional probabilities
+        tau = ((vtt_grid > BVTT) == Choice).astype(int).sum(axis=0)
+        P = ((q**tau) * (1-q)**(T-tau))
+
         # Conditional probability
-        P = np.zeros((NP, len(vtt_grid)))
+        # P = np.zeros((NP, len(vtt_grid)))
 
-        for n in range(len(vtt_grid)):
-            tau = np.sum(((vtt_grid[n] > BVTT) == Choice).astype(int), axis=1)
-            P[:, n] = (q**tau) * ((1-q) ** (T-tau))
+        # for n in range(len(vtt_grid)):
+        #     tau = np.sum(((vtt_grid[n] > BVTT) == Choice).astype(int), axis=1)
+        #     P[:, n] = (q**tau) * ((1-q) ** (T-tau))
             
         # Maximise log-likelihood. L is computed by multiplying conditional P
         # with density fvtt, average and sum across all obs
         L = -np.sum(np.log(np.sum(fvtt*P, axis=1)))
 
         return L
```

### Comparing `py_np4vtt-1.0.4/src/py_np4vtt/model_rv.py` & `py-np4vtt-1.0.5/src/py_np4vtt/model_rv.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 #
 #  The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 #
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """Modules to configure and estimate a Random Valuation model."""
 from dataclasses import dataclass
 from typing import Optional, Tuple
-from scipy.optimize import minimize
 from numdifftools import Hessian
 import numpy as np
+import time
 
 from py_np4vtt.data_format import ModelArrays
-
+from py_np4vtt.utils import _bfgsmin
 
 @dataclass
 class ConfigRV:
     """Configuration class of the random valuation model.
     
     This class stores the configuration parameters of a random valuation
     model and performs integrity checks before being passed to the model 
@@ -93,37 +93,44 @@
         init_ll : float
             Log-likelihood at the starting values
         ll : float
             Log-likelihood in the optimum.
         exitflag : int
             Exit flag of the optimisation routine. If `exitflag=0`, the 
             optimisation succeeded. Otherwise, check the configuration parameters.
+        est_time : float
+            The estimation time in seconds.
         """
         # Set vector of starting values of parameters to estimate
         x0 = np.array([self.cfg.startScale, self.cfg.startVTT])
 
         BVTT=self.arrays.BVTT.flatten()
         y_regress=self.arrays.Choice.flatten()
 
         init_ll = -ModelRV.objectiveFunction(x0, BVTT, y_regress)
 
         # Starting arguments and values for minimizer
         argTuple = (BVTT, y_regress)
 
         # Start minimization routine
-        results = minimize(ModelRV.objectiveFunction, x0, args=argTuple, method='L-BFGS-B',options={'gtol': 1e-6,'maxiter': self.cfg.maxIterations})
+        t0 = time.time()
+        results = _bfgsmin(ModelRV.objectiveFunction, x0, args=argTuple, tol=1e-6,maxiter=self.cfg.maxIterations,verbose=True)
+
+        # Compute elapsed time
+        t1 = time.time()
+        est_time = t1 - t0
 
         # Collect results
         x = results['x']
         hess = Hessian(ModelRV.objectiveFunction,method='forward')(x, BVTT, y_regress)
         se = np.sqrt(np.diag(np.linalg.inv(hess)))
         ll = -results['fun']
-        exitflag = results['status']
+        exitflag = results['convergence']
 
-        return x, se, init_ll, ll, exitflag
+        return x, se, init_ll, ll, exitflag, est_time
 
     @staticmethod
     def objectiveFunction(x: np.ndarray, BVTT: np.ndarray, y_regress: np.ndarray):
         # Separate parameters: x is the estimated (multi-dimensional) parameter
         scale, VTT = x
 
         # Create value functions
```

### Comparing `py_np4vtt-1.0.4/src/py_np4vtt/plots.py` & `py-np4vtt-1.0.5/src/py_np4vtt/plots.py`

 * *Files identical despite different names*

### Comparing `py_np4vtt-1.0.4/setup.py` & `py-np4vtt-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,21 +15,21 @@
  'numdifftools>=0.9.40,<0.10.0',
  'pandas>=1.3.1,<2.0.0',
  'scikit-learn>=1.0.2,<2.0.0',
  'scipy>=1.7.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'py-np4vtt',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': 'Python library providing NonParametric models for Value of Travel Time analysis',
     'long_description': '# NP4VTT\n\nNP4VTT is a Python package that enables researchers to estimate and compare nonparametric models in a fast and convenient way. It comprises five nonparametric models for estimating the VTT distribution from data coming from two-attribute-two-alternative stated choice experiments:\n\n   * Local constant model  (Fosgerau, 2006, 2007)\n   * Local logit (Fosgerau, 2007)\n   * Rouwendal model (Rouwendal et al., 2010)\n   * Artificial Neural Network (ANN) based VTT model (van Cranenburgh & Kouwenhoven, 2021)\n   * Logistic Regression based VTT model (van Cranenburgh & Kouwenhoven, 2021)\n\nAdditionally, a Random Valuation model (Ojeda-Cabral, 2006) is included for benchmarking purposes\n\n## Installation steps\n\n* Use `pip` to install the `py-np4vtt` library normally:\n    - `python3 -m pip install py-np4vtt`\n\n\n## Examples\n\nWe provide Jupyter Notebooks that show how to configure and estimate each model included in NP4VTT:\n\n   * Local constant model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/lconstant.ipynb)\n   * Local logit: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/loclogit.ipynb)\n   * Rouwendal model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/rouwendal.ipynb)\n   * ANN-based VTT model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/ann.ipynb)\n   * Logistic Regression-based VTT model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/logistic.ipynb)\n\nThese examples guide the user through the process of loading a dataset, estimating a nonparametric model, and visualising the VTT distribution using scatter and histogram plots. We use the Norwegian 2009 VTT data to illustrate each example.\n\n**Take, for example, the VTT distribution from the Rouwendal model using NP4VTT:**\n\n![VTT distribution from the Rouwendal model using NP4VTT](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/raw/master/examples/outcomes/rouwendal.png)\n\n## References\n\n   * Fosgerau, M. (2006). Investigating the distribution of the value of travel time savings. Transportation Research Part B: Methodological, 40(8), 688–707. https://doi.org/10.1016/j.trb.2005.09.007\n   * Fosgerau, M. (2007). Using nonparametrics to specify a model to measure the value of travel time. Transportation Research Part A: Policy and Practice, 41(9), 842–856. https://doi.org/10.1016/j.tra.2006.10.004\n   * Rouwendal, J., de Blaeij, A., Rietveld, P., & Verhoef, E. (2010). The information content of a stated choice experiment: A new method and its application to the value of a statistical life. Transportation Research Part B: Methodological, 44(1), 136–151. https://doi.org/10.1016/j.trb.2009.04.006\n   * Ojeda-Cabral, M., Batley, R., & Hess, S. (2016). The value of travel time: Random utility versus random valuation. Transportmetrica A: Transport Science, 12(3), 230–248. https://doi.org/10.1080/23249935.2015.1125398\n   * van Cranenburgh, S., & Kouwenhoven, M. (2021). An artificial neural network based method to uncover the value-of-travel-time distribution. Transportation, 48(5), 2545–2583. https://doi.org/10.1007/s11116-020-10139-3',
-    'author': 'João Paulo Pizani Flor',
-    'author_email': 'paulopizani@posteo.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
+    'author': 'José Ignacio Hernández',
+    'author_email': 'J.I.Hernandez@tudelft.nl',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://gitlab.tudelft.nl/np4vtt/py-np4vtt',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<=3.10',
 }
```

### Comparing `py_np4vtt-1.0.4/PKG-INFO` & `py-np4vtt-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: py-np4vtt
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python library providing NonParametric models for Value of Travel Time analysis
 Home-page: https://gitlab.tudelft.nl/np4vtt/py-np4vtt
-Author: João Paulo Pizani Flor
-Author-email: paulopizani@posteo.net
+Author: José Ignacio Hernández
+Author-email: J.I.Hernandez@tudelft.nl
 Requires-Python: >=3.8,<=3.10
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: numdifftools (>=0.9.40,<0.10.0)
 Requires-Dist: pandas (>=1.3.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
 Requires-Dist: scipy (>=1.7.1,<2.0.0)
 Project-URL: Repository, https://gitlab.tudelft.nl/np4vtt/py-np4vtt
 Description-Content-Type: text/markdown
```


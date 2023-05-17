# Comparing `tmp/msapy-1.2.1.tar.gz` & `tmp/msapy-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msapy-1.2.1.tar", last modified: Mon Feb 13 14:51:00 2023, max compression
+gzip compressed data, was "msapy-1.3.tar", last modified: Wed May 17 10:52:23 2023, max compression
```

## Comparing `msapy-1.2.1.tar` & `msapy-1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-02-13 14:51:00.252596 msapy-1.2.1/
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     1069 2021-10-28 14:21:00.000000 msapy-1.2.1/LICENSE
--rw-rw-r--   0 kayson    (1000) kayson    (1000)    11448 2023-02-13 14:51:00.252596 msapy-1.2.1/PKG-INFO
-drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-02-13 14:51:00.252596 msapy-1.2.1/msapy/
--rw-rw-r--   0 kayson    (1000) kayson    (1000)       68 2023-02-13 14:50:52.000000 msapy-1.2.1/msapy/__init__.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     4423 2023-02-13 13:04:08.000000 msapy-1.2.1/msapy/checks.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     3491 2023-02-13 14:48:52.000000 msapy-1.2.1/msapy/datastructures.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)    50135 2023-02-13 14:48:52.000000 msapy-1.2.1/msapy/msa.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     3248 2022-03-30 13:09:51.000000 msapy-1.2.1/msapy/plottings.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)    13913 2022-08-09 14:21:40.000000 msapy-1.2.1/msapy/utils.py
-drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-02-13 14:51:00.252596 msapy-1.2.1/msapy.egg-info/
--rw-rw-r--   0 kayson    (1000) kayson    (1000)    11448 2023-02-13 14:51:00.000000 msapy-1.2.1/msapy.egg-info/PKG-INFO
--rw-rw-r--   0 kayson    (1000) kayson    (1000)      442 2023-02-13 14:51:00.000000 msapy-1.2.1/msapy.egg-info/SOURCES.txt
--rw-rw-r--   0 kayson    (1000) kayson    (1000)        1 2023-02-13 14:51:00.000000 msapy-1.2.1/msapy.egg-info/dependency_links.txt
--rw-rw-r--   0 kayson    (1000) kayson    (1000)      155 2023-02-13 14:51:00.000000 msapy-1.2.1/msapy.egg-info/requires.txt
--rw-rw-r--   0 kayson    (1000) kayson    (1000)       12 2023-02-13 14:51:00.000000 msapy-1.2.1/msapy.egg-info/top_level.txt
--rw-rw-r--   0 kayson    (1000) kayson    (1000)       38 2023-02-13 14:51:00.252596 msapy-1.2.1/setup.cfg
--rw-rw-r--   0 kayson    (1000) kayson    (1000)      992 2023-02-13 14:48:52.000000 msapy-1.2.1/setup.py
-drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-02-13 14:51:00.252596 msapy-1.2.1/tests/
--rw-rw-r--   0 kayson    (1000) kayson    (1000)        0 2021-10-28 15:26:21.000000 msapy-1.2.1/tests/__init__.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     2125 2022-08-09 14:21:40.000000 msapy-1.2.1/tests/test_bad_inputs.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     3747 2023-02-13 13:04:08.000000 msapy-1.2.1/tests/test_ground_truth.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     1660 2023-02-13 13:04:08.000000 msapy-1.2.1/tests/test_ground_truth_multiscores.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     1334 2023-02-13 13:04:08.000000 msapy-1.2.1/tests/test_ground_truth_nd.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     2856 2023-02-13 13:04:08.000000 msapy-1.2.1/tests/test_ground_truth_timeseries.py
+drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-05-17 10:52:23.025582 msapy-1.3/
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     1069 2021-10-28 14:21:00.000000 msapy-1.3/LICENSE
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)    11446 2023-05-17 10:52:23.025582 msapy-1.3/PKG-INFO
+drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-05-17 10:52:23.021582 msapy-1.3/msapy/
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)       66 2023-05-17 10:42:09.000000 msapy-1.3/msapy/__init__.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     4423 2023-02-13 13:04:08.000000 msapy-1.3/msapy/checks.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     3630 2023-05-17 10:42:09.000000 msapy-1.3/msapy/datastructures.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)    51816 2023-05-17 10:42:09.000000 msapy-1.3/msapy/msa.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     3248 2022-03-30 13:09:51.000000 msapy-1.3/msapy/plottings.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)    14020 2023-05-17 10:42:09.000000 msapy-1.3/msapy/utils.py
+drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-05-17 10:52:23.025582 msapy-1.3/msapy.egg-info/
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)    11446 2023-05-17 10:52:22.000000 msapy-1.3/msapy.egg-info/PKG-INFO
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)      442 2023-05-17 10:52:22.000000 msapy-1.3/msapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)        1 2023-05-17 10:52:22.000000 msapy-1.3/msapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)      180 2023-05-17 10:52:22.000000 msapy-1.3/msapy.egg-info/requires.txt
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)       12 2023-05-17 10:52:22.000000 msapy-1.3/msapy.egg-info/top_level.txt
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)       38 2023-05-17 10:52:23.025582 msapy-1.3/setup.cfg
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)      990 2023-05-17 10:42:09.000000 msapy-1.3/setup.py
+drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-05-17 10:52:23.025582 msapy-1.3/tests/
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)        0 2021-10-28 15:26:21.000000 msapy-1.3/tests/__init__.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     2125 2022-08-09 14:21:40.000000 msapy-1.3/tests/test_bad_inputs.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     3747 2023-02-13 13:04:08.000000 msapy-1.3/tests/test_ground_truth.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     1660 2023-02-13 13:04:08.000000 msapy-1.3/tests/test_ground_truth_multiscores.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     1334 2023-02-13 13:04:08.000000 msapy-1.3/tests/test_ground_truth_nd.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     2856 2023-02-13 13:04:08.000000 msapy-1.3/tests/test_ground_truth_timeseries.py
```

### Comparing `msapy-1.2.1/LICENSE` & `msapy-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msapy-1.2.1/PKG-INFO` & `msapy-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msapy
-Version: 1.2.1
+Version: 1.3
 Summary: Multi-perturbation Shapley value Analysis (MSA)
 Home-page: https://github.com/kuffmode/msa
 Author: Kayson Fakhar, Shrey Dixit
 Author-email: kayson.fakhar@gmail.com, shrey.akshaj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `msapy-1.2.1/msapy/checks.py` & `msapy-1.3/msapy/checks.py`

 * *Files identical despite different names*

### Comparing `msapy-1.2.1/msapy/datastructures.py` & `msapy-1.3/msapy/datastructures.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import cached_property
 from typing import Optional
 from msapy import utils as ut, plottings as pl
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 
+#TODO: Update Code To Use Custom Accessors Instead: https://pandas.pydata.org/docs/development/extending.html#registering-custom-accessors
 
 class ShapleyTable(pd.DataFrame):
     @property
     def _constructor(self):
         return ShapleyTable
 
     @property
@@ -112,8 +113,8 @@
     def _constructor(self):
         return ShapleyModeND
 
     def get_shapley_mode(self, element):
         return self[element].values.reshape(self._shape)
 
     def get_total_contributions(self):
-        return self.sum(1).values.reshape(self._shape)
+        return self.values.sum(1).reshape(self._shape)
```

### Comparing `msapy-1.2.1/msapy/msa.py` & `msapy-1.3/msapy/msa.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from joblib import Parallel, delayed
 import numpy as np
 import pandas as pd
 from ordered_set import OrderedSet
 from itertools import combinations
 from typeguard import typechecked
 from tqdm import tqdm
+from fastprogress.fastprogress import master_bar, progress_bar, MasterBar
+from tqdm_joblib import tqdm_joblib
 
 from msapy import utils as ut
 from msapy.checks import _check_get_shapley_table_args, _check_valid_combination_space, _check_valid_elements, _check_valid_n_permutations, _check_valid_permutation_space, _get_contribution_type, _is_number
 from msapy.datastructures import ShapleyModeND, ShapleyTable, ShapleyTableMultiScores, ShapleyTableTimeSeries
 
 
 @typechecked
@@ -192,15 +194,16 @@
 
 @typechecked
 def take_contributions(*,
                        elements: list,
                        complement_space: OrderedSet,
                        combination_space: OrderedSet,
                        objective_function: Callable,
-                       objective_function_params: Optional[Dict] = None) -> Tuple[Dict, Dict]:
+                       objective_function_params: Optional[Dict] = None,
+                       mbar: Optional[MasterBar] = None) -> Tuple[Dict, Dict]:
     """
     This function fills up the combination_space with the game you define (objective function). There is an important
     point to keep in mind, Shapley values are the added contributions of elements while in MSA we calculate them by
     perturbation so although it's intuitive to think the combination in combination space is the element that will be
     lesioned, it is not the case, it will be everything else but the coalition, i.e., the target coalition are the
     only intact elements. This function takes care of this by passing the complement of each coalition to the
     game while assigning the results to the target coalition, just keep the logic in mind.
@@ -269,30 +272,32 @@
         warnings.warn("Are you sure you're not mistaking complement and combination spaces?"
                       "Length of the first element in complement space (really, complement_space[1]) is 0. "
                       "It should be equal to the number of elements.",
                       stacklevel=2)
     # ------------------------------#
 
     # run the objective function over all complement space
-    for combination, complement in tqdm(zip(combination_space, complement_space)):
+    for combination, complement in progress_bar(zip(combination_space, complement_space), parent=mbar, total=len(combination_space), leave=False):
         result = objective_function(complement, **objective_function_params)
 
         contributions[combination] = result
         lesion_effects[complement] = result
     return contributions, lesion_effects
 
 
 @typechecked
 def get_shapley_table(*,
                       permutation_space: list,
                       contributions: Optional[Dict] = None,
                       lesioned: Optional[any] = None,
                       objective_function: Optional[Callable] = None,
                       objective_function_params: Optional[Dict] = None,
-                      lazy=False) -> pd.DataFrame:
+                      lazy=False,
+                      dual_progress_bars: bool=True,
+                      mbar: Optional[MasterBar] = None,) -> pd.DataFrame:
     """
     Calculates Shapley values based on the filled contribution_space.
     Briefly, for a permutation (A,B,C) it will be:
 
     (A,B,C) - (B,C) = Contribution of A to the coalition (B,C).
     (B,C) - (C) = Contribution of B to the coalition formed with (C).
     (C) = Contribution of C alone.
@@ -331,19 +336,27 @@
         scores = list(arbitrary_contrib.keys())
         contributions = {k: np.array(list(v.values()))
                          for k, v in contributions.items()}
 
     lesioned = set(lesioned) if lesioned else set()
     shapley_table = {} if contribution_type != 'nd' else 0
 
-    for i, permutation in tqdm(enumerate(set(permutation_space)), total=len(permutation_space)):
-        isolated_contributions = []  # got to be a better way!
+    if not lazy:
+        parent_bar = enumerate(set(permutation_space))
+    elif (not dual_progress_bars) or mbar:
+        parent_bar = progress_bar(enumerate(set(permutation_space)), total=len(permutation_space), leave=False, parent=mbar)
+    elif lazy:
+        parent_bar = master_bar(enumerate(set(permutation_space)), total=len(permutation_space))
+        
 
+    for i, permutation in parent_bar:
+        isolated_contributions = []  # got to be a better way!
+        child_bar = enumerate(permutation) if not (dual_progress_bars and lazy) else progress_bar(enumerate(permutation), total=len(permutation), leave=False, parent=parent_bar)
         # iterate over all elements in the permutation to calculate their isolated contributions
-        for index, _ in tqdm(enumerate(permutation), leave=bool(i == 2), total=len(permutation)):
+        for index, _ in child_bar:
             including = frozenset(permutation[:index + 1]) - lesioned
             excluding = frozenset(permutation[:index]) - lesioned
 
             # the isolated contribution of an element is the difference of contribution with that element and without that element
             if lazy:
                 contributions_including = objective_function(tuple(excluding), **objective_function_params)
                 contributions_excluding = objective_function(tuple(including), **objective_function_params)
@@ -398,14 +411,16 @@
               pair: Optional[Tuple] = None,
               lesioned: Optional[any] = None,
               multiprocessing_method: str = 'joblib',
               rng: Optional[np.random.Generator] = None,
               random_seed: Optional[int] = None,
               n_parallel_games: int = -1,
               lazy: bool = True,
+              dual_progress_bars: bool=True,
+              mbar: Optional[MasterBar] = None
               ) -> Tuple[pd.DataFrame, Dict, Dict]:
     """
     A wrapper function to call other related functions internally and produces an easy-to-use pipeline.
 
     Args:
         n_permutations (int):
             Number of permutations (samples) per element.
@@ -466,15 +481,15 @@
                 - ray: 65 sec
 
             That makes sense since I have 16 cores and 1000/16 is around 62.
 
         rng (Optional[np.random.Generator]): Numpy random generator object used for reproducable results. Default is None.
 
         random_seed (Optional[int]):
-            sets the random seed of the sampling process. Only used when `rng` is None. Default is None.
+            sets the random seed of tdual_progress_bars=dual_progress_bars,he sampling process. Only used when `rng` is None. Default is None.
 
         n_parallel_games (int):
             Number of parallel jobs (number of to-be-occupied cores),
             -1 means all CPU cores and 1 means a serial process.
             I suggest using 1 for debugging since things get messy in parallel!
 
     Returns:
@@ -502,15 +517,17 @@
                       stacklevel=2)
 
     if lazy:
         shapley_table = get_shapley_table(permutation_space=permutation_space,
                                           lesioned=lesioned,
                                           lazy=True,
                                           objective_function=objective_function,
-                                          objective_function_params=objective_function_params)[elements]
+                                          objective_function_params=objective_function_params,
+                                          dual_progress_bars=dual_progress_bars,
+                                          mbar=mbar)[elements]
         return shapley_table, {}, {}
 
 
     combination_space = make_combination_space(permutation_space=permutation_space,
                                                 pair=pair,
                                                 lesioned=lesioned)
     complement_space = make_complement_space(combination_space=combination_space,
@@ -518,27 +535,30 @@
                                                 lesioned=lesioned)
 
     if n_parallel_games == 1:
         contributions, lesion_effects = take_contributions(elements=elements,
                                                            complement_space=complement_space,
                                                            combination_space=combination_space,
                                                            objective_function=objective_function,
-                                                           objective_function_params=objective_function_params)
+                                                           objective_function_params=objective_function_params,
+                                                           mbar=mbar)
     else:
         contributions, lesion_effects = ut.parallelized_take_contributions(
             multiprocessing_method=multiprocessing_method,
             n_cores=n_parallel_games,
             complement_space=complement_space,
             combination_space=combination_space,
             objective_function=objective_function,
-            objective_function_params=objective_function_params)
+            objective_function_params=objective_function_params,
+            mbar=mbar)
 
     shapley_table = get_shapley_table(contributions=contributions,
                                       permutation_space=permutation_space,
-                                      lesioned=lesioned)[elements]
+                                      dual_progress_bars=dual_progress_bars,
+                                      lesioned=lesioned, mbar=mbar)[elements]
     return shapley_table, contributions, lesion_effects
 
 
 @typechecked
 def interaction_2d(*,
                    n_permutations: int,
                    elements: list,
@@ -795,15 +815,16 @@
                                objective_function: Callable,
                                objective_function_params: Optional[dict] = None,
                                target_elements: Optional[list] = None,
                                multiprocessing_method: str = 'joblib',
                                n_cores: int = -1,
                                n_permutations: int = 1000,
                                permutation_seed: Optional[int] = None,
-                               parallelize_over_games=False
+                               parallelize_over_games=False,
+                               lazy=True
                                ) -> pd.DataFrame:
     """
     Estimates the causal contribution (Shapley values) of each node on the rest of the network. Basically, this function
     performs MSA iteratively on each node and tracks the changes in the objective_function of the target node.
     For example we have a chain A -> B -> C, and we want to know how much A and B are contributing to C. We first need to
     define a metric for C (objective_function) which here let's say is the average activity of C. MSA then performs a
     multi-site lesioning analysis of A and B so for each we will end up with a number indicating their contributions to
@@ -890,21 +911,21 @@
     Returns:
         causal_influences (pd.DataFrame)
 
     """
     target_elements = target_elements if target_elements else elements
     objective_function_params = objective_function_params if objective_function_params else {}
 
-    # run causal_influence_single_element for all target elements.
-
     if parallelize_over_games:
+        # run causal_influence_single_element for all target elements.
+        mbar = master_bar(enumerate(target_elements), total=len(target_elements))
         results = [causal_influence_single_element(elements, objective_function,
                                                    objective_function_params, n_permutations,
                                                    n_cores, multiprocessing_method,
-                                                   permutation_seed, index, element) for index, element in tqdm(enumerate(target_elements))]
+                                                   permutation_seed, index, element, lazy, mbar) for index, element in mbar]
 
     elif multiprocessing_method == 'ray':
         if importlib.util.find_spec("ray") is None:
             raise ImportError(
                 "The ray package is required to run this algorithm. Install and use at your own risk.")
 
         import ray
@@ -915,40 +936,46 @@
             ray.init()
         else:
             ray.init(num_cpus=n_cores)
 
         result_ids = [ray.remote(causal_influence_single_element).remote(elements, objective_function,
                                                                          objective_function_params, n_permutations,
                                                                          1, 'joblib',
-                                                                         permutation_seed, index, element) for index, element in enumerate(target_elements)]
+                                                                         permutation_seed, index, element, lazy, None) for index, element in enumerate(target_elements)]
 
         for _ in tqdm(ut.ray_iterator(result_ids), total=len(result_ids)):
             pass
 
         results = ray.get(result_ids)
         ray.shutdown()
 
     else:
-        results = (Parallel(n_jobs=n_cores)(delayed(causal_influence_single_element)(elements, objective_function,
+        with tqdm_joblib(desc="Doing Nodes: ", total=len(target_elements)) as pb:
+            results = (Parallel(n_jobs=n_cores)(delayed(causal_influence_single_element)(elements, objective_function,
                                                                                      objective_function_params, n_permutations,
                                                                                      1, 'joblib',
-                                                                                     permutation_seed, index, element) for index, element in tqdm(enumerate(target_elements))))
+                                                                                     permutation_seed, index, element, lazy) for index, element in enumerate(target_elements)))
 
     _, contribution_type = results[0]
     shapley_values = [r[0] for r in results]
 
     causal_influences = pd.DataFrame(
         shapley_values, columns=elements) if contribution_type == "scaler" else pd.concat(shapley_values, keys=elements)
-    return causal_influences.swaplevel().sort_index(level=0) if contribution_type == "multi_scores" else causal_influences
+    
+    if contribution_type == "scaler":
+        return causal_influences
+    if contribution_type == "multi_scores":
+        return causal_influences.swaplevel().sort_index(level=0) 
+    return causal_influences[causal_influences.index.levels[0]]
 
 
 def causal_influence_single_element(elements, objective_function,
                                     objective_function_params, n_permutations,
                                     n_parallel_games, multiprocessing_method,
-                                    permutation_seed, index, element):
+                                    permutation_seed, index, element, lazy=True, mbar=None):
     """
     Estimates the causal contribution (Shapley values) of a node on the rest of the network. Basically, this function
     performs MSA and tracks the changes in the objective_function of the target node.
 
     Args:
         elements (list):
             List of the players (elements). Can be strings (names), integers (indicies), and tuples.
@@ -1007,24 +1034,26 @@
     Returns:
         causal_influences (pd.DataFrame)
         multi_scores (bool)
         is_timeseries (bool)
 
     """
 
-    print(f"working on node number {index} from {len(elements)} nodes.")
     objective_function_params['index'] = index
 
     # Takes the target out of the to_be_lesioned list
     without_target = set(elements).difference({element})
 
     shapley_output, _, _ = interface(n_permutations=n_permutations,
                                                 elements=list(without_target),
+                                                dual_progress_bars= False,
                                                 objective_function=objective_function,
                                                 objective_function_params=objective_function_params,
                                                 n_parallel_games=n_parallel_games,
                                                 multiprocessing_method=multiprocessing_method,
-                                                random_seed=permutation_seed)
+                                                random_seed=permutation_seed,
+                                                lazy=lazy,
+                                                mbar=mbar)
 
     if shapley_output.contribution_type in ("scaler", "multi_scores"):
         return shapley_output.shapley_values, shapley_output.contribution_type
     return shapley_output.shapley_modes, shapley_output.contribution_type
```

### Comparing `msapy-1.2.1/msapy/plottings.py` & `msapy-1.3/msapy/plottings.py`

 * *Files identical despite different names*

### Comparing `msapy-1.2.1/msapy/utils.py` & `msapy-1.3/msapy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import gc
 import importlib
 import warnings
 from typing import Any, Generator, Iterable, Callable, Optional, Dict, Tuple
+from fastprogress import progress_bar
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel, delayed
 from joblib.externals.loky import get_reusable_executor
 from ordered_set import OrderedSet
 from tqdm import tqdm
@@ -25,15 +26,16 @@
 @typechecked
 def parallelized_take_contributions(*,
                                     multiprocessing_method: str = 'joblib',
                                     n_cores: int = -1,
                                     complement_space: OrderedSet,
                                     combination_space: OrderedSet,
                                     objective_function: Callable,
-                                    objective_function_params: Optional[Dict] = None) -> Tuple[Dict, Dict]:
+                                    objective_function_params: Optional[Dict] = None,
+                                    mbar=None) -> Tuple[Dict, Dict]:
     """
     Same as the take_contribution function but parallelized over CPU cores to boost performance.
     I'd first try the single msapy version on a toy example to make sure everything makes sense then
     go for this because debugging parallel jobs is a disaster. Also, you don't need this if your game
     is happening on GPU. For HPC systems, I guess either dask or ray will be better options.
     ---------------
     Note on returns:
@@ -105,14 +107,15 @@
 
     Returns:
         (Tuple[Dict, Dict]): 
             - contributions: A dictionary of coalitions:results
             - lesion_effects: A dictionary of lesions:results
     """
     objective_function_params = objective_function_params if objective_function_params else {}
+    cbar = progress_bar(complement_space, total=len(complement_space), parent=mbar, leave=False)
 
     if len(complement_space.items[0]) == 1:
         warnings.warn("Are you sure you're not mistaking complement and combination spaces?"
                       "Length of the first element in complement space is 1, that is usually n_elements-1",
                       stacklevel=2)
     if multiprocessing_method == 'ray':
         if importlib.util.find_spec("ray") is None:
@@ -135,15 +138,15 @@
             pass
 
         results = ray.get(result_ids)
         ray.shutdown()
 
     elif multiprocessing_method == 'joblib':
         results = (Parallel(n_jobs=n_cores)(delayed(objective_function)(
-            complement, **objective_function_params) for complement in tqdm(complement_space, total=len(complement_space), desc='Playing the games: ')))
+            complement, **objective_function_params) for complement in cbar))
     else:
         raise NotImplemented("Available multiprocessing backends are 'ray' and 'joblib'")
 
     contributions = dict(zip(combination_space, results))
     lesion_effects = dict(zip(complement_space, results))
 
     gc.collect()
```

### Comparing `msapy-1.2.1/msapy.egg-info/PKG-INFO` & `msapy-1.3/msapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msapy
-Version: 1.2.1
+Version: 1.3
 Summary: Multi-perturbation Shapley value Analysis (MSA)
 Home-page: https://github.com/kuffmode/msa
 Author: Kayson Fakhar, Shrey Dixit
 Author-email: kayson.fakhar@gmail.com, shrey.akshaj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `msapy-1.2.1/setup.py` & `msapy-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("requirements.txt", "r") as f:
     base_packages = f.read().split("\n")
 
 test_packages = ["pytest~=6.2.5"]
 
 setup(name="msapy",
-      version="1.2.1",
+      version="1.3",
       description=DESCRIPTION,
       long_description=LONG_DESCRIPTION,
       long_description_content_type='text/markdown',
       author='Kayson Fakhar, Shrey Dixit',
       author_email='kayson.fakhar@gmail.com, shrey.akshaj@gmail.com',
       url="https://github.com/kuffmode/msa",
       packages=find_packages(),
```

### Comparing `msapy-1.2.1/tests/test_bad_inputs.py` & `msapy-1.3/tests/test_bad_inputs.py`

 * *Files identical despite different names*

### Comparing `msapy-1.2.1/tests/test_ground_truth.py` & `msapy-1.3/tests/test_ground_truth.py`

 * *Files identical despite different names*

### Comparing `msapy-1.2.1/tests/test_ground_truth_multiscores.py` & `msapy-1.3/tests/test_ground_truth_multiscores.py`

 * *Files identical despite different names*

### Comparing `msapy-1.2.1/tests/test_ground_truth_nd.py` & `msapy-1.3/tests/test_ground_truth_nd.py`

 * *Files identical despite different names*

### Comparing `msapy-1.2.1/tests/test_ground_truth_timeseries.py` & `msapy-1.3/tests/test_ground_truth_timeseries.py`

 * *Files identical despite different names*


# Comparing `tmp/AutoCarver-4.1.0.tar.gz` & `tmp/AutoCarver-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AutoCarver-4.1.0.tar", last modified: Mon May 15 17:51:59 2023, max compression
+gzip compressed data, was "dist\AutoCarver-4.2.0.tar", last modified: Wed May 17 09:52:51 2023, max compression
```

## Comparing `AutoCarver-4.1.0.tar` & `AutoCarver-4.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 17:51:59.000000 AutoCarver-4.1.0/
-drwxrwxrwx   0        0        0        0 2023-05-15 17:51:59.000000 AutoCarver-4.1.0/AutoCarver/
--rw-rw-rw-   0        0        0    22860 2023-05-15 17:49:41.000000 AutoCarver-4.1.0/AutoCarver/AutoCarver.py
--rw-rw-rw-   0        0        0    51141 2023-05-15 17:25:48.000000 AutoCarver-4.1.0/AutoCarver/Discretizers.py
--rw-rw-rw-   0        0        0    16742 2023-05-15 07:01:19.000000 AutoCarver-4.1.0/AutoCarver/FeatureSelector.py
--rw-rw-rw-   0        0        0        0 2023-01-10 08:49:10.000000 AutoCarver-4.1.0/AutoCarver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:51:59.000000 AutoCarver-4.1.0/AutoCarver.egg-info/
--rw-rw-rw-   0        0        0     7119 2023-05-15 17:51:52.000000 AutoCarver-4.1.0/AutoCarver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-05-15 17:51:57.000000 AutoCarver-4.1.0/AutoCarver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 17:51:52.000000 AutoCarver-4.1.0/AutoCarver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 17:51:52.000000 AutoCarver-4.1.0/AutoCarver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-01-05 13:13:13.000000 AutoCarver-4.1.0/LICENSE
--rw-rw-rw-   0        0        0     7119 2023-05-15 17:51:59.000000 AutoCarver-4.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6346 2023-05-14 13:54:01.000000 AutoCarver-4.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 17:51:59.000000 AutoCarver-4.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-15 17:20:11.000000 AutoCarver-4.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:52:51.000000 AutoCarver-4.2.0/
+drwxrwxrwx   0        0        0        0 2023-05-17 09:52:51.000000 AutoCarver-4.2.0/AutoCarver/
+-rw-rw-rw-   0        0        0    23090 2023-05-17 08:09:57.000000 AutoCarver-4.2.0/AutoCarver/AutoCarver.py
+-rw-rw-rw-   0        0        0     4687 2023-05-17 07:51:12.000000 AutoCarver-4.2.0/AutoCarver/Converters.py
+-rw-rw-rw-   0        0        0    50777 2023-05-17 09:48:49.000000 AutoCarver-4.2.0/AutoCarver/Discretizers.py
+-rw-rw-rw-   0        0        0    23882 2023-05-17 09:47:05.000000 AutoCarver-4.2.0/AutoCarver/FeatureSelector.py
+-rw-rw-rw-   0        0        0        0 2023-01-10 08:49:10.000000 AutoCarver-4.2.0/AutoCarver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:52:51.000000 AutoCarver-4.2.0/AutoCarver.egg-info/
+-rw-rw-rw-   0        0        0     7119 2023-05-17 09:52:44.000000 AutoCarver-4.2.0/AutoCarver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-17 09:52:49.000000 AutoCarver-4.2.0/AutoCarver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 09:52:44.000000 AutoCarver-4.2.0/AutoCarver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-17 09:52:44.000000 AutoCarver-4.2.0/AutoCarver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-01-05 13:13:13.000000 AutoCarver-4.2.0/LICENSE
+-rw-rw-rw-   0        0        0     7119 2023-05-17 09:52:51.000000 AutoCarver-4.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6346 2023-05-14 13:54:01.000000 AutoCarver-4.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 09:52:51.000000 AutoCarver-4.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-17 09:50:35.000000 AutoCarver-4.2.0/setup.py
```

### Comparing `AutoCarver-4.1.0/AutoCarver/AutoCarver.py` & `AutoCarver-4.2.0/AutoCarver/AutoCarver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .Discretizers import GroupedList, GroupedListDiscretizer, is_equal
+from Discretizers import GroupedList, GroupedListDiscretizer, is_equal
 from IPython.display import display_html
 from matplotlib.pyplot import subplots, show
 from matplotlib.ticker import PercentFormatter
 from numpy import sort, nan, inf, float32, where, isin, argsort, array, append, quantile, linspace, argmin, sqrt, random
 from pandas import DataFrame, Series, isna, qcut, notna, unique, concat, crosstab
 from pandas.api.types import is_string_dtype
 from scipy.stats import chi2_contingency
@@ -93,29 +93,30 @@
     # applying pipe to a validation set or in production
     X_val = pipe.transform(X_val)
 
     """
    
     def __init__(self, values_orders: Dict[str, Any], *, sort_by: str='tschuprowt',
                  copy: bool=False, max_n_mod: int=5, dropna: bool=True,
-                 verbose: bool=True) -> None:
+                 verbose: bool=True, str_nan: str='__NAN__') -> None:
         
         self.features = list(values_orders.keys())
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.non_viable_features: List[str] = []  # list of features non viable features
         self.max_n_mod = max_n_mod  # maximum number of modality per feature
         self.dropna = dropna  # whether or not to group NaNs with other modalities
         
         # association measure used to find the best groups
         implemented = ['tschuprowt', 'cramerv']
         assert sort_by in implemented, f"Measure {sort_by} is not yet implemented. Choose from: {', '.join(implemented)}."
         self.sort_by = sort_by
 
         self.copy = copy
         self.verbose = verbose
+        self.str_nan = str_nan
     
     def prepare_data(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Tuple[DataFrame, Series, DataFrame, Series]:
         """ Checks validity of provided data"""
         
         # preparing train sample
         # checking for binary target
         y_values = unique(y)
@@ -168,60 +169,60 @@
             best_groups = self.get_best_combination(feature, Xc, y, Xtestc, y_test)
 
             # feature can not be carved robustly
             if not bool(best_groups):
                 self.non_viable_features += [feature]  # adding it to list of non viable features
 
         # discretizing features based on each feature's values_order
-        super().__init__(self.values_orders, copy=self.copy, output=float)
+        super().__init__(self.values_orders, str_nan=self.str_nan, copy=self.copy, output=float)
         super().fit(X, y)
 
         return self
 
     def get_best_combination(self, feature: str, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Dict[str, Any]:
 
-        # getting all possible combinations for the feature without NaNS
-        combinations = get_all_combinations(self.values_orders.get(feature), X[feature].nunique(dropna=True), self.max_n_mod)
-        combinations = [GroupedList({group[0]: group for group in combination}) for combination in combinations]
-
         # computing crosstabs
         # crosstab on TRAIN
-        xtab = nan_crosstab(X[feature], y)
+        xtab = nan_crosstab(X[feature], y, self.str_nan)
+        notna_xtab = xtab[xtab.index != self.str_nan]  # filtering out nans
+
         # crosstab on TEST
-        xtab_test = None
+        xtab_test, notna_xtab_test = None, None
         if X_test is not None:
-            xtab_test = nan_crosstab(X_test[feature], y_test)
+            xtab_test = nan_crosstab(X_test[feature], y_test, self.str_nan)
+            notna_xtab_test = xtab_test[xtab_test.index != self.str_nan]  # filtering out nans
 
         # printing the group statistics
         if self.verbose:
             self.display_xtabs(feature, 'Raw', xtab, xtab_test)
-            
-        # filtering out nans
-        notna_xtab = xtab[notna(xtab.index)]
-        notna_xtab_test = None
-        if xtab_test is not None:
-            notna_xtab_test = xtab_test[notna(xtab_test.index)]
+
+        # getting all possible combinations for the feature without NaNS
+        combinations = get_all_combinations(self.values_orders.get(feature), self.max_n_mod)
 
         # measuring association with target for each combination and testing for stability on TEST
         best_groups = best_combination(combinations, self.sort_by, notna_xtab, notna_xtab_test)
 
         # update of the values_orders grouped modalities in values_orders
         if best_groups:
             xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
 
         # testing adding NaNs to built groups
         order = self.values_orders.get(feature)
-        if any(isna(X[feature])) & self.dropna & (len(order) <= self.max_n_mod) & (len(order)>1):
+        if (self.str_nan in xtab.index) & self.dropna:
 
-            # getting all possible combinations for the feature with NaNS
-            combinations = get_all_nan_combinations(order)
-            combinations = [GroupedList({group[0]: group for group in combination}) for combination in combinations]
-            
             # adding nans at the end of the order
-            order.append(nan)
+            order = order.append(self.str_nan)
+
+            # reordering order according to target rate
+            new_order = xtab[1].divide(xtab.sum(axis=1)).sort_values().index.tolist()
+            order = order.sort_by(new_order)
+            self.values_orders.update({feature: order})
+
+            # getting all possible combinations for the feature without NaNS
+            combinations = get_all_combinations(order, self.max_n_mod)
 
             # measuring association with target for each combination and testing for stability on TEST
             best_groups = best_combination(combinations, self.sort_by, xtab, xtab_test)
 
             # update of the values_orders grouped modalities in values_orders
             if best_groups:
                 xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
@@ -231,20 +232,16 @@
             self.display_xtabs(feature, 'Fitted', xtab, xtab_test)
 
         return best_groups
 
     def update_order(self, feature: str, best_groups: GroupedList, xtab: DataFrame, xtab_test: DataFrame=None) -> Tuple[DataFrame, DataFrame]:
         """ Updates the values_orders and xtabs according to the best_groups"""
 
-        # accessing current order for specified feature
-        order = self.values_orders.get(feature)
-
-        # grouping for each group of the combination
-        for kept, discarded in best_groups.contained.items():
-            order.group_list(discarded, kept)
+        # updating values_orders with best_combination 
+        self.values_orders.update({feature: best_groups})
 
         # update of the TRAIN crosstab
         best_combi = list(map(best_groups.get_group, xtab.index))
         xtab = xtab.groupby(best_combi, dropna=False).sum()
 
         # update of the TEST crosstab
         if xtab_test is not None:
@@ -282,23 +279,32 @@
             test_style = test_style.set_table_attributes("style='display:inline'")  # printing in notebook
             test_style = test_style.set_caption(f'{caption} distribution on X_test:')  # title
             html += ' ' + test_style._repr_html_()
 
         # displaying html of colored DataFrame
         display_html(html, raw=True)
 
+def groupedlist_combination(combination: List[List[Any]], order: GroupedList) -> GroupedList:
+    """ Converts a list of combination to a GroupedList"""
+    
+    order_copy = GroupedList(order)
+    for combi in combination:
+        order_copy.group_list(combi, combi[0])
+    
+    return order_copy
+
 def stats_xtab(xtab: DataFrame, known_order: List[Any]=None, known_labels: List[Any]=None) -> DataFrame:
     """ Computes column (target) rate per row (modality) and row frequency"""
     
     # target rate and frequency statistics per modality
     stats = DataFrame({
         # target rate per modality
-        'target_rate': xtab[1].divide(xtab[0].add(xtab[1])),
+        'target_rate': xtab[1].divide(xtab.sum(axis=1)),
         # frequency per modality
-        'frequency': xtab[1].add(xtab[0]) / xtab.sum().sum()
+        'frequency': xtab.sum(axis=1) / xtab.sum().sum()
     })
     
     # sorting statistics
     # case 0: default ordering based on observed target rate
     if known_order is None:
         order = list(stats.sort_values('target_rate', ascending=True).index)
     
@@ -396,26 +402,30 @@
             if viability:
 
                 association.update({'combi_xtab_test': combi_xtab_test})
 
                 return association
 
 
-def get_all_combinations(values: list, q: int, max_n_mod: int=None):
+def get_all_combinations(values: GroupedList, max_n_mod: int=None):
 
-    # max number of classes
+    # maximum number of classes
+    q = len(values)
+
+    # desired max number of classes
     if max_n_mod is None:
     	max_n_mod = q
 
     # all possible combinations
     combinations = list()
     for n_class in range(2, max_n_mod + 1):
         combinations += get_combinations(n_class, q)
 
     combinations = [[values[int(c[0]): int(c[1]) + 1] for c in combi] for combi in combinations]  # getting real feature values
+    combinations = [groupedlist_combination(combination, values) for combination in combinations]  # converting back to GroupedList
 
     return combinations
 
 def get_all_nan_combinations(order: List[Any]):
     """ all possible combinations of modalities with numpy.nan"""
 
     # computing all non-NaN combinations
@@ -511,26 +521,22 @@
     if dof_mods > 0:
         tschuprowt = sqrt(chi2 / n_obs / dof_mods)
 
     results = {'cramerv': cramerv, 'tschuprowt': tschuprowt}
     
     return results
 
-def nan_crosstab(x: Series, y: Series):
+def nan_crosstab(x: Series, y: Series, str_nan: str='__NAN__'):
     """ Crosstab that keeps nans as a specific value"""
     
     # keeping NaNs as a specific modality
-    nan_val = '__NAN__'  # value to be imputed as NaN
-    x_filled = x.fillna(nan_val)  # filling NaNs
+    x_filled = x.fillna(str_nan)  # filling NaNs
 
     # computing initial crosstabs
     xtab = crosstab(x_filled, y)
-
-    # keeping track of nans if there are any
-    xtab.index = [idx if idx != nan_val else nan for idx in xtab.index]
     
     return xtab
 
 
 def plot_stats(stats):
     """ Barplot of the volume and target rate"""
```

### Comparing `AutoCarver-4.1.0/AutoCarver/Discretizers.py` & `AutoCarver-4.2.0/AutoCarver/Discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,38 +17,38 @@
     
     return uniques
 
 class GroupedList(list):
     
     def __init__(self, iterable=()) -> None:
         """ An ordered list that historizes its elements' merges."""
-        
-        # case 0: iterable est le dictionnaire contained
+
+        # case 0: iterable is the contained dict
         if isinstance(iterable, dict):
             
             # récupération des valeurs de la liste (déjà ordonné)
-            values = [key for key, _ in iterable.items()]
+            values = [key for key in iterable]
 
             # initialsiation de la liste
             super().__init__(values)
 
             # attribution des valeurs contenues
             self.contained = {k: v for k, v in iterable.items()}
         
-        # case 1: s'il ne s'agit pas déjà d'une liste groupée -> création des groupes
-        elif isinstance(iterable, GroupedList):
+        # case 1: copying a GroupedList
+        elif hasattr(iterable, 'contained'):
 
             # initialsiation de la liste
             super().__init__(iterable)
 
             # copie des groupes
             self.contained = {k: v for k, v in iterable.contained.items()}
         
-        # case 2: il s'agit d'une GroupedList -> copie des groupes
-        else:
+        # case 2: initiating GroupedList from a list
+        elif isinstance(iterable, list):
 
             # initialsiation de la liste
             super().__init__(iterable)
 
             # création des groupes
             self.contained = {v: [v] for v in iterable}
 
@@ -57,27 +57,32 @@
 
         for discarded, kept in zip(to_discard, [to_keep] * len(to_discard)):
             self.group(discarded, kept)
 
     def group(self, discarded: Any, kept: Any) -> None:
         """ Groups the discarded value with the kept value"""
 
+        # checking that those values are distinct
         if not is_equal(discarded, kept):
 
+            # checking that those values exist in the list
             assert discarded in self, f"{discarded} not in list"
             assert kept in self, f"{kept} not in list"
 
+            # accessing values contained in each value
             contained_discarded = self.contained.get(discarded)
             contained_kept = self.contained.get(kept)
 
+            # updating contained dict
             self.contained.update({
                 kept: contained_discarded + contained_kept,
                 discarded: []
             })
 
+            # removing discarded from the list
             self.remove(discarded)
         
         return self
         
     def append(self, new_value: Any) -> None:
         """ Appends a new_value to the GroupedList"""
         
@@ -96,22 +101,26 @@
         # non-str values
         keys_float = [key for key in self if not isinstance(key, str)]
 
         # sorting and merging keys
         keys = list(sort(keys_str)) + list(sort(keys_float)) 
 
         # recreating an ordered GroupedList
-        self = GroupedList({key: self.get(key) for key in keys})
+        self = GroupedList({k: self.get(k) for k in keys})
 
         return self
 
     def sort_by(self, ordering: List[Any]) -> None:
         """ Sorts the values of the list and dict, if any, NaNs are the last. """
 
-        # recreating an ordered GroupedList
+        # checking that all values are given an order
+        assert all([o in self for o in ordering]), f"Unknown values in ordering: {', '.join([str(v) for v in ordering if v not in self])}"
+        assert all([s in ordering for s in self]), f"Missing value from ordering: {', '.join([str(v) for v in self if v not in ordering])}"
+
+        # ordering the contained
         self = GroupedList({k: self.get(k) for k in ordering})
 
         return self
 
     
     def remove(self, value: Any) -> None:
         
@@ -126,26 +135,28 @@
     def get(self, key: Any) -> List[Any]:
         """ returns list of values contained in key"""
 
         # default to fing an element
         found = self.contained.get(key)
 
         # copying with dictionnaries (not working with numpy.nan)
-        if isna(key):
-            found = [value for dict_key, value in self.contained.items() if is_equal(dict_key, key)][0]
+        # if isna(key):
+            # found = [value for dict_key, value in self.contained.items() if is_equal(dict_key, key)][0]
 
         return found
 
     def get_group(self, value: Any) -> Any:
         """ returns the group containing the specified value """
         
         found = [key for key, values in self.contained.items() if any(is_equal(value, elt) for elt in values)]
 
         if any(found):
             return found[0]
+        else:
+        	return value
 
     def values(self) -> List[Any]:
         """ returns all values contained in each group """
 
         known = [value for values in self.contained.values() for value in values]
 
         return known
@@ -164,15 +175,15 @@
         repr: List[str] = []
 
         # iterating over each group
         for group in self:
 
             # accessing group's values
             values = self.get(group)
-            
+
             if len(values) == 0:  # case 0: there are no value in this group
                 pass
             
             elif len(values) == 1:  # case 1: there is only one value in this group
                 repr += [values[0]]
             
             elif len(values) == 2:  # case 2: two values in this group
@@ -180,60 +191,70 @@
             
             elif len(values) > 2:  # case 3: more than two values in this group
                 repr += [f'{values[-1]}'[:char_limit]+' to '+f'{values[0]}'[:char_limit]]
                 
         return repr
 
 
-class StringConverter(BaseEstimator, TransformerMixin):
-    """ Converts specified columns a DataFrame into str
-    
-     - Keeps NaN inplace
-     - Converts floats of int to int
-
-    Parameters
-    ----------
-    features: list, default []
-        List of columns to be converted to string.
-    """
-    
-    def __init__(self, features: List[str]=[], copy: bool=False) -> None:
+class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
     
-        self.features = features[:]
-        self.copy = copy
+    def __init__(self, values_orders: Dict[str, Any], *, 
+    	copy: bool=False, output: type= float,
+    	str_nan: str=None, verbose: bool=False) -> None:
         
-    def fit(self, X: DataFrame, y: Series=None):
+        self.features = list(values_orders.keys())
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.copy = copy
+        self.output = output
+        self.verbose = verbose
+        self.str_nan = str_nan
         
+    def fit(self, X, y=None) -> None:
+
         return self
-        
+    
     def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
-        # copying DataFrame if requested
+
+        # copying dataframes
         Xc = X
         if self.copy:
             Xc = X.copy()
 
-        # storing nans
-        nans = isna(Xc[self.features])
+        # filling up nans with specified value
+        if self.str_nan:
+            Xc[self.features] = Xc[self.features].fillna(self.str_nan)
+
+        # iterating over each feature
+        for n, feature in enumerate(self.features):
+            
+            # verbose if requested
+            if self.verbose: 
+                print(f" - [GroupedListDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
+            
+            # bucketizing feature
+            order = self.values_orders.get(feature)  # récupération des groupes
+            to_discard = [order.get(group) for group in order]  # identification des valeur à regrouper
+            to_input = [Xc[feature].isin(discarded) for discarded in to_discard]  # identifying main bucket value
+            to_keep = [n if self.output == float else group for n, group in enumerate(order)]  # récupération du groupe dans lequel regrouper
+
+            # case when there are no values
+            if len(to_input)==0 & len(to_keep)==0:
+                pass
+
+            # grouping modalities
+            else:
+                Xc[feature] = select(to_input, to_keep, default=Xc[feature])
+
+        # converting to float
+        if self.output == float:
+            Xc[self.features] = Xc[self.features].astype(float16)
 
-        # storing ints
-        ints = Xc[self.features].applymap(lambda u: isinstance(u, float) and float.is_integer(u))
-        
-        # converting to string
-        Xc[self.features] = Xc[self.features].astype(str)
-        
-        # converting to int-strings
-        converted_ints = Xc[ints][self.features].applymap(lambda u: str(int(float(u))) if isinstance(u, str) else u)
-        Xc[self.features] = select([ints], [converted_ints], default=Xc[self.features])
-        
-        # converting back to nan
-        Xc[nans] = nan
-        
         return Xc
 
+
 class QualitativeDiscretizer(BaseEstimator, TransformerMixin):
     """ Automatic discretizing of categorical and categorical ordinal features.
 
     Modalities/values of features are grouped according to there respective orders:
      - [Qualitative features] order based on modality target rate.
      - [Qualitative ordinal features] user-specified order.
 
@@ -257,32 +278,31 @@
         (smallest frequency or closest target rate), between the superior and inferior values (described
         by the `values_orders`).
         Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
     """
     
     def __init__(self, features: List[str], min_freq: float, *,
                  values_orders: Dict[str, Any]={}, copy: bool=False, 
-                 verbose: bool=False, dropna: bool=False) -> None:
+                 verbose: bool=False) -> None:
     
         self.features = features[:]
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.ordinal_features = [f for f in values_orders if f in features]
+        self.ordinal_features = [f for f in values_orders if f in features]  # ignores non qualitative features
         self.non_ordinal_features = [f for f in features if f not in self.ordinal_features]
         self.min_freq = min_freq
         self.pipe: List[BaseEstimator] = []
         self.copy = copy
         self.verbose = verbose
-        self.dropna = dropna
         
     def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """ Checking data for bucketization"""
         
         # checking for quantitative columns
         is_object = X[self.features].dtypes.apply(is_string_dtype)
-        assert all(is_object), f"Non-string features: {', '.join(is_object[~is_object].index)}, consider using StringConverter."
+        assert all(is_object), f"Non-string features: {', '.join(is_object[~is_object].index)}, consider using Converters.StringConverter."
         
         # checking for binary target
         y_values = unique(y)
         assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
         assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
         
         # checking that all unique values in X are in values_orders
@@ -302,30 +322,31 @@
         # checking data before bucketization
         Xc = self.prepare_data(X, y)
 
         # [Qualitative ordinal features] Grouping rare values into closest common one
         if len(self.ordinal_features) > 0:
 
             # discretizing
-            ordinal_orders = {f: self.values_orders[f] for f in self.ordinal_features}
-            discretizer = ClosestDiscretizer(ordinal_orders, min_freq=self.min_freq, 
-                                             verbose=self.verbose)
+            ordinal_orders = {k: GroupedList(v) for k, v in self.values_orders.items() if k in self.ordinal_features}
+            discretizer = ClosestDiscretizer(
+                ordinal_orders, min_freq=self.min_freq, verbose=self.verbose
+            )
             discretizer.fit(Xc, y)
 
             # storing results
             self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
             self.pipe += [('QualitativeClosestDiscretizer', discretizer)]  # adding discretizer to pipe
 
         # [Qualitative non-ordinal features] Grouping rare values into default_value '__OTHER__'
         if len(self.non_ordinal_features) > 0:
 
             # Grouping rare modalities
             discretizer = DefaultDiscretizer(self.non_ordinal_features, min_freq=self.min_freq, 
                                              values_orders=self.values_orders,
-                                             verbose=self.verbose, dropna=self.dropna)
+                                             verbose=self.verbose)
             discretizer.fit(Xc, y)
 
             # storing results
             self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
             self.pipe += [('DefaultDiscretizer', discretizer)]  # adding discretizer to pipe
 
         return self
@@ -363,15 +384,15 @@
         Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be 
         cut in q=5 quantiles.
         Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
 
     """
     
     def __init__(self, features: List[str], q: int, *, values_orders: Dict[str, Any]={}, copy: bool=False, 
-                 verbose: bool=False, dropna: bool=False) -> None:
+                 verbose: bool=False) -> None:
         
         self.features = features[:]
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.q = q
         self.pipe: List[BaseEstimator] = []
         self.copy = copy
         self.verbose = verbose
@@ -484,42 +505,43 @@
         [Qualitative ordinal features] dict of features values and list of orders of their values.
          - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
         (smallest frequency or closest target rate), between the superior and inferior values (described
         by the `values_orders`).
         Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
     """
 
-    def __init__(self, quanti_features: List[str], quali_features: List[str], q: int, min_freq: float, *, 
-                 values_orders: Dict[str, Any]={}, copy: bool=False, verbose: bool=False, dropna: bool=False) -> None:
+    def __init__(self, quanti_features: List[str], quali_features: List[str], min_freq: float, *, 
+                 values_orders: Dict[str, Any]={}, copy: bool=False, verbose: bool=False) -> None:
 
         self.features = quanti_features[:] + quali_features[:]
         self.quanti_features = quanti_features[:]
+        assert len(list(set(quanti_features))) == len(quanti_features), "Column duplicates in quanti_features"
         self.quali_features = quali_features[:]
+        assert len(list(set(quali_features))) == len(quali_features), "Column duplicates in quali_features"
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.min_freq = min_freq
-        self.q = q
+        self.q = int(1 / min_freq)  # number of quantiles
         self.pipe: List[BaseEstimator] = []
         self.copy = copy
         self.verbose = verbose
-        self.dropna = dropna
 
     def fit(self, X: DataFrame, y: Series) -> None:
 
         # [Qualitative features] Grouping qualitative features
         if len(self.quali_features) > 0:
 
             # verbose if requested
             if self.verbose:
                 print("\n---\n[Discretizer] Fit Qualitative Features")
 
             # grouping qualitative features
             discretizer = QualitativeDiscretizer(
                 self.quali_features, min_freq=self.min_freq,
                 values_orders=self.values_orders, copy=self.copy,
-                verbose=self.verbose, dropna=self.dropna
+                verbose=self.verbose
             )
             discretizer.fit(X, y)
 
             # storing results
             self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
             self.pipe += discretizer.pipe  # adding discretizer to pipe
 
@@ -530,15 +552,15 @@
             if self.verbose:
                 print("\n---\n[Discretizer] Fit Quantitative Features")
 
             # grouping quantitative features
             discretizer = QuantitativeDiscretizer(
                 self.quanti_features, q=self.q,
                 values_orders=self.values_orders, copy=self.copy,
-                verbose=self.verbose, dropna=self.dropna
+                verbose=self.verbose
             )
             discretizer.fit(X, y)
 
             # storing results
             self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
             self.pipe += discretizer.pipe  # adding discretizer to pipe
 
@@ -558,62 +580,14 @@
         # iterating over each transformer
         for _, step in self.pipe:
             Xc = step.transform(Xc)
 
         return Xc
 
 
-class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
-    
-    def __init__(self, values_orders: Dict[str, Any], *, copy: bool=False, output: type= float, verbose: bool=False) -> None:
-        
-        self.features = list(values_orders.keys())
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.copy = copy
-        self.output = output
-        self.verbose = verbose
-        
-    def fit(self, X, y=None) -> None:
-        """ Does nothing, info is found in values_orders"""
-
-        return self
-    
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-
-        # copying dataframes
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-
-        # iterating over each feature
-        for n, feature in enumerate(self.features):
-            
-            # verbose if requested
-            if self.verbose: 
-                print(f" - [GroupedListDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
-            
-            # bucketizing feature
-            order = self.values_orders.get(feature)  # récupération des groupes
-            to_discard = [order.get(group) for group in order]  # identification des valeur à regrouper
-            to_input = [Xc[feature].isin(discarded) for discarded in to_discard]  # identifying main bucket value
-            to_keep = [n if self.output == float else group for n, group in enumerate(order)]  # récupération du groupe dans lequel regrouper
-
-            # case when there are no values
-            if len(to_input)==0 & len(to_keep)==0:
-                pass
-
-            # grouping modalities
-            else:
-                Xc[feature] = select(to_input, to_keep, default=Xc[feature])
-
-        # converting to float
-        if self.output == float:
-            Xc[self.features] = Xc[self.features].astype(float16)
-
-        return Xc
 
 class ChainedDiscretizer(GroupedListDiscretizer):
     
     def __init__(self, features: List[str], min_freq: float, chained_orders: List[List[Any]], *, copy: bool=False, verbose: bool=False) -> None:       
         
         self.min_freq = min_freq
         self.features = features[:]
@@ -628,15 +602,18 @@
     def fit(self, X: DataFrame, y: Series=None) -> None:
         
         # copying dataframe
         Xc = X[self.features].copy()
         
         # iterating over each feature
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [ChainedDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
+
+            # verbose if requested
+            if self.verbose:
+                print(f" - [ChainedDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
 
             # computing frequencies of each modality
             frequencies = Xc[feature].value_counts(dropna=False, normalize=True).drop(nan, errors='ignore')  # dropping nans to keep them anyways
             values, frequencies = frequencies.index, frequencies.values
 
             # checking for unknown values (values to present in an order of self.chained_orders)
             missing = [value for value in values if notna(value) and (value not in self.known_values)]
@@ -723,15 +700,18 @@
         # copying dataset if requested
         Xc = X
         if self.copy:
             Xc = X.copy()
         
         # iterating over each feature
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [QuantileDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
+
+            # verbose if requested
+            if self.verbose:
+                print(f" - [QuantileDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
 
             nans = isna(Xc[feature])  # keeping track of nans
 
             # grouping values inside quantiles
             to_input = [Xc[feature] <= q for q in self.quantiles.get(feature)]  # values that will be imputed
             values = [[v] * len(X) for v in self.values_orders.get(feature)]  # new values to imput
             Xc[feature] = select(to_input, values, default=Xc[feature])  # grouping modalities
@@ -852,49 +832,55 @@
     return n
 
 class DefaultDiscretizer(BaseEstimator, TransformerMixin):
     
     def __init__(
         self, features: List[str], min_freq: float, *, 
         values_orders: Dict[str, Any]={},
-        default_value: str='__OTHER__', dropna: bool=False, 
+        default_value: str='__OTHER__',
         copy: bool=False, verbose: bool=False) -> None:
         """ Groups a qualitative features' values less frequent than min_freq into a default_value"""
         
         self.features = features[:]
         self.min_freq = min_freq
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.default_value = default_value[:]
         self.copy = copy
         self.verbose = verbose
-        self.dropna = dropna
 
     def fit(self, X: DataFrame, y: Series) -> None:
 
         # computing frequencies of each modality
         frequencies = X[self.features].apply(value_counts, dropna=False, normalize=True, axis=0)
 
         # computing ordered target rate per modality for ordering
         target_rates = X[self.features].apply(target_rate, y=y, dropna=True, ascending=True, axis=0)
 
         # attributing orders to each feature
-        self.values_orders.update({feature: GroupedList(list(target_rates[feature])) for feature in self.features})
+        self.values_orders.update({f: GroupedList(list(target_rates[f])) for f in self.features})
         
-        #number of unique modality perf feature
-        nuniques = X[self.features].apply(nunique, dropna=self.dropna, axis=0)
+        #number of unique modality per feature
+        nuniques = X[self.features].apply(nunique, dropna=False, axis=0)
             
         # identifying modalities which are the most common
-        kept_nan = [nan] * (~self.dropna)  # whether or not to keep nans whatever there frequency
-        self.to_keep = {
-            feature: kept_nan[:] + [
-                value for value, frequency in frequencies[feature].items()
-                    if ((frequency >= self.min_freq) & notna(value)) | (nuniques[feature] <= 2)
-            ] for feature in self.features
-        }
-        
+        self.to_keep: Dict[str, Any] = {}  # dict of features and corresponding kept modalities
+
+        # iterating over each feature
+        for feature in self.features:
+
+            # checking for binary features
+            if nuniques[feature] > 2:
+                kept = [val for val, freq in frequencies[feature].items() if freq >= self.min_freq]
+
+            # keeping all modalities of binary features
+            else:
+                kept = [val for val, freq in frequencies[feature].items()]
+
+            self.to_keep.update({feature: kept})
+
         # grouping rare modalities 
         for n, feature in enumerate(self.features):
 
         	# printing verbose
             if self.verbose:
                 print(f" - [DefaultDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
             
@@ -929,15 +915,18 @@
         # copying dataset if requested
         Xc = X
         if self.copy:
             Xc = X.copy()
 
         # grouping values inside groups of modalities
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [DefaultDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
+
+        	# verbose if requested
+            if self.verbose: 
+                print(f" - [DefaultDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
 
             # grouping modalities
             Xc[feature] = select([~Xc[feature].isin(self.to_keep[feature])], [self.default_value], default=Xc[feature])
 
         return Xc
 
 
@@ -1042,15 +1031,15 @@
         return find_common_modalities(df_feature[notna(df_feature)], y[notna(df_feature)], min_freq, order, len_df)
 
 
     # cas 2 : il n'y a que des valeurs dans le dataframe (pas de NaN)
     else:
         
         # computing frequencies and target rate of each modality
-        init_frequencies = df_feature.value_counts(dropna=False, normalize=True).drop(nan, errors='ignore')  # dropping nans to keep them anyways
+        init_frequencies = df_feature.value_counts(dropna=False, normalize=False) / len_df
         init_values, init_frequencies = init_frequencies.index, init_frequencies.values
         
         # ordering
         frequencies = [init_frequencies[init_values == value][0] if any(init_values == value) else 0 for value in order]  # sort selon l'ordre des modalités
         values = [init_values[init_values == value][0] if any(init_values == value) else value for value in order]  # sort selon l'ordre des modalités
         target_rate = y.groupby(df_feature).sum().reindex(order) / frequencies / len_df # target rate per modality
         underrepresented = [value for value, frequency in zip(values, frequencies) if frequency < min_freq]  # valeur peu fréquentes
```

### Comparing `AutoCarver-4.1.0/AutoCarver/FeatureSelector.py` & `AutoCarver-4.2.0/AutoCarver/FeatureSelector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from IPython.display import display_html
 from math import sqrt
 from numpy import triu, ones, nan, inf
-from pandas import DataFrame, Series, notna
-from scipy.stats import kruskal
+from pandas import DataFrame, Series, notna, crosstab
+from scipy.stats import kruskal, chi2_contingency
 from sklearn.base import BaseEstimator, TransformerMixin
 from statsmodels.formula.api import ols
 from statsmodels.stats.outliers_influence import variance_inflation_factor
-from typing import List, Dict, Any, Callable
+from typing import List, Dict, Any, Callable, Tuple
 
 
 class FeatureSelector(BaseEstimator, TransformerMixin):
     """ A pipeline of measures to perform EDA and feature pre-selection
+     
+     - best features are the n_best of each measure
+     - selected features are stored in FeatureSelector.best_features
         
     Parameters
     ----------
     features: List[str]
         Features on which to compute association.
     n_best, int:
         Number of features to be selected
@@ -48,18 +51,19 @@
     
     def __init__(self, features: List[str], n_best: int, measures: List[Callable]=list(), filters: List[Callable]=list(),
                  copy: bool=True, verbose: bool=True, **params) -> None:
         
         self.features = features[:]
         self.n_best = n_best
         assert n_best <= len(features), "Must set n_best <= len(features)"
-
-        self.measures = [dtype_measure, nans_measure, mode_measure, zscore_measure] + measures[:]
+        self.best_features = features[:]
+        
+        self.measures = [dtype_measure, nans_measure, mode_measure] + measures[:]
         self.filters = [thresh_filter] + filters[:]
-        self.sort_measures = [measure.__name__ for measure in measures[-1::]]
+        self.sort_measures = [measure.__name__ for measure in measures[::-1]]
 
         self.copy = copy
         self.verbose = verbose
         self.params = params
     
     def measure(self, x: Series, y: Series) -> Dict[str, Any]:
         """ Measures association between x and y """
@@ -80,15 +84,23 @@
     ----------
     ascending, bool: default False
       Ascending of Descending sort by sort_measure
     """
         
         # applying association measure to each column
         self.associations = X[self.features].apply(self.measure, y=y, result_type='expand', axis=0).T
-        self.associations = self.associations.sort_values(self.sort_measures[0], ascending=self.params.get('ascending', False))
+        
+        # filtering non association measure (pct_zscore, pct_iqr...)
+        asso_measures = [c for c in self.associations if '_measure' in c]
+        self.sort_measures = [c for c in self.sort_measures if c in asso_measures]
+        
+        # sorting statistics if an association measure was provided
+        self.associations = self.associations.sort_values(
+            self.sort_measures, ascending=self.params.get('ascending', False)
+        )
     
     def filter_apply(self, X: DataFrame, sort_measure: str) -> DataFrame:
         """ Filters out too correlated features (least relevant first)
 
     Parameters
     ----------
     ascending, bool: default False
@@ -104,15 +116,15 @@
             # ordered filtering
             self.filtered_associations = filtering(X, self.filtered_associations, **self.params)
     
     def display_stats(self, association: DataFrame, caption: str) -> None:
         """ EDA of fitted associations"""
         
         # appllying style 
-        subset = [c for c in association if 'pct_' in c or '_measure' in c]
+        subset = [c for c in association if 'pct_' in c or '_measure' in c or '_filter' in c]
         style = association.style.background_gradient(cmap='coolwarm', subset=subset)
         style = style.set_table_attributes("style='display:inline'")
         style = style.set_caption(caption)
         display_html(style._repr_html_(), raw=True)
         
     
     def fit(self, X: DataFrame, y: Series) -> None:
@@ -131,24 +143,21 @@
         for n, sort_measure in enumerate(self.sort_measures):
             
             # filtering by sort_measure
             self.filter_apply(X, sort_measure)
             ranks += [list(self.filtered_associations.index)]
 
             # displaying filtered out association measure
-            if n == 0 and self.verbose:
+            if n == 0 and self.verbose and len(self.filters) > 1:
                 self.display_stats(self.filtered_associations, 'Filtered association')
 
         # retrieving the n_best features per ranking
-        self.best_features = [feature for rank in ranks for feature in rank[:self.n_best]]
-        self.best_features = list(set(self.best_features))  # deduplicating
-
-        # displaying filtered out association measure
-        # if n == 0 and self.verbose:
-        #     self.display_stats(self.associations.reindex(self.best_features), 'Filtered association')
+        if len(self.sort_measures) > 0:
+            self.best_features = [feature for rank in ranks for feature in rank[:self.n_best]]
+            self.best_features = list(set(self.best_features))  # deduplicating
 
         return self
 
     def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
 
         # copying dataset
         Xc = X
@@ -316,28 +325,112 @@
         })
 
         # Excluding feature with too frequent modes
         passed = pct_iqr < params.get('thresh_outlier', 1.)
         
     return active, association
 
+def chi2_measure(active: bool, association: Dict[str, Any], x: Series,
+                 y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Chi2 Measure between two Series of qualitative features"""
+        
+    # check that previous steps where passed
+    if active:
+    
+        # computing crosstab between x and y
+        xtab = crosstab(x, y)
+
+        # numnber of observations
+        n_obs = xtab.sum(axis=None)
+
+        # number of values taken by the features
+        n_mod_x, n_mod_y = len(xtab.index), len(xtab.columns)
+
+        # Chi2 statistic
+        chi2 = chi2_contingency(xtab)[0]
+
+        # updating association
+        association.update({'chi2_measure': chi2})
+    
+    return active, association
+
+def cramerv_measure(active: bool, association: Dict[str, Any], x: Series,
+                    y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Carmer's V between two Series of qualitative features"""
+
+    # check that previous steps where passed
+    if active:
+    
+        # computing chi2
+        if 'chi2_measure' not in association:
+            active, association = chi2_measure(active, association, x, y, **params)
+
+        # numnber of observations
+        n_obs = (notna(x) & notna(y)).sum()
+
+        # number of values taken by the features
+        n_mod_x, n_mod_y = x.nunique(), y.nunique()
+        min_n_mod = min(n_mod_x, n_mod_y)
+        
+        # Chi2 statistic
+        chi2 = association.get('chi2_measure')
+
+        # Cramer's V
+        cramerv = sqrt(chi2 / n_obs / (min_n_mod - 1))
+
+        # updating association
+        association.update({'cramerv_measure': cramerv})
+    
+    return active, association
+
+def tschuprowt_measure(active: bool, association: Dict[str, Any],x: Series,
+                       y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Tschuprow's T between two Series of qualitative features"""
+        
+    # check that previous steps where passed
+    if active:
+    
+        # computing chi2
+        if 'chi2_measure' not in association:
+            active, association = chi2_measure(active, association, x, y, **params)
+
+        # numnber of observations
+        n_obs = (notna(x) & notna(y)).sum()
+
+        # number of values taken by the features
+        n_mod_x, n_mod_y = x.nunique(), y.nunique()
+        
+        # Chi2 statistic
+        chi2 = association.get('chi2_measure')
+
+        # Tschuprow's T
+        dof_mods = sqrt((n_mod_x - 1) * (n_mod_y - 1))
+        tschuprowt = 0
+        if dof_mods > 0:
+            tschuprowt = sqrt(chi2 / n_obs / dof_mods)
+
+        # updating association
+        association.update({'tschuprowt_measure': tschuprowt})
+    
+    return active, association
+
     
 # FILTERS        
 def thresh_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
     """ Filters out missing association measure (did not pass a threshold)"""
     
     # drops rows with nans
     associations = ranks.dropna(axis=0)
     
     return associations
 
 def quantitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: str, **params) -> Dict[str, Any]:
     """ Computes max association between X and X (quantitative) excluding features 
     that are correlated to a feature more associated with the target 
-    (defined by the prefered_order).
+    (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
       Maximum association between features
     """
     
@@ -357,22 +450,22 @@
         # correlation with features more associated to the target
         corr_with_better_features = X_corr.loc[:feature, feature]
         
         # maximum correlation with a better feature
         corr_with, worst_corr = corr_with_better_features.agg(['idxmax', 'max'])
         
         # dropping the feature if it was too correlated to a better feature
-        if worst_corr > params.get('thresh_corr', 1.):
+        if worst_corr > params.get('thresh_corr', 1):
             X_corr = X_corr.drop(feature, axis=0).drop(feature, axis=1)
             
         # kept feature: updating associations with this feature
         else:
             associations += [{
                 'feature': feature, 
-                f'{corr_measure}_measure': worst_corr,
+                f'{corr_measure}_filter': worst_corr,
                 f'{corr_measure}_with': corr_with
             }]
             
     # formatting ouput to DataFrame
     associations = DataFrame(associations).set_index('feature')
             
     # applying filter on association
@@ -380,42 +473,38 @@
     
     return associations 
 
 
 def spearman_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
     """ Computes max Spearman between X and X (quantitative) excluding features 
     that are correlated to a feature more associated with the target 
-    (defined by the prefered_order).
+    (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
       Maximum association between features
     """
             
     # applying quantitative filter with spearman correlation
-    associations = quantitative_filter(X, ranks, 'spearman', **params)
-    
-    return associations
+    return quantitative_filter(X, ranks, 'spearman', **params)
 
 def pearson_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
     """ Computes max Pearson between X and X (quantitative) excluding features 
     that are correlated to a feature more associated with the target 
-    (defined by the prefered_order).
+    (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
       Maximum association between features
     """
             
     # applying quantitative filter with spearman correlation
-    associations = quantitative_filter(X, ranks, 'pearson', **params)
-    
-    return associations
+    return quantitative_filter(X, ranks, 'pearson', **params)
 
 def vif_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
     """ Computes Variance Inflation Factor (multicolinearity)
 
     Parameters
     ----------
     thresh_vif, float: default inf
@@ -447,16 +536,123 @@
         
         # dropping the feature if it was too correlated to a better feature
         if vif > params.get('thresh_vif', inf) and notna(vif):
             dropped += [feature]
             
         # kept feature: updating associations with this feature
         else:
-            associations += [{'feature': feature, 'vif_measure': vif}]
+            associations += [{'feature': feature, 'vif_filter': vif}]
     
     # formatting ouput to DataFrame
     associations = DataFrame(associations).set_index('feature')
             
     # applying filter on association
     associations = ranks.join(associations, how='right')
     
     return associations
+
+def qualitative_worst_corr(X: DataFrame, feature: str, ranks: DataFrame, corr_measure: Callable, **params):
+    """ Computes maximum association between a feature and features 
+    more associated to the target (according to ranks)
+    """
+    
+    # measure name
+    measure_name = corr_measure.__name__
+    measure = measure_name.replace('_measure', '')
+        
+    # initiating worst correlation
+    worst_corr = {'feature': feature}
+    
+    # features more associated with target
+    better_features = list(ranks.loc[:feature].index)[:-1]
+
+    # iterating over each better feature
+    for better_feature in better_features:
+
+        # computing association with better feature
+        _, association = corr_measure(True, {f'{measure}_with': better_feature}, 
+                                      X[feature], X[better_feature], **params)
+
+
+        # updating association if it's greater than previous better features
+        if association.get(measure_name) > worst_corr.get(measure_name, 0):
+
+            # renaming association measure as filter
+            association[f'{measure}_filter'] = association.pop(measure_name)
+            
+            # removing temporary measures
+            association = {k: v for k, v in association.items() if '_measure' not in k}
+
+            # updating worst known association
+            worst_corr.update(association)
+
+        # stopping measurements if association is greater than threshold
+        if association.get(f'{measure}_filter') > params.get('thresh_corr', 1):
+            ranks = ranks.drop(feature, axis=0)  # removing feature from ranks
+            
+            return ranks, None
+    
+    return ranks, worst_corr
+
+def qualitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: Callable, **params) -> Dict[str, Any]:
+    """ Computes max association between X and X (qualitative) excluding features 
+    that are correlated to a feature more associated with the target 
+    (defined by the ranks).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+        Maximum association between features
+    """
+    
+    # accessing the prefered order
+    prefered_order = ranks.index
+
+    # initiating list of maximum association per feature
+    associations = []
+    
+    # iterating over each feature by target association order
+    for feature in prefered_order:
+        
+        
+        # computing correlation with better features anf filtering out ranks
+        ranks, worst_corr = qualitative_worst_corr(X, feature, ranks, corr_measure, **params)
+        
+        # updating associations
+        if worst_corr:
+            associations += [worst_corr]
+
+    # formatting ouput to DataFrame
+    associations = DataFrame(associations).set_index('feature')
+            
+    # applying filter on association
+    associations = ranks.join(associations, how='right')
+    
+    return associations 
+
+def cramerv_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Computes max Cramer's V between X and X (qualitative) excluding features 
+    that are correlated to a feature more associated with the target 
+    (defined by the ranks).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+        Maximum association between features
+    """
+            
+    # applying quantitative filter with Cramer's V correlation    
+    return qualitative_filter(X, ranks, cramerv_measure, **params)
+
+def tschuprowt_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Computes max Tschuprow's T between X and X (qualitative) excluding features 
+    that are correlated to a feature more associated with the target 
+    (defined by the ranks).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+        Maximum association between features
+    """
+            
+    # applying quantitative filter with Tschuprow's T correlation
+    return qualitative_filter(X, ranks, tschuprowt_measure, **params)
```

### Comparing `AutoCarver-4.1.0/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-4.2.0/AutoCarver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.1.0
+Version: 4.2.0
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AutoCarver-4.1.0/LICENSE` & `AutoCarver-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.1.0/PKG-INFO` & `AutoCarver-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.1.0
+Version: 4.2.0
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AutoCarver-4.1.0/README.md` & `AutoCarver-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.1.0/setup.py` & `AutoCarver-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='AutoCarver',
-    version='4.1.0',
+    version='4.2.0',
     author='Mario DEFRANCE',
     author_email='defrancemario@gmail.com',
     description='Automatic Bucketizing of Features with Optimal Association',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mdefrance/AutoCarver',
     project_urls = {
```


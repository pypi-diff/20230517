# Comparing `tmp/dustgoggles-0.6.0.tar.gz` & `tmp/dustgoggles-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dustgoggles-0.6.0.tar", last modified: Tue Nov 22 18:17:27 2022, max compression
+gzip compressed data, was "dustgoggles-0.7.0.tar", last modified: Wed May 17 00:54:22 2023, max compression
```

## Comparing `dustgoggles-0.6.0.tar` & `dustgoggles-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-11-22 18:17:27.558404 dustgoggles-0.6.0/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1524 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/LICENSE
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      326 2022-11-22 18:17:27.556613 dustgoggles-0.6.0/PKG-INFO
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-11-22 18:17:27.409155 dustgoggles-0.6.0/dustgoggles/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       22 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/__init__.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-11-22 18:17:27.521315 dustgoggles-0.6.0/dustgoggles/codex/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/codex/__init__.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3518 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/codex/_array_holding_area.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5794 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/codex/codecs.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    33342 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/codex/implements.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3351 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/codex/memutilz.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     8366 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/composition.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     2981 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/func.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5401 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/mosaic.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5721 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/pivot.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     4035 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/scrape.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     9428 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/structures.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-11-22 18:17:27.544505 dustgoggles-0.6.0/dustgoggles/test_utils/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       20 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/test_utils/__init__.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     2519 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/dustgoggles/test_utils/core.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-11-22 18:17:27.456973 dustgoggles-0.6.0/dustgoggles.egg-info/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      326 2022-11-22 18:17:27.000000 dustgoggles-0.6.0/dustgoggles.egg-info/PKG-INFO
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      579 2022-11-22 18:17:27.000000 dustgoggles-0.6.0/dustgoggles.egg-info/SOURCES.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)        1 2022-11-22 18:17:27.000000 dustgoggles-0.6.0/dustgoggles.egg-info/dependency_links.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       87 2022-11-22 18:17:27.000000 dustgoggles-0.6.0/dustgoggles.egg-info/requires.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       12 2022-11-22 18:17:27.000000 dustgoggles-0.6.0/dustgoggles.egg-info/top_level.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       38 2022-11-22 18:17:27.558404 dustgoggles-0.6.0/setup.cfg
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      494 2022-11-22 17:27:47.000000 dustgoggles-0.6.0/setup.py
+drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-17 00:54:22.021237 dustgoggles-0.7.0/
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1524 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/LICENSE
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)      326 2023-05-17 00:54:22.016133 dustgoggles-0.7.0/PKG-INFO
+drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-17 00:54:21.446418 dustgoggles-0.7.0/dustgoggles/
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)       22 2023-05-17 00:39:26.000000 dustgoggles-0.7.0/dustgoggles/__init__.py
+drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-17 00:54:21.876911 dustgoggles-0.7.0/dustgoggles/codex/
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/codex/__init__.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3518 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/codex/_array_holding_area.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5794 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/codex/codecs.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)    33342 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/codex/implements.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3351 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/codex/memutilz.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     8366 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/composition.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5772 2023-05-17 00:39:32.000000 dustgoggles-0.7.0/dustgoggles/dynamic.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3738 2023-05-17 00:39:32.000000 dustgoggles-0.7.0/dustgoggles/func.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5422 2023-02-21 14:57:17.000000 dustgoggles-0.7.0/dustgoggles/mosaic.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     8112 2023-05-17 00:39:32.000000 dustgoggles-0.7.0/dustgoggles/pivot.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     4035 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/scrape.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)    10211 2023-05-17 00:39:32.000000 dustgoggles-0.7.0/dustgoggles/structures.py
+drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-17 00:54:21.970492 dustgoggles-0.7.0/dustgoggles/test_utils/
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)       20 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/test_utils/__init__.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     2519 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/test_utils/core.py
+drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-17 00:54:21.626714 dustgoggles-0.7.0/dustgoggles.egg-info/
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)      326 2023-05-17 00:54:20.000000 dustgoggles-0.7.0/dustgoggles.egg-info/PKG-INFO
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)      602 2023-05-17 00:54:21.000000 dustgoggles-0.7.0/dustgoggles.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)        1 2023-05-17 00:54:20.000000 dustgoggles-0.7.0/dustgoggles.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)       87 2023-05-17 00:54:20.000000 dustgoggles-0.7.0/dustgoggles.egg-info/requires.txt
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)       12 2023-05-17 00:54:20.000000 dustgoggles-0.7.0/dustgoggles.egg-info/top_level.txt
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)       38 2023-05-17 00:54:22.021899 dustgoggles-0.7.0/setup.cfg
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)      494 2023-05-17 00:31:09.000000 dustgoggles-0.7.0/setup.py
```

### Comparing `dustgoggles-0.6.0/LICENSE` & `dustgoggles-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.6.0/dustgoggles/codex/_array_holding_area.py` & `dustgoggles-0.7.0/dustgoggles/codex/_array_holding_area.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.6.0/dustgoggles/codex/codecs.py` & `dustgoggles-0.7.0/dustgoggles/codex/codecs.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.6.0/dustgoggles/codex/implements.py` & `dustgoggles-0.7.0/dustgoggles/codex/implements.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.6.0/dustgoggles/codex/memutilz.py` & `dustgoggles-0.7.0/dustgoggles/codex/memutilz.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.6.0/dustgoggles/composition.py` & `dustgoggles-0.7.0/dustgoggles/composition.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.6.0/dustgoggles/func.py` & `dustgoggles-0.7.0/dustgoggles/func.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """functional utilities and generators"""
-from functools import wraps, partial, reduce
+from functools import partial, reduce, wraps
 from itertools import accumulate, repeat
-from operator import add, contains, and_
-from typing import Callable, Iterable, Any, Sequence, Collection
+from operator import add, and_, contains
+from typing import Any, Callable, Collection, Iterable, Sequence
 
 
 def pass_parameters(func, *args, **kwargs):
     return func(*args, **kwargs)
 
 
 def catch_interaction(
@@ -96,25 +96,48 @@
 def gmap(
     func: Callable,
     *iterables: Iterable,
     mapper: Callable[[Callable, tuple[Iterable]], Iterable] = map,
     evaluator: Callable[[Iterable], Any] = tuple
 ):
     """
-    'greedy map' function. map func across iterables using mapper and
-    evaluate with evaluator.
-
+    'greedy map' function. map `func` across `iterables` using `mapper` and
+    evaluate with `evaluator`.
+    because we splat the variadic `iterables` argument into `mapper`, behavior
+    is roughly equivalent to `itertools.starmap` if you pass more than one
+    iterable.
     for cases in which you need a terse or configurable way to map and
     immediately evaluate functions.
     """
     return evaluator(mapper(func, *iterables))
 
 
+def filtern(func: Callable, iterable: Iterable):
+    """
+    similar to gmap(func, things, mapper=filter, evaluator=next).
+    for slightly faster or simpler cases.
+    """
+    return next(filter(func, iterable))
+
+
 def argstop(func, arg_count=0, unpack=True):
     @wraps(func)
     def stopargs(*args, **kwargs):
         if (len(args) == 1) and (unpack is True):
             args = args[0]
         args = args[:arg_count]
         return func(*args, **kwargs)
 
     return stopargs
+
+
+def optionalize(func: Callable, exc_callback: Callable = zero) -> Callable:
+    """return an optional version of `func`."""
+    @wraps(func)
+    def optionally(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except KeyboardInterrupt:
+            raise
+        except Exception as e:
+            exc_callback(e)
+    return optionally
```

### Comparing `dustgoggles-0.6.0/dustgoggles/mosaic.py` & `dustgoggles-0.7.0/dustgoggles/mosaic.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,28 +88,31 @@
     )
     metadata.index = metadata["column"]
     metadata.index.name = None
     return metadata.T
 
 
 # noinspection PyUnresolvedReferences
-def read_between(parquet_file, field, bounds, meta_records, verbose=True):
+def read_between(
+    parquet_file, field, bounds, meta_records, columns=None, verbose=True
+):
     """
     managed read-between bounds operation, more efficient in some cases
     than parquet.read_table with specified filters
     """
     bound_records = []
     for rec in meta_records:
         if not ((rec["min"] > bounds[1]) or (rec["max"] < bounds[0])):
             bound_records.append(rec)
     if verbose is True:
         print(len(bound_records), len(meta_records))
     if len(bound_records) == 0:
         return
     bound_groups = []
+
     for rec in bound_records:
         group = parquet_file.read_row_group(rec["row_group"])
         less_than = pac.filter(group, pac.less(group[field], bounds[1]))
         more_than = pac.filter(
             less_than, pac.greater_equal(less_than[field], bounds[0])
         )
         bound_groups.append(more_than)
```

### Comparing `dustgoggles-0.6.0/dustgoggles/pivot.py` & `dustgoggles-0.7.0/dustgoggles/pivot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 preprocessing and shorthand functions for dataframes, mappings, and ndarrays.
 """
 from functools import reduce
+from itertools import product
 from operator import attrgetter
-from typing import Any
+import re
+from typing import Any, Optional
 
 from cytoolz import valfilter
 import numpy as np
 import pandas as pd
 
 from dustgoggles.structures import listify
 
@@ -64,15 +66,15 @@
     """
     if how == "rows":
         axis = 0
     elif how == "columns":
         axis = 1
     else:
         raise ValueError(f"unknown how {how}")
-    constant_indices = df.nunique(axis=axis, dropna=dropna) == 1
+    constant_indices = df.nunique(axis=axis, dropna=dropna) <= 1
     if axis == 0:
         constants = df.loc[:, constant_indices]
         variables = df.loc[:, ~constant_indices]
     else:
         constants = df.loc[constant_indices]
         variables = df.loc[~constant_indices]
     if to_dict:
@@ -100,41 +102,87 @@
     return replacer
 
 
 def typed_columns(df, typenames):
     """return columns of df of types that match patterns given in typenames."""
     if isinstance(typenames, str):
         typenames = (typenames,)
-    names = df.dtypes.apply(attrgetter("name"))
-    return df[df.dtypes.loc[names.str.match("|".join(typenames))].index]
+    if isinstance(df.dtypes, np.dtype):
+        if re.match("|".join(typenames).lower(), df.dtypes.name.lower()):
+            return df
+        return pd.DataFrame(index=df.index)
+    names = df.dtypes.apply(attrgetter("name")).str.lower()
+    type_pattern = f"u?({'|'.join(typenames)})".lower()
+    return df[df.dtypes.loc[names.str.match(type_pattern)].index]
 
 
 def numeric_columns(df):
     """return 'numeric" columns of df."""
     return typed_columns(df, ("int", "float"))
 
 
-def demote(df, dtype, typenames=("int", "float")):
-    """
-    cast columns of df matching typenames to dtype.
-    return worst-case absolute and relative errors along with demoted df.
-    """
-    candidates = typed_columns(df, typenames)
-    demoted = candidates.astype(dtype)
-    offsets = (candidates - demoted).abs()
-    a_err = offsets.abs().max()
-    r_err = (offsets / candidates).abs().max()
-    return demoted, a_err, r_err
-
-
-def check_demote(df, dtype, typenames=("int", "float"), rtol=0.001, atol=0.01):
-    demoted, a_err, r_err = demote(df, dtype, typenames)
-    a_ok = a_err.loc[a_err < atol]
-    r_ok = r_err.loc[r_err < rtol]
-    return demoted[list(set(a_ok.index).intersection(set(r_ok.index)))]
+DTYPES = (
+    "uint8", "int8", "uint16", "int16",
+    "uint32", "int32", "uint64", "int64",
+    "float32", "float64"
+)
+
+
+def downcast(arr, atol=0.01, rtol=0.001):
+    # NaNs and infs don't count but should
+    # be preserved
+    nonfinite = ~np.isfinite(arr)
+    nonfinite_vals = arr[nonfinite]
+    arr[nonfinite] = 0
+    recast = None
+    for dtype in DTYPES:
+        recast = arr.astype(dtype)
+        offsets = np.abs(arr - recast)
+        if (aerr := np.nanmax(np.abs(offsets))) > atol:
+            continue
+        if (rerr := np.nanmax(np.abs(offsets / arr))) > rtol:
+            continue
+        break
+    if recast is None:
+        raise TypeError
+    # noinspection PyUnboundLocalVariable
+    return {
+        'recast': recast,
+        'nonfinite_mask': nonfinite,
+        'nonfinite_vals': nonfinite_vals,
+        'aerr': aerr,
+        'rerr': rerr
+    }
+
+
+def downcast_df(df, atol=0.01, rtol=0.001):
+    num = numeric_columns(df)
+    cast_series, cast_records = [], []
+    for name, col in num.items():
+        rec = downcast(col.values.T.copy(), atol, rtol) | {'name': name}
+        cast_records.append(rec)
+    while len(cast_records) > 0:
+        rec = cast_records.pop()
+        hasna = rec['nonfinite_mask'].any()
+        if hasna and ("int" in (dname := rec['recast'].dtype.name)):
+            prefix = "U" if dname.startswith("u") else ""
+            depth = (rec['recast'].dtype.itemsize * 8)
+            dtype = getattr(pd, f"{prefix}Int{depth}Dtype")()
+            series = pd.Series(rec['recast'], name=rec['name'], dtype=dtype)
+        else:
+            series = pd.Series(rec['recast'], name=rec['name'])
+        if hasna:
+            series.loc[rec['nonfinite_mask']] = rec['nonfinite_vals']
+        cast_series.append(series)
+    castdown = pd.concat(list(reversed(cast_series)), axis=1)
+    castdown.index = df.index
+    # TODO: inefficient inserts
+    for c in castdown:
+        df[c] = castdown[c]
+    return df
 
 
 def junction(df1, df2, columns, set_method="difference"):
     keys1 = df1[list(columns)].value_counts().index.to_list()
     keys2 = df2[list(columns)].value_counts().index.to_list()
     return getattr(set(keys1), set_method)(set(keys2))
 
@@ -147,37 +195,56 @@
     names = reduce(
         lambda x, y: x + "_" + y,
         [v for _, v in df[by + ["variable"]].astype(str).items()],
     )
     return pd.Series(df["value"].to_numpy(), index=names)
 
 
-def categorizable(df, threshold=255):
-    uniques = {}
-    for c in df.columns:
-        try:
-            uniques[c] = len(df[c].unique())
-        except TypeError:
-            continue
-    categories = valfilter(lambda v: v <= threshold, uniques)
-    return list(categories.keys())
+def unpack(series: pd.Series):
+    """unpack nested listlikes to columns"""
+    dropped = series.dropna()
+    df = pd.DataFrame(dropped.tolist(), index=dropped.index)
+    df.columns = [f"{dropped.name}_{i}" for i, _ in enumerate(df.columns)]
+    return df
 
 
-def categorize(df, threshold=255):
-    cat_columns = categorizable(df, threshold)
-    columns = [
-        df[c]
-        if c not in cat_columns
-        else pd.Series(pd.Categorical(df[c]), name=c)
-        for c in df.columns
-    ]
-    return pd.concat(columns, axis=1)
+def unpack_column(df: pd.DataFrame, colname):
+    """unpack a nested listlike column by name"""
+    unpacked = unpack(df[colname])
+    df.loc[unpacked.index, unpacked.columns] = unpacked
+    return df.drop(columns=colname)
 
 
 def unique_to_records(df, cols):
     unique_tuples = df[cols].value_counts().index.to_list()
     records = [
         {col: value for col, value in zip(cols, values)}
         for values in unique_tuples
     ]
     # noinspection PyTypeChecker
     return pd.DataFrame.from_dict(records)
+
+
+def squeeze(series: pd.Series, aggfunc: Optional[str] = None) -> pd.Series:
+    """
+    removes duplicate index labels from a Series, aggregating values
+    associated with each duplicate label using `aggfunc`. if aggfunc is
+    None, `squeeze` uses "any" if the Series is boolean and simply returns
+    the first element associated with each unique index label if the Series
+    is not.
+    """
+    if aggfunc is None:
+        if series.dtype.char == "?":
+            aggfunc = "any"
+        else:
+            return series.loc[~series.index.duplicated()]
+    df = pd.DataFrame(series).reset_index()
+    ixname = "index" if series.index.name is None else series.index.name
+    sname = 0 if series.name is None else series.name
+    squeezed = df.pivot_table(
+        values=series.name,
+        index=ixname,
+        aggfunc=aggfunc,
+    )[sname]
+    squeezed.index.name = series.index.name
+    squeezed.name = series.name
+    return squeezed
```

### Comparing `dustgoggles-0.6.0/dustgoggles/scrape.py` & `dustgoggles-0.7.0/dustgoggles/scrape.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.6.0/dustgoggles/structures.py` & `dustgoggles-0.7.0/dustgoggles/structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """structured data and manipulators thereof"""
-from collections import defaultdict
+from collections import defaultdict, OrderedDict
 from copy import copy
 from functools import reduce, partial
+from itertools import chain
 from operator import methodcaller, add, getitem, eq
 from typing import (
     Mapping,
     Collection,
     Any,
     Union,
     Sequence,
@@ -39,15 +40,15 @@
 
     return records
 
 
 def _unnest(nested, mtypes, escape, levels):
     if not isinstance(nested, mtypes):
         return nested
-    prefix = f"{escape}_{escape}".join(levels)
+    prefix = f"{escape}_{escape}".join(map(str, levels))
     if len(prefix) > 0:
         prefix = f"{escape}{prefix}{escape}_"
     long_records = []
     for level, maybe_mapping in nested.items():
         if not isinstance(maybe_mapping, mtypes):
             long_records.append({f"{prefix}{level}": maybe_mapping})
             continue
@@ -285,14 +286,34 @@
         if ref(item) is True:
             hits.append(item)
         else:
             misses.append(item)
     return hits, misses
 
 
+def rmerge(map1, map2, mtypes=(dict, OrderedDict)):
+    """
+    recursively merge map1 and map2. result is similar to map1 | map2, but
+    also merges any mappings at lower levels. for example:
+
+    >>> rmerge({'a': 1, 'b': {'a': 1}}, {'b': {'b': 1}, 'c': 2})
+    {'a': 1, 'b': {'a': 1, 'b': 1}, 'c': 2}
+    """
+    output = {}
+    only_in_one = set(map1.keys()).symmetric_difference(map2.keys())
+    for kv in chain(map1.items(), map2.items()):
+        if kv[0] in only_in_one:
+            output[kv[0]] = kv[1]
+        elif all(map(lambda m: isinstance(m, mtypes), (map1[kv[0]], map2[kv[0]]))):
+            output[kv[0]] = rmerge(map1[kv[0]], map2[kv[0]])
+        else:
+            output[kv[0]] = map2[kv[0]]
+    return output
+
+
 class HashDict:
     def __init__(self, equivalence: Callable[[Any], Hashable] = hash):
         self.dict_ = {}
         self.reverse = {}
         self.hasher = equivalence
 
     def __setitem__(self, key, item):
```

### Comparing `dustgoggles-0.6.0/dustgoggles/test_utils/core.py` & `dustgoggles-0.7.0/dustgoggles/test_utils/core.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.6.0/dustgoggles.egg-info/SOURCES.txt` & `dustgoggles-0.7.0/dustgoggles.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 setup.py
 dustgoggles/__init__.py
 dustgoggles/composition.py
+dustgoggles/dynamic.py
 dustgoggles/func.py
 dustgoggles/mosaic.py
 dustgoggles/pivot.py
 dustgoggles/scrape.py
 dustgoggles/structures.py
 dustgoggles.egg-info/PKG-INFO
 dustgoggles.egg-info/SOURCES.txt
```


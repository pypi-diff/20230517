# Comparing `tmp/intake_dataframe_catalog-0.1.1.post1.tar.gz` & `tmp/intake_dataframe_catalog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake_dataframe_catalog-0.1.1.post1.tar", last modified: Mon May 15 00:12:23 2023, max compression
+gzip compressed data, was "intake_dataframe_catalog-0.2.0.tar", last modified: Wed May 17 05:20:44 2023, max compression
```

## Comparing `intake_dataframe_catalog-0.1.1.post1.tar` & `intake_dataframe_catalog-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:12:23.630255 intake_dataframe_catalog-0.1.1.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 00:12:02.000000 intake_dataframe_catalog-0.1.1.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-15 00:12:23.630255 intake_dataframe_catalog-0.1.1.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-15 00:12:02.000000 intake_dataframe_catalog-0.1.1.post1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-15 00:12:02.000000 intake_dataframe_catalog-0.1.1.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 00:12:23.630255 intake_dataframe_catalog-0.1.1.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-15 00:12:02.000000 intake_dataframe_catalog-0.1.1.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:12:23.630255 intake_dataframe_catalog-0.1.1.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:12:23.630255 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-15 00:12:02.000000 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-15 00:12:02.000000 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-15 00:12:23.630255 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-05-15 00:12:02.000000 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:12:23.630255 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-15 00:12:23.000000 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-15 00:12:23.000000 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 00:12:23.000000 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 00:12:23.000000 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 00:12:23.000000 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 00:12:23.000000 intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:12:23.630255 intake_dataframe_catalog-0.1.1.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21910 2023-05-15 00:12:02.000000 intake_dataframe_catalog-0.1.1.post1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-15 00:12:02.000000 intake_dataframe_catalog-0.1.1.post1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-15 00:12:02.000000 intake_dataframe_catalog-0.1.1.post1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:20:44.761790 intake_dataframe_catalog-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20958 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21350 2023-05-17 05:20:29.000000 intake_dataframe_catalog-0.2.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-17 05:20:29.000000 intake_dataframe_catalog-0.2.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-17 05:20:29.000000 intake_dataframe_catalog-0.2.0/versioneer.py
```

### Comparing `intake_dataframe_catalog-0.1.1.post1/LICENSE` & `intake_dataframe_catalog-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.1.1.post1/PKG-INFO` & `intake_dataframe_catalog-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake_dataframe_catalog
-Version: 0.1.1.post1
+Version: 0.2.0
 Summary: An intake driver for a searchable table of intake sources and associated metadata
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `intake_dataframe_catalog-0.1.1.post1/README.rst` & `intake_dataframe_catalog-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.1.1.post1/pyproject.toml` & `intake_dataframe_catalog-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog/_search.py` & `intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import itertools
 import re
 import typing
 
 import numpy as np
 import pandas as pd
+import tlz
 
 
 def _is_pattern(value: typing.Union[str, typing.Pattern]) -> bool:
     """
     Check whether the passed value is a pattern
 
     Parameters
@@ -32,26 +33,25 @@
         return False
 
 
 def _match_iterables(
     strings: typing.Union[list, tuple, set], pattern: str, regex: bool
 ):
     """
-    Given an iterable of strings, return all that match the provided pattern
-    as a set.
+    Given an iterable of strings, return all that match the provided pattern.
     """
     matches = []
     for string in strings:
         if regex:
             match = re.match(pattern, string, flags=0)
         else:
             match = pattern == string
         if match:
             matches.append(string)
-    return matches
+    return type(strings)(matches)
 
 
 def search(
     df: pd.DataFrame,
     query: dict[str, typing.Any],
     columns_with_iterables: list,
     name_column: str,
@@ -98,15 +98,17 @@
             matches = df[column].apply(
                 lambda values: _match_iterables(values, value, is_pattern)
             )
             match = matches.astype(bool)
 
             # Keep track of which iterables matched
             if column in matched_iterables.columns:
-                matched_iterables[column] = matched_iterables[column] + matches
+                matched_iterables[column] = matched_iterables[column].combine(
+                    matches, func=lambda s1, s2: type(s1)(tlz.concat([s1, s2]))
+                )
             else:
                 matched_iterables[column] = matches
 
         elif is_pattern:
             match = df[column].str.contains(value, regex=True, case=True, flags=0)
         else:
             match = df[column] == value
@@ -133,16 +135,15 @@
             groups
         ).any().astype(int)
 
         global_match = global_match | condition_match
 
     # 3. Replace queried columns with iterables with reduced versions
     if not matched_iterables.empty:
-        types = {col: type(df[col].iloc[0]) for col in matched_iterables.columns}
-        df[matched_iterables.columns] = matched_iterables.apply(types)
+        df[matched_iterables.columns] = matched_iterables
 
     if require_all:
         has_all = n_conditions_in_group == len(conditions)
         # Expand has_all_mask across all groups
         has_all = has_all.loc[groups].reset_index(drop=True)
         global_match = global_match & has_all
     else:
```

### Comparing `intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog/core.py` & `intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
 import ast
 import typing
 import warnings
 from io import UnsupportedOperation
-from warnings import warn
 
 import fsspec
 import intake
 import pandas as pd
 import tlz
 import yaml
 from intake.catalog import Catalog
@@ -486,68 +485,14 @@
             return source
         else:
             raise ValueError(
                 f"Expected exactly one source, received {len(self)}. Please refine your search or use "
                 "`.to_source_dict()`."
             )
 
-    def to_subcatalog_dict(
-        self, **kwargs: dict[str, typing.Any]
-    ) -> dict[str, typing.Any]:
-        """
-        Load dataframe catalog entries into a dictionary of intake sources. NOTE, THIS METHOD WILL BE DEPRECIATED
-        IN THE NEXT RELEASE, PLEASE USE `to_source_dict` instead.
-
-        Parameters
-        ----------
-        kwargs: dict
-            Arguments/user parameters to use for opening the sources. For example, many intake drivers support
-            a `storage_options` argument with parameters to be passed to the backend file-system. Note, this function
-            passes the same kwargs to all sources in the dataframe catalog. To pass different kwargs to different
-            sources, load each source using it's key (name), e.g. `cat["<source_name>"](**kwargs)`.
-
-        Returns
-        -------
-        sources: dict
-            A dictionary of intake sources.
-        """
-
-        warn(
-            "This method will be depreciated in the next release. Please using `to_source_dict` instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-        return self.to_source_dict(**kwargs)
-
-    def to_subcatalog(self, **kwargs: dict[str, typing.Any]) -> intake.DataSource:
-        """
-        Load intake source. This is only possible if there is only one remaining source in the dataframe
-        catalog. NOTE, THIS METHOD WILL BE DEPRECIATED IN THE NEXT RELEASE, PLEASE USE `to_source` instead.
-
-        Parameters
-        ----------
-        kwargs: dict
-            Arguments/user parameters to use for opening the intake source. For example, many intake drivers support
-            a `storage_options` argument with parameters to be passed to the backend file-system.`.
-
-        Returns
-        -------
-        source: :py:class:`intake.DataSource`
-            A dictionary of sources.
-        """
-
-        warn(
-            "This method will be depreciated in the next release. Please using `to_source` instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-        return self.to_source(**kwargs)
-
     @property
     def df(self) -> pd.DataFrame:
         """
         Return a pandas :py:class:`~pandas.DataFrame` representation of the dataframe catalog. This property is
         mostly for internal use. Users may find the `df_summary` property more useful.
         """
         return self._df
```

### Comparing `intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog.egg-info/PKG-INFO` & `intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-dataframe-catalog
-Version: 0.1.1.post1
+Version: 0.2.0
 Summary: An intake driver for a searchable table of intake sources and associated metadata
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `intake_dataframe_catalog-0.1.1.post1/src/intake_dataframe_catalog.egg-info/SOURCES.txt` & `intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.1.1.post1/tests/test_core.py` & `intake_dataframe_catalog-0.2.0/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -678,35 +678,14 @@
         columns_with_iterables=["variable"],
         mode="r",
     )
     scat = cat.search(variable="tas")
     assert type(scat) is ChildCatalog
 
 
-def test_to_subcatalog_depreciated(catalog_path):
-    cat = intake.open_df_catalog(
-        path=str(catalog_path / "dfcat.csv"),
-        columns_with_iterables=["variable"],
-        mode="a",
-    )
-
-    with pytest.warns(
-        DeprecationWarning,
-        match="This method will be depreciated in the next release",
-    ):
-        cat.to_subcatalog_dict()
-
-    cat_new = cat.search(name="cesm")
-    with pytest.warns(
-        DeprecationWarning,
-        match="This method will be depreciated in the next release",
-    ):
-        cat_new.to_subcatalog()
-
-
 def _assert_DfFileCatalog(cat, empty=False):
     """
     Assert that the input is a DfFileCatalog
     """
     assert isinstance(cat, DfFileCatalog)
     assert isinstance(cat.df, pd.DataFrame)
     assert isinstance(cat.df_summary, pd.DataFrame)
```

### Comparing `intake_dataframe_catalog-0.1.1.post1/tests/test_search.py` & `intake_dataframe_catalog-0.2.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.1.1.post1/versioneer.py` & `intake_dataframe_catalog-0.2.0/versioneer.py`

 * *Files identical despite different names*


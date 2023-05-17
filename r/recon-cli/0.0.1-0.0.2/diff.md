# Comparing `tmp/recon_cli-0.0.1.tar.gz` & `tmp/recon_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recon_cli-0.0.1.tar", last modified: Tue May 16 14:48:33 2023, max compression
+gzip compressed data, was "recon_cli-0.0.2.tar", last modified: Wed May 17 02:19:21 2023, max compression
```

## Comparing `recon_cli-0.0.1.tar` & `recon_cli-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0       51 2023-05-16 14:48:33.000000 recon_cli-0.0.1/.flake8
--rw-r--r--   0        0        0      231 2023-05-16 14:48:33.000000 recon_cli-0.0.1/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      948 2023-05-16 14:48:33.000000 recon_cli-0.0.1/.gitignore
--rw-r--r--   0        0        0      563 2023-05-16 14:48:33.000000 recon_cli-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1069 2023-05-16 14:48:33.000000 recon_cli-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1225 2023-05-16 14:48:33.000000 recon_cli-0.0.1/README.md
--rw-r--r--   0        0        0      911 2023-05-16 14:48:33.000000 recon_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       58 2023-05-16 14:48:33.000000 recon_cli-0.0.1/recon/__init__.py
--rw-r--r--   0        0        0     8651 2023-05-16 14:48:33.000000 recon_cli-0.0.1/recon/main.py
--rw-r--r--   0        0        0     1058 2023-05-16 14:48:33.000000 recon_cli-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-16 14:48:33.000000 recon_cli-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2483 2023-05-16 14:48:33.000000 recon_cli-0.0.1/tests/test_main.py
--rw-r--r--   0        0        0      339 2023-05-16 14:48:33.000000 recon_cli-0.0.1/tox.ini
--rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 recon_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.flake8
+-rw-r--r--   0        0        0      231 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      655 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      625 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.github/workflows/tox.yml
+-rw-r--r--   0        0        0      948 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.gitignore
+-rw-r--r--   0        0        0      563 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1069 2023-05-17 02:19:21.000000 recon_cli-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1225 2023-05-17 02:19:21.000000 recon_cli-0.0.2/README.md
+-rw-r--r--   0        0        0      911 2023-05-17 02:19:21.000000 recon_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-05-17 02:19:21.000000 recon_cli-0.0.2/recon/__init__.py
+-rw-r--r--   0        0        0     9837 2023-05-17 02:19:21.000000 recon_cli-0.0.2/recon/main.py
+-rw-r--r--   0        0        0      364 2023-05-17 02:19:21.000000 recon_cli-0.0.2/recon/utils.py
+-rw-r--r--   0        0        0     1058 2023-05-17 02:19:21.000000 recon_cli-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-17 02:19:21.000000 recon_cli-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3113 2023-05-17 02:19:21.000000 recon_cli-0.0.2/tests/test_main.py
+-rw-r--r--   0        0        0      385 2023-05-17 02:19:21.000000 recon_cli-0.0.2/tox.ini
+-rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 recon_cli-0.0.2/PKG-INFO
```

### Comparing `recon_cli-0.0.1/.gitignore` & `recon_cli-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.1/.pre-commit-config.yaml` & `recon_cli-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.1/LICENSE.txt` & `recon_cli-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.1/README.md` & `recon_cli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.1/pyproject.toml` & `recon_cli-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "recon-cli"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mynhardt Burger", email="mynhardt+recon@gmail.com" },
 ]
 description = "Simple reconciliation of two lists based on a common field"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Financial and Insurance Industry",
     "Natural Language :: English"]
```

### Comparing `recon_cli-0.0.1/recon/main.py` & `recon_cli-0.0.2/recon/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+from __future__ import annotations
+
 import sys
 from enum import Enum
 from functools import cached_property
 from os import PathLike
 from pathlib import PurePath
 from textwrap import dedent
 from typing import Any, Literal, Union
 
 import pandas as pd
 
+from recon.utils import ensure_df
+
 FilePath = Union[str, "PathLike[str]"]
 Suffixes = Union[
     list[Union[str, None]], tuple[str, None], tuple[None, str], tuple[str, str]
 ]
 
 RECON_COMPONENTS = Literal[
     "left_both",
@@ -37,26 +41,25 @@
         self.left: pd.DataFrame
         self.right: pd.DataFrame
         self.left_on: str
         self.right_on: str
 
         self.suffixes: tuple[str, str]
 
-        self.output_dispatch: dict[str, Union[pd.Series, pd.DataFrame]] = {
-            "left_only": self.left_only,
-            "right_only": self.right_only,
-            "left_duplicate": self.left_duplicate,
-            "right_duplicate": self.right_duplicate,
-            "left_both": self.left_both,
-            "right_both": self.right_both,
-            "left": self.left,
-            "right": self.right,
-            "both": self.both,
-            "all": self.all_data,
-        }
+        self.output_dispatch = [
+            "left_only",
+            "right_only",
+            "left_duplicate",
+            "right_duplicate",
+            "left_both",
+            "right_both",
+            "left",
+            "right",
+        ]
+        """Set of property names available for export."""
 
     def _map_column_names(self):
         left_columns = set(self.left.reset_index(names="index").columns)
         right_columns = set(self.right.reset_index(names="index").columns)
         common_columns = left_columns & right_columns
         left_only = left_columns - right_columns
         right_only = right_columns - left_columns
@@ -97,51 +100,71 @@
             indicator=True,
             how="outer",
             suffixes=self.suffixes,
         )
 
     @cached_property
     def both(self) -> pd.DataFrame:
-        return self.all_data.loc[self.all_data["_merge"] == "both"]
+        return self.all_data.loc[self.all_data["_merge"] == "both"].convert_dtypes()
 
     @cached_property
     def left_both(self) -> pd.DataFrame:
         return (
             self.both[self._left_name_map.values()]
             .drop_duplicates()
+            .convert_dtypes()
             .set_index(f"index{self.suffixes[0]}")
         )
 
     @cached_property
     def right_both(self) -> pd.DataFrame:
         return (
             self.both[self._right_name_map.values()]
             .drop_duplicates()
+            .convert_dtypes()
             .set_index(f"index{self.suffixes[1]}")
         )
 
     @cached_property
     def left_only(self) -> pd.DataFrame:
-        return self.all_data.loc[
-            self.all_data["_merge"] == "left_only", list(self._left_name_map.values())
-        ].set_index(f"index{self.suffixes[0]}")
+        return (
+            self.all_data.loc[
+                self.all_data["_merge"] == "left_only",
+                list(self._left_name_map.values()),
+            ]
+            .convert_dtypes()
+            .set_index(f"index{self.suffixes[0]}")
+        )
 
     @cached_property
     def right_only(self) -> pd.DataFrame:
-        return self.all_data.loc[
-            self.all_data["_merge"] == "right_only", list(self._right_name_map.values())
-        ].set_index(f"index{self.suffixes[1]}")
+        return (
+            self.all_data.loc[
+                self.all_data["_merge"] == "right_only",
+                list(self._right_name_map.values()),
+            ]
+            .convert_dtypes()
+            .set_index(f"index{self.suffixes[1]}")
+        )
 
     @cached_property
     def left_duplicate(self) -> pd.DataFrame:
-        return self.left.loc[self.left.duplicated(keep="first")]
+        return (
+            self.left.loc[self.left.duplicated(keep="first")]
+            .rename_axis(index=f"index{self.suffixes[0]}")
+            .convert_dtypes()
+        )
 
     @cached_property
     def right_duplicate(self) -> pd.DataFrame:
-        return self.right.loc[self.right.duplicated(keep="first")]
+        return (
+            self.right.loc[self.right.duplicated(keep="first")]
+            .rename_axis(index=f"index{self.suffixes[1]}")
+            .convert_dtypes()
+        )
 
     @cached_property
     def is_left_unique(self) -> bool:
         return self.left[self.left_on].is_unique
 
     @cached_property
     def is_right_unique(self) -> bool:
@@ -180,91 +203,120 @@
         )
         print(report)
 
     def to_xlsx(
         self, path: FilePath, recon_components: list[RECON_COMPONENTS], **kwargs
     ) -> None:
         write_list = (
-            self.output_dispatch.keys()
-            if "all_data" in recon_components
-            else recon_components
+            self.output_dispatch if "all_data" in recon_components else recon_components
         )
 
         with pd.ExcelWriter(path, **kwargs) as writer:
             for component in write_list:
-                self.output_dispatch[component].to_excel(
+                getattr(self, component).to_excel(
                     writer, sheet_name=component, index_label="index"
                 )
 
     def to_stdout(self, recon_components: list[RECON_COMPONENTS], **kwargs) -> None:
         write_list = (
-            self.output_dispatch.keys()
-            if "all_data" in recon_components
-            else recon_components
+            self.output_dispatch if "all_data" in recon_components else recon_components
         )
 
+        print("--------- START ----------")
         for component in write_list:
             print(f"--------- {component} ----------")
-            self.output_dispatch[component].to_csv(
-                sys.stdout, index_label="index", **kwargs
-            )
-            print("--------- END ----------")
+            getattr(self, component).to_csv(sys.stdout, index_label="index", **kwargs)
+        print("--------- END ----------")
 
     @staticmethod
     def _read_file(
-        data: Union[pd.Series, pd.DataFrame, FilePath],
-        position: Literal["left", "right"],
+        data: FilePath,
         sheet_name: str = "Sheet1",
         **kwargs,
     ):
-        if isinstance(data, pd.DataFrame):
-            return data
-
-        if isinstance(data, pd.Series):
-            return data.to_frame(name=position)
-
         file_path = PurePath(data)
-        if file_path.suffix.lower() in {"xlsx", "xls", "xlsm", "xlsb"}:
+        if file_path.suffix.lower() in {".xlsx", ".xls", ".xlsm", ".xlsb"}:
             if not isinstance(sheet_name, (str, int)):
                 raise ValueError("Importing of multiple sheets is not supported")
             return pd.read_excel(file_path, sheet_name, **kwargs)
         else:
             return pd.read_csv(file_path, **kwargs)
 
     @staticmethod
+    def _load_df(
+        recon_obj: "Reconcile",
+        left_df: pd.DataFrame,
+        right_df: pd.DataFrame,
+        left_on: str,
+        right_on: str,
+        suffixes: tuple[str, str] = ("_left", "_right"),
+    ):
+        recon_obj.left = left_df
+        if left_on in recon_obj.left.columns:
+            recon_obj.left_on = left_on
+        else:
+            raise ValueError(
+                f"left_on ({left_on}) doesn't exist within the left dataset."
+            )
+
+        recon_obj.right = right_df
+        if right_on in recon_obj.right.columns:
+            recon_obj.right_on = right_on
+        else:
+            raise ValueError(
+                f"right_on ({right_on}) doesn't exist within the right dataset."
+            )
+
+        recon_obj.suffixes = suffixes
+
+        return recon_obj
+
+    @staticmethod
     def read_files(
-        left: FilePath,
-        right: FilePath,
+        left_file: FilePath,
+        right_file: FilePath,
         left_on: str,
         right_on: str,
         suffixes: tuple[str, str] = ("_left", "_right"),
         left_kwargs: dict[str, Any] = {},
         right_kwargs: dict[str, Any] = {},
     ):
         """
-        Returns a :class:`Reconcile` object which can be queried.
+        Returns a :class:`Reconcile` object populated with data which can be queried.
 
-        Excel files are identified by the ".xlsx" extension. All other extensions
+        Excel files are identified by their extension. All other extensions
         are assumed to be csv. :param:`left_kwargs` and :param:`right_kwargs` are
         passed onto the `pandas.read_excel()` and `pandas.read_csv()` methods.
         """
-        recon = Reconcile()
 
-        recon.left = Reconcile._read_file(left, "left", **left_kwargs)
-        if left_on in recon.left.columns:
-            recon.left_on = left_on
-        else:
-            raise ValueError(
-                f"left_on ({left_on}) doesn't exist within the left dataset."
-            )
+        left_df = Reconcile._read_file(left_file, **left_kwargs)
+        right_df = Reconcile._read_file(right_file, **right_kwargs)
 
-        recon.right = Reconcile._read_file(right, "right", **right_kwargs)
-        if right_on in recon.right.columns:
-            recon.right_on = right_on
-        else:
-            raise ValueError(
-                f"right_on ({right_on}) doesn't exist within the right dataset."
-            )
+        recon = Reconcile()
+        recon = Reconcile._load_df(
+            recon, left_df, right_df, left_on, right_on, suffixes
+        )
+
+        return recon
 
-        recon.suffixes = suffixes
+    @staticmethod
+    def read_df(
+        left_df: Union[pd.DataFrame, pd.Series[Any]],
+        right_df: Union[pd.DataFrame, pd.Series[Any]],
+        left_on: str,
+        right_on: str,
+        suffixes: tuple[str, str] = ("_left", "_right"),
+    ):
+        """
+        Returns a :class:`Reconcile` object populated with data which can be queried.
+        """
+        recon = Reconcile()
+        recon = Reconcile._load_df(
+            recon,
+            ensure_df(left_df, "left"),
+            ensure_df(right_df, "right"),
+            left_on,
+            right_on,
+            suffixes,
+        )
 
         return recon
```

### Comparing `recon_cli-0.0.1/requirements.txt` & `recon_cli-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.1/PKG-INFO` & `recon_cli-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: recon-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple reconciliation of two lists based on a common field
 Author-email: Mynhardt Burger <mynhardt+recon@gmail.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Natural Language :: English
 Requires-Dist: pandas == 2.0.1
```


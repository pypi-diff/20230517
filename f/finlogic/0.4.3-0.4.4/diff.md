# Comparing `tmp/finlogic-0.4.3.tar.gz` & `tmp/finlogic-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.4.3.tar", last modified: Wed May 17 10:29:50 2023, max compression
+gzip compressed data, was "finlogic-0.4.4.tar", last modified: Wed May 17 10:53:06 2023, max compression
```

## Comparing `finlogic-0.4.3.tar` & `finlogic-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.3/LICENSE
--rw-r--r--   0        0        0     9611 2023-05-15 08:41:19.853254 finlogic-0.4.3/README.md
--rw-r--r--   0        0        0      423 2023-05-17 09:42:06.408604 finlogic-0.4.3/finlogic/__init__.py
--rw-r--r--   0        0        0    23425 2023-05-17 09:42:06.409605 finlogic-0.4.3/finlogic/company.py
--rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.3/finlogic/config.py
--rw-r--r--   0        0        0     9775 2023-05-17 10:25:31.301270 finlogic-0.4.3/finlogic/cvm.py
--rw-r--r--   0        0        0     4443 2023-05-17 03:27:27.153327 finlogic-0.4.3/finlogic/database.py
--rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.3/finlogic/finprint.py
--rw-r--r--   0        0        0     3156 2023-05-17 03:27:27.153327 finlogic-0.4.3/finlogic/fl_duckdb.py
--rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.3/finlogic/language.py
--rw-r--r--   0        0        0     1005 2023-05-17 10:29:50.344668 finlogic-0.4.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0     3314 2023-05-12 00:21:10.028393 finlogic-0.4.3/tests/test_company.py
--rw-r--r--   0        0        0      902 2023-05-14 15:04:47.183513 finlogic-0.4.3/tests/test_database.py
--rw-r--r--   0        0        0    11655 1970-01-01 00:00:00.000000 finlogic-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.4/LICENSE
+-rw-r--r--   0        0        0     9611 2023-05-15 08:41:19.853254 finlogic-0.4.4/README.md
+-rw-r--r--   0        0        0      423 2023-05-17 10:51:22.833432 finlogic-0.4.4/finlogic/__init__.py
+-rw-r--r--   0        0        0    23507 2023-05-17 10:44:23.276617 finlogic-0.4.4/finlogic/company.py
+-rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.4/finlogic/config.py
+-rw-r--r--   0        0        0     9775 2023-05-17 10:25:31.301270 finlogic-0.4.4/finlogic/cvm.py
+-rw-r--r--   0        0        0     4460 2023-05-17 10:44:29.881677 finlogic-0.4.4/finlogic/database.py
+-rw-r--r--   0        0        0     3156 2023-05-17 03:27:27.153327 finlogic-0.4.4/finlogic/fduckdb.py
+-rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.4/finlogic/fprint.py
+-rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.4/finlogic/language.py
+-rw-r--r--   0        0        0     1005 2023-05-17 10:53:06.688384 finlogic-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     3314 2023-05-12 00:21:10.028393 finlogic-0.4.4/tests/test_company.py
+-rw-r--r--   0        0        0      900 2023-05-17 10:44:08.373481 finlogic-0.4.4/tests/test_database.py
+-rw-r--r--   0        0        0    11655 1970-01-01 00:00:00.000000 finlogic-0.4.4/PKG-INFO
```

### Comparing `finlogic-0.4.3/LICENSE` & `finlogic-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.3/README.md` & `finlogic-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.3/finlogic/company.py` & `finlogic-0.4.4/finlogic/company.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     FinLogic Dataframe uses category dtype for efficiency.
 
 """
 from typing import Literal
 import numpy as np
 import pandas as pd
 from .language import language_df
-from .finprint import print_dict
-from .fl_duckdb import execute
+from .fprint import print_dict
+from .fduckdb import execute
 
 
 class Company:
     """A class to represent a company financial data.
 
     This class provides methods to create financial reports and to calculate
     financial indicators based on a company's accounting data. The class also
@@ -286,14 +286,17 @@
         self._dfc = dfc
 
     def info(self) -> dict:
         """Print a concise summary of a company."""
         # Some companies have no quarterly reports (see cvm_id 9784)
         if self._last_quarterly is pd.NaT:
             last_quarterly = "No quarterly reports"
+        else:
+            last_quarterly = self._last_quarterly.strftime("%Y-%m-%d")
+
         company_info = {
             "Name": self.name_id,
             "CVM ID": self._cvm_id,
             "Fiscal ID (CNPJ)": self.tax_id,
             "Total Accounting Rows": len(self._dfc.index),
             "Selected Accounting Method": self._acc_method,
             "Selected Accounting Unit": self._acc_unit,
```

### Comparing `finlogic-0.4.3/finlogic/cvm.py` & `finlogic-0.4.4/finlogic/cvm.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.3/finlogic/database.py` & `finlogic-0.4.4/finlogic/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 about the database itself.
 """
 from typing import Literal
 import pandas as pd
 from . import cvm
 from . import config as cfg
 from . import language as lng
-from . import finprint as fpr
-from . import fl_duckdb as fdb
+from . import fprint as fpr
+from . import fduckdb as fdb
 
 CHECKMARK = "\033[32m\u2714\033[0m"
 
 
 def get_filepaths_to_process() -> list[str]:
     """Return a list of CVM files that has to be processed by comparing
     the files mtimes from the raw folder with the database.
     """
     df_raw = cvm.get_raw_file_mtimes()
     df_fdb = fdb.get_file_mtimes()
     df_new = pd.concat([df_raw, df_fdb]).drop_duplicates(keep=False)
-    file_sources = set(df_new["file_source"])
+    file_sources = sorted(df_new["file_source"].drop_duplicates())
     return [cfg.CVM_RAW_DIR / file_source for file_source in file_sources]
 
 
 def update_database(rebuild: bool = False):
     """Verify changes in CVM files and update Finlogic Database if necessary.
 
     Args:
```

### Comparing `finlogic-0.4.3/finlogic/finprint.py` & `finlogic-0.4.4/finlogic/fprint.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.3/finlogic/fl_duckdb.py` & `finlogic-0.4.4/finlogic/fduckdb.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.3/finlogic/language.py` & `finlogic-0.4.4/finlogic/language.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.3/pyproject.toml` & `finlogic-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 dependencies = [
     "pandas>=1.4.0",
     "requests>=2.27.0",
     "duckdb>=0.7.0",
     "rich>=13.0.0",
 ]
-version = "0.4.3"
+version = "0.4.4"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.0.0",
```

### Comparing `finlogic-0.4.3/tests/test_company.py` & `finlogic-0.4.4/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.3/tests/test_database.py` & `finlogic-0.4.4/tests/test_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import finlogic as fl
-from finlogic import fl_duckdb as fdb
+from finlogic import fduckdb as fdb
 
 
 class TestDatabase(unittest.TestCase):
     def test_info(self):
         """Test the info method of the Database module."""
         db_info = fdb.get_info()
         self.assertEqual(db_info["first_report"], "2009-01-31")
```

### Comparing `finlogic-0.4.3/PKG-INFO` & `finlogic-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.4.3
+Version: 0.4.4
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
```


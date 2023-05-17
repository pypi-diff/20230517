# Comparing `tmp/finlogic-0.4.2.tar.gz` & `tmp/finlogic-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.4.2.tar", last modified: Sun May 14 15:29:06 2023, max compression
+gzip compressed data, was "finlogic-0.4.3.tar", last modified: Wed May 17 10:29:50 2023, max compression
```

## Comparing `finlogic-0.4.2.tar` & `finlogic-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.2/LICENSE
--rw-r--r--   0        0        0     9612 2023-05-14 10:36:12.075362 finlogic-0.4.2/README.md
--rw-r--r--   0        0        0      423 2023-05-12 00:21:10.028393 finlogic-0.4.2/finlogic/__init__.py
--rw-r--r--   0        0        0    23323 2023-05-14 15:04:47.182513 finlogic-0.4.2/finlogic/company.py
--rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.2/finlogic/config.py
--rw-r--r--   0        0        0     9656 2023-05-14 15:04:47.183513 finlogic-0.4.2/finlogic/cvm.py
--rw-r--r--   0        0        0     4357 2023-05-14 15:04:47.183513 finlogic-0.4.2/finlogic/database.py
--rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.2/finlogic/finprint.py
--rw-r--r--   0        0        0     3223 2023-05-14 15:11:20.236277 finlogic-0.4.2/finlogic/fl_duckdb.py
--rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.2/finlogic/language.py
--rw-r--r--   0        0        0     1005 2023-05-14 15:29:06.969571 finlogic-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     3314 2023-05-12 00:21:10.028393 finlogic-0.4.2/tests/test_company.py
--rw-r--r--   0        0        0      902 2023-05-14 15:04:47.183513 finlogic-0.4.2/tests/test_database.py
--rw-r--r--   0        0        0    11656 1970-01-01 00:00:00.000000 finlogic-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.3/LICENSE
+-rw-r--r--   0        0        0     9611 2023-05-15 08:41:19.853254 finlogic-0.4.3/README.md
+-rw-r--r--   0        0        0      423 2023-05-17 09:42:06.408604 finlogic-0.4.3/finlogic/__init__.py
+-rw-r--r--   0        0        0    23425 2023-05-17 09:42:06.409605 finlogic-0.4.3/finlogic/company.py
+-rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.3/finlogic/config.py
+-rw-r--r--   0        0        0     9775 2023-05-17 10:25:31.301270 finlogic-0.4.3/finlogic/cvm.py
+-rw-r--r--   0        0        0     4443 2023-05-17 03:27:27.153327 finlogic-0.4.3/finlogic/database.py
+-rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.3/finlogic/finprint.py
+-rw-r--r--   0        0        0     3156 2023-05-17 03:27:27.153327 finlogic-0.4.3/finlogic/fl_duckdb.py
+-rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.3/finlogic/language.py
+-rw-r--r--   0        0        0     1005 2023-05-17 10:29:50.344668 finlogic-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     3314 2023-05-12 00:21:10.028393 finlogic-0.4.3/tests/test_company.py
+-rw-r--r--   0        0        0      902 2023-05-14 15:04:47.183513 finlogic-0.4.3/tests/test_database.py
+-rw-r--r--   0        0        0    11655 1970-01-01 00:00:00.000000 finlogic-0.4.3/PKG-INFO
```

### Comparing `finlogic-0.4.2/LICENSE` & `finlogic-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.2/README.md` & `finlogic-0.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 <!-- [![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic)" -->
 
 ## FinLogic: finance toolkit for listed Brazilian companies.
 
 ---
 
-**FinLogic** offers a Pythonic way to analyze financial data of listed companies in Brazil from information made publicly avaible by local securities market authority (CVM). FinLogic uses DuckDB as an OLAP database management system and Pandas to process the data to and from the locally builted accounting database (aprox. 21 million rows).
+**FinLogic** offers a Pythonic way to analyze financial data of listed companies in Brazil from information made publicly avaible by local securities market authority (CVM). FinLogic uses DuckDB as an OLAP database management system and Pandas to process the data to and from the locally builted accounting database (aprox. 8 million rows).
 
 ---
 
 ## Installation
 
 The source code is currently hosted on GitHub at:
 https://github.com/crdcj/FinLogic
```

### Comparing `finlogic-0.4.2/finlogic/company.py` & `finlogic-0.4.3/finlogic/company.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 set the accounting method, unit, tax rate, and language for the company object.
 
 Classes:
     Company: Represents a company with its financial information and allows
     users to generate financial reports and indicators.
 
 Abreviations used in code:
+    dfc = company dataframe
     dfi = input dataframe
     dfo = output dataframe
 
 RuntimeWarning:
     Pandas query + numexpr module -> Engine has switched to 'python' because
     numexpr does not support extension array dtypes (category not supported
     yet). Please set your engine to python manually. That means that the query
@@ -55,15 +56,15 @@
         self.identifier = identifier
         self.acc_method = acc_method
         self.acc_unit = acc_unit
         self.tax_rate = tax_rate
         self.language = language
         self._initialized = True
         # Only set company dataframe after identifier, acc_method and acc_unit are set
-        self._set_co_df()
+        self._set_dfc()
 
     @property
     def identifier(self) -> int | str:
         """Set a unique identifier to select the company in FinLogic Database.
 
         This method sets the company's CVM and fiscal ID based on a given
         identifier. The identifier can be either the CVM ID or the Fiscal ID
@@ -99,15 +100,15 @@
             self.tax_id = df.loc[0, "tax_id"]
             self.name_id = df.loc[0, "name_id"]
             self._identifier = identifier
         else:
             raise KeyError(f"Company 'identifier' {identifier} not found.")
         # If object was already initialized, reset company dataframe
         if self._initialized:
-            self._set_co_df()
+            self._set_dfc()
 
     @property
     def acc_method(self) -> Literal["consolidated", "separate"]:
         """Gets or sets the accounting method for registering investments in
         subsidiaries.
 
         The "acc_method" must be "consolidated" or "separate". Consolidated
@@ -125,15 +126,15 @@
         if value in {"consolidated", "separate"}:
             # Set accounting method to upper case as in FinLogic Database
             self._acc_method = value.upper()
         else:
             raise ValueError("acc_method expects 'consolidated' or 'separate'")
         # If object was already initialized, reset company dataframe
         if self._initialized:
-            self._set_co_df()
+            self._set_dfc()
 
     @property
     def acc_unit(self) -> float:
         """Gets or sets the accounting unit for the financial statements.
 
         The "acc_unit" is a constant that will divide all company
         accounting values. The constant must be a number greater than
@@ -171,15 +172,15 @@
             case v if v > 0:
                 self._acc_unit = v
             case _:
                 raise ValueError("Accounting Unit is invalid")
 
         # If object was already initialized, reset company dataframe
         if self._initialized:
-            self._set_co_df()
+            self._set_dfc()
 
     @property
     def tax_rate(self) -> float:
         """Gets or sets company 'tax_rate' property.
 
         The "tax_rate" is used to calculate some of the company
         indicators, such as EBIT and net income. The default value
@@ -231,79 +232,81 @@
         list_languages = ["english", "portuguese"]
         if language.lower() in list_languages:
             self._language = language.capitalize()
         else:
             sup_lang = f"Supported languages: {', '.join(list_languages)}"
             raise KeyError(f"'{language}' not supported. {sup_lang}")
 
-    def _set_co_df(self) -> pd.DataFrame:
+    def _set_dfc(self) -> pd.DataFrame:
         """Sets the company data frame.
 
         This method creates a data frame with the company's financial
         statements.
         """
         # Create the company data frame
         query = f"""
             SELECT *
               FROM reports
              WHERE cvm_id = {self._cvm_id}
                AND acc_method = '{self._acc_method}'
              ORDER BY acc_code, period_reference, period_end
         """
-        co_df = execute(query, "df")
+        dfc = execute(query, "df")
 
         # Change acc_unit only for accounts different from 3.99
-        co_df["acc_value"] = np.where(
-            co_df["acc_code"].str.startswith("3.99"),
-            co_df["acc_value"],
-            co_df["acc_value"] / self._acc_unit,
+        dfc["acc_value"] = np.where(
+            dfc["acc_code"].str.startswith("3.99"),
+            dfc["acc_value"],
+            dfc["acc_value"] / self._acc_unit,
         )
-        annual_reports = co_df.query('report_type == "ANNUAL"')
+        annual_reports = dfc.query('report_type == "ANNUAL"')
         self._first_annual = annual_reports["period_end"].min()
         self._last_annual = annual_reports["period_end"].max()
-        quarterly_reports = co_df.query('report_type == "QUARTERLY"')
+        quarterly_reports = dfc.query('report_type == "QUARTERLY"')
         self._last_quarterly = quarterly_reports["period_end"].max()
 
         # Drop columns that are already company atributes
-        co_df.drop(columns=["name_id", "cvm_id", "tax_id", "acc_method"], inplace=True)
+        dfc.drop(columns=["name_id", "cvm_id", "tax_id", "acc_method"], inplace=True)
 
         # Keep only the newest 'report_version' in df
         cols = [
             "report_type",
             "report_version",
             "period_reference",
             "period_order",
             "acc_code",
         ]
-        co_df.sort_values(by=cols, ignore_index=True, inplace=True)
-        cols = co_df.columns.tolist()
+        dfc.sort_values(by=cols, ignore_index=True, inplace=True)
+        cols = dfc.columns.tolist()
         cols_remove = ["report_version", "acc_value", "acc_fixed"]
         [cols.remove(col) for col in cols_remove]
         # Ascending order --> last is the newest report_version
-        co_df.drop_duplicates(cols, keep="last", inplace=True, ignore_index=True)
+        dfc.drop_duplicates(cols, keep="last", inplace=True, ignore_index=True)
 
         # Set company data frame
-        self._co_df = co_df
+        self._dfc = dfc
 
     def info(self) -> dict:
         """Print a concise summary of a company."""
+        # Some companies have no quarterly reports (see cvm_id 9784)
+        if self._last_quarterly is pd.NaT:
+            last_quarterly = "No quarterly reports"
         company_info = {
             "Name": self.name_id,
             "CVM ID": self._cvm_id,
             "Fiscal ID (CNPJ)": self.tax_id,
-            "Total Accounting Rows": len(self._co_df.index),
+            "Total Accounting Rows": len(self._dfc.index),
             "Selected Accounting Method": self._acc_method,
             "Selected Accounting Unit": self._acc_unit,
             "Selected Tax Rate": self._tax_rate,
             "First Annual Report": self._first_annual.strftime("%Y-%m-%d"),
             "Last Annual Report": self._last_annual.strftime("%Y-%m-%d"),
-            "Last Quarterly Report": self._last_quarterly.strftime("%Y-%m-%d"),
+            "Last Quarterly Report": last_quarterly,
         }
         print_dict(info_dict=company_info, table_name="Company Info")
-        return None
 
     def _build_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
         # keep only last quarterly fs
         if self._last_annual > self._last_quarterly:
             df = dfi.query('report_type == "ANNUAL"').copy()
             df.query(
                 "period_order == 'PREVIOUS' or \
@@ -323,15 +326,15 @@
             )
 
         # Create output dataframe with only the index
         dfo = df.sort_values(by="period_end", ascending=True)[
             ["acc_name", "acc_code", "acc_fixed"]
         ].drop_duplicates(subset="acc_code", ignore_index=True, keep="last")
 
-        periods = list(df["period_end"].sort_values().unique())
+        periods = sorted(df["period_end"].drop_duplicates())
         for period in periods:
             year_cols = ["acc_value", "acc_code"]
             df_year = df.query("period_end == @period")[year_cols].copy()
             period_str = period.strftime("%Y-%m-%d")
             if period == self._last_quarterly:
                 period_str += " (ttm)"
             df_year.rename(columns={"acc_value": period_str}, inplace=True)
@@ -373,15 +376,15 @@
         Raises:
             ValueError: If some argument is invalid.
         """
         # Check input arguments.
         if acc_level not in {None, 2, 3, 4}:
             raise ValueError("acc_level expects None, 2, 3 or 4")
 
-        df = self._co_df.copy()
+        df = self._dfc.copy()
 
         # Set language
         class MyDict(dict):
             """Custom dictionary class to return key if key is not found."""
 
             def __missing__(self, key):
                 return "(pt) " + key
```

### Comparing `finlogic-0.4.2/finlogic/cvm.py` & `finlogic-0.4.3/finlogic/cvm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module to download and process CVM data."""
 import re
-from typing import List, Dict
+from typing import List
 import zipfile as zf
 from pathlib import Path
 import duckdb
 import pandas as pd
 import requests
 from . import config as cfg
 
@@ -91,15 +91,15 @@
         child_df = pd.read_csv(child_zf, sep=";", encoding="iso-8859-1")
         df_list.append(child_df)
     df = pd.concat(df_list, ignore_index=True)
     return df
 
 
 def remove_empty_spaces(s: pd.Series) -> pd.Series:
-    """Remove empty spaces in a pandas Series of strings."""
+    """Remove empty spaces in a pandas Series of repeated strings."""
     s_unique_original = pd.Series(s.unique())
     s_unique_adjusted = s_unique_original.replace("\s+", " ", regex=True).str.strip()
     mapping_dict = dict(zip(s_unique_original, s_unique_adjusted))
     return s.map(mapping_dict)
 
 
 def process_df(df: pd.DataFrame, filepath: Path) -> pd.DataFrame:
@@ -142,14 +142,17 @@
     else:
         df.insert(loc=3, column="report_type", value="QUARTERLY")
 
     # Remove any extra spaces (line breaks, tabs, etc.) from columns below.
     columns = ["name_id", "acc_name", "equity_statement"]
     df[columns] = df[columns].apply(remove_empty_spaces)
 
+    # Replace "BCO " with "BANCO " in "name_id" column.
+    df["name_id"] = df["name_id"].str.replace("BCO ", "BANCO ")
+
     # Convert string columns to categorical before mapping.
     columns = df.select_dtypes(include="object").columns
     df[columns] = df[columns].astype("category")
 
     # "acc_fixed" values are: 'S', 'N'
     map_dic = {"S": True, "N": False}
     df["acc_fixed"] = df["acc_fixed"].map(map_dic).astype(bool)
@@ -230,15 +233,12 @@
     df = process_df(df, raw_filepath)
     processed_filepath = cfg.CVM_PROCESSED_DIR / (raw_filepath.stem + ".parquet")
     save_processed_df(df, processed_filepath)
     print(f"    {CHECKMARK} {raw_filepath.name} processed.")
     return processed_filepath
 
 
-def get_raw_files_mtime() -> Dict[str, float]:
-    """Return a dictionary with the files and their modification time."""
-    raw_filepaths = list(cfg.CVM_RAW_DIR.glob("*.zip"))
-    raw_filepaths.sort()
-    files_mtime = {}
-    for filepath in raw_filepaths:
-        files_mtime[filepath.name] = filepath.stat().st_mtime
-    return files_mtime
+def get_raw_file_mtimes() -> pd.DataFrame:
+    """Return a Pandas DataFrame with file_source and file_mtime columns."""
+    filepaths = sorted(cfg.CVM_RAW_DIR.glob("*.zip"))
+    d_mtimes = {filepath.name: filepath.stat().st_mtime for filepath in filepaths}
+    return pd.DataFrame(d_mtimes.items(), columns=["file_source", "file_mtime"])
```

### Comparing `finlogic-0.4.2/finlogic/database.py` & `finlogic-0.4.3/finlogic/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,57 +3,61 @@
 This module provides functions to handle financial data from the CVM Portal. It
 allows updating, processing and consolidating financial statements, as well as
 searching for company names in the FinLogic Database and retrieving information
 about the database itself.
 """
 from typing import Literal
 import pandas as pd
-from . import config as cfg
 from . import cvm
+from . import config as cfg
 from . import language as lng
 from . import finprint as fpr
 from . import fl_duckdb as fdb
 
 CHECKMARK = "\033[32m\u2714\033[0m"
 
 
 def get_filepaths_to_process() -> list[str]:
-    """Return a list of files in raw folder that must be processed."""
-    filenames_in_dir = cvm.get_raw_files_mtime()
-    filenames_in_db = fdb.get_db_files_mtime()
-    for key, value in filenames_in_db.items():
-        if key in filenames_in_dir and filenames_in_dir[key] == value:
-            del filenames_in_dir[key]
-    filenames_to_process = list(filenames_in_dir.keys())
-    return [cfg.CVM_RAW_DIR / filename for filename in filenames_to_process]
+    """Return a list of CVM files that has to be processed by comparing
+    the files mtimes from the raw folder with the database.
+    """
+    df_raw = cvm.get_raw_file_mtimes()
+    df_fdb = fdb.get_file_mtimes()
+    df_new = pd.concat([df_raw, df_fdb]).drop_duplicates(keep=False)
+    file_sources = set(df_new["file_source"])
+    return [cfg.CVM_RAW_DIR / file_source for file_source in file_sources]
 
 
-def update_database(reset: bool = False):
+def update_database(rebuild: bool = False):
     """Verify changes in CVM files and update Finlogic Database if necessary.
 
     Args:
-        reset (bool, optional): If True, delete the database file and create a
-            new one. Defaults to False.
+        rebuild (bool, optional): If True, processes all CVM files and rebuilds
+            the database. Defaults to False.
     Returns:
         None
     """
     # Language files
     print('\nUpdating "language" database...')
     lng.process_language_df()
 
     # CVM raw files
     print("Updating CVM files...")
     urls = cvm.get_all_file_urls()
-    # urls = urls[:1]  # Test
     updated_raw_filepaths = cvm.update_raw_files(urls)
     print(f"Number of CVM files updated = {len(updated_raw_filepaths)}")
 
     # CVM processed files
     print("\nProcessing CVM files...")
-    filepaths_to_process = get_filepaths_to_process()
+    if rebuild:
+        # Process all files
+        filepaths_to_process = sorted(cfg.CVM_RAW_DIR.glob("*.zip"))
+    else:
+        # Process only updated files
+        filepaths_to_process = get_filepaths_to_process()
     print(f"Number of new files to process = {len(filepaths_to_process)}")
     if filepaths_to_process:
         [cvm.process_file(filepath) for filepath in filepaths_to_process]
 
     # FinLogic Database
     fdb.build()
     print(f"\n{CHECKMARK} FinLogic Database updated!")
@@ -71,18 +75,18 @@
     Args:
         return_dict (bool, optional): If True, returns a dictionary with the
             database information and do not print it.
 
     Returns: None
     """
     info_dict = fdb.get_info()
-    if not info_dict:
-        print("FinLogic Database has no data.")
-        return
-    fpr.print_dict(info_dict=info_dict, table_name="FinLogic Database Info")
+    if info_dict:
+        fpr.print_dict(info_dict=info_dict, table_name="FinLogic Database Info")
+    else:
+        print("FinLogic Database is empty.")
 
 
 def search_company(
     search_value: str, search_by: Literal["name_id", "cvm_id", "tax_id"] = "name_id"
 ) -> pd.DataFrame:
     """Search for a company name in FinLogic Database.
 
@@ -108,14 +112,14 @@
         case "cvm_id":
             sql_condition = f"= {search_value}"
         case "tax_id":
             sql_condition = f"LIKE '%{search_value}%'"
         case _:
             raise ValueError("Invalid value for 'search_by' argument.")
 
-    query = f"""
+    query = f"""--sql
         SELECT DISTINCT name_id, cvm_id, tax_id
           FROM reports
          WHERE {search_by} {sql_condition}
          ORDER BY cvm_id;
     """
     return fdb.execute(query, "df")
```

### Comparing `finlogic-0.4.2/finlogic/finprint.py` & `finlogic-0.4.3/finlogic/finprint.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.2/finlogic/fl_duckdb.py` & `finlogic-0.4.3/finlogic/fl_duckdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """FinLogic Database module."""
-from typing import Dict, Literal
+from typing import Literal
 import duckdb
+import pandas as pd
 from datetime import datetime
 from . import config as cfg
 
 # Start FinLogic Database connection
 FINLOGIC_DB_PATH = cfg.DATA_PATH / "finlogic.db"
 # Create a new database file and connect to it
 con = duckdb.connect(database=f"{FINLOGIC_DB_PATH}")
@@ -53,28 +54,28 @@
 
 def get_info() -> dict:
     """Return a dictionary with information about the database."""
     info_dict = {}
     if is_empty():
         return info_dict
 
-    query = """
+    query = """--sql
         SELECT DISTINCT cvm_id, report_version, report_type, period_reference
           FROM reports;
     """
+    num_of_reports = execute(query, "df").shape[0]
     db_last_modified = datetime.fromtimestamp(FINLOGIC_DB_PATH.stat().st_mtime)
     query = "SELECT COUNT(*) FROM reports"
-    number_of_rows = execute(query, "fetchall")[0][0]
-    num_of_reports = execute(query, "df").shape[0]
+    number_of_rows = execute(query, "fetchone")[0]
     query = "SELECT MIN(period_end) FROM reports"
-    first_statement = execute(query, "fetchall")[0][0]
+    first_statement = execute(query, "fetchone")[0]
     query = "SELECT MAX(period_end) FROM reports"
-    last_statement = execute(query, "fetchall")[0][0]
+    last_statement = execute(query, "fetchone")[0]
     query = "SELECT COUNT(DISTINCT cvm_id) FROM reports"
-    number_of_companies = execute(query, "fetchall")[0][0]
+    number_of_companies = execute(query, "fetchone")[0]
 
     info_dict = {
         "db_path": f"{FINLOGIC_DB_PATH}",
         "db_size": f"{FINLOGIC_DB_PATH.stat().st_size / 1024**2:.2f} MB",
         "db_last_modified": db_last_modified.strftime("%Y-%m-%d %H:%M:%S"),
         "number_of_rows": number_of_rows,
         "number_of_reports": num_of_reports,
@@ -82,19 +83,18 @@
         "first_report": f"{first_statement}",
         "last_report": f"{last_statement}",
     }
 
     return info_dict
 
 
-def get_db_files_mtime() -> Dict[str, float]:
-    """Return a dictionary with the file sources and their respective modified times in
-    database."""
+def get_file_mtimes() -> pd.DataFrame:
+    """Return a Pandas DataFrame with unique file_source and file_mtime."""
     if is_empty():
-        return {}
+        return pd.DataFrame()
 
     sql = """
-        SELECT DISTINCT file_source, file_mtime FROM reports
-        ORDER BY file_source
+        SELECT DISTINCT file_source, file_mtime
+          FROM reports
+         ORDER BY file_source
     """
-    df = execute(sql, "df")
-    return df.set_index("file_source")["file_mtime"].to_dict()
+    return execute(sql, "df")
```

### Comparing `finlogic-0.4.2/finlogic/language.py` & `finlogic-0.4.3/finlogic/language.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.2/pyproject.toml` & `finlogic-0.4.3/pyproject.toml`

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
-version = "0.4.2"
+version = "0.4.3"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.0.0",
```

### Comparing `finlogic-0.4.2/tests/test_company.py` & `finlogic-0.4.3/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.2/tests/test_database.py` & `finlogic-0.4.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.2/PKG-INFO` & `finlogic-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.4.2
+Version: 0.4.3
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -47,15 +47,15 @@
 
 <!-- [![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic)" -->
 
 ## FinLogic: finance toolkit for listed Brazilian companies.
 
 ---
 
-**FinLogic** offers a Pythonic way to analyze financial data of listed companies in Brazil from information made publicly avaible by local securities market authority (CVM). FinLogic uses DuckDB as an OLAP database management system and Pandas to process the data to and from the locally builted accounting database (aprox. 21 million rows).
+**FinLogic** offers a Pythonic way to analyze financial data of listed companies in Brazil from information made publicly avaible by local securities market authority (CVM). FinLogic uses DuckDB as an OLAP database management system and Pandas to process the data to and from the locally builted accounting database (aprox. 8 million rows).
 
 ---
 
 ## Installation
 
 The source code is currently hosted on GitHub at:
 https://github.com/crdcj/FinLogic
```


# Comparing `tmp/cvxsimulator-0.3.2.tar.gz` & `tmp/cvxsimulator-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.3.2.tar", max compression
+gzip compressed data, was "cvxsimulator-0.3.3.tar", max compression
```

## Comparing `cvxsimulator-0.3.2.tar` & `cvxsimulator-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1102 2023-05-15 16:53:35.626777 cvxsimulator-0.3.2/LICENSE
--rw-r--r--   0        0        0     4907 2023-05-15 16:53:35.626777 cvxsimulator-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     3796 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1163 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1341 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/month.py
--rw-r--r--   0        0        0     4307 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      596 2023-05-15 16:53:59.707195 cvxsimulator-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 cvxsimulator-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-17 06:36:29.470680 cvxsimulator-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4907 2023-05-17 06:36:29.470680 cvxsimulator-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     6722 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1163 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1422 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/month.py
+-rw-r--r--   0        0        0    14504 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      596 2023-05-17 06:37:03.414800 cvxsimulator-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 cvxsimulator-0.3.3/PKG-INFO
```

### Comparing `cvxsimulator-0.3.2/LICENSE` & `cvxsimulator-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.2/README.md` & `cvxsimulator-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.2/cvx/simulator/metrics.py` & `cvxsimulator-0.3.3/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.2/cvx/simulator/month.py` & `cvxsimulator-0.3.3/cvx/simulator/month.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,47 +5,45 @@
 from __future__ import annotations
 
 import calendar
 
 import numpy as np
 import pandas as pd
 
+def _compound(rets):
+    """
+    Helper function for compounded return calculation.
+    """
+    return (1.0 + rets).prod() - 1.0
+
 
 def monthlytable(returns: pd.Series):
     """
     Get a table of monthly returns.
 
     Args:
         returns: Series of individual returns.
 
     Returns:
         DataFrame with monthly returns, their STDev and YTD.
     """
 
-    def _compound(rets):
-        """
-        Helper function for compounded return calculation.
-
-        Args:
-            rets: Series of individual returns.
-
-        Returns:
-            Series of compounded returns.
-        """
-        return (1.0 + rets).prod() - 1.0
-
     # Works better in the first month
     # Compute all the intramonth-returns, instead of reapplying some monthly resampling of the NAV
+    returns = returns.dropna()
+
     return_monthly = returns.groupby([returns.index.year, returns.index.month]).apply(
         _compound
-    )
+    ).unstack(level=1)
+
+    # make sure all months are in the table!
+    frame = pd.DataFrame(index=return_monthly.index, columns=range(1, 13), data=np.NaN)
+    frame[return_monthly.columns] = return_monthly
 
-    frame = return_monthly.unstack(level=1).rename(
-        columns=lambda x: calendar.month_abbr[x]
-    )
+    frame = frame.rename(columns={month: calendar.month_abbr[month] for month in frame.columns})
 
     ytd = frame.apply(_compound, axis=1)
     frame["STDev"] = np.sqrt(12) * frame.std(axis=1)
     # make sure that you don't include the column for the STDev in your computation
     frame["YTD"] = ytd
     frame.index.name = "Year"
     frame.columns.name = None
```

### Comparing `cvxsimulator-0.3.2/pyproject.toml` & `cvxsimulator-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.3.2"
+version = "v0.3.3"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.3.2/PKG-INFO` & `cvxsimulator-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.3.2
+Version: 0.3.3
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


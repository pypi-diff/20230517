# Comparing `tmp/bias_adjustment-1.0.2.tar.gz` & `tmp/bias_adjustment-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bias_adjustment-1.0.2.tar", max compression
+gzip compressed data, was "bias_adjustment-1.0.3.tar", max compression
```

## Comparing `bias_adjustment-1.0.2.tar` & `bias_adjustment-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-10 14:11:11.340594 bias_adjustment-1.0.2/LICENSE
--rw-r--r--   0        0        0      274 2022-11-15 06:42:37.967412 bias_adjustment-1.0.2/README.md
--rw-r--r--   0        0        0      705 2023-05-10 14:11:11.341594 bias_adjustment-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      205 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/__init__.py
--rw-r--r--   0        0        0     2401 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/bias_adjustment.py
--rw-r--r--   0        0        0       97 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/distributions/__init__.py
--rw-r--r--   0        0        0     5089 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/distributions/distributions.py
--rw-r--r--   0        0        0      300 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/__init__.py
--rw-r--r--   0        0        0     1264 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/dqm.py
--rw-r--r--   0        0        0     1018 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/qdm.py
--rw-r--r--   0        0        0     1870 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/qm.py
--rw-r--r--   0        0        0      376 2023-05-10 14:11:11.362595 bias_adjustment-1.0.2/src/bias_adjustment/utils.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 bias_adjustment-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-10 14:11:11.340594 bias_adjustment-1.0.3/LICENSE
+-rw-r--r--   0        0        0      274 2022-11-15 06:42:37.967412 bias_adjustment-1.0.3/README.md
+-rw-r--r--   0        0        0      705 2023-05-17 05:03:44.704870 bias_adjustment-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      205 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/__init__.py
+-rw-r--r--   0        0        0     2443 2023-05-17 03:07:09.528586 bias_adjustment-1.0.3/src/bias_adjustment/bias_adjustment.py
+-rw-r--r--   0        0        0       37 2023-05-17 03:12:37.290749 bias_adjustment-1.0.3/src/bias_adjustment/const.py
+-rw-r--r--   0        0        0       97 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/distributions/__init__.py
+-rw-r--r--   0        0        0     5089 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/distributions/distributions.py
+-rw-r--r--   0        0        0      300 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/__init__.py
+-rw-r--r--   0        0        0     1264 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/dqm.py
+-rw-r--r--   0        0        0     1018 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/qdm.py
+-rw-r--r--   0        0        0     2554 2023-05-17 05:05:23.303464 bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/qm.py
+-rw-r--r--   0        0        0      647 2023-05-17 03:56:00.857244 bias_adjustment-1.0.3/src/bias_adjustment/utils.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 bias_adjustment-1.0.3/PKG-INFO
```

### Comparing `bias_adjustment-1.0.2/LICENSE` & `bias_adjustment-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.2/pyproject.toml` & `bias_adjustment-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bias-adjustment"
-version = "1.0.2"
+version = "1.0.3"
 description = "Bias Adjusment by Quantile Mapping"
 authors = ["Emilio Gozo <emiliogozo@proton.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/emiliogozo/bias_adjustment"
 keywords = ["climatology", "data analysis", "quantile mapping", "bias correction"]
 packages = [{include = "bias_adjustment", from = "src"}]
```

### Comparing `bias_adjustment-1.0.2/src/bias_adjustment/bias_adjustment.py` & `bias_adjustment-1.0.3/src/bias_adjustment/bias_adjustment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 
+from bias_adjustment.const import MAX_CDF
 from bias_adjustment.quantile_mapping import (
     DetrendedQuantileMapping,
     QuantileDeltaMapping,
     QuantileMapping,
 )
 from bias_adjustment.utils import FloatNDArray, is_float_ndarray
 
@@ -15,15 +16,15 @@
     return
 
 
 @dataclass
 class BiasAdjustment:
     obs: FloatNDArray
     mod: FloatNDArray
-    max_cdf: float = 0.99999
+    max_cdf: float = MAX_CDF
 
     def __post_init__(self):
         for name in ["obs", "mod"]:
             attr = getattr(self, name)
             if not is_float_ndarray(attr):
                 raise TypeError(f"`{name}` is not a numpy array.")
             min_len = 10
```

### Comparing `bias_adjustment-1.0.2/src/bias_adjustment/distributions/distributions.py` & `bias_adjustment-1.0.3/src/bias_adjustment/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/dqm.py` & `bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/dqm.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/qdm.py` & `bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/qdm.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.2/PKG-INFO` & `bias_adjustment-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bias-adjustment
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bias Adjusment by Quantile Mapping
 Home-page: https://github.com/emiliogozo/bias_adjustment
 License: MIT
 Keywords: climatology,data analysis,quantile mapping,bias correction
 Author: Emilio Gozo
 Author-email: emiliogozo@proton.me
 Requires-Python: >=3.8.1,<3.9
```


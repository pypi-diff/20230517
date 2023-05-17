# Comparing `tmp/bias_adjustment-1.0.3.tar.gz` & `tmp/bias_adjustment-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bias_adjustment-1.0.3.tar", max compression
+gzip compressed data, was "bias_adjustment-1.0.4.tar", max compression
```

## Comparing `bias_adjustment-1.0.3.tar` & `bias_adjustment-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-10 14:11:11.340594 bias_adjustment-1.0.3/LICENSE
--rw-r--r--   0        0        0      274 2022-11-15 06:42:37.967412 bias_adjustment-1.0.3/README.md
--rw-r--r--   0        0        0      705 2023-05-17 05:03:44.704870 bias_adjustment-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      205 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/__init__.py
--rw-r--r--   0        0        0     2443 2023-05-17 03:07:09.528586 bias_adjustment-1.0.3/src/bias_adjustment/bias_adjustment.py
--rw-r--r--   0        0        0       37 2023-05-17 03:12:37.290749 bias_adjustment-1.0.3/src/bias_adjustment/const.py
--rw-r--r--   0        0        0       97 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/distributions/__init__.py
--rw-r--r--   0        0        0     5089 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/distributions/distributions.py
--rw-r--r--   0        0        0      300 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/__init__.py
--rw-r--r--   0        0        0     1264 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/dqm.py
--rw-r--r--   0        0        0     1018 2023-05-10 14:11:11.361595 bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/qdm.py
--rw-r--r--   0        0        0     2554 2023-05-17 05:05:23.303464 bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/qm.py
--rw-r--r--   0        0        0      647 2023-05-17 03:56:00.857244 bias_adjustment-1.0.3/src/bias_adjustment/utils.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 bias_adjustment-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-10 14:11:11.340594 bias_adjustment-1.0.4/LICENSE
+-rw-r--r--   0        0        0      274 2022-11-15 06:42:37.967412 bias_adjustment-1.0.4/README.md
+-rw-r--r--   0        0        0      705 2023-05-17 05:28:09.092888 bias_adjustment-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      205 2023-05-10 14:11:11.361595 bias_adjustment-1.0.4/src/bias_adjustment/__init__.py
+-rw-r--r--   0        0        0     2443 2023-05-17 03:07:09.528586 bias_adjustment-1.0.4/src/bias_adjustment/bias_adjustment.py
+-rw-r--r--   0        0        0       37 2023-05-17 03:12:37.290749 bias_adjustment-1.0.4/src/bias_adjustment/const.py
+-rw-r--r--   0        0        0       97 2023-05-10 14:11:11.361595 bias_adjustment-1.0.4/src/bias_adjustment/distributions/__init__.py
+-rw-r--r--   0        0        0     5089 2023-05-10 14:11:11.361595 bias_adjustment-1.0.4/src/bias_adjustment/distributions/distributions.py
+-rw-r--r--   0        0        0      300 2023-05-10 14:11:11.361595 bias_adjustment-1.0.4/src/bias_adjustment/quantile_mapping/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-17 05:20:35.485008 bias_adjustment-1.0.4/src/bias_adjustment/quantile_mapping/dqm.py
+-rw-r--r--   0        0        0     1206 2023-05-17 05:23:57.053434 bias_adjustment-1.0.4/src/bias_adjustment/quantile_mapping/qdm.py
+-rw-r--r--   0        0        0     2779 2023-05-17 05:18:00.598322 bias_adjustment-1.0.4/src/bias_adjustment/quantile_mapping/qm.py
+-rw-r--r--   0        0        0      647 2023-05-17 03:56:00.857244 bias_adjustment-1.0.4/src/bias_adjustment/utils.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 bias_adjustment-1.0.4/PKG-INFO
```

### Comparing `bias_adjustment-1.0.3/LICENSE` & `bias_adjustment-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.3/pyproject.toml` & `bias_adjustment-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bias-adjustment"
-version = "1.0.3"
+version = "1.0.4"
 description = "Bias Adjusment by Quantile Mapping"
 authors = ["Emilio Gozo <emiliogozo@proton.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/emiliogozo/bias_adjustment"
 keywords = ["climatology", "data analysis", "quantile mapping", "bias correction"]
 packages = [{include = "bias_adjustment", from = "src"}]
```

### Comparing `bias_adjustment-1.0.3/src/bias_adjustment/bias_adjustment.py` & `bias_adjustment-1.0.4/src/bias_adjustment/bias_adjustment.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.3/src/bias_adjustment/distributions/distributions.py` & `bias_adjustment-1.0.4/src/bias_adjustment/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/dqm.py` & `bias_adjustment-1.0.4/src/bias_adjustment/quantile_mapping/dqm.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,20 +18,25 @@
             return dat_mean - mod_mean
         return None
 
     def compute(
         self,
         mode: BAMode = "rel",
         dist_type="hist",
+        ignore_trace: bool = False,
     ) -> FloatNDArray:
         if mode not in get_args(BAMode):
             raise ValueError(f"Length of `mode` must be {get_args(BAMode)}.")
 
-        o_dist = self.generate_distribution(self.obs, dist_type)
-        m_dist = self.generate_distribution(self.mod, dist_type)
+        o_dist = self.generate_distribution(
+            self.obs, dist_type, ignore_trace, self.trace_val
+        )
+        m_dist = self.generate_distribution(
+            self.mod, dist_type, ignore_trace, self.trace_val
+        )
 
         delta = self.delta(mode)
         if mode == "rel":
             m_cdf = np.minimum(self.max_cdf, m_dist.cdf(self.data / delta))
             return o_dist.ppf(m_cdf) * delta
         elif mode == "abs":
             m_cdf = np.minimum(self.max_cdf, m_dist.cdf(self.data - delta))
```

### Comparing `bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/qdm.py` & `bias_adjustment-1.0.4/src/bias_adjustment/quantile_mapping/qdm.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,23 +9,29 @@
 
 @dataclass
 class QuantileDeltaMapping(QuantileMapping):
     def compute(
         self,
         mode: BAMode = "rel",
         dist_type="hist",
+        ignore_trace: bool = False,
     ) -> FloatNDArray:
         if mode not in get_args(BAMode):
             raise ValueError(f"Length of `mode` must be {get_args(BAMode)}.")
 
-        o_dist = self.generate_distribution(self.obs, dist_type)
-        mh_dist = self.generate_distribution(self.mod, dist_type)
-        mf_dist = self.generate_distribution(self.data, dist_type)
+        o_dist = self.generate_distribution(
+            self.obs, dist_type, ignore_trace, self.trace_val
+        )
+        mh_dist = self.generate_distribution(
+            self.mod, dist_type, ignore_trace, self.trace_val
+        )
+        mf_dist = self.generate_distribution(
+            self.data, dist_type, ignore_trace, self.trace_val
+        )
 
         mf_cdf = np.minimum(self.max_cdf, mf_dist.cdf(self.data))
 
         if mode == "rel":  # Relative
             return o_dist.ppf(mf_cdf) * (self.data / mh_dist.ppf(mf_cdf))
         elif mode == "abs":  # Absolute
             return o_dist.ppf(mf_cdf) + self.data - mh_dist.ppf(mf_cdf)
-        else:
-            return None
+        return o_dist.ppf(mf_cdf)
```

### Comparing `bias_adjustment-1.0.3/src/bias_adjustment/quantile_mapping/qm.py` & `bias_adjustment-1.0.4/src/bias_adjustment/quantile_mapping/qm.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,21 +54,27 @@
         else:
             _data = data.copy()
         return Distributions(_data).fit(dist_type)
 
     def compute(
         self,
         dist_type="hist",
+        ignore_trace: bool = False,
     ) -> FloatNDArray:
         """Adjust the bias
 
         Args:
             dist_type (str, optional): Valid scipy.stats distribution name. Defaults to "hist".
+            ignore_trace (bool, optional): Ignore trace values? Defaults to "False".
 
         Returns:
             FloatNDArray: The adjusted values.
         """
-        o_dist = self.generate_distribution(self.obs, dist_type)
-        m_dist = self.generate_distribution(self.mod, dist_type)
+        o_dist = self.generate_distribution(
+            self.obs, dist_type, ignore_trace, self.trace_val
+        )
+        m_dist = self.generate_distribution(
+            self.mod, dist_type, ignore_trace, self.trace_val
+        )
 
         m_cdf = np.minimum(self.max_cdf, m_dist.cdf(self.data))
         return o_dist.ppf(m_cdf)
```

### Comparing `bias_adjustment-1.0.3/src/bias_adjustment/utils.py` & `bias_adjustment-1.0.4/src/bias_adjustment/utils.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.3/PKG-INFO` & `bias_adjustment-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bias-adjustment
-Version: 1.0.3
+Version: 1.0.4
 Summary: Bias Adjusment by Quantile Mapping
 Home-page: https://github.com/emiliogozo/bias_adjustment
 License: MIT
 Keywords: climatology,data analysis,quantile mapping,bias correction
 Author: Emilio Gozo
 Author-email: emiliogozo@proton.me
 Requires-Python: >=3.8.1,<3.9
```


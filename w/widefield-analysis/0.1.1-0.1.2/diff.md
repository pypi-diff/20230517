# Comparing `tmp/widefield_analysis-0.1.1.tar.gz` & `tmp/widefield_analysis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widefield_analysis-0.1.1.tar", max compression
+gzip compressed data, was "widefield_analysis-0.1.2.tar", max compression
```

## Comparing `widefield_analysis-0.1.1.tar` & `widefield_analysis-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       55 2023-03-28 09:53:25.190532 widefield_analysis-0.1.1/README.md
--rw-r--r--   0        0        0      497 2023-03-31 13:15:37.073249 widefield_analysis-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 08:46:58.435982 widefield_analysis-0.1.1/widefield_analysis/__init__.py
--rw-r--r--   0        0        0     3364 2023-03-31 13:15:08.809441 widefield_analysis-0.1.1/widefield_analysis/animation.py
--rw-r--r--   0        0        0     1405 2023-03-28 09:06:15.591145 widefield_analysis-0.1.1/widefield_analysis/filter.py
--rw-r--r--   0        0        0      739 2023-03-31 09:51:47.977442 widefield_analysis-0.1.1/widefield_analysis/resample.py
--rw-r--r--   0        0        0      832 2023-03-28 09:15:07.411967 widefield_analysis-0.1.1/widefield_analysis/smooth.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 widefield_analysis-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-03-28 09:53:25.190532 widefield_analysis-0.1.2/README.md
+-rw-r--r--   0        0        0      497 2023-05-17 10:08:31.435369 widefield_analysis-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 08:46:58.435982 widefield_analysis-0.1.2/widefield_analysis/__init__.py
+-rw-r--r--   0        0        0     3364 2023-03-31 13:15:08.809441 widefield_analysis-0.1.2/widefield_analysis/animation.py
+-rw-r--r--   0        0        0     4142 2023-05-10 08:26:55.916576 widefield_analysis-0.1.2/widefield_analysis/files.py
+-rw-r--r--   0        0        0     1405 2023-03-28 09:06:15.591145 widefield_analysis-0.1.2/widefield_analysis/filter.py
+-rw-r--r--   0        0        0      739 2023-03-31 09:51:47.977442 widefield_analysis-0.1.2/widefield_analysis/resample.py
+-rw-r--r--   0        0        0      832 2023-03-28 09:15:07.411967 widefield_analysis-0.1.2/widefield_analysis/smooth.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 widefield_analysis-0.1.2/PKG-INFO
```

### Comparing `widefield_analysis-0.1.1/widefield_analysis/animation.py` & `widefield_analysis-0.1.2/widefield_analysis/animation.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.1/widefield_analysis/filter.py` & `widefield_analysis-0.1.2/widefield_analysis/filter.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.1/widefield_analysis/resample.py` & `widefield_analysis-0.1.2/widefield_analysis/resample.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.1/widefield_analysis/smooth.py` & `widefield_analysis-0.1.2/widefield_analysis/smooth.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.1/PKG-INFO` & `widefield_analysis-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: widefield-analysis
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Mathis
 Author-email: mathis.bassler@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
```


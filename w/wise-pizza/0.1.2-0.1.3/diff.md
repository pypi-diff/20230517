# Comparing `tmp/wise-pizza-0.1.2.tar.gz` & `tmp/wise-pizza-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-pizza-0.1.2.tar", last modified: Tue May 16 08:39:14 2023, max compression
+gzip compressed data, was "wise-pizza-0.1.3.tar", last modified: Wed May 17 08:39:06 2023, max compression
```

## Comparing `wise-pizza-0.1.2.tar` & `wise-pizza-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-16 08:39:14.928177 wise-pizza-0.1.2/
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/LICENSE
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5960 2023-05-16 08:39:14.927897 wise-pizza-0.1.2/PKG-INFO
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     5434 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/README.md
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      220 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/pyproject.toml
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-05-16 08:39:14.928259 wise-pizza-0.1.2/setup.cfg
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-05-16 08:33:11.000000 wise-pizza-0.1.2/setup.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-16 08:39:14.920141 wise-pizza-0.1.2/wise_pizza/
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      118 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/__init__.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    11404 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/explain.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/find_alpha.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3799 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/make_matrix.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8974 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/plotting.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      518 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/segment_data.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/slicer.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/solver.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/utils.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-16 08:39:14.927497 wise-pizza-0.1.2/wise_pizza.egg-info/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5960 2023-05-16 08:39:14.000000 wise-pizza-0.1.2/wise_pizza.egg-info/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-05-16 08:39:14.000000 wise-pizza-0.1.2/wise_pizza.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-05-16 08:39:14.000000 wise-pizza-0.1.2/wise_pizza.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-05-16 08:39:14.000000 wise-pizza-0.1.2/wise_pizza.egg-info/requires.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-05-16 08:39:14.000000 wise-pizza-0.1.2/wise_pizza.egg-info/top_level.txt
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-17 08:39:06.047671 wise-pizza-0.1.3/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/LICENSE
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-05-17 08:39:06.046801 wise-pizza-0.1.3/PKG-INFO
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/README.md
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      220 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/pyproject.toml
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-05-17 08:39:06.047910 wise-pizza-0.1.3/setup.cfg
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-05-17 08:18:02.000000 wise-pizza-0.1.3/setup.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-17 08:39:06.030587 wise-pizza-0.1.3/wise_pizza/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      118 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/wise_pizza/__init__.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    11404 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/wise_pizza/explain.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/wise_pizza/find_alpha.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3799 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/wise_pizza/make_matrix.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8974 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/wise_pizza/plotting.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      518 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/wise_pizza/segment_data.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/wise_pizza/slicer.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/wise_pizza/solver.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-05-17 08:36:49.000000 wise-pizza-0.1.3/wise_pizza/utils.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-17 08:39:06.045430 wise-pizza-0.1.3/wise_pizza.egg-info/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-05-17 08:39:05.000000 wise-pizza-0.1.3/wise_pizza.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-05-17 08:39:05.000000 wise-pizza-0.1.3/wise_pizza.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-05-17 08:39:05.000000 wise-pizza-0.1.3/wise_pizza.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-05-17 08:39:05.000000 wise-pizza-0.1.3/wise_pizza.egg-info/requires.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-05-17 08:39:05.000000 wise-pizza-0.1.3/wise_pizza.egg-info/top_level.txt
```

### Comparing `wise-pizza-0.1.2/LICENSE` & `wise-pizza-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.2/PKG-INFO` & `wise-pizza-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,11 @@
-Metadata-Version: 2.1
-Name: wise-pizza
-Version: 0.1.2
-Summary: A library to find and visualise the most interesting slices in multidimensional data
-Home-page: https://github.com/transferwise/wise-pizza
-Author: Wise
-Keywords: wise-pizza
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
+<img src="https://github.com/transferwise/wise-pizza/blob/main/docs/Wise_Logo.png?raw=True" width=10% height=10%>
 
 # Wise Pizza: A library for automated figuring out most unusual segments
 
-<img src="./docs/Wise_Logo.png" width=50% height=50%>
-
 **WisePizza** is a library to find and visualise the most interesting slices in multidimensional data based on Lasso and LP solvers, which provides different functions to find segments whose average is most different from the global one or find segments most useful in explaining the difference between two datasets.
 
 ## The approach
 WisePizza assumes you have a dataset with a number of discrete *dimensions* (could be currency, region, etc). For each
 combination of dimensions, the dataset must have a *total* value (total of the metric over that segment, for example
 the total volume in that region and currency), and an optional *size* value (set to 1 if not specified), this could for
 example be the total number of customers for that region and currency. The *average* value of the outcome for the segment
@@ -94,15 +79,15 @@
     size_name=size,
     max_depth=2,
     min_segments=20,
     solver="lasso"
 )
 ```
 
-![plot](./docs/explain_levels.png)
+![plot](https://github.com/transferwise/wise-pizza/blob/main/docs/explain_levels.png?raw=True)
 
 Or for finding changes between two datasets in totals:
 
 ```Python
 sf1 = explain_changes_in_totals(
     df1=pre_data,
     df2=data,
@@ -112,15 +97,15 @@
     max_depth=2,
     min_segments=20,
     how="totals",
     solver="lasso"
 )
 ```
 
-![plot](./docs/explain_changes_in_totals.png)
+![plot](https://github.com/transferwise/wise-pizza/blob/main/docs/explain_changes_in_totals.png?raw=True)
 
 Or for finding changes between two datasets in average:
 
 ```Python
 sf1 = explain_changes_in_average(
     df1=pre_data,
     df2=data,
@@ -130,15 +115,15 @@
     max_depth=2,
     min_segments=20,
     how="totals",
     solver="lasso"
 )
 ```
 
-![plot](./docs/explain_changes_in_average(totals).png)
+![plot](https://github.com/transferwise/wise-pizza/blob/main/docs/explain_changes_in_average(totals).png?raw=True)
 
 And then you can visualize differences:
 
 ```Python
 sf.plot()
 ```
 
@@ -148,11 +133,13 @@
 sf.segments
 ```
 Please see the full example [here](https://github.com/transferwise/wise-pizza/blob/main/notebooks/Finding%20interesting%20segments.ipynb)
 
 ## For Developers
 
 
-Wise-pizza is open sourced and maintained by Wise Plc. Copyright 2023 Wise Plc.
+
 
 ### Testing
 We use [PyTest](https://docs.pytest.org/) for testing. If you want to contribute code, make sure that the tests in tests/ run without errors.
+
+*Wise-pizza is open sourced and maintained by Wise Plc. Copyright 2023 Wise Plc.*
```

### Comparing `wise-pizza-0.1.2/README.md` & `wise-pizza-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,25 @@
-# Wise Pizza: A library for automated figuring out most unusual segments
+Metadata-Version: 2.1
+Name: wise-pizza
+Version: 0.1.3
+Summary: A library to find and visualise the most interesting slices in multidimensional data
+Home-page: https://github.com/transferwise/wise-pizza
+Author: Wise
+Keywords: wise-pizza
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+<img src="https://github.com/transferwise/wise-pizza/blob/main/docs/Wise_Logo.png?raw=True" width=10% height=10%>
 
-<img src="./docs/Wise_Logo.png" width=50% height=50%>
+# Wise Pizza: A library for automated figuring out most unusual segments
 
 **WisePizza** is a library to find and visualise the most interesting slices in multidimensional data based on Lasso and LP solvers, which provides different functions to find segments whose average is most different from the global one or find segments most useful in explaining the difference between two datasets.
 
 ## The approach
 WisePizza assumes you have a dataset with a number of discrete *dimensions* (could be currency, region, etc). For each
 combination of dimensions, the dataset must have a *total* value (total of the metric over that segment, for example
 the total volume in that region and currency), and an optional *size* value (set to 1 if not specified), this could for
@@ -79,15 +94,15 @@
     size_name=size,
     max_depth=2,
     min_segments=20,
     solver="lasso"
 )
 ```
 
-![plot](./docs/explain_levels.png)
+![plot](https://github.com/transferwise/wise-pizza/blob/main/docs/explain_levels.png?raw=True)
 
 Or for finding changes between two datasets in totals:
 
 ```Python
 sf1 = explain_changes_in_totals(
     df1=pre_data,
     df2=data,
@@ -97,15 +112,15 @@
     max_depth=2,
     min_segments=20,
     how="totals",
     solver="lasso"
 )
 ```
 
-![plot](./docs/explain_changes_in_totals.png)
+![plot](https://github.com/transferwise/wise-pizza/blob/main/docs/explain_changes_in_totals.png?raw=True)
 
 Or for finding changes between two datasets in average:
 
 ```Python
 sf1 = explain_changes_in_average(
     df1=pre_data,
     df2=data,
@@ -115,15 +130,15 @@
     max_depth=2,
     min_segments=20,
     how="totals",
     solver="lasso"
 )
 ```
 
-![plot](./docs/explain_changes_in_average(totals).png)
+![plot](https://github.com/transferwise/wise-pizza/blob/main/docs/explain_changes_in_average(totals).png?raw=True)
 
 And then you can visualize differences:
 
 ```Python
 sf.plot()
 ```
 
@@ -133,11 +148,13 @@
 sf.segments
 ```
 Please see the full example [here](https://github.com/transferwise/wise-pizza/blob/main/notebooks/Finding%20interesting%20segments.ipynb)
 
 ## For Developers
 
 
-Wise-pizza is open sourced and maintained by Wise Plc. Copyright 2023 Wise Plc.
+
 
 ### Testing
 We use [PyTest](https://docs.pytest.org/) for testing. If you want to contribute code, make sure that the tests in tests/ run without errors.
+
+*Wise-pizza is open sourced and maintained by Wise Plc. Copyright 2023 Wise Plc.*
```

### Comparing `wise-pizza-0.1.2/setup.py` & `wise-pizza-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="wise-pizza",
-    version="0.1.2",
+    version="0.1.3",
     description="A library to find and visualise the most interesting slices in multidimensional data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Wise",
     url='https://github.com/transferwise/wise-pizza',
     classifiers=[
         'Programming Language :: Python :: 3 :: Only',
```

### Comparing `wise-pizza-0.1.2/wise_pizza/explain.py` & `wise-pizza-0.1.3/wise_pizza/explain.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.2/wise_pizza/find_alpha.py` & `wise-pizza-0.1.3/wise_pizza/find_alpha.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.2/wise_pizza/make_matrix.py` & `wise-pizza-0.1.3/wise_pizza/make_matrix.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.2/wise_pizza/plotting.py` & `wise-pizza-0.1.3/wise_pizza/plotting.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.2/wise_pizza/segment_data.py` & `wise-pizza-0.1.3/wise_pizza/segment_data.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.2/wise_pizza/slicer.py` & `wise-pizza-0.1.3/wise_pizza/slicer.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.2/wise_pizza/solver.py` & `wise-pizza-0.1.3/wise_pizza/solver.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.2/wise_pizza/utils.py` & `wise-pizza-0.1.3/wise_pizza/utils.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.2/wise_pizza.egg-info/PKG-INFO` & `wise-pizza-0.1.3/wise_pizza.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# Wise Pizza: A library for automated figuring out most unusual segments
+<img src="https://github.com/transferwise/wise-pizza/blob/main/docs/Wise_Logo.png?raw=True" width=10% height=10%>
 
-<img src="./docs/Wise_Logo.png" width=50% height=50%>
+# Wise Pizza: A library for automated figuring out most unusual segments
 
 **WisePizza** is a library to find and visualise the most interesting slices in multidimensional data based on Lasso and LP solvers, which provides different functions to find segments whose average is most different from the global one or find segments most useful in explaining the difference between two datasets.
 
 ## The approach
 WisePizza assumes you have a dataset with a number of discrete *dimensions* (could be currency, region, etc). For each
 combination of dimensions, the dataset must have a *total* value (total of the metric over that segment, for example
 the total volume in that region and currency), and an optional *size* value (set to 1 if not specified), this could for
@@ -94,15 +94,15 @@
     size_name=size,
     max_depth=2,
     min_segments=20,
     solver="lasso"
 )
 ```
 
-![plot](./docs/explain_levels.png)
+![plot](https://github.com/transferwise/wise-pizza/blob/main/docs/explain_levels.png?raw=True)
 
 Or for finding changes between two datasets in totals:
 
 ```Python
 sf1 = explain_changes_in_totals(
     df1=pre_data,
     df2=data,
@@ -112,15 +112,15 @@
     max_depth=2,
     min_segments=20,
     how="totals",
     solver="lasso"
 )
 ```
 
-![plot](./docs/explain_changes_in_totals.png)
+![plot](https://github.com/transferwise/wise-pizza/blob/main/docs/explain_changes_in_totals.png?raw=True)
 
 Or for finding changes between two datasets in average:
 
 ```Python
 sf1 = explain_changes_in_average(
     df1=pre_data,
     df2=data,
@@ -130,15 +130,15 @@
     max_depth=2,
     min_segments=20,
     how="totals",
     solver="lasso"
 )
 ```
 
-![plot](./docs/explain_changes_in_average(totals).png)
+![plot](https://github.com/transferwise/wise-pizza/blob/main/docs/explain_changes_in_average(totals).png?raw=True)
 
 And then you can visualize differences:
 
 ```Python
 sf.plot()
 ```
 
@@ -148,11 +148,13 @@
 sf.segments
 ```
 Please see the full example [here](https://github.com/transferwise/wise-pizza/blob/main/notebooks/Finding%20interesting%20segments.ipynb)
 
 ## For Developers
 
 
-Wise-pizza is open sourced and maintained by Wise Plc. Copyright 2023 Wise Plc.
+
 
 ### Testing
 We use [PyTest](https://docs.pytest.org/) for testing. If you want to contribute code, make sure that the tests in tests/ run without errors.
+
+*Wise-pizza is open sourced and maintained by Wise Plc. Copyright 2023 Wise Plc.*
```


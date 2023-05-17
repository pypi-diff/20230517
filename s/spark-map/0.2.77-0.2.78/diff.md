# Comparing `tmp/spark_map-0.2.77.tar.gz` & `tmp/spark_map-0.2.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_map-0.2.77.tar", last modified: Mon Jan 30 15:53:13 2023, max compression
+gzip compressed data, was "spark_map-0.2.78.tar", last modified: Wed May 17 16:03:52 2023, max compression
```

## Comparing `spark_map-0.2.77.tar` & `spark_map-0.2.78.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-01-30 15:53:13.347151 spark_map-0.2.77/
--rw-rw-rw-   0        0        0     1063 2023-01-30 15:51:37.000000 spark_map-0.2.77/LICENSE.txt
--rw-rw-rw-   0        0        0     6801 2023-01-30 15:53:13.346152 spark_map-0.2.77/PKG-INFO
--rw-rw-rw-   0        0        0     5058 2023-01-30 15:51:37.000000 spark_map-0.2.77/README.md
--rw-rw-rw-   0        0        0     5381 2023-01-30 15:51:37.000000 spark_map-0.2.77/README.rst
--rw-rw-rw-   0        0        0      934 2023-01-30 15:51:37.000000 spark_map-0.2.77/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-30 15:53:13.347151 spark_map-0.2.77/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-30 15:53:13.304152 spark_map-0.2.77/src/
-drwxrwxrwx   0        0        0        0 2023-01-30 15:53:13.321164 spark_map-0.2.77/src/spark_map/
--rw-rw-rw-   0        0        0       52 2023-01-30 15:51:37.000000 spark_map-0.2.77/src/spark_map/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-01-30 15:51:37.000000 spark_map-0.2.77/src/spark_map/functions.py
--rw-rw-rw-   0        0        0     4795 2023-01-30 15:51:37.000000 spark_map-0.2.77/src/spark_map/mapping.py
--rw-rw-rw-   0        0        0     1528 2023-01-30 15:51:37.000000 spark_map-0.2.77/src/spark_map/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-30 15:53:13.343152 spark_map-0.2.77/src/spark_map.egg-info/
--rw-rw-rw-   0        0        0     6801 2023-01-30 15:53:13.000000 spark_map-0.2.77/src/spark_map.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-01-30 15:53:13.000000 spark_map-0.2.77/src/spark_map.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-30 15:53:13.000000 spark_map-0.2.77/src/spark_map.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-01-30 15:53:13.000000 spark_map-0.2.77/src/spark_map.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-30 15:53:13.000000 spark_map-0.2.77/src/spark_map.egg-info/top_level.txt
+drwxrwxr-x   0 pedro     (1000) pedro     (1000)        0 2023-05-17 16:03:52.323870 spark_map-0.2.78/
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)     1057 2023-01-30 16:05:34.000000 spark_map-0.2.78/LICENSE.txt
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)     6704 2023-05-17 16:03:52.323870 spark_map-0.2.78/PKG-INFO
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)     4983 2023-05-17 15:58:06.000000 spark_map-0.2.78/README.md
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)     5252 2023-01-30 16:05:34.000000 spark_map-0.2.78/README.rst
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)      894 2023-05-17 15:58:26.000000 spark_map-0.2.78/pyproject.toml
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)       38 2023-05-17 16:03:52.323870 spark_map-0.2.78/setup.cfg
+drwxrwxr-x   0 pedro     (1000) pedro     (1000)        0 2023-05-17 16:03:52.319870 spark_map-0.2.78/src/
+drwxrwxr-x   0 pedro     (1000) pedro     (1000)        0 2023-05-17 16:03:52.319870 spark_map-0.2.78/src/spark_map/
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)       43 2023-05-17 15:58:55.000000 spark_map-0.2.78/src/spark_map/__init__.py
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)     2574 2023-05-17 15:58:11.000000 spark_map-0.2.78/src/spark_map/functions.py
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)     4669 2023-05-17 15:58:11.000000 spark_map-0.2.78/src/spark_map/mapping.py
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)     1500 2023-05-17 15:52:44.000000 spark_map-0.2.78/src/spark_map/utils.py
+drwxrwxr-x   0 pedro     (1000) pedro     (1000)        0 2023-05-17 16:03:52.323870 spark_map-0.2.78/src/spark_map.egg-info/
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)     6704 2023-05-17 16:03:52.000000 spark_map-0.2.78/src/spark_map.egg-info/PKG-INFO
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)      332 2023-05-17 16:03:52.000000 spark_map-0.2.78/src/spark_map.egg-info/SOURCES.txt
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)        1 2023-05-17 16:03:52.000000 spark_map-0.2.78/src/spark_map.egg-info/dependency_links.txt
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)       24 2023-05-17 16:03:52.000000 spark_map-0.2.78/src/spark_map.egg-info/requires.txt
+-rw-rw-r--   0 pedro     (1000) pedro     (1000)       10 2023-05-17 16:03:52.000000 spark_map-0.2.78/src/spark_map.egg-info/top_level.txt
```

### Comparing `spark_map-0.2.77/LICENSE.txt` & `spark_map-0.2.78/LICENSE.txt`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 Pedro Duarte Faria
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2022 Pedro Duarte Faria
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `spark_map-0.2.77/PKG-INFO` & `spark_map-0.2.78/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-Metadata-Version: 2.1
-Name: spark_map
-Version: 0.2.77
-Summary: Pyspark implementation of `map()` function for spark DataFrames
-Author-email: Pedro Faria <pedropark99@gmail.com>
-License: Copyright 2022 Pedro Duarte Faria
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Homepage, https://pedropark99.github.io/spark_map/
-Project-URL: Repo, https://github.com/pedropark99/spark_map
-Project-URL: Issues, https://github.com/pedropark99/spark_map/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
-
-<!-- badges: start -->
-[![pytest](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml/badge.svg)](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml)
-<!-- badges: end -->
-
-# Overview <img src="doc/spark-map-logo.png" align="right" style="height:200px" />
-
-`spark_map` is a python package that offers some tools that help you to apply a function over multiple columns of Apache Spark DataFrames, using `pyspark`. The package offers two main functions (or "two main methods") to distribute your calculations, which are `spark_map()` and `spark_across()`. Furthermore, the package offers several methods to map (or select) the columns to which you want to apply your calculations (these methods are called *mapping methods* in the package).
-
-# Installation
-
-To get the latest version of `spark_map` at PyPI, use:
-
-```bash
-pip install spark-map
-```
-
-# Documentation
-
-The full documentation for `spark_map` package is available at the [website of the package](https://pedropark99.github.io/spark_map/). To access it, just use the `Function Reference` and `Articles` menus located at the top navigation bar of the website.
-
-
-
-# What problem `spark_map` solves?
-
-When you work a lot with data pipelines using Apache Spark and `pyspark`, at some day, you might find yourself writing a very long `agg()` statement to aggregate multiple columns of my Spark DataFrame with the same function, like this one below:
-
-```python
-from pyspark.sql.functions import sum, column
-aggregates = (
-    spark.table('cards.detailed_sales_per_user')
-        .groupBy('day')
-        .agg(
-            sum(column('cards_lite')).alias('cards_lite'),
-            sum(column('cards_silver')).alias('cards_silver'),
-            sum(column('cards_gold')).alias('cards_gold'),
-            sum(column('cards_premium')).alias('cards_premium'),
-            sum(column('cards_enterprise')).alias('cards_enterprise'),
-            sum(column('cards_business')).alias('cards_business')
-        )
-)
-```
-The problem with this code is that: it is not elegant; and it is error-prone. Because it involves copy and paste, and very subtle changes in each line. Following the golden rule of DRY (*do not repeat yourself*), we need a better way to write this code. That is the exact problem that `spark_map` solves for you!
-
-When you want to apply the same function (like `sum()`) over multiple columns of a Spark DataFrame (like `spark.table('cards.detailed_sales_per_user')`) that might be grouped by a variable (like `day`), you can use the `spark_map` package, to declare this operation in a much better, elegant and concise way, by using the `spark_map()` function.
-
-```python
-from spark_map.functions import spark_map
-from spark_map.mapping import starts_with
-grouped_by_day = spark.table('cards.detailed_sales_per_user')\
-    .groupBy('day')
-
-aggregates = spark_map(grouped_by_day, starts_with('cards'), sum)
-```
-
-# How `spark_map()` works ?
-
-The `spark_map()` function receives three inputs, which are `table` (i.e. the Spark DataFrame you want to use), `mapping` (i.e. a "mapping" that describes which columns you want to apply your function), and `function` (i.e. the function you want to apply to each column in the Spark DataFrame).
-
-In short, the `starts_with('cards')` section in the above example tells `spark_map()` that you want to apply the input function on all columns of `grouped_by_day` whose name starts with the text `'cards'`. In other words, all `spark_map()` does is to apply the function you want (in the above example this function is `sum()`) to whatever column it finds in the input DataFrame which fits in the description of your mapping method.
-
-You can use different mapping methods to select the columns of your DataFrame, and the package offers several built-in methods which can be very useful for you, which are available through the `spark_map.mapping` module of the package. You can select columns based on:
-
-- `at_position()`: their position (i.e. 3rd, 4th and 5th columns);
-- `matches()`: a regex to which their match;
-- `are_of_type()`: the type of data their store (i.e. all columns of type `int`);
-- `starts_with()` and `ends_with()`: its name starting or ending with a particular pattern;
-- `all_of()`: its name being inside a specific list of options;
-
-# Check the documentation for more examples and details
-
-The [website](https://pedropark99.github.io/spark_map) have documentation for all functions of the package. If you have any trouble to understand or to find examples, is a good idea to check the [Function Reference](https://pedropark99.github.io/spark_map/reference-en.html) of the package, to see examples and more details about how each function works.
-
-To understand how the mapping methods works, and how you can create your own mapping method, a good place to start is to read the article [Building the mapping](https://pedropark99.github.io/spark_map/english/articles/building-mapping.html) available at the website of the package.
+Metadata-Version: 2.1
+Name: spark_map
+Version: 0.2.78
+Summary: Pyspark implementation of `map()` function for spark DataFrames
+Author-email: Pedro Faria <pedropark99@gmail.com>
+License: Copyright 2022 Pedro Duarte Faria
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: Homepage, https://pedropark99.github.io/spark_map/
+Project-URL: Repo, https://github.com/pedropark99/spark_map
+Project-URL: Issues, https://github.com/pedropark99/spark_map/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+
+<!-- badges: start -->
+[![pytest](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml/badge.svg)](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml)
+<!-- badges: end -->
+
+# Overview <img src="doc/spark-map-logo.png" align="right" style="height:200px" />
+
+`spark_map` is a python package that offers some tools that help you to apply a function over multiple columns of Apache Spark DataFrames, using `pyspark`. The package offers two main functions (or "two main methods") to distribute your calculations, which are `spark_map()` and `spark_across()`. Furthermore, the package offers several methods to map (or select) the columns to which you want to apply your calculations (these methods are called *mapping methods* in the package).
+
+# Installation
+
+To get the latest version of `spark_map` at PyPI, use:
+
+```bash
+pip install spark-map
+```
+
+# Documentation
+
+The full documentation for `spark_map` package is available at the [website of the package](https://pedropark99.github.io/spark_map/). To access it, just use the `Function Reference` and `Articles` menus located at the top navigation bar of the website.
+
+
+
+# What problem `spark_map` solves?
+
+When you work a lot with data pipelines using Apache Spark and `pyspark`, at some day, you might find yourself writing a very long `agg()` statement to aggregate multiple columns of my Spark DataFrame with the same function, like this one below:
+
+```python
+from pyspark.sql.functions import sum, column
+aggregates = (
+    spark.table('cards.detailed_sales_per_user')
+        .groupBy('day')
+        .agg(
+            sum(column('cards_lite')).alias('cards_lite'),
+            sum(column('cards_silver')).alias('cards_silver'),
+            sum(column('cards_gold')).alias('cards_gold'),
+            sum(column('cards_premium')).alias('cards_premium'),
+            sum(column('cards_enterprise')).alias('cards_enterprise'),
+            sum(column('cards_business')).alias('cards_business')
+        )
+)
+```
+The problem with this code is that: it is not elegant; and it is error-prone. Because it involves copy and paste, and very subtle changes in each line. Following the golden rule of DRY (*do not repeat yourself*), we need a better way to write this code. That is the exact problem that `spark_map` solves for you!
+
+When you want to apply the same function (like `sum()`) over multiple columns of a Spark DataFrame (like `spark.table('cards.detailed_sales_per_user')`) that might be grouped by a variable (like `day`), you can use the `spark_map` package, to declare this operation in a much better, elegant and concise way, by using the `spark_map()` function.
+
+```python
+from spark_map.functions import spark_map
+from spark_map.mapping import starts_with
+grouped_by_day = spark.table('cards.detailed_sales_per_user')\
+    .groupBy('day')
+
+aggregates = spark_map(grouped_by_day, starts_with('cards'), sum)
+```
+
+# How `spark_map()` works ?
+
+The `spark_map()` function receives three inputs, which are `table` (i.e. the Spark DataFrame you want to use), `mapping` (i.e. a "mapping" that describes which columns you want to apply your function), and `function` (i.e. the function you want to apply to each column in the Spark DataFrame).
+
+In short, the `starts_with('cards')` section in the above example tells `spark_map()` that you want to apply the input function on all columns of `grouped_by_day` whose name starts with the text `'cards'`. In other words, all `spark_map()` does is to apply the function you want (in the above example this function is `sum()`) to whatever column it finds in the input DataFrame which fits in the description of your mapping method.
+
+You can use different mapping methods to select the columns of your DataFrame, and the package offers several built-in methods which can be very useful for you, which are available through the `spark_map.mapping` module of the package. You can select columns based on:
+
+- `at_position()`: their position (i.e. 3rd, 4th and 5th columns);
+- `matches()`: a regex to which their match;
+- `are_of_type()`: the type of data their store (i.e. all columns of type `int`);
+- `starts_with()` and `ends_with()`: its name starting or ending with a particular pattern;
+- `all_of()`: its name being inside a specific list of options;
+
+# Check the documentation for more examples and details
+
+The [website](https://pedropark99.github.io/spark_map) have documentation for all functions of the package. If you have any trouble to understand or to find examples, is a good idea to check the [Function Reference](https://pedropark99.github.io/spark_map/reference-en.html) of the package, to see examples and more details about how each function works.
+
+To understand how the mapping methods works, and how you can create your own mapping method, a good place to start is to read the article [Building the mapping](https://pedropark99.github.io/spark_map/english/articles/building-mapping.html) available at the website of the package.
```

### Comparing `spark_map-0.2.77/README.md` & `spark_map-0.2.78/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-
-
-<!-- badges: start -->
-[![pytest](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml/badge.svg)](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml)
-<!-- badges: end -->
-
-# Overview <img src="doc/spark-map-logo.png" align="right" style="height:200px" />
-
-`spark_map` is a python package that offers some tools that help you to apply a function over multiple columns of Apache Spark DataFrames, using `pyspark`. The package offers two main functions (or "two main methods") to distribute your calculations, which are `spark_map()` and `spark_across()`. Furthermore, the package offers several methods to map (or select) the columns to which you want to apply your calculations (these methods are called *mapping methods* in the package).
-
-# Installation
-
-To get the latest version of `spark_map` at PyPI, use:
-
-```bash
-pip install spark-map
-```
-
-# Documentation
-
-The full documentation for `spark_map` package is available at the [website of the package](https://pedropark99.github.io/spark_map/). To access it, just use the `Function Reference` and `Articles` menus located at the top navigation bar of the website.
-
-
-
-# What problem `spark_map` solves?
-
-When you work a lot with data pipelines using Apache Spark and `pyspark`, at some day, you might find yourself writing a very long `agg()` statement to aggregate multiple columns of my Spark DataFrame with the same function, like this one below:
-
-```python
-from pyspark.sql.functions import sum, column
-aggregates = (
-    spark.table('cards.detailed_sales_per_user')
-        .groupBy('day')
-        .agg(
-            sum(column('cards_lite')).alias('cards_lite'),
-            sum(column('cards_silver')).alias('cards_silver'),
-            sum(column('cards_gold')).alias('cards_gold'),
-            sum(column('cards_premium')).alias('cards_premium'),
-            sum(column('cards_enterprise')).alias('cards_enterprise'),
-            sum(column('cards_business')).alias('cards_business')
-        )
-)
-```
-The problem with this code is that: it is not elegant; and it is error-prone. Because it involves copy and paste, and very subtle changes in each line. Following the golden rule of DRY (*do not repeat yourself*), we need a better way to write this code. That is the exact problem that `spark_map` solves for you!
-
-When you want to apply the same function (like `sum()`) over multiple columns of a Spark DataFrame (like `spark.table('cards.detailed_sales_per_user')`) that might be grouped by a variable (like `day`), you can use the `spark_map` package, to declare this operation in a much better, elegant and concise way, by using the `spark_map()` function.
-
-```python
-from spark_map.functions import spark_map
-from spark_map.mapping import starts_with
-grouped_by_day = spark.table('cards.detailed_sales_per_user')\
-    .groupBy('day')
-
-aggregates = spark_map(grouped_by_day, starts_with('cards'), sum)
-```
-
-# How `spark_map()` works ?
-
-The `spark_map()` function receives three inputs, which are `table` (i.e. the Spark DataFrame you want to use), `mapping` (i.e. a "mapping" that describes which columns you want to apply your function), and `function` (i.e. the function you want to apply to each column in the Spark DataFrame).
-
-In short, the `starts_with('cards')` section in the above example tells `spark_map()` that you want to apply the input function on all columns of `grouped_by_day` whose name starts with the text `'cards'`. In other words, all `spark_map()` does is to apply the function you want (in the above example this function is `sum()`) to whatever column it finds in the input DataFrame which fits in the description of your mapping method.
-
-You can use different mapping methods to select the columns of your DataFrame, and the package offers several built-in methods which can be very useful for you, which are available through the `spark_map.mapping` module of the package. You can select columns based on:
-
-- `at_position()`: their position (i.e. 3rd, 4th and 5th columns);
-- `matches()`: a regex to which their match;
-- `are_of_type()`: the type of data their store (i.e. all columns of type `int`);
-- `starts_with()` and `ends_with()`: its name starting or ending with a particular pattern;
-- `all_of()`: its name being inside a specific list of options;
-
-# Check the documentation for more examples and details
-
-The [website](https://pedropark99.github.io/spark_map) have documentation for all functions of the package. If you have any trouble to understand or to find examples, is a good idea to check the [Function Reference](https://pedropark99.github.io/spark_map/reference-en.html) of the package, to see examples and more details about how each function works.
-
-To understand how the mapping methods works, and how you can create your own mapping method, a good place to start is to read the article [Building the mapping](https://pedropark99.github.io/spark_map/english/articles/building-mapping.html) available at the website of the package.
+
+
+<!-- badges: start -->
+[![pytest](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml/badge.svg)](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml)
+<!-- badges: end -->
+
+# Overview <img src="doc/spark-map-logo.png" align="right" style="height:200px" />
+
+`spark_map` is a python package that offers some tools that help you to apply a function over multiple columns of Apache Spark DataFrames, using `pyspark`. The package offers two main functions (or "two main methods") to distribute your calculations, which are `spark_map()` and `spark_across()`. Furthermore, the package offers several methods to map (or select) the columns to which you want to apply your calculations (these methods are called *mapping methods* in the package).
+
+# Installation
+
+To get the latest version of `spark_map` at PyPI, use:
+
+```bash
+pip install spark-map
+```
+
+# Documentation
+
+The full documentation for `spark_map` package is available at the [website of the package](https://pedropark99.github.io/spark_map/). To access it, just use the `Function Reference` and `Articles` menus located at the top navigation bar of the website.
+
+
+
+# What problem `spark_map` solves?
+
+When you work a lot with data pipelines using Apache Spark and `pyspark`, at some day, you might find yourself writing a very long `agg()` statement to aggregate multiple columns of my Spark DataFrame with the same function, like this one below:
+
+```python
+from pyspark.sql.functions import sum, column
+aggregates = (
+    spark.table('cards.detailed_sales_per_user')
+        .groupBy('day')
+        .agg(
+            sum(column('cards_lite')).alias('cards_lite'),
+            sum(column('cards_silver')).alias('cards_silver'),
+            sum(column('cards_gold')).alias('cards_gold'),
+            sum(column('cards_premium')).alias('cards_premium'),
+            sum(column('cards_enterprise')).alias('cards_enterprise'),
+            sum(column('cards_business')).alias('cards_business')
+        )
+)
+```
+The problem with this code is that: it is not elegant; and it is error-prone. Because it involves copy and paste, and very subtle changes in each line. Following the golden rule of DRY (*do not repeat yourself*), we need a better way to write this code. That is the exact problem that `spark_map` solves for you!
+
+When you want to apply the same function (like `sum()`) over multiple columns of a Spark DataFrame (like `spark.table('cards.detailed_sales_per_user')`) that might be grouped by a variable (like `day`), you can use the `spark_map` package, to declare this operation in a much better, elegant and concise way, by using the `spark_map()` function.
+
+```python
+from spark_map.functions import spark_map
+from spark_map.mapping import starts_with
+grouped_by_day = spark.table('cards.detailed_sales_per_user')\
+    .groupBy('day')
+
+aggregates = spark_map(grouped_by_day, starts_with('cards'), sum)
+```
+
+# How `spark_map()` works ?
+
+The `spark_map()` function receives three inputs, which are `table` (i.e. the Spark DataFrame you want to use), `mapping` (i.e. a "mapping" that describes which columns you want to apply your function), and `function` (i.e. the function you want to apply to each column in the Spark DataFrame).
+
+In short, the `starts_with('cards')` section in the above example tells `spark_map()` that you want to apply the input function on all columns of `grouped_by_day` whose name starts with the text `'cards'`. In other words, all `spark_map()` does is to apply the function you want (in the above example this function is `sum()`) to whatever column it finds in the input DataFrame which fits in the description of your mapping method.
+
+You can use different mapping methods to select the columns of your DataFrame, and the package offers several built-in methods which can be very useful for you, which are available through the `spark_map.mapping` module of the package. You can select columns based on:
+
+- `at_position()`: their position (i.e. 3rd, 4th and 5th columns);
+- `matches()`: a regex to which their match;
+- `are_of_type()`: the type of data their store (i.e. all columns of type `int`);
+- `starts_with()` and `ends_with()`: its name starting or ending with a particular pattern;
+- `all_of()`: its name being inside a specific list of options;
+
+# Check the documentation for more examples and details
+
+The [website](https://pedropark99.github.io/spark_map) have documentation for all functions of the package. If you have any trouble to understand or to find examples, is a good idea to check the [Function Reference](https://pedropark99.github.io/spark_map/reference-en.html) of the package, to see examples and more details about how each function works.
+
+To understand how the mapping methods works, and how you can create your own mapping method, a good place to start is to read the article [Building the mapping](https://pedropark99.github.io/spark_map/english/articles/building-mapping.html) available at the website of the package.
```

### Comparing `spark_map-0.2.77/README.rst` & `spark_map-0.2.78/README.rst`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-.. raw:: html
-
-   <!-- badges: start -->
-
-|pytest|
-
-Overview
-========
-
-``spark_map`` is a python package that offers some tools that help you
-to apply a function over multiple columns of Apache Spark DataFrames,
-using ``pyspark``. The package offers two main functions (or “two main
-methods”) to distribute your calculations, which are ``spark_map()`` and
-``spark_across()``. Furthermore, the package offers several methods to
-map (or select) the columns to which you want to apply your calculations
-(these methods are called *mapping methods* in the package).
-
-Installation
-============
-
-To get the latest version of ``spark_map`` at PyPI, use:
-
-.. code:: bash
-
-   pip install spark_map
-
-Documentation
-=============
-
-The full documentation for ``spark_map`` package is available at the
-`website of the package <https://pedropark99.github.io/spark_map/>`__.
-To access it, just use the ``Function Reference`` and ``Articles`` menus
-located at the top navigation bar of the website.
-
-What problem ``spark_map`` solves?
-==================================
-
-When you work a lot with data pipelines using Apache Spark and
-``pyspark``, at some day, you might find yourself writing a very long
-``agg()`` statement to aggregate multiple columns of my Spark DataFrame
-with the same function, like this one below:
-
-.. code:: python
-
-   from pyspark.sql.functions import sum, column
-   aggregates = (
-       spark.table('cards.detailed_sales_per_user')
-           .groupBy('day')
-           .agg(
-               sum(column('cards_lite')).alias('cards_lite'),
-               sum(column('cards_silver')).alias('cards_silver'),
-               sum(column('cards_gold')).alias('cards_gold'),
-               sum(column('cards_premium')).alias('cards_premium'),
-               sum(column('cards_enterprise')).alias('cards_enterprise'),
-               sum(column('cards_business')).alias('cards_business')
-           )
-   )
-
-The problem with this code is that: it is not elegant; and it is
-error-prone. Because it involves copy and paste, and very subtle changes
-in each line. Following the golden rule of DRY (*do not repeat
-yourself*), we need a better way to write this code. That is the exact
-problem that ``spark_map`` solves for you!
-
-When you want to apply the same function (like ``sum()``) over multiple
-columns of a Spark DataFrame (like
-``spark.table('cards.detailed_sales_per_user')``) that might be grouped
-by a variable (like ``day``), you can use the ``spark_map`` package, to
-declare this operation in a much better, elegant and concise way, by
-using the ``spark_map()`` function.
-
-.. code:: python
-
-   from spark_map.functions import spark_map
-   from spark_map.mapping import starts_with
-   grouped_by_day = spark.table('cards.detailed_sales_per_user')\
-       .groupBy('day')
-
-   aggregates = spark_map(grouped_by_day, starts_with('cards'), sum)
-
-How ``spark_map()`` works ?
-===========================
-
-The ``spark_map()`` function receives three inputs, which are ``table``
-(i.e. the Spark DataFrame you want to use), ``mapping`` (i.e. a
-“mapping” that describes which columns you want to apply your function),
-and ``function`` (i.e. the function you want to apply to each column in
-the Spark DataFrame).
-
-In short, the ``starts_with('cards')`` section in the above example
-tells ``spark_map()`` that you want to apply the input function on all
-columns of ``grouped_by_day`` whose name starts with the text
-``'cards'``. In other words, all ``spark_map()`` does is to apply the
-function you want (in the above example this function is ``sum()``) to
-whatever column it finds in the input DataFrame which fits in the
-description of your mapping method.
-
-You can use different mapping methods to select the columns of your
-DataFrame, and the package offers several built-in methods which can be
-very useful for you, which are available through the
-``spark_map.mapping`` module of the package. You can select columns
-based on:
-
--  ``at_position()``: their position (i.e. 3rd, 4th and 5th columns);
--  ``matches()``: a regex to which their match;
--  ``are_of_type()``: the type of data their store (i.e. all columns of
-   type ``int``);
--  ``starts_with()`` and ``ends_with()``: its name starting or ending
-   with a particular pattern;
--  ``all_of()``: its name being inside a specific list of options;
-
-Check the documentation for more examples and details
-=====================================================
-
-The `website <https://pedropark99.github.io/spark_map>`__ have
-documentation for all functions of the package. If you have any trouble
-to understand or to find examples, is a good idea to check the `Function
-Reference <https://pedropark99.github.io/spark_map/reference-en.html>`__
-of the package, to see examples and more details about how each function
-works.
-
-To understand how the mapping methods works, and how you can create your
-own mapping method, a good place to start is to read the article
-`Building the
-mapping <https://pedropark99.github.io/spark_map/english/articles/building-mapping.html>`__
-available at the website of the package.
-
-.. |pytest| image:: https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml/badge.svg
-   :target: https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml
+.. raw:: html
+
+   <!-- badges: start -->
+
+|pytest|
+
+Overview
+========
+
+``spark_map`` is a python package that offers some tools that help you
+to apply a function over multiple columns of Apache Spark DataFrames,
+using ``pyspark``. The package offers two main functions (or “two main
+methods”) to distribute your calculations, which are ``spark_map()`` and
+``spark_across()``. Furthermore, the package offers several methods to
+map (or select) the columns to which you want to apply your calculations
+(these methods are called *mapping methods* in the package).
+
+Installation
+============
+
+To get the latest version of ``spark_map`` at PyPI, use:
+
+.. code:: bash
+
+   pip install spark_map
+
+Documentation
+=============
+
+The full documentation for ``spark_map`` package is available at the
+`website of the package <https://pedropark99.github.io/spark_map/>`__.
+To access it, just use the ``Function Reference`` and ``Articles`` menus
+located at the top navigation bar of the website.
+
+What problem ``spark_map`` solves?
+==================================
+
+When you work a lot with data pipelines using Apache Spark and
+``pyspark``, at some day, you might find yourself writing a very long
+``agg()`` statement to aggregate multiple columns of my Spark DataFrame
+with the same function, like this one below:
+
+.. code:: python
+
+   from pyspark.sql.functions import sum, column
+   aggregates = (
+       spark.table('cards.detailed_sales_per_user')
+           .groupBy('day')
+           .agg(
+               sum(column('cards_lite')).alias('cards_lite'),
+               sum(column('cards_silver')).alias('cards_silver'),
+               sum(column('cards_gold')).alias('cards_gold'),
+               sum(column('cards_premium')).alias('cards_premium'),
+               sum(column('cards_enterprise')).alias('cards_enterprise'),
+               sum(column('cards_business')).alias('cards_business')
+           )
+   )
+
+The problem with this code is that: it is not elegant; and it is
+error-prone. Because it involves copy and paste, and very subtle changes
+in each line. Following the golden rule of DRY (*do not repeat
+yourself*), we need a better way to write this code. That is the exact
+problem that ``spark_map`` solves for you!
+
+When you want to apply the same function (like ``sum()``) over multiple
+columns of a Spark DataFrame (like
+``spark.table('cards.detailed_sales_per_user')``) that might be grouped
+by a variable (like ``day``), you can use the ``spark_map`` package, to
+declare this operation in a much better, elegant and concise way, by
+using the ``spark_map()`` function.
+
+.. code:: python
+
+   from spark_map.functions import spark_map
+   from spark_map.mapping import starts_with
+   grouped_by_day = spark.table('cards.detailed_sales_per_user')\
+       .groupBy('day')
+
+   aggregates = spark_map(grouped_by_day, starts_with('cards'), sum)
+
+How ``spark_map()`` works ?
+===========================
+
+The ``spark_map()`` function receives three inputs, which are ``table``
+(i.e. the Spark DataFrame you want to use), ``mapping`` (i.e. a
+“mapping” that describes which columns you want to apply your function),
+and ``function`` (i.e. the function you want to apply to each column in
+the Spark DataFrame).
+
+In short, the ``starts_with('cards')`` section in the above example
+tells ``spark_map()`` that you want to apply the input function on all
+columns of ``grouped_by_day`` whose name starts with the text
+``'cards'``. In other words, all ``spark_map()`` does is to apply the
+function you want (in the above example this function is ``sum()``) to
+whatever column it finds in the input DataFrame which fits in the
+description of your mapping method.
+
+You can use different mapping methods to select the columns of your
+DataFrame, and the package offers several built-in methods which can be
+very useful for you, which are available through the
+``spark_map.mapping`` module of the package. You can select columns
+based on:
+
+-  ``at_position()``: their position (i.e. 3rd, 4th and 5th columns);
+-  ``matches()``: a regex to which their match;
+-  ``are_of_type()``: the type of data their store (i.e. all columns of
+   type ``int``);
+-  ``starts_with()`` and ``ends_with()``: its name starting or ending
+   with a particular pattern;
+-  ``all_of()``: its name being inside a specific list of options;
+
+Check the documentation for more examples and details
+=====================================================
+
+The `website <https://pedropark99.github.io/spark_map>`__ have
+documentation for all functions of the package. If you have any trouble
+to understand or to find examples, is a good idea to check the `Function
+Reference <https://pedropark99.github.io/spark_map/reference-en.html>`__
+of the package, to see examples and more details about how each function
+works.
+
+To understand how the mapping methods works, and how you can create your
+own mapping method, a good place to start is to read the article
+`Building the
+mapping <https://pedropark99.github.io/spark_map/english/articles/building-mapping.html>`__
+available at the website of the package.
+
+.. |pytest| image:: https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml/badge.svg
+   :target: https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml
```

### Comparing `spark_map-0.2.77/src/spark_map/functions.py` & `spark_map-0.2.78/src/spark_map/functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from pyspark.sql.functions import column
-from pyspark.sql import DataFrame, GroupedData
-from typing import Callable
-from spark_map.mapping import __map_columns
-
-
-
-def spark_map(table: DataFrame, mapping: dict, function: Callable):
-    """
-    With `spark_map()`, you can apply a aggregate function to a set of columns in a spark DataFrame.
-    It receives a spark DataFrame as input, and returns a new aggregated spark DataFrame as output.
-    For example, to apply the `mean()` function, to the third, fourth and fifth columns, you do: 
-    
-    Example
-    --------
-    >>> import pyspark.sql.functions as F
-    >>> tb = spark.table('sales.sales_by_day')
-    >>> spark_map(tb, at_position(3,4,5), F.mean)
-    """
-    if __is_spark_grouped_data(table):
-        cols = table._df.columns
-        schema = list(table._df.schema)
-    if __is_spark_dataframe(table):
-        cols = table.columns
-        schema = list(table.schema)
-    
-    mapping = __map_columns(mapping, cols, schema)
-    __report_mapped_columns(mapping)
-    
-    params = []
-    for col in mapping:
-        params.append(
-            function(column(col)).alias(col)
-        )
-      
-    result = table.agg(*params)
-    
-    return result
-
-
-
-def spark_across(table: DataFrame, mapping: dict, function: Callable, **kwargs):
-    """
-    With `spark_across()` you can apply a function across multiple columns of a spark DataFrame.
-    While `spark_map()` calculates aggregates in a set of columns, `spark_across()` uses
-    `withColumn()` to apply a function over each row of a set of columns.
-
-    Example
-    --------
-    >>> import pyspark.sql.functions as F
-    >>> tb = spark.table('sales.sales_by_day')
-    >>> spark_across(tb, at_position(3,4,5), F.cast, 'double')
-    """
-    if __is_spark_grouped_data(table):
-        raise ValueError("You gave a grouped Spark DataFrame to `spark_across()`. However, this function work solely with plain Spark DataFrames. Did you meant to use `spark_map()` instead?")
-    
-    cols = table.columns
-    schema = list(table.schema)
-    
-    mapping = __map_columns(mapping, cols, schema)
-    __report_mapped_columns(mapping)
-    
-    for col in mapping:
-        table = table.withColumn(
-            col,
-            function(column(col), **kwargs)
-        )
-
-    return table
-
-
-
-
-
-def __is_spark_dataframe(x):
-    return isinstance(x, DataFrame)
-
-def __is_spark_grouped_data(x):
-    return isinstance(x, GroupedData)
-
-
-def __report_mapped_columns(mapping: list[str]):
-    message = f"Selected columns by `spark_map()`: {', '.join(mapping)}\n"
-    print(message)
+from pyspark.sql.functions import column
+from pyspark.sql import DataFrame, GroupedData
+from typing import Callable, List
+from spark_map.mapping import __map_columns
+
+
+
+def spark_map(table: DataFrame, mapping: dict, function: Callable):
+    """
+    With `spark_map()`, you can apply a aggregate function to a set of columns in a spark DataFrame.
+    It receives a spark DataFrame as input, and returns a new aggregated spark DataFrame as output.
+    For example, to apply the `mean()` function, to the third, fourth and fifth columns, you do: 
+    
+    Example
+    --------
+    >>> import pyspark.sql.functions as F
+    >>> tb = spark.table('sales.sales_by_day')
+    >>> spark_map(tb, at_position(3,4,5), F.mean)
+    """
+    if __is_spark_grouped_data(table):
+        cols = table._df.columns
+        schema = list(table._df.schema)
+    if __is_spark_dataframe(table):
+        cols = table.columns
+        schema = list(table.schema)
+    
+    mapping = __map_columns(mapping, cols, schema)
+    __report_mapped_columns(mapping)
+    
+    params = []
+    for col in mapping:
+        params.append(
+            function(column(col)).alias(col)
+        )
+      
+    result = table.agg(*params)
+    
+    return result
+
+
+
+def spark_across(table: DataFrame, mapping: dict, function: Callable, **kwargs):
+    """
+    With `spark_across()` you can apply a function across multiple columns of a spark DataFrame.
+    While `spark_map()` calculates aggregates in a set of columns, `spark_across()` uses
+    `withColumn()` to apply a function over each row of a set of columns.
+
+    Example
+    --------
+    >>> import pyspark.sql.functions as F
+    >>> tb = spark.table('sales.sales_by_day')
+    >>> spark_across(tb, at_position(3,4,5), F.cast, 'double')
+    """
+    if __is_spark_grouped_data(table):
+        raise ValueError("You gave a grouped Spark DataFrame to `spark_across()`. However, this function work solely with plain Spark DataFrames. Did you meant to use `spark_map()` instead?")
+    
+    cols = table.columns
+    schema = list(table.schema)
+    
+    mapping = __map_columns(mapping, cols, schema)
+    __report_mapped_columns(mapping)
+    
+    for col in mapping:
+        table = table.withColumn(
+            col,
+            function(column(col), **kwargs)
+        )
+
+    return table
+
+
+
+
+
+def __is_spark_dataframe(x):
+    return isinstance(x, DataFrame)
+
+def __is_spark_grouped_data(x):
+    return isinstance(x, GroupedData)
+
+
+def __report_mapped_columns(mapping: List[str]):
+    message = f"Selected columns by `spark_map()`: {', '.join(mapping)}\n"
+    print(message)
```

### Comparing `spark_map-0.2.77/src/spark_map/mapping.py` & `spark_map-0.2.78/src/spark_map/mapping.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,150 +1,151 @@
-import re
-from pyspark.sql.types import StructType
-from pyspark.sql.types import (
-    StringType
-    , IntegerType
-    , LongType
-    , DoubleType
-    , DateType
-    , TimestampType
-)
-
-
-
-from spark_map.utils import (
-    __check_list_input
-    , __check_string_input
-    , __is_string
-)
-
-
-
-
-    
-def all_of(list_cols: list[str]):
-    __check_list_input(list_cols, str, "all_of()")
-    return {'fun': 'all_of', 'val': list_cols}
-    
-def matches(regex: str):
-    __check_string_input(regex, "matches()")
-    return {'fun': "matches", 'val': regex} 
-
-  
-def at_position(*indexes: list[int], zero_index: bool = False):
-    __check_list_input(indexes, int, "at_position()")
-
-    if zero_index == False:
-        indexes = [index - 1 for index in indexes]
-    # Check if any of the indexes are negative:
-    negative = [index < 0 for index in indexes]
-    if any(negative):
-        raise ValueError("One (or more) of the provided indexes are negative! Did you provided a zero index, and not set the `zero_index` argument to True?")
-
-    # Transform to `set` to avoid duplicated indexes
-    indexes = list(set(indexes))
-    indexes.sort()
-    return {'fun': "at_position", 'val': indexes}
-
-
-def starts_with(text: str):
-    __check_string_input(text, "starts_with()")
-    return {'fun': "starts_with", 'val': text}
-
-def ends_with(text: str):
-    __check_string_input(text, "ends_with()")
-    return {'fun': "ends_with", 'val': text}
-
-def are_of_type(arg_type: str):
-    __check_string_input(arg_type, "are_of_type()")
-    valid_types = ['string', 'int', 'long', 'double', 'date', 'datetime']
-    if arg_type not in valid_types:
-        types = [f"'{t}'" for t in valid_types]
-        types = ', '.join(types)
-        message = f'You must choose one of the following values: {types}'
-        raise ValueError(message)
-    return {'fun': "are_of_type", 'val': arg_type}
-
-
-
-
-
-
-
-def __map_columns(mapping: dict, cols: list[str], schema: StructType):
-    mapping_function = mapping['fun']
-    mapping_value = mapping['val']
-    if __is_string(mapping_function):
-        m = Mapping()
-        method_to_call = getattr(m, mapping_function)
-        method_to_call(mapping_value, cols, schema)
-        selected_cols = m.mapped_cols
-    else:
-        selected_cols = mapping_function(mapping_value, cols, schema)
-    
-    if len(selected_cols) == 0:
-        message = "`spark_map()` did not found any column that matches your mapping!"
-        raise KeyError(message)
-    
-    return selected_cols
-
-
-
-    
-### ====================================================================================
-### We use the Mapping class to store the default mapping methods available in the package.
-### If the user wants to use a custom mapping method, he should provide its own
-### methods. These custom methods will not have anything in commom with this class;
-### ====================================================================================
-class Mapping:
-    
-    def __init__(self):
-        self.mapped_cols = []
-    
-    
-  
-    def all_of(self, list_cols: list[str], cols: list[str], schema: StructType):
-        selected_cols = [col for col in list_cols if col in cols]
-        self.mapped_cols = selected_cols
-
-    def at_position(self, indexes: list[int], cols: list[str], schema: StructType):
-        selected_cols = [cols[i] for i in indexes]
-        self.mapped_cols = selected_cols
-
-    def ends_with(self, text: str, cols: list[str], schema: StructType):
-        selected_cols = list()
-        for col in cols:
-            if col.endswith(text):
-                selected_cols.append(col)
-
-        self.mapped_cols = selected_cols
-
-    def starts_with(self, text: str, cols: list[str], schema: StructType):
-        selected_cols = list()
-        for col in cols:
-            if col.startswith(text):
-                selected_cols.append(col)
-
-        self.mapped_cols = selected_cols
-
-
-    def matches(self, regex: str, cols: list[str], schema: StructType):
-        regex = re.compile(regex)
-        selected_cols = [col for col in cols if re.match(regex, col)]
-        self.mapped_cols = selected_cols
-
-
-    def are_of_type(self, str_type: str, cols: list[str], schema: StructType):
-        valid_types = {
-            'int' : IntegerType(), 'double' : DoubleType(), 
-            'string' : StringType(), 'date' : DateType(),
-            'datetime' : TimestampType(), 'long': LongType()
-        }
-
-        target_type = valid_types[str_type]
-        selected_cols = list()
-        for name, field in zip(cols, schema):
-            if field.dataType == target_type:
-                selected_cols.append(name)
-
-        self.mapped_cols = selected_cols
-
+import re
+from typing import List
+from pyspark.sql.types import StructType
+from pyspark.sql.types import (
+    StringType
+    , IntegerType
+    , LongType
+    , DoubleType
+    , DateType
+    , TimestampType
+)
+
+
+
+from spark_map.utils import (
+    __check_list_input
+    , __check_string_input
+    , __is_string
+)
+
+
+
+
+    
+def all_of(list_cols: List[str]):
+    __check_list_input(list_cols, str, "all_of()")
+    return {'fun': 'all_of', 'val': list_cols}
+    
+def matches(regex: str):
+    __check_string_input(regex, "matches()")
+    return {'fun': "matches", 'val': regex} 
+
+  
+def at_position(*indexes: List[int], zero_index: bool = False):
+    __check_list_input(indexes, int, "at_position()")
+
+    if zero_index == False:
+        indexes = [index - 1 for index in indexes]
+    # Check if any of the indexes are negative:
+    negative = [index < 0 for index in indexes]
+    if any(negative):
+        raise ValueError("One (or more) of the provided indexes are negative! Did you provided a zero index, and not set the `zero_index` argument to True?")
+
+    # Transform to `set` to avoid duplicated indexes
+    indexes = list(set(indexes))
+    indexes.sort()
+    return {'fun': "at_position", 'val': indexes}
+
+
+def starts_with(text: str):
+    __check_string_input(text, "starts_with()")
+    return {'fun': "starts_with", 'val': text}
+
+def ends_with(text: str):
+    __check_string_input(text, "ends_with()")
+    return {'fun': "ends_with", 'val': text}
+
+def are_of_type(arg_type: str):
+    __check_string_input(arg_type, "are_of_type()")
+    valid_types = ['string', 'int', 'long', 'double', 'date', 'datetime']
+    if arg_type not in valid_types:
+        types = [f"'{t}'" for t in valid_types]
+        types = ', '.join(types)
+        message = f'You must choose one of the following values: {types}'
+        raise ValueError(message)
+    return {'fun': "are_of_type", 'val': arg_type}
+
+
+
+
+
+
+
+def __map_columns(mapping: dict, cols: List[str], schema: StructType):
+    mapping_function = mapping['fun']
+    mapping_value = mapping['val']
+    if __is_string(mapping_function):
+        m = Mapping()
+        method_to_call = getattr(m, mapping_function)
+        method_to_call(mapping_value, cols, schema)
+        selected_cols = m.mapped_cols
+    else:
+        selected_cols = mapping_function(mapping_value, cols, schema)
+    
+    if len(selected_cols) == 0:
+        message = "`spark_map()` did not found any column that matches your mapping!"
+        raise KeyError(message)
+    
+    return selected_cols
+
+
+
+    
+### ====================================================================================
+### We use the Mapping class to store the default mapping methods available in the package.
+### If the user wants to use a custom mapping method, he should provide its own
+### methods. These custom methods will not have anything in commom with this class;
+### ====================================================================================
+class Mapping:
+    
+    def __init__(self):
+        self.mapped_cols = []
+    
+    
+  
+    def all_of(self, list_cols: List[str], cols: List[str], schema: StructType):
+        selected_cols = [col for col in list_cols if col in cols]
+        self.mapped_cols = selected_cols
+
+    def at_position(self, indexes: List[int], cols: List[str], schema: StructType):
+        selected_cols = [cols[i] for i in indexes]
+        self.mapped_cols = selected_cols
+
+    def ends_with(self, text: str, cols: List[str], schema: StructType):
+        selected_cols = list()
+        for col in cols:
+            if col.endswith(text):
+                selected_cols.append(col)
+
+        self.mapped_cols = selected_cols
+
+    def starts_with(self, text: str, cols: List[str], schema: StructType):
+        selected_cols = list()
+        for col in cols:
+            if col.startswith(text):
+                selected_cols.append(col)
+
+        self.mapped_cols = selected_cols
+
+
+    def matches(self, regex: str, cols: List[str], schema: StructType):
+        regex = re.compile(regex)
+        selected_cols = [col for col in cols if re.match(regex, col)]
+        self.mapped_cols = selected_cols
+
+
+    def are_of_type(self, str_type: str, cols: List[str], schema: StructType):
+        valid_types = {
+            'int' : IntegerType(), 'double' : DoubleType(), 
+            'string' : StringType(), 'date' : DateType(),
+            'datetime' : TimestampType(), 'long': LongType()
+        }
+
+        target_type = valid_types[str_type]
+        selected_cols = list()
+        for name, field in zip(cols, schema):
+            if field.dataType == target_type:
+                selected_cols.append(name)
+
+        self.mapped_cols = selected_cols
+
```

### Comparing `spark_map-0.2.77/src/spark_map/utils.py` & `spark_map-0.2.78/src/spark_map/utils.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-
-def __is_string(x):
-    return isinstance(x, str)
-
-def __is_list_or_tuple(x):
-    return isinstance(x, list) | isinstance(x, tuple)
-
-def __check_string_input(x, mapping_function:str):
-    if not __is_string(x):
-        raise TypeError(f"Input of `{mapping_function}` needs to be a string (data of type `str`). Not {type(x)}.")
-    if x == '':
-        raise ValueError(f"Looks like you gave an empty string as input for `{mapping_function}`. This string should not be empty!")
-
-
-
-
-def __check_list_input(x, type, mapping_function:str):
-    if not __is_list_or_tuple(x):
-        raise TypeError(f"Input of `{mapping_function}` needs to be a list. Not {type(x)}.")
-    if len(x) == 0:
-        raise ValueError(f"You provided an empty list as input for `{mapping_function}`. However, this list should not be empty!")
-    if __is_list_or_tuple(x[0]) and mapping_function == 'at_position()':
-        raise ValueError("Did you provided your column indexes inside a list to `at_position()`? You should not encapsulate these indexes inside a list. For example, if you want to select 1° and 3° columns, just do `at_position(1, 3)` instead of `at_position([1, 3])`.")
-
-    are_of_type = map(lambda x: isinstance(x, type), x)
-    # Check if all elements are of designated type
-    all_elements_of_type = all(are_of_type)
-    if not all_elements_of_type:
+
+def __is_string(x):
+    return isinstance(x, str)
+
+def __is_list_or_tuple(x):
+    return isinstance(x, list) | isinstance(x, tuple)
+
+def __check_string_input(x, mapping_function:str):
+    if not __is_string(x):
+        raise TypeError(f"Input of `{mapping_function}` needs to be a string (data of type `str`). Not {type(x)}.")
+    if x == '':
+        raise ValueError(f"Looks like you gave an empty string as input for `{mapping_function}`. This string should not be empty!")
+
+
+
+
+def __check_list_input(x, type, mapping_function:str):
+    if not __is_list_or_tuple(x):
+        raise TypeError(f"Input of `{mapping_function}` needs to be a list. Not {type(x)}.")
+    if len(x) == 0:
+        raise ValueError(f"You provided an empty list as input for `{mapping_function}`. However, this list should not be empty!")
+    if __is_list_or_tuple(x[0]) and mapping_function == 'at_position()':
+        raise ValueError("Did you provided your column indexes inside a list to `at_position()`? You should not encapsulate these indexes inside a list. For example, if you want to select 1° and 3° columns, just do `at_position(1, 3)` instead of `at_position([1, 3])`.")
+
+    are_of_type = map(lambda x: isinstance(x, type), x)
+    # Check if all elements are of designated type
+    all_elements_of_type = all(are_of_type)
+    if not all_elements_of_type:
         raise TypeError(f"`{mapping_function}` should receive a list of `{type}` values. But some of the elements in the input list are not of this type.")
```

### Comparing `spark_map-0.2.77/src/spark_map.egg-info/PKG-INFO` & `spark_map-0.2.78/src/spark_map.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-Metadata-Version: 2.1
-Name: spark-map
-Version: 0.2.77
-Summary: Pyspark implementation of `map()` function for spark DataFrames
-Author-email: Pedro Faria <pedropark99@gmail.com>
-License: Copyright 2022 Pedro Duarte Faria
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Homepage, https://pedropark99.github.io/spark_map/
-Project-URL: Repo, https://github.com/pedropark99/spark_map
-Project-URL: Issues, https://github.com/pedropark99/spark_map/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
-
-<!-- badges: start -->
-[![pytest](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml/badge.svg)](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml)
-<!-- badges: end -->
-
-# Overview <img src="doc/spark-map-logo.png" align="right" style="height:200px" />
-
-`spark_map` is a python package that offers some tools that help you to apply a function over multiple columns of Apache Spark DataFrames, using `pyspark`. The package offers two main functions (or "two main methods") to distribute your calculations, which are `spark_map()` and `spark_across()`. Furthermore, the package offers several methods to map (or select) the columns to which you want to apply your calculations (these methods are called *mapping methods* in the package).
-
-# Installation
-
-To get the latest version of `spark_map` at PyPI, use:
-
-```bash
-pip install spark-map
-```
-
-# Documentation
-
-The full documentation for `spark_map` package is available at the [website of the package](https://pedropark99.github.io/spark_map/). To access it, just use the `Function Reference` and `Articles` menus located at the top navigation bar of the website.
-
-
-
-# What problem `spark_map` solves?
-
-When you work a lot with data pipelines using Apache Spark and `pyspark`, at some day, you might find yourself writing a very long `agg()` statement to aggregate multiple columns of my Spark DataFrame with the same function, like this one below:
-
-```python
-from pyspark.sql.functions import sum, column
-aggregates = (
-    spark.table('cards.detailed_sales_per_user')
-        .groupBy('day')
-        .agg(
-            sum(column('cards_lite')).alias('cards_lite'),
-            sum(column('cards_silver')).alias('cards_silver'),
-            sum(column('cards_gold')).alias('cards_gold'),
-            sum(column('cards_premium')).alias('cards_premium'),
-            sum(column('cards_enterprise')).alias('cards_enterprise'),
-            sum(column('cards_business')).alias('cards_business')
-        )
-)
-```
-The problem with this code is that: it is not elegant; and it is error-prone. Because it involves copy and paste, and very subtle changes in each line. Following the golden rule of DRY (*do not repeat yourself*), we need a better way to write this code. That is the exact problem that `spark_map` solves for you!
-
-When you want to apply the same function (like `sum()`) over multiple columns of a Spark DataFrame (like `spark.table('cards.detailed_sales_per_user')`) that might be grouped by a variable (like `day`), you can use the `spark_map` package, to declare this operation in a much better, elegant and concise way, by using the `spark_map()` function.
-
-```python
-from spark_map.functions import spark_map
-from spark_map.mapping import starts_with
-grouped_by_day = spark.table('cards.detailed_sales_per_user')\
-    .groupBy('day')
-
-aggregates = spark_map(grouped_by_day, starts_with('cards'), sum)
-```
-
-# How `spark_map()` works ?
-
-The `spark_map()` function receives three inputs, which are `table` (i.e. the Spark DataFrame you want to use), `mapping` (i.e. a "mapping" that describes which columns you want to apply your function), and `function` (i.e. the function you want to apply to each column in the Spark DataFrame).
-
-In short, the `starts_with('cards')` section in the above example tells `spark_map()` that you want to apply the input function on all columns of `grouped_by_day` whose name starts with the text `'cards'`. In other words, all `spark_map()` does is to apply the function you want (in the above example this function is `sum()`) to whatever column it finds in the input DataFrame which fits in the description of your mapping method.
-
-You can use different mapping methods to select the columns of your DataFrame, and the package offers several built-in methods which can be very useful for you, which are available through the `spark_map.mapping` module of the package. You can select columns based on:
-
-- `at_position()`: their position (i.e. 3rd, 4th and 5th columns);
-- `matches()`: a regex to which their match;
-- `are_of_type()`: the type of data their store (i.e. all columns of type `int`);
-- `starts_with()` and `ends_with()`: its name starting or ending with a particular pattern;
-- `all_of()`: its name being inside a specific list of options;
-
-# Check the documentation for more examples and details
-
-The [website](https://pedropark99.github.io/spark_map) have documentation for all functions of the package. If you have any trouble to understand or to find examples, is a good idea to check the [Function Reference](https://pedropark99.github.io/spark_map/reference-en.html) of the package, to see examples and more details about how each function works.
-
-To understand how the mapping methods works, and how you can create your own mapping method, a good place to start is to read the article [Building the mapping](https://pedropark99.github.io/spark_map/english/articles/building-mapping.html) available at the website of the package.
+Metadata-Version: 2.1
+Name: spark-map
+Version: 0.2.78
+Summary: Pyspark implementation of `map()` function for spark DataFrames
+Author-email: Pedro Faria <pedropark99@gmail.com>
+License: Copyright 2022 Pedro Duarte Faria
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: Homepage, https://pedropark99.github.io/spark_map/
+Project-URL: Repo, https://github.com/pedropark99/spark_map
+Project-URL: Issues, https://github.com/pedropark99/spark_map/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+
+<!-- badges: start -->
+[![pytest](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml/badge.svg)](https://github.com/pedropark99/spark_map/actions/workflows/pytest.yml)
+<!-- badges: end -->
+
+# Overview <img src="doc/spark-map-logo.png" align="right" style="height:200px" />
+
+`spark_map` is a python package that offers some tools that help you to apply a function over multiple columns of Apache Spark DataFrames, using `pyspark`. The package offers two main functions (or "two main methods") to distribute your calculations, which are `spark_map()` and `spark_across()`. Furthermore, the package offers several methods to map (or select) the columns to which you want to apply your calculations (these methods are called *mapping methods* in the package).
+
+# Installation
+
+To get the latest version of `spark_map` at PyPI, use:
+
+```bash
+pip install spark-map
+```
+
+# Documentation
+
+The full documentation for `spark_map` package is available at the [website of the package](https://pedropark99.github.io/spark_map/). To access it, just use the `Function Reference` and `Articles` menus located at the top navigation bar of the website.
+
+
+
+# What problem `spark_map` solves?
+
+When you work a lot with data pipelines using Apache Spark and `pyspark`, at some day, you might find yourself writing a very long `agg()` statement to aggregate multiple columns of my Spark DataFrame with the same function, like this one below:
+
+```python
+from pyspark.sql.functions import sum, column
+aggregates = (
+    spark.table('cards.detailed_sales_per_user')
+        .groupBy('day')
+        .agg(
+            sum(column('cards_lite')).alias('cards_lite'),
+            sum(column('cards_silver')).alias('cards_silver'),
+            sum(column('cards_gold')).alias('cards_gold'),
+            sum(column('cards_premium')).alias('cards_premium'),
+            sum(column('cards_enterprise')).alias('cards_enterprise'),
+            sum(column('cards_business')).alias('cards_business')
+        )
+)
+```
+The problem with this code is that: it is not elegant; and it is error-prone. Because it involves copy and paste, and very subtle changes in each line. Following the golden rule of DRY (*do not repeat yourself*), we need a better way to write this code. That is the exact problem that `spark_map` solves for you!
+
+When you want to apply the same function (like `sum()`) over multiple columns of a Spark DataFrame (like `spark.table('cards.detailed_sales_per_user')`) that might be grouped by a variable (like `day`), you can use the `spark_map` package, to declare this operation in a much better, elegant and concise way, by using the `spark_map()` function.
+
+```python
+from spark_map.functions import spark_map
+from spark_map.mapping import starts_with
+grouped_by_day = spark.table('cards.detailed_sales_per_user')\
+    .groupBy('day')
+
+aggregates = spark_map(grouped_by_day, starts_with('cards'), sum)
+```
+
+# How `spark_map()` works ?
+
+The `spark_map()` function receives three inputs, which are `table` (i.e. the Spark DataFrame you want to use), `mapping` (i.e. a "mapping" that describes which columns you want to apply your function), and `function` (i.e. the function you want to apply to each column in the Spark DataFrame).
+
+In short, the `starts_with('cards')` section in the above example tells `spark_map()` that you want to apply the input function on all columns of `grouped_by_day` whose name starts with the text `'cards'`. In other words, all `spark_map()` does is to apply the function you want (in the above example this function is `sum()`) to whatever column it finds in the input DataFrame which fits in the description of your mapping method.
+
+You can use different mapping methods to select the columns of your DataFrame, and the package offers several built-in methods which can be very useful for you, which are available through the `spark_map.mapping` module of the package. You can select columns based on:
+
+- `at_position()`: their position (i.e. 3rd, 4th and 5th columns);
+- `matches()`: a regex to which their match;
+- `are_of_type()`: the type of data their store (i.e. all columns of type `int`);
+- `starts_with()` and `ends_with()`: its name starting or ending with a particular pattern;
+- `all_of()`: its name being inside a specific list of options;
+
+# Check the documentation for more examples and details
+
+The [website](https://pedropark99.github.io/spark_map) have documentation for all functions of the package. If you have any trouble to understand or to find examples, is a good idea to check the [Function Reference](https://pedropark99.github.io/spark_map/reference-en.html) of the package, to see examples and more details about how each function works.
+
+To understand how the mapping methods works, and how you can create your own mapping method, a good place to start is to read the article [Building the mapping](https://pedropark99.github.io/spark_map/english/articles/building-mapping.html) available at the website of the package.
```


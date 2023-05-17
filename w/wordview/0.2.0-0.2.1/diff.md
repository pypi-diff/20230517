# Comparing `tmp/wordview-0.2.0.tar.gz` & `tmp/wordview-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.2.0.tar", max compression
+gzip compressed data, was "wordview-0.2.1.tar", max compression
```

## Comparing `wordview-0.2.0.tar` & `wordview-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      339 2023-05-17 09:03:13.609346 wordview-0.2.0/CHANGES.rst
--rw-r--r--   0        0        0     1074 2022-06-16 16:46:04.846999 wordview-0.2.0/LICENSE
--rw-r--r--   0        0        0     4613 2023-04-20 12:24:54.126503 wordview-0.2.0/README.rst
--rw-r--r--   0        0        0      871 2023-05-17 09:14:47.935996 wordview-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      151 2022-06-16 16:46:04.892361 wordview-0.2.0/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-03-30 15:57:29.123003 wordview-0.2.0/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-02-19 17:09:47.466124 wordview-0.2.0/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4788 2023-03-31 14:18:45.152428 wordview-0.2.0/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-02-24 14:54:27.524967 wordview-0.2.0/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-03-02 08:17:36.835194 wordview-0.2.0/wordview/clustering/cluster.py
--rw-r--r--   0        0        0       84 2023-01-11 13:24:40.126952 wordview-0.2.0/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-01-24 17:56:38.022613 wordview-0.2.0/wordview/mwes/am.py
--rw-r--r--   0        0        0     5305 2023-05-10 15:53:47.791178 wordview-0.2.0/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     6711 2023-05-10 15:53:47.792472 wordview-0.2.0/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0       55 2023-03-08 15:49:42.676986 wordview-0.2.0/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-04-20 12:24:54.167225 wordview-0.2.0/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0       75 2023-03-27 11:57:05.780678 wordview-0.2.0/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    11825 2023-02-09 12:17:50.008926 wordview-0.2.0/wordview/text_analysis/core.py
--rw-r--r--   0        0        0   938013 2022-12-31 16:48:35.212911 wordview-0.2.0/wordview/text_analysis/lid.176.ftz
--rw-r--r--   0        0        0     7345 2023-05-01 15:17:11.759292 wordview-0.2.0/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     5499 1970-01-01 00:00:00.000000 wordview-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      456 2023-05-17 10:24:45.148827 wordview-0.2.1/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2022-06-16 16:46:04.846999 wordview-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4613 2023-04-20 12:24:54.126503 wordview-0.2.1/README.rst
+-rw-r--r--   0        0        0      871 2023-05-17 10:23:54.336785 wordview-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      151 2022-06-16 16:46:04.892361 wordview-0.2.1/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-03-30 15:57:29.123003 wordview-0.2.1/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-02-19 17:09:47.466124 wordview-0.2.1/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4788 2023-03-31 14:18:45.152428 wordview-0.2.1/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-02-24 14:54:27.524967 wordview-0.2.1/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-03-02 08:17:36.835194 wordview-0.2.1/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0       84 2023-01-11 13:24:40.126952 wordview-0.2.1/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-01-24 17:56:38.022613 wordview-0.2.1/wordview/mwes/am.py
+-rw-r--r--   0        0        0     5305 2023-05-10 15:53:47.791178 wordview-0.2.1/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     6711 2023-05-10 15:53:47.792472 wordview-0.2.1/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0       55 2023-03-08 15:49:42.676986 wordview-0.2.1/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-04-20 12:24:54.167225 wordview-0.2.1/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0       75 2023-03-27 11:57:05.780678 wordview-0.2.1/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    11825 2023-02-09 12:17:50.008926 wordview-0.2.1/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0   938013 2022-12-31 16:48:35.212911 wordview-0.2.1/wordview/text_analysis/lid.176.ftz
+-rw-r--r--   0        0        0     7345 2023-05-01 15:17:11.759292 wordview-0.2.1/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5499 1970-01-01 00:00:00.000000 wordview-0.2.1/PKG-INFO
```

### Comparing `wordview-0.2.0/LICENSE` & `wordview-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/README.rst` & `wordview-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/pyproject.toml` & `wordview-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "wordview"
-version = "0.2.0"
+version = "0.2.1"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 fasttext = "0.9.2"
-pandas = "1.3.5"
-scikit-learn = "1.0.1"
+pandas = "2.0.1"
+scikit-learn = "1.2.2"
 scipy = "1.10.0"
 nltk = "3.6.6"
 tqdm = "4.62.3"
 wordcloud = "1.8.1"
 plotly = "5.5.0"
 tabulate = "0.9.0"
 sentence-transformers = "2.2.2"
```

### Comparing `wordview-0.2.0/wordview/anomaly/gaussianize.py` & `wordview-0.2.1/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/wordview/anomaly/normaldist.py` & `wordview-0.2.1/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/wordview/clustering/cluster.py` & `wordview-0.2.1/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/wordview/mwes/am.py` & `wordview-0.2.1/wordview/mwes/am.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/wordview/mwes/mwe.py` & `wordview-0.2.1/wordview/mwes/mwe.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/wordview/mwes/mwe_utils.py` & `wordview-0.2.1/wordview/mwes/mwe_utils.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/wordview/preprocessing/cleaning.py` & `wordview-0.2.1/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/wordview/text_analysis/core.py` & `wordview-0.2.1/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/wordview/text_analysis/lid.176.ftz` & `wordview-0.2.1/wordview/text_analysis/lid.176.ftz`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/wordview/text_analysis/wrapper.py` & `wordview-0.2.1/wordview/text_analysis/wrapper.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.0/PKG-INFO` & `wordview-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fasttext (==0.9.2)
 Requires-Dist: nltk (==3.6.6)
-Requires-Dist: pandas (==1.3.5)
+Requires-Dist: pandas (==2.0.1)
 Requires-Dist: plotly (==5.5.0)
-Requires-Dist: scikit-learn (==1.0.1)
+Requires-Dist: scikit-learn (==1.2.2)
 Requires-Dist: scipy (==1.10.0)
 Requires-Dist: sentence-transformers (==2.2.2)
 Requires-Dist: tabulate (==0.9.0)
 Requires-Dist: tqdm (==4.62.3)
 Requires-Dist: wordcloud (==1.8.1)
 Description-Content-Type: text/x-rst
```


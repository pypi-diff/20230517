# Comparing `tmp/tmplot-0.0.8.tar.gz` & `tmp/tmplot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmplot-0.0.8.tar", last modified: Sat Mar 26 20:12:58 2022, max compression
+gzip compressed data, was "tmplot-0.0.9.tar", last modified: Sat Aug 20 10:43:07 2022, max compression
```

## Comparing `tmplot-0.0.8.tar` & `tmplot-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 20:12:58.258248 tmplot-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-03-26 20:11:59.000000 tmplot-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-03-26 20:12:58.258248 tmplot-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-03-26 20:11:59.000000 tmplot-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-03-26 20:11:59.000000 tmplot-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-03-26 20:12:58.258248 tmplot-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-03-26 20:11:59.000000 tmplot-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 20:12:58.254248 tmplot-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 20:12:58.258248 tmplot-0.0.8/src/tmplot/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-03-26 20:11:59.000000 tmplot-0.0.8/src/tmplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6206 2022-03-26 20:11:59.000000 tmplot-0.0.8/src/tmplot/_distance.py
--rw-r--r--   0 runner    (1001) docker     (121)    12326 2022-03-26 20:11:59.000000 tmplot-0.0.8/src/tmplot/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-03-26 20:11:59.000000 tmplot-0.0.8/src/tmplot/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    11299 2022-03-26 20:11:59.000000 tmplot-0.0.8/src/tmplot/_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     6256 2022-03-26 20:11:59.000000 tmplot-0.0.8/src/tmplot/_stability.py
--rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-03-26 20:11:59.000000 tmplot-0.0.8/src/tmplot/_vis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 20:12:58.258248 tmplot-0.0.8/src/tmplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-03-26 20:12:58.000000 tmplot-0.0.8/src/tmplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-03-26 20:12:58.000000 tmplot-0.0.8/src/tmplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-26 20:12:58.000000 tmplot-0.0.8/src/tmplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-03-26 20:12:58.000000 tmplot-0.0.8/src/tmplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-26 20:12:58.000000 tmplot-0.0.8/src/tmplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-26 20:12:58.000000 tmplot-0.0.8/src/tmplot.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 10:43:07.003854 tmplot-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-08-20 10:42:22.000000 tmplot-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-08-20 10:43:07.003854 tmplot-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-08-20 10:42:22.000000 tmplot-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-08-20 10:42:22.000000 tmplot-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-08-20 10:43:07.007854 tmplot-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-08-20 10:42:22.000000 tmplot-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 10:43:07.003854 tmplot-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 10:43:07.003854 tmplot-0.0.9/src/tmplot/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-20 10:42:22.000000 tmplot-0.0.9/src/tmplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6351 2022-08-20 10:42:22.000000 tmplot-0.0.9/src/tmplot/_distance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12318 2022-08-20 10:42:22.000000 tmplot-0.0.9/src/tmplot/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-08-20 10:42:22.000000 tmplot-0.0.9/src/tmplot/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11404 2022-08-20 10:42:22.000000 tmplot-0.0.9/src/tmplot/_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6256 2022-08-20 10:42:22.000000 tmplot-0.0.9/src/tmplot/_stability.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8417 2022-08-20 10:42:22.000000 tmplot-0.0.9/src/tmplot/_vis.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 10:43:07.003854 tmplot-0.0.9/src/tmplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-08-20 10:43:06.000000 tmplot-0.0.9/src/tmplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-08-20 10:43:06.000000 tmplot-0.0.9/src/tmplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-20 10:43:06.000000 tmplot-0.0.9/src/tmplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-20 10:43:06.000000 tmplot-0.0.9/src/tmplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-20 10:43:06.000000 tmplot-0.0.9/src/tmplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-20 10:43:06.000000 tmplot-0.0.9/src/tmplot.egg-info/zip-safe
```

### Comparing `tmplot-0.0.8/LICENSE` & `tmplot-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tmplot-0.0.8/PKG-INFO` & `tmplot-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tmplot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Visualization of Topic Modeling Results
 Home-page: https://github.com/maximtrp/tmplot
 Author: maximtrp
 Author-email: maximtrp@gmail.com
 License: MIT
 Keywords: data science,data analytics
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: General
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -101,9 +100,7 @@
 tmp.plot_terms(terms_probs)
 
 # Running report interface
 tmp.report(model, docs=docs, width=250)
 ```
 
 You can find more examples in the [tutorial](https://tmplot.readthedocs.io/en/latest/tutorial.html).
-
-
```

### Comparing `tmplot-0.0.8/README.md` & `tmplot-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tmplot-0.0.8/setup.cfg` & `tmplot-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `tmplot-0.0.8/src/tmplot/_distance.py` & `tmplot-0.0.9/src/tmplot/_distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,18 @@
     DataFrame
         Topics scatter coordinates.
     """
     if not method_kws:
         method_kws = {'n_components': 2}
 
     if method == 'tsne':
-        method_kws.setdefault('metric',  'precomputed')
+        method_kws.setdefault('init', 'pca')
+        method_kws.setdefault('learning_rate', 'auto')
+        method_kws.setdefault(
+            'perplexity', min(50, max(topic_dists.shape[0] // 2, 5)))
         transformer = TSNE(**method_kws)
 
     elif method == 'sem':
         method_kws.setdefault('affinity', 'precomputed')
         transformer = SpectralEmbedding(**method_kws)
 
     elif method == 'mds':
```

### Comparing `tmplot-0.0.8/src/tmplot/_helpers.py` & `tmplot-0.0.9/src/tmplot/_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     if model and not theta:
         theta = get_theta(model, corpus=corpus).values
 
     def _select_docs(docs, theta, topic_id: int):
         probs = theta[topic_id, :]
         idx = argsort(probs)[:-docs_num-1:-1]
         result = Series(list(map(lambda x: docs[x], idx)))
-        result.name = 'topic{}'.format(topic_id)
+        result.name = f'topic{topic_id}'
         return result
 
     topics_num = theta.shape[0]
     topics_idx = arange(topics_num) if topics is None else topics
     return concat(
         map(lambda x: _select_docs(docs, theta, x), topics_idx), axis=1)
```

### Comparing `tmplot-0.0.8/src/tmplot/_metrics.py` & `tmplot-0.0.9/src/tmplot/_metrics.py`

 * *Files identical despite different names*

### Comparing `tmplot-0.0.8/src/tmplot/_report.py` & `tmplot-0.0.9/src/tmplot/_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 __all__ = ['prepare_coords', 'report']
+import warnings
 from typing import Optional, Sequence, List
 from copy import deepcopy
 from ipywidgets import widgets as wdg
 from pandas import DataFrame
 from ._distance import get_topics_dist, get_topics_scatter
 from ._vis import plot_scatter_topics, plot_terms, plot_docs
 from ._helpers import (
     calc_terms_probs_ratio,
     get_phi, get_theta,
     get_top_docs)
 
+warnings.filterwarnings("ignore", category=DeprecationWarning)
+warnings.filterwarnings("ignore", category=FutureWarning)
+
 
 def prepare_coords(
         model: object,
         labels: Optional[Sequence] = None,
         dist_kws: dict = None,
         scatter_kws: dict = None) -> DataFrame:
     """Prepare coordinates for topics scatter plot.
@@ -39,37 +43,38 @@
     topics_dists = get_topics_dist(phi, **dist_kws)
     topics_coords = get_topics_scatter(topics_dists, theta, **scatter_kws)
     topics_coords['label'] = labels or theta.index
     return topics_coords
 
 
 def report(
-        model: object = None,
-        docs: Optional[Sequence[str]] = None,
+        model: object,
+        docs: Sequence[str],
+        *,
         topics_labels: Optional[Sequence[str]] = None,
         corpus: Optional[List] = None,
         layout: wdg.Layout = None,
         show_headers: bool = True,
         show_docs: bool = True,
         show_words: bool = True,
         show_topics: bool = True,
         topics_kws: dict = None,
         height: int = 500,
-        width: int = 250,
+        width: int = 300,
         coords_kws: dict = None,
         words_kws: dict = None,
         docs_kws: dict = None,
         top_docs_kws: dict = None) -> wdg.VBox:
     """Interactive report interface.
 
     Parameters
     ----------
-    model : object, optional
+    model : object
         Topic model instance.
-    docs : Optional[Sequence[str]], optional
+    docs : Sequence[str]
         Documents.
     topics_labels : Optional[Sequence[str]], optional
         Topics labels.
     corpus : Optional[List[str]], optional
         Gensim corpus.
     layout : wdg.Layout, optional
         Interface layout instance.
@@ -106,15 +111,15 @@
     _words_kws = {
         'chart_kws': {'height': height, 'width': width}}\
         if not words_kws else deepcopy(words_kws)
     _top_docs_kws = {} if not docs_kws else deepcopy(top_docs_kws)
     _docs_kws = {} if not docs_kws else deepcopy(docs_kws)
 
     # Headers init
-    topics_header = wdg.HTML('<b>Topics scatter plot</b>')\
+    topics_header = wdg.HTML('<b>Intertopic distance plot</b>')\
         if show_headers and show_topics else None
     words_header = wdg.HTML('<b>Relevant words (terms)</b>')\
         if show_headers and show_words else None
     docs_header = wdg.HTML('<b>Top documents in a topic</b>')\
         if show_headers and show_docs else None
 
     # Layout init
@@ -194,18 +199,18 @@
             })
             display(plot_scatter_topics(**_topics_kws))
 
     if show_topics:
         topics_plot_children = [topics_header] if show_headers else []
         options_methods = [
             ('TSNE', 'tsne'),
-            ('SpectralEmbedding', 'sem'),
+            ('Spectral Embedding', 'sem'),
             ('MDS', 'mds'),
-            ('LocallyLinearEmbedding (Standard)', 'lle'),
-            ('LocallyLinearEmbedding (LTSA)', 'ltsa'),
+            ('Locally Linear Embedding (Standard)', 'lle'),
+            ('Locally Linear Embedding (LTSA)', 'ltsa'),
             ('Isomap', 'isomap')
         ]
         topics_method_header = wdg.HTML('Select a method:')
         topics_method = wdg.Dropdown(
             options=options_methods,
             value='tsne',
             layout=wdg.Layout(width=f'{width/1.25}px')
```

### Comparing `tmplot-0.0.8/src/tmplot/_stability.py` & `tmplot-0.0.9/src/tmplot/_stability.py`

 * *Files identical despite different names*

### Comparing `tmplot-0.0.8/src/tmplot/_vis.py` & `tmplot-0.0.9/src/tmplot/_vis.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,18 +79,18 @@
     altair.Chart
         Topics scatter plot.
     """
     if not chart_kws:
         chart_kws = {}
 
     if not x_kws:
-        x_kws = {'shorthand': x_col}
+        x_kws = {'shorthand': x_col, 'axis': None}
 
     if not y_kws:
-        y_kws = {'shorthand': y_col}
+        y_kws = {'shorthand': y_col, 'axis': None}
 
     if not circle_kws:
         circle_kws = {"opacity": 0.33, "stroke": 'black', "strokeWidth": 1}
 
     if not size_kws:
         size_kws = {
             'title': 'Marginal topic distribution',
@@ -165,15 +165,14 @@
 
     text = base\
         .mark_text(**text_kws)\
         .encode(**text_enc_kws)
 
     return (rule + rule2 + points + text)\
         .configure_axis(labelFontSize=font_size, titleFontSize=font_size, grid=False)\
-        .configure(axis=AxisConfig(disable=True))\
         .configure_view(stroke='transparent', strokeWidth=0)\
         .configure_legend(
             orient='bottom',
             labelFontSize=font_size,
             titleFontSize=font_size)
```

### Comparing `tmplot-0.0.8/src/tmplot.egg-info/PKG-INFO` & `tmplot-0.0.9/src/tmplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tmplot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Visualization of Topic Modeling Results
 Home-page: https://github.com/maximtrp/tmplot
 Author: maximtrp
 Author-email: maximtrp@gmail.com
 License: MIT
 Keywords: data science,data analytics
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: General
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -101,9 +100,7 @@
 tmp.plot_terms(terms_probs)
 
 # Running report interface
 tmp.report(model, docs=docs, width=250)
 ```
 
 You can find more examples in the [tutorial](https://tmplot.readthedocs.io/en/latest/tutorial.html).
-
-
```


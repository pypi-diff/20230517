# Comparing `tmp/topic_wizard-0.2.4.tar.gz` & `tmp/topic_wizard-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topic_wizard-0.2.4.tar", max compression
+gzip compressed data, was "topic_wizard-0.2.5.tar", max compression
```

## Comparing `topic_wizard-0.2.4.tar` & `topic_wizard-0.2.5.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0     1071 2023-01-29 12:25:42.522855 topic_wizard-0.2.4/LICENSE
--rw-r--r--   0        0        0     2142 2023-05-05 08:47:51.298632 topic_wizard-0.2.4/README.md
--rw-r--r--   0        0        0      640 2023-05-10 13:43:20.671757 topic_wizard-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      404 2023-05-10 13:39:02.256545 topic_wizard-0.2.4/topicwizard/__init__.py
--rw-r--r--   0        0        0     7219 2023-05-06 10:19:10.654488 topic_wizard-0.2.4/topicwizard/app.py
--rw-r--r--   0        0        0   177216 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/blueprints/__init__.py
--rw-r--r--   0        0        0     5602 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/blueprints/app.py
--rw-r--r--   0        0        0     4339 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/blueprints/documents.py
--rw-r--r--   0        0        0     1355 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/blueprints/template.py
--rw-r--r--   0        0        0     5195 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/blueprints/topics.py
--rw-r--r--   0        0        0     3143 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/blueprints/words.py
--rw-r--r--   0        0        0     3080 2023-05-10 12:08:24.294778 topic_wizard-0.2.4/topicwizard/compatibility/bertopic.py
--rw-r--r--   0        0        0     6652 2023-05-06 08:12:06.292221 topic_wizard-0.2.4/topicwizard/compatibility/gensim.py
--rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/__init__.py
--rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/documents/__init__.py
--rw-r--r--   0        0        0     1993 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/documents/document_map.py
--rw-r--r--   0        0        0     1399 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/documents/document_pie.py
--rw-r--r--   0        0        0     1318 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/documents/document_selector.py
--rw-r--r--   0        0        0     1468 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/documents/document_timeline.py
--rw-r--r--   0        0        0     1131 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/documents/document_wordcloud.py
--rw-r--r--   0        0        0     1362 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/documents/window_slider.py
--rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/__init__.py
--rw-r--r--   0        0        0     1906 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/intertopic_map.py
--rw-r--r--   0        0        0     1006 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/relevance_slider.py
--rw-r--r--   0        0        0      224 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/topic_barplot.py
--rw-r--r--   0        0        0     1568 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/topic_namer.py
--rw-r--r--   0        0        0     1447 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/topic_switcher.py
--rw-r--r--   0        0        0      228 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/wordcloud.py
--rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/words/__init__.py
--rw-r--r--   0        0        0     1880 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/words/association_slider.py
--rw-r--r--   0        0        0     1762 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/words/word_barplot.py
--rw-r--r--   0        0        0     2514 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/words/word_map.py
--rw-r--r--   0        0        0     1300 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/words/word_selector.py
--rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/plots/__init__.py
--rw-r--r--   0        0        0     5183 2023-05-06 08:17:16.043369 topic_wizard-0.2.4/topicwizard/plots/documents.py
--rw-r--r--   0        0        0     4257 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/plots/topics.py
--rw-r--r--   0        0        0     3503 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/plots/words.py
--rw-r--r--   0        0        0     2708 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/prepare/documents.py
--rw-r--r--   0        0        0     4895 2023-05-10 13:42:17.894976 topic_wizard-0.2.4/topicwizard/prepare/topics.py
--rw-r--r--   0        0        0     1102 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/prepare/utils.py
--rw-r--r--   0        0        0     4923 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/prepare/words.py
--rw-r--r--   0        0        0     3165 1970-01-01 00:00:00.000000 topic_wizard-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2908 2023-05-17 11:35:28.098112 topic_wizard-0.2.5/README.md
+-rw-r--r--   0        0        0      640 2023-05-17 11:35:19.210098 topic_wizard-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-05-17 10:58:27.942406 topic_wizard-0.2.5/topicwizard/__init__.py
+-rw-r--r--   0        0        0     7219 2023-05-17 10:58:27.942406 topic_wizard-0.2.5/topicwizard/app.py
+-rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.2.5/topicwizard/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.5/topicwizard/blueprints/__init__.py
+-rw-r--r--   0        0        0     5602 2023-02-19 17:44:29.048902 topic_wizard-0.2.5/topicwizard/blueprints/app.py
+-rw-r--r--   0        0        0     4322 2023-05-17 11:05:13.211055 topic_wizard-0.2.5/topicwizard/blueprints/documents.py
+-rw-r--r--   0        0        0        0 2023-05-17 11:09:41.951533 topic_wizard-0.2.5/topicwizard/blueprints/groups.py
+-rw-r--r--   0        0        0     1355 2023-01-17 16:03:27.727135 topic_wizard-0.2.5/topicwizard/blueprints/template.py
+-rw-r--r--   0        0        0     5082 2023-05-17 11:05:33.415089 topic_wizard-0.2.5/topicwizard/blueprints/topics.py
+-rw-r--r--   0        0        0     3015 2023-05-17 11:05:57.615132 topic_wizard-0.2.5/topicwizard/blueprints/words.py
+-rw-r--r--   0        0        0     3010 2023-05-17 11:32:05.865790 topic_wizard-0.2.5/topicwizard/compatibility/bertopic.py
+-rw-r--r--   0        0        0     6425 2023-05-17 11:33:07.273886 topic_wizard-0.2.5/topicwizard/compatibility/gensim.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.5/topicwizard/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.5/topicwizard/components/documents/__init__.py
+-rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.2.5/topicwizard/components/documents/document_map.py
+-rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.2.5/topicwizard/components/documents/document_pie.py
+-rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.2.5/topicwizard/components/documents/document_selector.py
+-rw-r--r--   0        0        0     1468 2023-04-24 14:04:50.954173 topic_wizard-0.2.5/topicwizard/components/documents/document_timeline.py
+-rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/documents/document_wordcloud.py
+-rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/documents/window_slider.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/__init__.py
+-rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/intertopic_map.py
+-rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/relevance_slider.py
+-rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/topic_barplot.py
+-rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/topic_namer.py
+-rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/topic_switcher.py
+-rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/wordcloud.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/words/__init__.py
+-rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.2.5/topicwizard/components/words/association_slider.py
+-rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/words/word_barplot.py
+-rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.2.5/topicwizard/components/words/word_map.py
+-rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.2.5/topicwizard/components/words/word_selector.py
+-rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.2.5/topicwizard/plots/__init__.py
+-rw-r--r--   0        0        0     5183 2023-05-17 10:58:27.942406 topic_wizard-0.2.5/topicwizard/plots/documents.py
+-rw-r--r--   0        0        0     4257 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/plots/topics.py
+-rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.2.5/topicwizard/plots/words.py
+-rw-r--r--   0        0        0     2708 2023-04-24 13:29:18.682128 topic_wizard-0.2.5/topicwizard/prepare/documents.py
+-rw-r--r--   0        0        0     4895 2023-05-17 10:58:27.942406 topic_wizard-0.2.5/topicwizard/prepare/topics.py
+-rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.2.5/topicwizard/prepare/utils.py
+-rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.2.5/topicwizard/prepare/words.py
+-rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 topic_wizard-0.2.5/setup.py
+-rw-r--r--   0        0        0     3931 1970-01-01 00:00:00.000000 topic_wizard-0.2.5/PKG-INFO
```

### Comparing `topic_wizard-0.2.4/LICENSE` & `topic_wizard-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/README.md` & `topic_wizard-0.2.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,25 +13,31 @@
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 
 
 
 https://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4
 
+## New in version 0.2.5 🌟 🌟
+
+ - [Compatiblity with Gensim topic models](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html) 💥
+ - [Compatibility with BERTopic](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html)(experimental 🧪)
+ - Topic name inference 🧠
 
 
 ## Features
 
 -   Investigate complex relations between topics, words and documents
 -   Highly interactive
--   Name topics
+-   Automatically infer topic names
+-   Name topics manually
 -   Pretty :art:
 -   Intuitive :cow:
 -   Clean API :candy:
--   Sklearn compatible :nut_and_bolt:
+-   Sklearn, Gensim and BERTopic compatible :nut_and_bolt:
 -   Easy deployment :earth_africa:
 
 ## Installation
 
 Install from PyPI:
 
 ```bash
@@ -39,37 +45,43 @@
 ```
 
 ## Usage ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))
 
 ### Step 1:
 
 Train a scikit-learn compatible topic model.
+(If you want to use non-scikit-learn topic models, check [compatibility](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html))
 
 ```python
 from sklearn.decomposition import NMF
 from sklearn.feature_extraction.text import CountVectorizer
-from sklearn.pipeline import Pipeline
+from sklearn.pipeline import make_pipeline
 
-topic_pipeline = Pipeline(
-    [
-        ("bow", CountVectorizer()),
-        ("nmf", NMF(n_components=10)),
-    ]
+# Create topic pipeline
+topic_pipeline = make_pipeline(
+    CountVectorizer(),
+    NMF(n_components=10),
 )
+
+# Then fit it on the given texts
 topic_pipeline.fit(texts)
 ```
 
 ### Step 2:
 
 Visualize with topicwizard.
 
 ```python
 import topicwizard
 
-topicwizard.visualize(pipeline=topic_pipeline, corpus=texts)
+# You can get automatically assigned topic labels, that you can change manually later
+topic_names = topicwizard.infer_topic_names(pipeline=pipeline)
+
+# Then you can visualize your results
+topicwizard.visualize(pipeline=topic_pipeline, corpus=texts, topic_names=topic_names)
 ```
 
 ### Step 3:
 
 Investigate :eyes: .
 
 #### a) Topics
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `topic_wizard-0.2.4/pyproject.toml` & `topic_wizard-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "topic-wizard"
-version = "0.2.4"
+version = "0.2.5"
 description = "Pretty and opinionated topic model visualization in Python."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "topicwizard"}]
 
 [tool.poetry.dependencies]
```

### Comparing `topic_wizard-0.2.4/topicwizard/app.py` & `topic_wizard-0.2.5/topicwizard/app.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/assets/favicon.ico` & `topic_wizard-0.2.5/topicwizard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/blueprints/app.py` & `topic_wizard-0.2.5/topicwizard/blueprints/app.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/blueprints/documents.py` & `topic_wizard-0.2.5/topicwizard/blueprints/documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 import numpy as np
 from dash_extensions.enrich import DashBlueprint, dcc, html
 from plotly import colors
 
 import topicwizard.prepare.documents as prepare
 from topicwizard.components.documents.document_map import create_document_map
 from topicwizard.components.documents.document_pie import create_document_pie
-from topicwizard.components.documents.document_selector import \
-    create_document_selector
+from topicwizard.components.documents.document_selector import create_document_selector
 from topicwizard.components.documents.document_timeline import create_timeline
-from topicwizard.components.documents.document_wordcloud import \
-    create_document_wordcloud
+from topicwizard.components.documents.document_wordcloud import (
+    create_document_wordcloud,
+)
 from topicwizard.components.documents.window_slider import create_window_slider
 
 
 def create_blueprint(
     vocab: np.ndarray,
     document_term_matrix: np.ndarray,
     document_topic_matrix: np.ndarray,
     topic_term_matrix: np.ndarray,
     document_names: List[str],
     corpus: List[str],
     vectorizer: Any,
     topic_model: Any,
-    topic_names: List[str],
+    **kwargs,
 ) -> DashBlueprint:
     # --------[ Preparing data ]--------
     n_topics = topic_term_matrix.shape[0]
     document_positions = prepare.document_positions(
         document_term_matrix=document_term_matrix
     )
     dominant_topics = prepare.dominant_topic(
```

### Comparing `topic_wizard-0.2.4/topicwizard/blueprints/template.py` & `topic_wizard-0.2.5/topicwizard/blueprints/template.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/blueprints/topics.py` & `topic_wizard-0.2.5/topicwizard/blueprints/topics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 import functools
-from typing import Tuple, List, Any
+from typing import Any, List, Tuple
 
 import dash_mantine_components as dmc
 import numpy as np
 import plotly.graph_objects as go
-from dash_extensions.enrich import (
-    DashBlueprint,
-    Input,
-    Output,
-    State,
-    dcc,
-    html,
-)
+from dash_extensions.enrich import DashBlueprint, Input, Output, State, dcc, html
 
 import topicwizard.plots.topics as plots
 import topicwizard.prepare.topics as prepare
 from topicwizard.components.topics.intertopic_map import create_intertopic_map
 from topicwizard.components.topics.relevance_slider import relevance_slider
 from topicwizard.components.topics.topic_barplot import topic_barplot
 from topicwizard.components.topics.topic_namer import topic_namer
@@ -51,21 +44,17 @@
 
 
 def create_blueprint(
     vocab: np.ndarray,
     document_term_matrix: np.ndarray,
     document_topic_matrix: np.ndarray,
     topic_term_matrix: np.ndarray,
-    document_names: List[str],
-    corpus: List[str],
-    vectorizer: Any,
-    topic_model: Any,
     topic_names: List[str],
+    **kwargs,
 ) -> DashBlueprint:
-
     # --------[ Preparing data ]--------
     topic_positions = prepare.topic_positions(topic_term_matrix)
     (
         topic_importances,
         term_importances,
         topic_term_importances,
     ) = prepare.topic_importances(
```

### Comparing `topic_wizard-0.2.4/topicwizard/blueprints/words.py` & `topic_wizard-0.2.5/topicwizard/blueprints/words.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,26 @@
 
 import dash_mantine_components as dmc
 import numpy as np
 from dash_extensions.enrich import DashBlueprint, dcc, html
 from plotly import colors
 
 import topicwizard.prepare.words as prepare
-from topicwizard.components.words.association_slider import \
-    create_association_slider
+from topicwizard.components.words.association_slider import create_association_slider
 from topicwizard.components.words.word_barplot import create_word_barplot
 from topicwizard.components.words.word_map import create_word_map
 from topicwizard.components.words.word_selector import create_word_selector
 
 
 def create_blueprint(
     vocab: np.ndarray,
     document_term_matrix: np.ndarray,
-    document_topic_matrix: np.ndarray,
     topic_term_matrix: np.ndarray,
-    document_names: List[str],
-    corpus: List[str],
-    vectorizer: Any,
-    topic_model: Any,
     topic_names: List[str],
+    **kwargs,
 ) -> DashBlueprint:
     # --------[ Preparing data ]--------
     word_positions = prepare.word_positions(topic_term_matrix=topic_term_matrix)
     word_frequencies = prepare.word_importances(document_term_matrix)
     dominant_topic = prepare.dominant_topic(topic_term_matrix)
     n_topics = len(topic_names)
     # Creating unified color scheme
```

### Comparing `topic_wizard-0.2.4/topicwizard/compatibility/bertopic.py` & `topic_wizard-0.2.5/topicwizard/compatibility/bertopic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from typing import Callable, Iterable, List, Tuple
+from typing import Iterable, List, Tuple
 
 import numpy as np
 import scipy.sparse as spr
-from bertopic import BERTopic
 from sklearn.base import BaseEstimator
 from sklearn.pipeline import Pipeline, make_pipeline
 
 
 class _SparseWithText(spr.csr_array):
     def __init__(self, *args, texts: Iterable[str] = None, **kwargs):
         super().__init__(*args, **kwargs)
         if texts is None:
             self.texts = None
         else:
             self.texts = list(texts)
 
 
 class _BERTopicVectorizer(BaseEstimator):
-    def __init__(self, topic_model: BERTopic):
+    def __init__(self, topic_model):
         self.topic_model = topic_model
         self.vectorizer = topic_model.vectorizer_model
         self.vocabulary_ = self.vectorizer.vocabulary_
         self.stop_words_ = self.vectorizer.stop_words_
         self.fixed_vocabulary_ = self.vectorizer.fixed_vocabulary_
 
     def fit(self, raw_documents: Iterable[str], y=None):
@@ -39,15 +38,15 @@
         return self.transform(raw_documents)
 
     def get_feature_names_out(self):
         return self.vectorizer.get_feature_names_out()
 
 
 class _BERTopicModel(BaseEstimator):
-    def __init__(self, topic_model: BERTopic):
+    def __init__(self, topic_model):
         self.topic_model = topic_model
         self.model = topic_model
 
     @property
     def _has_outliers(self):
         return -1 in self.model.topic_labels_
 
@@ -67,15 +66,15 @@
         return np.array(dist)
 
     def fit_transform(self, X, y=None):
         self.fit(X)
         return self.transform(X)
 
 
-def bertopic_pipeline(model: BERTopic) -> Tuple[Pipeline, List[str]]:
+def bertopic_pipeline(model) -> Tuple[Pipeline, List[str]]:
     """Creates sklearn compatible wrapper for a BERTopic topic pipeline.
 
     Parameters
     ----------
     model: BERTopic
         Any BERTopic model.
```

### Comparing `topic_wizard-0.2.4/topicwizard/compatibility/gensim.py` & `topic_wizard-0.2.5/topicwizard/compatibility/gensim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import warnings
 from typing import Iterable
 
 import numpy as np
 import scipy.sparse as spr
-from gensim.corpora.dictionary import Dictionary
-from gensim.models import LdaModel, LdaMulticore, LsiModel, Nmf
 from sklearn.base import BaseEstimator
 from sklearn.pipeline import Pipeline, make_pipeline
 from tqdm import tqdm
 
 
 class DictionaryVectorizer(BaseEstimator):
     """Wrapper for Gensim's dictionary object as an sklearn compatible vectorizer object.
@@ -25,15 +23,15 @@
         Mapping of feature indices to Gensim dictionary IDs.
     key_to_index: dict of int to int
         Mapping of Gensim Dictionary IDs to feature indices.
     vocabulary_: dict of str to int
         Mapping of terms to feature indices.
     """
 
-    def __init__(self, dictionary: Dictionary):
+    def __init__(self, dictionary):
         self.dictionary = dictionary
         self.index_to_key = np.array(dictionary.keys())
         self.key_to_index = {key: index for index, key in enumerate(self.index_to_key)}
         self.feature_names_out = np.array(
             [dictionary[key] for key in self.index_to_key]
         )
         self.vocabulary_ = {
@@ -114,15 +112,15 @@
     ----------
     components_: array of shape (n_components, n_features)
         Feature importances for each topic.
     """
 
     def __init__(
         self,
-        model: LdaModel | LdaMulticore | Nmf | LsiModel,
+        model,
         index_to_key: dict[int, int],
     ):
         self.model = model
         self.index_to_key = index_to_key
         self.components_ = model.get_topics()
         (self.n_components, _) = self.components_.shape
 
@@ -167,17 +165,15 @@
 
     def fit_transform(self, X, y=None):
         """Does the same as transform(), kept for compatiblity reasons."""
         self.fit(X)
         return self.transform(X)
 
 
-def gensim_pipeline(
-    dictionary: Dictionary, model: LdaModel | LdaMulticore | Nmf | LsiModel
-) -> Pipeline:
+def gensim_pipeline(dictionary, model) -> Pipeline:
     """Creates sklearn compatible wrapper for a Gensim topic pipeline.
 
     Parameters
     ----------
     dictionary: gensim.corpora.dictionary.Dictionary
         Gensim's dictionary object. Please only pass already fitted
         dictionary objects.
```

### Comparing `topic_wizard-0.2.4/topicwizard/components/documents/document_map.py` & `topic_wizard-0.2.5/topicwizard/components/documents/document_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/documents/document_pie.py` & `topic_wizard-0.2.5/topicwizard/components/documents/document_pie.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/documents/document_selector.py` & `topic_wizard-0.2.5/topicwizard/components/documents/document_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/documents/document_timeline.py` & `topic_wizard-0.2.5/topicwizard/components/documents/document_timeline.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/documents/document_wordcloud.py` & `topic_wizard-0.2.5/topicwizard/components/documents/document_wordcloud.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/documents/window_slider.py` & `topic_wizard-0.2.5/topicwizard/components/documents/window_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/topics/intertopic_map.py` & `topic_wizard-0.2.5/topicwizard/components/topics/intertopic_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/topics/relevance_slider.py` & `topic_wizard-0.2.5/topicwizard/components/topics/relevance_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/topics/topic_namer.py` & `topic_wizard-0.2.5/topicwizard/components/topics/topic_namer.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/topics/topic_switcher.py` & `topic_wizard-0.2.5/topicwizard/components/topics/topic_switcher.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/words/association_slider.py` & `topic_wizard-0.2.5/topicwizard/components/words/association_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/words/word_barplot.py` & `topic_wizard-0.2.5/topicwizard/components/words/word_barplot.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/words/word_map.py` & `topic_wizard-0.2.5/topicwizard/components/words/word_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/components/words/word_selector.py` & `topic_wizard-0.2.5/topicwizard/components/words/word_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/plots/documents.py` & `topic_wizard-0.2.5/topicwizard/plots/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/plots/topics.py` & `topic_wizard-0.2.5/topicwizard/plots/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/plots/words.py` & `topic_wizard-0.2.5/topicwizard/plots/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/prepare/documents.py` & `topic_wizard-0.2.5/topicwizard/prepare/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/prepare/topics.py` & `topic_wizard-0.2.5/topicwizard/prepare/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/prepare/utils.py` & `topic_wizard-0.2.5/topicwizard/prepare/utils.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/topicwizard/prepare/words.py` & `topic_wizard-0.2.5/topicwizard/prepare/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.4/PKG-INFO` & `topic_wizard-0.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topic-wizard
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pretty and opinionated topic model visualization in Python.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,25 +40,31 @@
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 
 
 
 https://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4
 
+## New in version 0.2.5 🌟 🌟
+
+ - [Compatiblity with Gensim topic models](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html) 💥
+ - [Compatibility with BERTopic](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html)(experimental 🧪)
+ - Topic name inference 🧠
 
 
 ## Features
 
 -   Investigate complex relations between topics, words and documents
 -   Highly interactive
--   Name topics
+-   Automatically infer topic names
+-   Name topics manually
 -   Pretty :art:
 -   Intuitive :cow:
 -   Clean API :candy:
--   Sklearn compatible :nut_and_bolt:
+-   Sklearn, Gensim and BERTopic compatible :nut_and_bolt:
 -   Easy deployment :earth_africa:
 
 ## Installation
 
 Install from PyPI:
 
 ```bash
@@ -66,37 +72,43 @@
 ```
 
 ## Usage ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))
 
 ### Step 1:
 
 Train a scikit-learn compatible topic model.
+(If you want to use non-scikit-learn topic models, check [compatibility](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html))
 
 ```python
 from sklearn.decomposition import NMF
 from sklearn.feature_extraction.text import CountVectorizer
-from sklearn.pipeline import Pipeline
+from sklearn.pipeline import make_pipeline
 
-topic_pipeline = Pipeline(
-    [
-        ("bow", CountVectorizer()),
-        ("nmf", NMF(n_components=10)),
-    ]
+# Create topic pipeline
+topic_pipeline = make_pipeline(
+    CountVectorizer(),
+    NMF(n_components=10),
 )
+
+# Then fit it on the given texts
 topic_pipeline.fit(texts)
 ```
 
 ### Step 2:
 
 Visualize with topicwizard.
 
 ```python
 import topicwizard
 
-topicwizard.visualize(pipeline=topic_pipeline, corpus=texts)
+# You can get automatically assigned topic labels, that you can change manually later
+topic_names = topicwizard.infer_topic_names(pipeline=pipeline)
+
+# Then you can visualize your results
+topicwizard.visualize(pipeline=topic_pipeline, corpus=texts, topic_names=topic_names)
 ```
 
 ### Step 3:
 
 Investigate :eyes: .
 
 #### a) Topics
```


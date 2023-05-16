# Comparing `tmp/text2graphapi-0.1.7.tar.gz` & `tmp/text2graphapi-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2graphapi-0.1.7.tar", last modified: Tue May 16 21:54:14 2023, max compression
+gzip compressed data, was "text2graphapi-0.1.8.tar", last modified: Tue May 16 22:28:27 2023, max compression
```

## Comparing `text2graphapi-0.1.7.tar` & `text2graphapi-0.1.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.460636 text2graphapi-0.1.7/
--rw-rw-rw-   0        0        0       82 2023-01-17 01:14:45.000000 text2graphapi-0.1.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2022-12-02 17:54:23.000000 text2graphapi-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2022-12-02 17:54:23.000000 text2graphapi-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5403 2023-05-16 21:54:14.459569 text2graphapi-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4877 2023-04-25 17:11:34.000000 text2graphapi-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.362593 text2graphapi-0.1.7/docs/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.313319 text2graphapi-0.1.7/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.314314 text2graphapi-0.1.7/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.379578 text2graphapi-0.1.7/docs/_build/html/_sources/
--rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.7/docs/_build/html/_sources/Cooocurrence.rst.txt
--rw-rw-rw-   0        0        0     1663 2023-03-30 14:12:11.000000 text2graphapi-0.1.7/docs/_build/html/_sources/index.rst.txt
--rw-rw-rw-   0        0        0       46 2022-12-05 21:50:59.000000 text2graphapi-0.1.7/docs/_build/html/_sources/modules.rst.txt
--rw-rw-rw-   0        0        0      408 2022-12-05 21:50:59.000000 text2graphapi-0.1.7/docs/_build/html/_sources/src.rst.txt
--rw-rw-rw-   0        0        0     1783 2022-12-05 21:50:59.000000 text2graphapi-0.1.7/docs/conf.py
--rw-rw-rw-   0        0        0      590 2023-03-30 04:06:40.000000 text2graphapi-0.1.7/notes.txt
--rw-rw-rw-   0        0        0      201 2023-01-17 01:14:45.000000 text2graphapi-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 21:54:14.461571 text2graphapi-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-05-16 21:49:34.000000 text2graphapi-0.1.7/setup.py
--rw-rw-rw-   0        0        0      379 2023-03-16 18:14:42.000000 text2graphapi-0.1.7/test_spacy.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.383602 text2graphapi-0.1.7/tests/
--rw-rw-rw-   0        0        0        0 2022-10-12 14:46:40.000000 text2graphapi-0.1.7/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.389913 text2graphapi-0.1.7/text2graphapi/
--rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.7/text2graphapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.327310 text2graphapi-0.1.7/text2graphapi/docs/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.324462 text2graphapi-0.1.7/text2graphapi/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.326307 text2graphapi-0.1.7/text2graphapi/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.409570 text2graphapi-0.1.7/text2graphapi/docs/build/html/_sources/
--rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.7/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt
--rw-rw-rw-   0        0        0     1768 2023-03-30 13:07:45.000000 text2graphapi-0.1.7/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt
--rw-rw-rw-   0        0        0     1702 2023-03-30 11:19:22.000000 text2graphapi-0.1.7/text2graphapi/docs/build/html/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.422577 text2graphapi-0.1.7/text2graphapi/docs/source/
--rw-rw-rw-   0        0        0     1352 2023-04-25 17:11:34.000000 text2graphapi-0.1.7/text2graphapi/docs/source/conf.py
--rw-rw-rw-   0        0        0     8092 2023-05-16 21:37:03.000000 text2graphapi-0.1.7/text2graphapi/main.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.451571 text2graphapi-0.1.7/text2graphapi/src/
--rw-rw-rw-   0        0        0     7212 2023-05-16 21:49:48.000000 text2graphapi-0.1.7/text2graphapi/src/Cooccurrence.py
--rw-rw-rw-   0        0        0     1088 2023-01-17 01:14:45.000000 text2graphapi-0.1.7/text2graphapi/src/Graph.py
--rw-rw-rw-   0        0        0     1018 2023-05-16 21:29:11.000000 text2graphapi-0.1.7/text2graphapi/src/GraphTransformation.py
--rw-rw-rw-   0        0        0    13721 2023-05-16 21:49:58.000000 text2graphapi-0.1.7/text2graphapi/src/Heterogeneous.py
--rw-rw-rw-   0        0        0     8828 2023-05-16 21:50:32.000000 text2graphapi-0.1.7/text2graphapi/src/Preprocessing.py
--rw-rw-rw-   0        0        0     1887 2023-05-16 21:53:00.000000 text2graphapi-0.1.7/text2graphapi/src/Utils.py
--rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.7/text2graphapi/src/__init__.py
--rw-rw-rw-   0        0        0      482 2023-04-25 17:11:34.000000 text2graphapi-0.1.7/text2graphapi/src/configs.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.457625 text2graphapi-0.1.7/text2graphapi/src/resources/
--rw-rw-rw-   0        0        0     4160 2023-01-17 01:14:45.000000 text2graphapi-0.1.7/text2graphapi/src/resources/stopwords_english.txt
--rw-rw-rw-   0        0        0     5256 2023-03-08 18:09:28.000000 text2graphapi-0.1.7/text2graphapi/src/resources/stopwords_french.txt
--rw-rw-rw-   0        0        0     4852 2023-01-17 01:14:45.000000 text2graphapi-0.1.7/text2graphapi/src/resources/stopwords_spanish.txt
--rw-rw-rw-   0        0        0     2248 2023-03-30 02:11:28.000000 text2graphapi-0.1.7/text2graphapi/testing.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:14.403571 text2graphapi-0.1.7/text2graphapi.egg-info/
--rw-rw-rw-   0        0        0     5403 2023-05-16 21:54:13.000000 text2graphapi-0.1.7/text2graphapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-05-16 21:54:14.000000 text2graphapi-0.1.7/text2graphapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 21:54:13.000000 text2graphapi-0.1.7/text2graphapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-05-16 21:54:13.000000 text2graphapi-0.1.7/text2graphapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-16 21:54:13.000000 text2graphapi-0.1.7/text2graphapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.556007 text2graphapi-0.1.8/
+-rw-rw-rw-   0        0        0       82 2023-01-17 01:14:45.000000 text2graphapi-0.1.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2022-12-02 17:54:23.000000 text2graphapi-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2022-12-02 17:54:23.000000 text2graphapi-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5403 2023-05-16 22:28:27.555005 text2graphapi-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4877 2023-04-25 17:11:34.000000 text2graphapi-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.446723 text2graphapi-0.1.8/docs/
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.409726 text2graphapi-0.1.8/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.410727 text2graphapi-0.1.8/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.462740 text2graphapi-0.1.8/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.8/docs/_build/html/_sources/Cooocurrence.rst.txt
+-rw-rw-rw-   0        0        0     1663 2023-03-30 14:12:11.000000 text2graphapi-0.1.8/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0       46 2022-12-05 21:50:59.000000 text2graphapi-0.1.8/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-rw-   0        0        0      408 2022-12-05 21:50:59.000000 text2graphapi-0.1.8/docs/_build/html/_sources/src.rst.txt
+-rw-rw-rw-   0        0        0     1783 2022-12-05 21:50:59.000000 text2graphapi-0.1.8/docs/conf.py
+-rw-rw-rw-   0        0        0      590 2023-03-30 04:06:40.000000 text2graphapi-0.1.8/notes.txt
+-rw-rw-rw-   0        0        0      201 2023-01-17 01:14:45.000000 text2graphapi-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 22:28:27.557003 text2graphapi-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-05-16 22:06:12.000000 text2graphapi-0.1.8/setup.py
+-rw-rw-rw-   0        0        0      379 2023-03-16 18:14:42.000000 text2graphapi-0.1.8/test_spacy.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.468732 text2graphapi-0.1.8/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-12 14:46:40.000000 text2graphapi-0.1.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.479730 text2graphapi-0.1.8/text2graphapi/
+-rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.8/text2graphapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.424724 text2graphapi-0.1.8/text2graphapi/docs/
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.421782 text2graphapi-0.1.8/text2graphapi/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.422723 text2graphapi-0.1.8/text2graphapi/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.501768 text2graphapi-0.1.8/text2graphapi/docs/build/html/_sources/
+-rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.8/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt
+-rw-rw-rw-   0        0        0     1768 2023-03-30 13:07:45.000000 text2graphapi-0.1.8/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt
+-rw-rw-rw-   0        0        0     1702 2023-03-30 11:19:22.000000 text2graphapi-0.1.8/text2graphapi/docs/build/html/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.514749 text2graphapi-0.1.8/text2graphapi/docs/source/
+-rw-rw-rw-   0        0        0     1352 2023-04-25 17:11:34.000000 text2graphapi-0.1.8/text2graphapi/docs/source/conf.py
+-rw-rw-rw-   0        0        0     8092 2023-05-16 21:37:03.000000 text2graphapi-0.1.8/text2graphapi/main.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.545723 text2graphapi-0.1.8/text2graphapi/src/
+-rw-rw-rw-   0        0        0     7185 2023-05-16 22:27:52.000000 text2graphapi-0.1.8/text2graphapi/src/Cooccurrence.py
+-rw-rw-rw-   0        0        0     1088 2023-01-17 01:14:45.000000 text2graphapi-0.1.8/text2graphapi/src/Graph.py
+-rw-rw-rw-   0        0        0     1018 2023-05-16 21:29:11.000000 text2graphapi-0.1.8/text2graphapi/src/GraphTransformation.py
+-rw-rw-rw-   0        0        0    13694 2023-05-16 22:20:14.000000 text2graphapi-0.1.8/text2graphapi/src/Heterogeneous.py
+-rw-rw-rw-   0        0        0     8832 2023-05-16 22:12:00.000000 text2graphapi-0.1.8/text2graphapi/src/Preprocessing.py
+-rw-rw-rw-   0        0        0     1887 2023-05-16 21:53:00.000000 text2graphapi-0.1.8/text2graphapi/src/Utils.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.8/text2graphapi/src/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-04-25 17:11:34.000000 text2graphapi-0.1.8/text2graphapi/src/configs.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.552005 text2graphapi-0.1.8/text2graphapi/src/resources/
+-rw-rw-rw-   0        0        0     4160 2023-01-17 01:14:45.000000 text2graphapi-0.1.8/text2graphapi/src/resources/stopwords_english.txt
+-rw-rw-rw-   0        0        0     5256 2023-03-08 18:09:28.000000 text2graphapi-0.1.8/text2graphapi/src/resources/stopwords_french.txt
+-rw-rw-rw-   0        0        0     4852 2023-01-17 01:14:45.000000 text2graphapi-0.1.8/text2graphapi/src/resources/stopwords_spanish.txt
+-rw-rw-rw-   0        0        0     2248 2023-03-30 02:11:28.000000 text2graphapi-0.1.8/text2graphapi/testing.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:28:27.495724 text2graphapi-0.1.8/text2graphapi.egg-info/
+-rw-rw-rw-   0        0        0     5403 2023-05-16 22:28:26.000000 text2graphapi-0.1.8/text2graphapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-05-16 22:28:27.000000 text2graphapi-0.1.8/text2graphapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:28:26.000000 text2graphapi-0.1.8/text2graphapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-05-16 22:28:26.000000 text2graphapi-0.1.8/text2graphapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-16 22:28:26.000000 text2graphapi-0.1.8/text2graphapi.egg-info/top_level.txt
```

### Comparing `text2graphapi-0.1.7/LICENSE.txt` & `text2graphapi-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/PKG-INFO` & `text2graphapi-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2graphapi
-Version: 0.1.7
+Version: 0.1.8
 Summary: Use this library to transform raw text into differents graph representations.
 Home-page: 
 Author: PLN-disca-iimas
 Author-email: andric.valdez@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `text2graphapi-0.1.7/README.md` & `text2graphapi-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/docs/_build/html/_sources/Cooocurrence.rst.txt` & `text2graphapi-0.1.8/docs/_build/html/_sources/Cooocurrence.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/docs/_build/html/_sources/index.rst.txt` & `text2graphapi-0.1.8/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/docs/conf.py` & `text2graphapi-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/notes.txt` & `text2graphapi-0.1.8/notes.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/setup.py` & `text2graphapi-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ROOT = path.abspath(path.dirname(__file__))
 
 with open(path.join(ROOT, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="text2graphapi",
-    version="0.1.7",
+    version="0.1.8",
     description="Use this library to transform raw text into differents graph representations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="PLN-disca-iimas",
     author_email="andric.valdez@gmail.com",
     license="MIT",
```

### Comparing `text2graphapi-0.1.7/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt` & `text2graphapi-0.1.8/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt` & `text2graphapi-0.1.8/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/docs/build/html/_sources/index.rst.txt` & `text2graphapi-0.1.8/text2graphapi/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/docs/source/conf.py` & `text2graphapi-0.1.8/text2graphapi/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/main.py` & `text2graphapi-0.1.8/text2graphapi/main.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/src/Cooccurrence.py` & `text2graphapi-0.1.8/text2graphapi/src/Cooccurrence.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,29 @@
 class Cooccurrence(Graph.Graph):
     """This module generate a word-coocurrence graph from raw text 
         
         :param str graph_type: graph type to generate, default=Graph (types: Graph, DiGraph, MultiGraph, MultiDiGraph)
         :param str output_format: output format to the graph default=networkx (formats: networkx, adj_matrix, adj_list, adj_pandas)
         :param int window_size: windows size for co-occurrence, default=1
         :param int language: language for text prepocessing, default=en (lang: en, es, fr)
-        :param bool apply_preprocessing: flag to exec text prepocessing, default=true
+        :param bool apply_prep: flag to exec text prepocessing, default=true
         :param bool parallel_exec: flag to exec tranformation in parallel, default=false
     """
     def __init__(self, 
                 graph_type, 
                 output_format='', 
-                apply_preprocessing=True, 
+                apply_prep=True, 
                 window_size=1,
                 parallel_exec=False, 
                 language='en', 
                 steps_preprocessing={}
             ):
         """Constructor method
         """
-        self.apply_prep = apply_preprocessing
+        self.apply_prep = apply_prep
         self.parallel_exec = parallel_exec
         self.window_size = window_size
         self.prep = Preprocessing(lang=language, steps_preprocessing=steps_preprocessing)
         self.utils = Utils()
         self.graph_trans = GraphTransformation()
         self.graph_type = graph_type
         self.output_format = output_format
```

### Comparing `text2graphapi-0.1.7/text2graphapi/src/Graph.py` & `text2graphapi-0.1.8/text2graphapi/src/Graph.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/src/GraphTransformation.py` & `text2graphapi-0.1.8/text2graphapi/src/GraphTransformation.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/src/Heterogeneous.py` & `text2graphapi-0.1.8/text2graphapi/src/Heterogeneous.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,30 +42,30 @@
 class Heterogeneous(Graph.Graph):
     """This module generate a Heterogeneous graph from raw text 
 
         :param str graph_type: graph type to generate, default=Graph (types: Graph, DiGraph, MultiGraph, MultiDiGraph)
         :param str output_format: output format to the graph default=networkx (formats: networkx, adj_matrix, adj_list, adj_pandas)
         :param int window_size: windows size for pmi measure, default=20
         :param int language: language for text prepocessing, default=en (lang: en, es)
-        :param bool apply_preprocessing: flag to exec text prepocessing, default=true
+        :param bool apply_prep: flag to exec text prepocessing, default=true
         :param bool parallel_exec: flag to exec tranformation in parallel, default=false
     """
     def __init__(self, 
                 graph_type, 
                 output_format='', 
                 window_size=20, 
                 parallel_exec=False, 
                 language='en', 
-                apply_preprocessing=True, 
+                apply_prep=True, 
                 steps_preprocessing={},
                 load_preprocessing=False
             ):
         """Constructor method
         """
-        self.apply_prep = apply_preprocessing
+        self.apply_prep = apply_prep
         self.parallel_exec = parallel_exec
         self.window_size = window_size
         self.prep = Preprocessing(lang=language, steps_preprocessing=steps_preprocessing)
         self.utils = Utils()
         self.graph_trans = GraphTransformation()
         self.graph_type = graph_type
         self.output_format = output_format
```

### Comparing `text2graphapi-0.1.7/text2graphapi/src/Preprocessing.py` & `text2graphapi-0.1.8/text2graphapi/src/Preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 logger.setLevel(logging.INFO)
 
 ROOT_DIR = os.path.dirname(os.path.dirname(__file__))
 RESOURCES_DIR = os.path.join(ROOT_DIR, 'src/resources')
 
 try:
     nltk.data.find('tokenizers/punkt')
-except OSError:
+except LookupError:
     nltk.download('punkt')
     
 
 class Preprocessing(object):
     """Text parser for the preprocessing.
     :params pos_tagger: Tagger for part of speech.
```

### Comparing `text2graphapi-0.1.7/text2graphapi/src/Utils.py` & `text2graphapi-0.1.8/text2graphapi/src/Utils.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/src/resources/stopwords_english.txt` & `text2graphapi-0.1.8/text2graphapi/src/resources/stopwords_english.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/src/resources/stopwords_french.txt` & `text2graphapi-0.1.8/text2graphapi/src/resources/stopwords_french.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/src/resources/stopwords_spanish.txt` & `text2graphapi-0.1.8/text2graphapi/src/resources/stopwords_spanish.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi/testing.py` & `text2graphapi-0.1.8/text2graphapi/testing.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.7/text2graphapi.egg-info/PKG-INFO` & `text2graphapi-0.1.8/text2graphapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2graphapi
-Version: 0.1.7
+Version: 0.1.8
 Summary: Use this library to transform raw text into differents graph representations.
 Home-page: 
 Author: PLN-disca-iimas
 Author-email: andric.valdez@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `text2graphapi-0.1.7/text2graphapi.egg-info/SOURCES.txt` & `text2graphapi-0.1.8/text2graphapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


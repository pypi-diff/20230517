# Comparing `tmp/paper-qa-1.6.0.tar.gz` & `tmp/paper-qa-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.6.0.tar", last modified: Tue May 16 23:07:09 2023, max compression
+gzip compressed data, was "paper-qa-1.6.1.tar", last modified: Wed May 17 03:50:50 2023, max compression
```

## Comparing `paper-qa-1.6.0.tar` & `paper-qa-1.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:07:09.970550 paper-qa-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 23:06:32.000000 paper-qa-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-16 23:07:09.970550 paper-qa-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-16 23:06:32.000000 paper-qa-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:07:09.966550 paper-qa-1.6.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-16 23:07:09.000000 paper-qa-1.6.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-16 23:07:09.000000 paper-qa-1.6.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:07:09.000000 paper-qa-1.6.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 23:07:09.000000 paper-qa-1.6.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 23:07:09.000000 paper-qa-1.6.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:07:09.970550 paper-qa-1.6.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:07:09.970550 paper-qa-1.6.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 23:07:09.970550 paper-qa-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-16 23:06:32.000000 paper-qa-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:07:09.970550 paper-qa-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-16 23:06:32.000000 paper-qa-1.6.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:50:50.379257 paper-qa-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 03:50:10.000000 paper-qa-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-17 03:50:50.375257 paper-qa-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-17 03:50:10.000000 paper-qa-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:50:50.375257 paper-qa-1.6.1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-17 03:50:50.000000 paper-qa-1.6.1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-17 03:50:50.000000 paper-qa-1.6.1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:50:50.000000 paper-qa-1.6.1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-17 03:50:50.000000 paper-qa-1.6.1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 03:50:50.000000 paper-qa-1.6.1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:50:50.375257 paper-qa-1.6.1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:50:50.375257 paper-qa-1.6.1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:50:50.379257 paper-qa-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-17 03:50:10.000000 paper-qa-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:50:50.375257 paper-qa-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-17 03:50:10.000000 paper-qa-1.6.1/tests/test_paperqa.py
```

### Comparing `paper-qa-1.6.0/LICENSE` & `paper-qa-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.0/PKG-INFO` & `paper-qa-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.6.0
+Version: 1.6.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.6.0/README.md` & `paper-qa-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.6.1/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.6.0
+Version: 1.6.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.6.0/paperqa/agent.py` & `paper-qa-1.6.1/paperqa/agent.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.0/paperqa/contrib/zotero.py` & `paper-qa-1.6.1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.0/paperqa/docs.py` & `paper-qa-1.6.1/paperqa/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,19 +167,20 @@
         key = metadatas[0]["dockey"]
         citation = metadatas[0]["citation"]
         if key in self.keys:
             new_key = self.get_unique_key(key)
             for metadata in metadatas:
                 metadata["dockey"] = new_key
                 metadata["key"] = metadata["key"].replace(key, new_key)
+            key = new_key
         if text_embeddings is None:
             text_embeddings = self.embeddings.embed_documents(texts)
         if self._faiss_index is not None:
             self._faiss_index.add_embeddings(
-                zip(texts, text_embeddings), metadatas=metadatas
+                list(zip(texts, text_embeddings)), metadatas=metadatas
             )
         elif self._doc_index is not None:
             self._doc_index.add_texts([citation], metadatas=[{"key": key}])
         self.docs.append(
             dict(
                 texts=texts,
                 metadata=metadatas,
```

### Comparing `paper-qa-1.6.0/paperqa/qaprompts.py` & `paper-qa-1.6.1/paperqa/qaprompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.0/paperqa/readers.py` & `paper-qa-1.6.1/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.0/paperqa/types.py` & `paper-qa-1.6.1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.0/paperqa/utils.py` & `paper-qa-1.6.1/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.0/setup.py` & `paper-qa-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.0/tests/test_paperqa.py` & `paper-qa-1.6.1/tests/test_paperqa.py`

 * *Files identical despite different names*


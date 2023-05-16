# Comparing `tmp/paper-qa-1.4.1.tar.gz` & `tmp/paper-qa-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.4.1.tar", last modified: Mon May 15 19:58:52 2023, max compression
+gzip compressed data, was "paper-qa-1.6.0.tar", last modified: Tue May 16 23:07:09 2023, max compression
```

## Comparing `paper-qa-1.4.1.tar` & `paper-qa-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:58:52.414824 paper-qa-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 19:58:09.000000 paper-qa-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-15 19:58:52.414824 paper-qa-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-15 19:58:09.000000 paper-qa-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:58:52.410824 paper-qa-1.4.1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-15 19:58:52.000000 paper-qa-1.4.1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-15 19:58:52.000000 paper-qa-1.4.1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:58:52.000000 paper-qa-1.4.1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 19:58:52.000000 paper-qa-1.4.1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 19:58:52.000000 paper-qa-1.4.1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:58:52.414824 paper-qa-1.4.1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:58:52.414824 paper-qa-1.4.1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:58:52.414824 paper-qa-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-15 19:58:09.000000 paper-qa-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:58:52.414824 paper-qa-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-05-15 19:58:09.000000 paper-qa-1.4.1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:07:09.970550 paper-qa-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 23:06:32.000000 paper-qa-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-16 23:07:09.970550 paper-qa-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-16 23:06:32.000000 paper-qa-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:07:09.966550 paper-qa-1.6.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-16 23:07:09.000000 paper-qa-1.6.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-16 23:07:09.000000 paper-qa-1.6.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:07:09.000000 paper-qa-1.6.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 23:07:09.000000 paper-qa-1.6.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 23:07:09.000000 paper-qa-1.6.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:07:09.970550 paper-qa-1.6.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:07:09.970550 paper-qa-1.6.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 23:06:32.000000 paper-qa-1.6.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 23:07:09.970550 paper-qa-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-16 23:06:32.000000 paper-qa-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:07:09.970550 paper-qa-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-16 23:06:32.000000 paper-qa-1.6.0/tests/test_paperqa.py
```

### Comparing `paper-qa-1.4.1/LICENSE` & `paper-qa-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.1/PKG-INFO` & `paper-qa-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.4.1
+Version: 1.6.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.4.1/README.md` & `paper-qa-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.1/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.6.0/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.4.1
+Version: 1.6.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.4.1/paperqa/agent.py` & `paper-qa-1.6.0/paperqa/agent.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.1/paperqa/contrib/zotero.py` & `paper-qa-1.6.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.1/paperqa/docs.py` & `paper-qa-1.6.0/paperqa/docs.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             chunk_size_limit: The maximum number of characters to use for a single chunk of text.
             llm: The language model to use for answering questions. Default - OpenAI chat-gpt-turbo
             summary_llm: The language model to use for summarizing documents. If None, llm is used.
             name: The name of the collection.
             index_path: The path to the index file IF pickled. If None, defaults to using name in $HOME/.paperqa/name
             embeddings: The embeddings to use for indexing documents. Default - OpenAI embeddings
         """
-        self.docs = dict()
+        self.docs = []
         self.chunk_size_limit = chunk_size_limit
         self.keys = set()
         self._faiss_index = None
         self._doc_index = None
         self.update_llm(llm, summary_llm)
         if index_path is None:
             index_path = Path.home() / ".paperqa" / name
@@ -79,36 +79,50 @@
         if type(summary_llm) is str:
             summary_llm = ChatOpenAI(temperature=0.1, model_name=summary_llm)
         self.llm = llm
         if summary_llm is None:
             summary_llm = llm
         self.summary_llm = summary_llm
 
+    def get_unique_key(self, key: str) -> str:
+        """Create a unique key given proposed key"""
+        suffix = ""
+        while key + suffix in self.keys:
+            # move suffix to next letter
+            if suffix == "":
+                suffix = "a"
+            else:
+                suffix = chr(ord(suffix) + 1)
+        key += suffix
+        return key
+
     def add(
         self,
         path: str,
         citation: Optional[str] = None,
         key: Optional[str] = None,
         disable_check: bool = False,
         chunk_chars: Optional[int] = 3000,
     ) -> None:
         """Add a document to the collection."""
 
         # first check to see if we already have this document
         # this way we don't make api call to create citation on file we already have
-        md5 = md5sum(path)
-        if path in self.docs:
+        hash = md5sum(path)
+        if hash in [d["hash"] for d in self.docs]:
             raise ValueError(f"Document {path} already in collection.")
 
         if citation is None:
-            cite_chain = make_chain(prompt=citation_prompt, llm=self.summary_llm)
+            cite_chain = make_chain(
+                prompt=citation_prompt, llm=self.summary_llm)
             # peak first chunk
             texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
             if len(texts) == 0:
-                raise ValueError(f"Could not read document {path}. Is it empty?")
+                raise ValueError(
+                    f"Could not read document {path}. Is it empty?")
             citation = cite_chain.run(texts[0])
             if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
                 citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
 
         if key is None:
             # get first name and year from citation
             try:
@@ -119,42 +133,70 @@
                     f"Could not parse key from citation {citation}. Consider just passing key explicitly - e.g. docs.py (path, citation, key='mykey')"
                 )
             try:
                 year = re.search(r"(\d{4})", citation).group(1)
             except AttributeError:
                 year = ""
             key = f"{author}{year}"
-        suffix = ""
-        while key + suffix in self.keys:
-            # move suffix to next letter
-            if suffix == "":
-                suffix = "a"
-            else:
-                suffix = chr(ord(suffix) + 1)
-        key += suffix
-
-        texts, metadata = read_doc(path, citation, key, chunk_chars=chunk_chars)
+        key = self.get_unique_key(key)
+        texts, metadata = read_doc(
+            path, citation, key, chunk_chars=chunk_chars)
         # loose check to see if document was loaded
         #
         if len("".join(texts)) < 10 or (
             not disable_check and not maybe_is_text("".join(texts))
         ):
             raise ValueError(
                 f"This does not look like a text document: {path}. Path disable_check to ignore this error."
             )
+        self.add_texts(texts, metadata, hash)
+
+    def add_texts(
+        self,
+        texts: List[str],
+        metadatas: List[dict],
+        hash: str,
+        text_embeddings: Optional[List[List[float]]] = None,
+    ):
+        """Add chunked texts to the collection. This is useful if you have already chunked the texts yourself.
+
+        The metadatas should have the following keys: citation, dockey (same as key arg), and key (unique key for each chunk).
+        The hash is a unique identifier for the document. It is used to check if the document has already been added.
+        """
+        if len(texts) != len(metadatas):
+            raise ValueError("texts and metadatas must have the same length.")
+        key = metadatas[0]["dockey"]
+        citation = metadatas[0]["citation"]
+        if key in self.keys:
+            new_key = self.get_unique_key(key)
+            for metadata in metadatas:
+                metadata["dockey"] = new_key
+                metadata["key"] = metadata["key"].replace(key, new_key)
+        if text_embeddings is None:
+            text_embeddings = self.embeddings.embed_documents(texts)
         if self._faiss_index is not None:
-            self._faiss_index.add_texts(texts, metadatas=metadata)
-        if self._doc_index is not None:
+            self._faiss_index.add_embeddings(
+                zip(texts, text_embeddings), metadatas=metadatas
+            )
+        elif self._doc_index is not None:
             self._doc_index.add_texts([citation], metadatas=[{"key": key}])
-        self.docs[path] = dict(texts=texts, metadata=metadata, key=key, md5=md5)
+        self.docs.append(
+            dict(
+                texts=texts,
+                metadata=metadatas,
+                key=key,
+                hash=hash,
+                text_embeddings=text_embeddings,
+            )
+        )
         self.keys.add(key)
 
     def clear(self) -> None:
         """Clear the collection of documents."""
-        self.docs = dict()
+        self.docs = []
         self.keys = set()
         self._faiss_index = None
         self._doc_index = None
         # delete index file
         pkl = self.index_path / "index.pkl"
         if pkl.exists():
             pkl.unlink()
@@ -166,68 +208,72 @@
         """Return a list of tuples of (key, citation) for each document."""
         return [
             (
                 len(doc["texts"]),
                 doc["metadata"][0]["dockey"],
                 doc["metadata"][0]["citation"],
             )
-            for doc in self.docs.values()
+            for doc in self.docs
         ]
 
     def doc_match(self, query: str, k: int = 25) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
             return ""
         if self._doc_index is None:
-            texts = [doc["metadata"][0]["citation"] for doc in self.docs.values()]
-            metadatas = [
-                {"key": doc["metadata"][0]["dockey"]} for doc in self.docs.values()
-            ]
+            texts = [doc["metadata"][0]["citation"] for doc in self.docs]
+            metadatas = [{"key": doc["metadata"][0]["dockey"]}
+                         for doc in self.docs]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         docs = self._doc_index.max_marginal_relevance_search(query, k=k)
         chain = make_chain(select_paper_prompt, self.summary_llm)
         papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
         result = chain.run(instructions=query, papers="\n".join(papers))
         return result
 
     # to pickle, we have to save the index as a file
 
     def __getstate__(self):
-        if self._faiss_index is None and len(self.docs) > 0:
-            self._build_faiss_index()
         state = self.__dict__.copy()
         if self._faiss_index is not None:
             state["_faiss_index"].save_local(self.index_path)
         del state["_faiss_index"]
         del state["_doc_index"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         try:
-            self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
+            self._faiss_index = FAISS.load_local(
+                self.index_path, self.embeddings)
         except:
             # they use some special exception type, but I don't want to import it
             self._faiss_index = None
         if not hasattr(self, "_doc_index"):
             self._doc_index = None
         self.update_llm(None, None)
 
     def _build_faiss_index(self):
         if self._faiss_index is None:
-            texts = reduce(
-                lambda x, y: x + y, [doc["texts"] for doc in self.docs.values()], []
+            texts = reduce(lambda x, y: x + y,
+                           [doc["texts"] for doc in self.docs], [])
+            text_embeddings = reduce(
+                lambda x, y: x + y, [doc["text_embeddings"]
+                                     for doc in self.docs], []
             )
             metadatas = reduce(
-                lambda x, y: x + y, [doc["metadata"] for doc in self.docs.values()], []
+                lambda x, y: x + y, [doc["metadata"] for doc in self.docs], []
             )
-            self._faiss_index = FAISS.from_texts(
-                texts, self.embeddings, metadatas=metadatas
+            self._faiss_index = FAISS.from_embeddings(
+                # wow adding list to the zip was tricky
+                text_embeddings=list(zip(texts, text_embeddings)),
+                embedding=self.embeddings,
+                metadatas=metadatas,
             )
 
     def get_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
```

### Comparing `paper-qa-1.4.1/paperqa/qaprompts.py` & `paper-qa-1.6.0/paperqa/qaprompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.1/paperqa/readers.py` & `paper-qa-1.6.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.1/paperqa/types.py` & `paper-qa-1.6.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.1/paperqa/utils.py` & `paper-qa-1.6.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.1/setup.py` & `paper-qa-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.1/tests/test_paperqa.py` & `paper-qa-1.6.0/tests/test_paperqa.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,40 +12,43 @@
 
 def test_maybe_is_text():
     assert paperqa.maybe_is_text(
         "This is a test. The sample conc. was 1.0 mM (at 245 ^F)"
     )
     assert not paperqa.maybe_is_text("\\C0\\C0\\B1\x00")
     # get front page of wikipedia
-    r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
+    r = requests.get(
+        "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
     assert paperqa.maybe_is_text(r.text)
 
     # now force it to contain lots of weird encoding
     bad_text = r.text.encode("latin1", "ignore").decode("utf-16", "ignore")
     assert not paperqa.maybe_is_text(bad_text)
 
 
 def test_docs():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
-        r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
         f.write(r.text)
     llm = OpenAI(temperature=0.1, model_name="text-ada-001")
     docs = paperqa.Docs(llm=llm)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    assert docs.docs[doc_path]["key"] == "Wiki2023"
+    assert docs.docs[0]["key"] == "Wiki2023"
     os.remove(doc_path)
 
 
 def test_evidence():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     evidence = docs.get_evidence(
         paperqa.Answer("For which state was he a governor"), k=1, max_sources=1
     )
     print(evidence.contexts[0].context, evidence.context)
@@ -53,15 +56,16 @@
     os.remove(doc_path)
 
 
 def test_query():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     docs.query("What is Frederick Bates's greatest accomplishment?")
     os.remove(doc_path)
 
 
@@ -80,31 +84,65 @@
         os.remove(doc_path)
 
 
 def test_doc_match():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     docs.doc_match("What is Frederick Bates's greatest accomplishment?")
     os.remove(doc_path)
 
 
 def test_docs_pickle():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
+        f.write(r.text)
+    llm = OpenAI(temperature=0.0, model_name="text-babbage-001")
+    docs = paperqa.Docs(llm=llm)
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
+    docs_pickle = pickle.dumps(docs)
+    docs2 = pickle.loads(docs_pickle)
+    docs2.update_llm(llm)
+    assert len(docs.docs) == len(docs2.docs)
+    assert (
+        strings_similarity(
+            docs.get_evidence(
+                paperqa.Answer("What date is flag day in Canada?"),
+                k=3,
+                max_sources=1,
+            ).context,
+            docs2.get_evidence(
+                paperqa.Answer("What date is flag day in Canada?"),
+                k=3,
+                max_sources=1,
+            ).context,
+        )
+        > 0.75
+    )
+    os.remove(doc_path)
+
+
+def test_docs_pickle_no_faiss():
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get front page of wikipedia
         r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
         f.write(r.text)
     llm = OpenAI(temperature=0.0, model_name="text-babbage-001")
     docs = paperqa.Docs(llm=llm)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
+    docs._faiss_index = None
     docs_pickle = pickle.dumps(docs)
     docs2 = pickle.loads(docs_pickle)
     docs2.update_llm(llm)
     assert len(docs.docs) == len(docs2.docs)
     assert (
         strings_similarity(
             docs.get_evidence(
@@ -123,15 +161,16 @@
     os.remove(doc_path)
 
 
 def test_bad_context():
     doc_path = "example.html"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     answer = docs.query(
         "What year was Barack Obama born?",
         length_prompt="about 20 words",
     )
@@ -139,65 +178,70 @@
     os.remove(doc_path)
 
 
 def test_repeat_keys():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     try:
         docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     except ValueError:
         pass
     assert len(docs.docs) == 1
 
     # now with different paths
     doc_path2 = "example2.txt"
     with open(doc_path2, "w", encoding="utf-8") as f:
         # get wiki page about politician
         f.write(r.text)
+        f.write("\n")  # so we don't have same hash
     docs.add(doc_path2, "WikiMedia Foundation, 2023, Accessed now")
     assert len(docs.docs) == 2
 
     # check keys
-    assert docs.docs[doc_path]["key"] == "Wiki2023"
-    assert docs.docs[doc_path2]["key"] == "Wiki2023a"
+    assert docs.docs[0]["key"] == "Wiki2023"
+    assert docs.docs[1]["key"] == "Wiki2023a"
 
     os.remove(doc_path)
     os.remove(doc_path2)
 
 
 def test_pdf_reader():
     tests_dir = os.path.dirname(os.path.abspath(__file__))
     doc_path = os.path.join(tests_dir, "paper.pdf")
-    docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-curie-001"))
+    docs = paperqa.Docs(llm=OpenAI(
+        temperature=0.0, model_name="text-curie-001"))
     docs.add(doc_path, "Wellawatte et al, XAI Review, 2023")
     answer = docs.query("Are counterfactuals actionable?")
     assert "yes" in answer.answer or "Yes" in answer.answer
 
 
 def test_prompt_length():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     docs.query("What is the name of the politician?", length_prompt="25 words")
 
 
 def test_doc_preview():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     assert len(docs.doc_previews()) == 1
 
 
 def test_code():
@@ -209,64 +253,74 @@
     docs.query("What function tests the preview?")
 
 
 def test_citation():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path)
     assert (
-        list(docs.docs.values())[0]["metadata"][0]["key"] == "Wikipedia2023"
-        or list(docs.docs.values())[0]["metadata"][0]["key"] == "Frederick2023"
+        list(docs.docs)[0]["metadata"][0]["key"] == "Wikipedia2023"
+        or list(docs.docs)[0]["metadata"][0]["key"] == "Frederick2023"
     )
 
 
 def test_dockey_filter():
     """Test that we can filter evidence with dockeys"""
     doc_path = "example2.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     # add with new dockey
+    with open("example.txt", "w", encoding="utf-8") as f:
+        f.write(r.text)
+        f.write("\n")  # so we don't have same hash
     docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
     answer = paperqa.Answer("What country is Bates from?")
     docs.get_evidence(answer, key_filter=["test"])
 
 
 def test_query_filter():
     """Test that we can filter evidence with in query"""
     doc_path = "example2.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(
         doc_path,
         "Information about Fredrick Bates, WikiMedia Foundation, 2023, Accessed now",
     )
     # add with new dockey
+    with open("example.txt", "w", encoding="utf-8") as f:
+        f.write(r.text)
+        f.write("\n")  # so we don't have same hash
     docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
     answer = docs.query("What country is Bates from?", key_filter=True)
     # the filter shouldn't trigger, so just checking that it doesn't crash
 
 
 def test_nonopenai_model():
     responses = ["This is a test", "This is another test"] * 50
     model = FakeListLLM(responses=responses)
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs(llm=model)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     answer = docs.query("What country is Bates from?")
 
 
 def test_agent():
```


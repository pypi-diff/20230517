# Comparing `tmp/bgnlp-0.3.0.tar.gz` & `tmp/bgnlp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgnlp-0.3.0.tar", last modified: Tue May 16 15:53:56 2023, max compression
+gzip compressed data, was "bgnlp-0.3.1.tar", last modified: Wed May 17 15:32:09 2023, max compression
```

## Comparing `bgnlp-0.3.0.tar` & `bgnlp-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 15:53:44.000000 bgnlp-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 15:53:44.000000 bgnlp-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-16 15:53:56.202476 bgnlp-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-16 15:53:44.000000 bgnlp-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.198475 bgnlp-0.3.0/bgnlp/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/bgnlp/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/models/seq2seq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/bgnlp/serialized/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/serialized/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/bgnlp/serialized/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/serialized/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/bgnlp/serialized/vocabs/
--rw-r--r--   0 runner    (1001) docker     (123)    82097 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/serialized/vocabs/cb-vocab.pt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/bgnlp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/taggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.198475 bgnlp-0.3.0/bgnlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-16 15:53:56.000000 bgnlp-0.3.0/bgnlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 15:53:56.000000 bgnlp-0.3.0/bgnlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:53:56.000000 bgnlp-0.3.0/bgnlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 15:53:56.000000 bgnlp-0.3.0/bgnlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 15:53:56.000000 bgnlp-0.3.0/bgnlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 15:53:44.000000 bgnlp-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:53:56.202476 bgnlp-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-16 15:53:44.000000 bgnlp-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:32:09.619518 bgnlp-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 15:31:56.000000 bgnlp-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 15:31:56.000000 bgnlp-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-17 15:32:09.619518 bgnlp-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-17 15:31:56.000000 bgnlp-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:32:09.619518 bgnlp-0.3.1/bgnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:32:09.619518 bgnlp-0.3.1/bgnlp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/models/seq2seq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:32:09.619518 bgnlp-0.3.1/bgnlp/serialized/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/serialized/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:32:09.619518 bgnlp-0.3.1/bgnlp/serialized/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/serialized/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:32:09.619518 bgnlp-0.3.1/bgnlp/serialized/vocabs/
+-rw-r--r--   0 runner    (1001) docker     (123)    82097 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/serialized/vocabs/cb-vocab.pt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:32:09.619518 bgnlp-0.3.1/bgnlp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/tools/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/tools/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/tools/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28162 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/tools/taggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-17 15:31:56.000000 bgnlp-0.3.1/bgnlp/tools/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:32:09.619518 bgnlp-0.3.1/bgnlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-17 15:32:09.000000 bgnlp-0.3.1/bgnlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-17 15:32:09.000000 bgnlp-0.3.1/bgnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:32:09.000000 bgnlp-0.3.1/bgnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 15:32:09.000000 bgnlp-0.3.1/bgnlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 15:32:09.000000 bgnlp-0.3.1/bgnlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 15:31:56.000000 bgnlp-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:32:09.619518 bgnlp-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-17 15:31:56.000000 bgnlp-0.3.1/setup.py
```

### Comparing `bgnlp-0.3.0/LICENSE` & `bgnlp-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bgnlp-0.3.0/PKG-INFO` & `bgnlp-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgnlp
-Version: 0.3.0
+Version: 0.3.1
 Summary: Package for Bulgarian Natural Language Processing (NLP)
 Author: Adam Fauzi
 Author-email: adamfzh98@gmail.com
 Keywords: pytorch,nlp,bulgaria,machine learning,deep learning,AI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bgnlp Version: 0.3.0 Summary: Package for Bulgarian
+Metadata-Version: 2.1 Name: bgnlp Version: 0.3.1 Summary: Package for Bulgarian
 Natural Language Processing (NLP) Author: Adam Fauzi Author-email:
 adamfzh98@gmail.com Keywords: pytorch,nlp,bulgaria,machine learning,deep
 learning,AI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
```

### Comparing `bgnlp-0.3.0/README.md` & `bgnlp-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bgnlp-0.3.0/bgnlp/models/bert.py` & `bgnlp-0.3.1/bgnlp/models/bert.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.3.0/bgnlp/models/seq2seq.py` & `bgnlp-0.3.1/bgnlp/models/seq2seq.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.3.0/bgnlp/serialized/vocabs/cb-vocab.pt` & `bgnlp-0.3.1/bgnlp/serialized/vocabs/cb-vocab.pt`

 * *Files identical despite different names*

### Comparing `bgnlp-0.3.0/bgnlp/tools/configs.py` & `bgnlp-0.3.1/bgnlp/tools/configs.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.3.0/bgnlp/tools/mappings.py` & `bgnlp-0.3.1/bgnlp/tools/mappings.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.3.0/bgnlp/tools/mixins.py` & `bgnlp-0.3.1/bgnlp/tools/mixins.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.3.0/bgnlp/tools/taggers.py` & `bgnlp-0.3.1/bgnlp/tools/taggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -550,14 +550,15 @@
             >>> text = "Барух Спиноза е роден в Амстердам"
             >>> print(f"Input: {text}")
             >>> print("Result:", ner(text))
             Input: Барух Спиноза е роден в Амстердам
             Result: [{'word': 'Барух Спиноза', 'entity_group': 'PER'}, {'word': 'Амстердам', 'entity_group': 'LOC'}]
 
         """
+        text = self._preprocess_text(text)
         return self.predict(text)
 
     def get_tokenizer(self):
         return AutoTokenizer.from_pretrained(self.config.model_path)
 
     def get_model(self):
         return AutoModelForTokenClassification.from_pretrained(self.config.model_path)
@@ -607,21 +608,32 @@
             if "I-" in entity:
                 curr_word.append(word)
             
             if "O" == entity:
                 if curr_word:
                     curr_word = " ".join(curr_word)
                     result.append({
-                        "word": curr_word,
+                        "word": self._remove_punctuation(curr_word),
                         "entity_group": entities[i][2:]
                     })
                 
                 curr_word = []
 
         return result
+    
+    def _preprocess_text(self, text: str) -> str:
+        # Remove the whitespace before punctuation.
+        text = re.sub(r"\s+([,\.\?!;:\'\"\(\)\[\]„”])", r"\1", text)
+        # Leave out only a single whitespace.
+        text = re.sub(r"\s+", " ", text)
+        
+        return text
+
+    def _remove_punctuation(self, text: str) -> str:
+        return re.sub(r"([,\.\?!;:\'\"\(\)\[\]„”])", "", text)
 
 
 class KeywordsTagger(BaseTagger):
     """Keyword Extraction tagger for Bulgarian texts.
 
     Args:
         config (ModelConfig): The model configuration.
```

### Comparing `bgnlp-0.3.0/bgnlp/tools/tokenizers.py` & `bgnlp-0.3.1/bgnlp/tools/tokenizers.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.3.0/bgnlp.egg-info/PKG-INFO` & `bgnlp-0.3.1/bgnlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgnlp
-Version: 0.3.0
+Version: 0.3.1
 Summary: Package for Bulgarian Natural Language Processing (NLP)
 Author: Adam Fauzi
 Author-email: adamfzh98@gmail.com
 Keywords: pytorch,nlp,bulgaria,machine learning,deep learning,AI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bgnlp Version: 0.3.0 Summary: Package for Bulgarian
+Metadata-Version: 2.1 Name: bgnlp Version: 0.3.1 Summary: Package for Bulgarian
 Natural Language Processing (NLP) Author: Adam Fauzi Author-email:
 adamfzh98@gmail.com Keywords: pytorch,nlp,bulgaria,machine learning,deep
 learning,AI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
```

### Comparing `bgnlp-0.3.0/bgnlp.egg-info/SOURCES.txt` & `bgnlp-0.3.1/bgnlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bgnlp-0.3.0/setup.py` & `bgnlp-0.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ROOT = os.path.abspath(os.path.dirname(__file__))
 README_PATH = os.path.join(ROOT, "README.md")
 REQUIREMENTS_PATH = os.path.join(ROOT, "requirements.txt")
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.3.0'
+VERSION = '0.3.1'
 DESCRIPTION = 'Package for Bulgarian Natural Language Processing (NLP)'
 
 
 def _get_requirements(path):
     with open(path, "r") as f:
         requirements_str = f.read()
         packages = re.findall(r"(.+=?=?[^\n]+)\n", requirements_str)
```


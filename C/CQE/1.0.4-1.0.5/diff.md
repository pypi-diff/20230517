# Comparing `tmp/CQE-1.0.4.tar.gz` & `tmp/CQE-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CQE-1.0.4.tar", last modified: Tue May 16 12:50:06 2023, max compression
+gzip compressed data, was "CQE-1.0.5.tar", last modified: Tue May 16 19:25:10 2023, max compression
```

## Comparing `CQE-1.0.4.tar` & `CQE-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:50:06.705724 CQE-1.0.4/
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:50:06.701716 CQE-1.0.4/CQE/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   106799 2023-05-16 11:51:34.000000 CQE-1.0.4/CQE/CQE.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    17260 2023-05-16 11:51:34.000000 CQE-1.0.4/CQE/NumberNormalizer.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.4/CQE/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    12489 2023-05-15 13:17:03.000000 CQE-1.0.4/CQE/classes.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7901 2023-05-14 12:56:44.000000 CQE-1.0.4/CQE/number_lookup.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    43173 2023-05-15 15:19:41.000000 CQE-1.0.4/CQE/rules.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-1.0.4/CQE/unit.json
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:50:06.705154 CQE-1.0.4/CQE/unit_classifier/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.4/CQE/unit_classifier/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-1.0.4/CQE/unit_classifier/sample_usage.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7024 2023-05-11 07:08:00.000000 CQE-1.0.4/CQE/unit_classifier/train_classifier_bert.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     1570 2023-05-11 11:07:05.000000 CQE-1.0.4/CQE/unit_classifier/unit_disambiguator.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)  1481390 2023-05-11 11:08:19.000000 CQE-1.0.4/CQE/unit_models.zip
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:50:06.704330 CQE-1.0.4/CQE.egg-info/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-16 12:50:06.000000 CQE-1.0.4/CQE.egg-info/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      452 2023-05-16 12:50:06.000000 CQE-1.0.4/CQE.egg-info/SOURCES.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-05-16 12:50:06.000000 CQE-1.0.4/CQE.egg-info/dependency_links.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      467 2023-05-16 12:50:06.000000 CQE-1.0.4/CQE.egg-info/requires.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-05-16 12:50:06.000000 CQE-1.0.4/CQE.egg-info/top_level.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-1.0.4/LICENSE.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-16 12:50:06.705486 CQE-1.0.4/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10037 2023-05-16 11:51:34.000000 CQE-1.0.4/README.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-05-16 12:50:06.705766 CQE-1.0.4/setup.cfg
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     1232 2023-05-16 12:46:46.000000 CQE-1.0.4/setup.py
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 19:25:10.573302 CQE-1.0.5/
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 19:25:10.566512 CQE-1.0.5/CQE/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   106837 2023-05-16 19:20:25.000000 CQE-1.0.5/CQE/CQE.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    17260 2023-05-16 11:51:34.000000 CQE-1.0.5/CQE/NumberNormalizer.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.5/CQE/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    12489 2023-05-15 13:17:03.000000 CQE-1.0.5/CQE/classes.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7901 2023-05-14 12:56:44.000000 CQE-1.0.5/CQE/number_lookup.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    43173 2023-05-15 15:19:41.000000 CQE-1.0.5/CQE/rules.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-1.0.5/CQE/unit.json
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 19:25:10.572310 CQE-1.0.5/CQE/unit_classifier/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.5/CQE/unit_classifier/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-1.0.5/CQE/unit_classifier/sample_usage.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7063 2023-05-16 19:21:43.000000 CQE-1.0.5/CQE/unit_classifier/train_classifier_bert.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     1570 2023-05-11 11:07:05.000000 CQE-1.0.5/CQE/unit_classifier/unit_disambiguator.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)  1481390 2023-05-11 11:08:19.000000 CQE-1.0.5/CQE/unit_models.zip
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 19:25:10.569096 CQE-1.0.5/CQE.egg-info/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-16 19:25:10.000000 CQE-1.0.5/CQE.egg-info/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      452 2023-05-16 19:25:10.000000 CQE-1.0.5/CQE.egg-info/SOURCES.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-05-16 19:25:10.000000 CQE-1.0.5/CQE.egg-info/dependency_links.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      209 2023-05-16 19:25:10.000000 CQE-1.0.5/CQE.egg-info/requires.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-05-16 19:25:10.000000 CQE-1.0.5/CQE.egg-info/top_level.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-1.0.5/LICENSE.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-16 19:25:10.572781 CQE-1.0.5/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10037 2023-05-16 11:51:34.000000 CQE-1.0.5/README.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-05-16 19:25:10.573360 CQE-1.0.5/setup.cfg
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      948 2023-05-16 19:25:08.000000 CQE-1.0.5/setup.py
```

### Comparing `CQE-1.0.4/CQE/CQE.py` & `CQE-1.0.5/CQE/CQE.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from spacy.matcher import DependencyMatcher, Matcher
 from spacy.tokens import Token
 from spacy.lang.lex_attrs import is_digit
 from spacy.lang.lex_attrs import like_num as sp_like_num
 from spacy.lang.char_classes import ALPHA, ALPHA_LOWER, ALPHA_UPPER, HYPHENS
 from spacy.lang.char_classes import CONCAT_QUOTES, LIST_ELLIPSES, LIST_ICONS
 from spacy.util import compile_infix_regex
+from spacy_download import load_spacy
 
 from fuzzywuzzy import fuzz
 
 from . import NumberNormalizer
 from .rules import rules
 from .number_lookup import maps, suffixes
 from .classes import Change, Value, Range, Unit, Quantity
@@ -293,15 +294,15 @@
     span = doc[start:end]
     if span:
         for token in span:
             token._.set("ignore", True)
 
 class NumParser:
     def __init__(self, overload=False, spacy_model: str = "en_core_web_sm"):
-        self.nlp = spacy.load(spacy_model)
+        self.nlp = load_spacy(spacy_model)
         self.overload = overload
         #self.nlp.add_pipe("sentencizer")
         self._modify_defaults_stopwords()
         prefixes = list(self.nlp.Defaults.prefixes)
 
         prefixes.append("~")
         prefixes.append(">")
```

### Comparing `CQE-1.0.4/CQE/NumberNormalizer.py` & `CQE-1.0.5/CQE/NumberNormalizer.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.4/CQE/classes.py` & `CQE-1.0.5/CQE/classes.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.4/CQE/number_lookup.py` & `CQE-1.0.5/CQE/number_lookup.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.4/CQE/rules.py` & `CQE-1.0.5/CQE/rules.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.4/CQE/unit.json` & `CQE-1.0.5/CQE/unit.json`

 * *Files identical despite different names*

### Comparing `CQE-1.0.4/CQE/unit_classifier/sample_usage.py` & `CQE-1.0.5/CQE/unit_classifier/sample_usage.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.4/CQE/unit_classifier/train_classifier_bert.py` & `CQE-1.0.5/CQE/unit_classifier/train_classifier_bert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 import spacy
+from spacy_download import load_spacy
+
 #before running :
 # python -m spacy download en_core_web_trf
 #following https://towardsdatascience.com/building-sentiment-classifier-using-spacy-3-0-transformers-c744bfc767b
 #to train:
 # python -m spacy train config.cfg --output ./data/units/unit_models/train_\".spacy --paths.train ./data/units/train/spacy_train/train_set_\".spacy --paths.dev ./data/units/train/spacy_train/train_set_\".spacy
 # python -m spacy train config.cfg --output ./data/units/unit_models/train_\'.spacy --paths.train ./data/units/train/spacy_train/train_set_\'.spacy --paths.dev ./data/units/train/spacy_train/train_set_\'.spacy
 # python -m spacy train config.cfg --output ./data/units/unit_models/train_a.spacy --paths.train ./data/units/train/spacy_train/train_set_a.spacy --paths.dev ./data/units/train/spacy_train/train_set_a.spacy
@@ -56,15 +58,15 @@
     for row in training_set_:
         tuples.append((row["text"],row["unit"]))
     return tuples,target_names_dict
 
 def document(data,target_names_dict):
     #Creating empty list called "text"
     text = []
-    nlp=spacy.load("en_core_web_trf")
+    nlp=load_spacy("en_core_web_trf")
     for doc, label in nlp.pipe(data, as_tuples = True):
         for name,i in target_names_dict.items():
             if name==label:
                 doc.cats[name]=1
             else:
                 doc.cats[name]=0
         text.append(doc)
```

### Comparing `CQE-1.0.4/CQE/unit_classifier/unit_disambiguator.py` & `CQE-1.0.5/CQE/unit_classifier/unit_disambiguator.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.4/CQE/unit_models.zip` & `CQE-1.0.5/CQE/unit_models.zip`

 * *Files identical despite different names*

### Comparing `CQE-1.0.4/CQE.egg-info/PKG-INFO` & `CQE-1.0.5/CQE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CQE
-Version: 1.0.4
+Version: 1.0.5
 Summary: quantity extractor
 Home-page: https://github.com/vivkaz/CQE
 Author: satyaalmasian and vivian kazakova
 Author-email: satya.almasian@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `CQE-1.0.4/LICENSE.md` & `CQE-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CQE-1.0.4/PKG-INFO` & `CQE-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CQE
-Version: 1.0.4
+Version: 1.0.5
 Summary: quantity extractor
 Home-page: https://github.com/vivkaz/CQE
 Author: satyaalmasian and vivian kazakova
 Author-email: satya.almasian@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `CQE-1.0.4/README.md` & `CQE-1.0.5/README.md`

 * *Files identical despite different names*


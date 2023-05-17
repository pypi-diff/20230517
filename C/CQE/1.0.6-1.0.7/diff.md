# Comparing `tmp/CQE-1.0.6.tar.gz` & `tmp/CQE-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CQE-1.0.6.tar", last modified: Wed May 17 11:58:02 2023, max compression
+gzip compressed data, was "CQE-1.0.7.tar", last modified: Wed May 17 12:14:02 2023, max compression
```

## Comparing `CQE-1.0.6.tar` & `CQE-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-17 11:58:02.296392 CQE-1.0.6/
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-17 11:58:02.291942 CQE-1.0.6/CQE/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   107392 2023-05-16 19:30:06.000000 CQE-1.0.6/CQE/CQE.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    17580 2023-05-16 19:30:06.000000 CQE-1.0.6/CQE/NumberNormalizer.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.6/CQE/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    12489 2023-05-15 13:17:03.000000 CQE-1.0.6/CQE/classes.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7901 2023-05-14 12:56:44.000000 CQE-1.0.6/CQE/number_lookup.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    43173 2023-05-15 15:19:41.000000 CQE-1.0.6/CQE/rules.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-1.0.6/CQE/unit.json
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-17 11:58:02.295827 CQE-1.0.6/CQE/unit_classifier/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.6/CQE/unit_classifier/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-1.0.6/CQE/unit_classifier/sample_usage.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7063 2023-05-16 19:21:43.000000 CQE-1.0.6/CQE/unit_classifier/train_classifier_bert.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     1706 2023-05-17 11:56:42.000000 CQE-1.0.6/CQE/unit_classifier/unit_disambiguator.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)  1482733 2023-05-17 11:57:02.000000 CQE-1.0.6/CQE/unit_models.zip
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-17 11:58:02.294793 CQE-1.0.6/CQE.egg-info/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-17 11:58:02.000000 CQE-1.0.6/CQE.egg-info/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      452 2023-05-17 11:58:02.000000 CQE-1.0.6/CQE.egg-info/SOURCES.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-05-17 11:58:02.000000 CQE-1.0.6/CQE.egg-info/dependency_links.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      209 2023-05-17 11:58:02.000000 CQE-1.0.6/CQE.egg-info/requires.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-05-17 11:58:02.000000 CQE-1.0.6/CQE.egg-info/top_level.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-1.0.6/LICENSE.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-17 11:58:02.296150 CQE-1.0.6/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10037 2023-05-16 11:51:34.000000 CQE-1.0.6/README.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-05-17 11:58:02.296441 CQE-1.0.6/setup.cfg
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      948 2023-05-17 11:57:51.000000 CQE-1.0.6/setup.py
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-17 12:14:02.331534 CQE-1.0.7/
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-17 12:14:02.327046 CQE-1.0.7/CQE/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   107392 2023-05-16 19:30:06.000000 CQE-1.0.7/CQE/CQE.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    17580 2023-05-16 19:30:06.000000 CQE-1.0.7/CQE/NumberNormalizer.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.7/CQE/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    12489 2023-05-15 13:17:03.000000 CQE-1.0.7/CQE/classes.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7901 2023-05-14 12:56:44.000000 CQE-1.0.7/CQE/number_lookup.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    43173 2023-05-15 15:19:41.000000 CQE-1.0.7/CQE/rules.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-1.0.7/CQE/unit.json
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-17 12:14:02.330875 CQE-1.0.7/CQE/unit_classifier/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.7/CQE/unit_classifier/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-1.0.7/CQE/unit_classifier/sample_usage.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7063 2023-05-16 19:21:43.000000 CQE-1.0.7/CQE/unit_classifier/train_classifier_bert.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     1705 2023-05-17 12:02:10.000000 CQE-1.0.7/CQE/unit_classifier/unit_disambiguator.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)  1482733 2023-05-17 11:57:02.000000 CQE-1.0.7/CQE/unit_models.zip
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-17 12:14:02.329806 CQE-1.0.7/CQE.egg-info/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-17 12:14:02.000000 CQE-1.0.7/CQE.egg-info/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      452 2023-05-17 12:14:02.000000 CQE-1.0.7/CQE.egg-info/SOURCES.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-05-17 12:14:02.000000 CQE-1.0.7/CQE.egg-info/dependency_links.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      209 2023-05-17 12:14:02.000000 CQE-1.0.7/CQE.egg-info/requires.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-05-17 12:14:02.000000 CQE-1.0.7/CQE.egg-info/top_level.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-1.0.7/LICENSE.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-17 12:14:02.331295 CQE-1.0.7/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10037 2023-05-16 11:51:34.000000 CQE-1.0.7/README.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-05-17 12:14:02.333134 CQE-1.0.7/setup.cfg
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      950 2023-05-17 12:13:45.000000 CQE-1.0.7/setup.py
```

### Comparing `CQE-1.0.6/CQE/CQE.py` & `CQE-1.0.7/CQE/CQE.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/CQE/NumberNormalizer.py` & `CQE-1.0.7/CQE/NumberNormalizer.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/CQE/classes.py` & `CQE-1.0.7/CQE/classes.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/CQE/number_lookup.py` & `CQE-1.0.7/CQE/number_lookup.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/CQE/rules.py` & `CQE-1.0.7/CQE/rules.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/CQE/unit.json` & `CQE-1.0.7/CQE/unit.json`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/CQE/unit_classifier/sample_usage.py` & `CQE-1.0.7/CQE/unit_classifier/sample_usage.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/CQE/unit_classifier/train_classifier_bert.py` & `CQE-1.0.7/CQE/unit_classifier/train_classifier_bert.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/CQE/unit_classifier/unit_disambiguator.py` & `CQE-1.0.7/CQE/unit_classifier/unit_disambiguator.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
                 file_name = os.path.join(path, "unit_models/train_yen.spacy/model-best")
             elif key=="′":
                 file_name = os.path.join(path, "unit_models/train_ascii'.spacy/model-best")
             elif key=="″":
                 file_name = os.path.join(path, "unit_models/train_ascii_doublequote.spacy/model-best")
             elif key=="\"":
                 file_name = os.path.join(path, "unit_models/train_doublequote.spacy/model-best")
-
             else:
                 file_name = os.path.join(path, "unit_models/train_" + key + ".spacy/model-best")
             self.models[key] = spacy.load(file_name)
 
     def disambiguate(self, sentence, surface_form):
         probabilities = self.models[surface_form](sentence).cats
         return max(probabilities.items(), key=operator.itemgetter(1))[0]
```

### Comparing `CQE-1.0.6/CQE/unit_models.zip` & `CQE-1.0.7/CQE/unit_models.zip`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/CQE.egg-info/PKG-INFO` & `CQE-1.0.7/CQE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CQE
-Version: 1.0.6
+Version: 1.0.7
 Summary: quantity extractor
 Home-page: https://github.com/vivkaz/CQE
 Author: satyaalmasian and vivian kazakova
 Author-email: satya.almasian@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `CQE-1.0.6/LICENSE.md` & `CQE-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/PKG-INFO` & `CQE-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CQE
-Version: 1.0.6
+Version: 1.0.7
 Summary: quantity extractor
 Home-page: https://github.com/vivkaz/CQE
 Author: satyaalmasian and vivian kazakova
 Author-email: satya.almasian@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `CQE-1.0.6/README.md` & `CQE-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `CQE-1.0.6/setup.py` & `CQE-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='CQE',
-    version='1.0.6',
+    version='1.0.7',
     packages=['CQE','CQE.unit_classifier'],
-    package_data={'': ['unit.json'],'': ['unit_models.zip']},# both has to be empty
+    package_data={'0': ['unit.json'],'1': ['unit_models.zip']},# both has to be empty
     url='https://github.com/vivkaz/CQE',
     license='',
     long_description_content_type="text/markdown",
     long_description=long_description,
     author='satyaalmasian and vivian kazakova',
     author_email='satya.almasian@gmail.com',
     description='quantity extractor',
```


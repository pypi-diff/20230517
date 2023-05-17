# Comparing `tmp/punctfix-0.10.0.tar.gz` & `tmp/punctfix-0.10.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punctfix-0.10.0.tar", last modified: Sun May  7 09:11:21 2023, max compression
+gzip compressed data, was "punctfix-0.10.1.tar", last modified: Wed May 17 11:03:09 2023, max compression
```

## Comparing `punctfix-0.10.0.tar` & `punctfix-0.10.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-07 09:11:21.688915 punctfix-0.10.0/
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)    11358 2023-05-06 18:27:41.000000 punctfix-0.10.0/LICENCE.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       63 2023-05-06 18:27:41.000000 punctfix-0.10.0/MANIFEST.in
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     2403 2023-05-07 09:11:21.688915 punctfix-0.10.0/PKG-INFO
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1979 2023-05-06 18:27:41.000000 punctfix-0.10.0/README.md
-drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-07 09:11:21.685582 punctfix-0.10.0/punctfix/
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       34 2023-05-06 18:27:41.000000 punctfix-0.10.0/punctfix/__init__.py
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)    10211 2023-05-06 18:27:41.000000 punctfix-0.10.0/punctfix/inference.py
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1905 2023-05-06 18:27:41.000000 punctfix-0.10.0/punctfix/models.py
-drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-07 09:11:21.685582 punctfix-0.10.0/punctfix.egg-info/
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     2403 2023-05-07 09:11:21.000000 punctfix-0.10.0/punctfix.egg-info/PKG-INFO
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      324 2023-05-07 09:11:21.000000 punctfix-0.10.0/punctfix.egg-info/SOURCES.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)        1 2023-05-07 09:11:21.000000 punctfix-0.10.0/punctfix.egg-info/dependency_links.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       44 2023-05-07 09:11:21.000000 punctfix-0.10.0/punctfix.egg-info/requires.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       15 2023-05-07 09:11:21.000000 punctfix-0.10.0/punctfix.egg-info/top_level.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       48 2023-05-06 18:27:41.000000 punctfix-0.10.0/requirements.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       38 2023-05-07 09:11:21.688915 punctfix-0.10.0/setup.cfg
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      847 2023-05-06 18:28:03.000000 punctfix-0.10.0/setup.py
-drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-07 09:11:21.688915 punctfix-0.10.0/tests/
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-06 18:27:41.000000 punctfix-0.10.0/tests/__init__.py
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)    12449 2023-05-06 18:27:41.000000 punctfix-0.10.0/tests/test_punctuation.py
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-17 11:03:09.605989 punctfix-0.10.1/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)    11358 2023-05-06 18:27:41.000000 punctfix-0.10.1/LICENCE.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       63 2023-05-06 18:27:41.000000 punctfix-0.10.1/MANIFEST.in
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     2842 2023-05-17 11:03:09.605989 punctfix-0.10.1/PKG-INFO
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     2418 2023-05-17 11:02:17.000000 punctfix-0.10.1/README.md
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-17 11:03:09.605989 punctfix-0.10.1/punctfix/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       34 2023-05-06 18:27:41.000000 punctfix-0.10.1/punctfix/__init__.py
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)    10318 2023-05-17 11:02:17.000000 punctfix-0.10.1/punctfix/inference.py
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1905 2023-05-12 09:37:32.000000 punctfix-0.10.1/punctfix/models.py
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-17 11:03:09.605989 punctfix-0.10.1/punctfix.egg-info/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     2842 2023-05-17 11:03:09.000000 punctfix-0.10.1/punctfix.egg-info/PKG-INFO
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      324 2023-05-17 11:03:09.000000 punctfix-0.10.1/punctfix.egg-info/SOURCES.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)        1 2023-05-17 11:03:09.000000 punctfix-0.10.1/punctfix.egg-info/dependency_links.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       44 2023-05-17 11:03:09.000000 punctfix-0.10.1/punctfix.egg-info/requires.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       15 2023-05-17 11:03:09.000000 punctfix-0.10.1/punctfix.egg-info/top_level.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       48 2023-05-06 18:27:41.000000 punctfix-0.10.1/requirements.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       38 2023-05-17 11:03:09.605989 punctfix-0.10.1/setup.cfg
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      847 2023-05-17 11:02:17.000000 punctfix-0.10.1/setup.py
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-17 11:03:09.605989 punctfix-0.10.1/tests/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-06 18:27:41.000000 punctfix-0.10.1/tests/__init__.py
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)    12486 2023-05-17 11:02:17.000000 punctfix-0.10.1/tests/test_punctuation.py
```

### Comparing `punctfix-0.10.0/LICENCE.txt` & `punctfix-0.10.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `punctfix-0.10.0/PKG-INFO` & `punctfix-0.10.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: punctfix
-Version: 0.10.0
-Summary: Punctuation restoration library
-Home-page: https://github.com/danspeech/punctfix
-Author: Martin Carsten Nielsen
-Author-email: martin@alvenir.ai
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
 # Punctuation restoration 
 Adds punctuation and capitalization for a given text without punctuation.
 
 Works on Danish, German and English. 
 
 Models hosted on huggingface! ❤️  🤗
 
@@ -39,22 +26,24 @@
 'Mit navn det er Rasmus og jeg kommer fra firmaet Alvenir. Det er mig som har trænet denne lækre model.'
 
 >>> example_text = "en dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning det fungerer da meget godt ikke"
 >>> print(fixer.punctuate(example_text)) 
 'En dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning. Det fungerer da meget godt, ikke?' 
 ```
 
+Note that, per default, the input text will be normalied. See next section for more details.
 
 ## Parameters for PunctFixer
 * Pass `device="cuda"` or `device="cpu"` to indicate where to run inference. Default is `device="cpu"`
 * To handle long sequences, we use a chunk size and an overlap. These can be modified. For higher speed but 
 lower acuracy use a chunk size of 150-200 and very little overlap i.e. 5-10. These parameters are set with 
 default values `word_chunk_size=100`, `word_overlap=70` which makes it run a bit slow. The default parameters
 will be updated when we have some results on variations. 
 * Supported languages are "en" for English, "da" for Danish and "de" for German. Default is `language="da"`.
-
+* Note that the fixer has been trained on normalized text (lowercase letters and numbers) and will per default normalize input text. You can instantiate the model with `skip_normalization=True` to disable this but this might yield errors on some input text.
+* To raise warnings every time the input is normalied, set `warn_on_normalization=True`.
 
 ## Contribute
 If you encounter issues, feel free to open issues in the repo and then we will fix. Even better, create issue and 
 then a PR that fixes the issue! ;-)
 
 Happy punctuating!
```

### Comparing `punctfix-0.10.0/README.md` & `punctfix-0.10.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: punctfix
+Version: 0.10.1
+Summary: Punctuation restoration library
+Home-page: https://github.com/danspeech/punctfix
+Author: Martin Carsten Nielsen
+Author-email: martin@alvenir.ai
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
 # Punctuation restoration 
 Adds punctuation and capitalization for a given text without punctuation.
 
 Works on Danish, German and English. 
 
 Models hosted on huggingface! ❤️  🤗
 
@@ -26,22 +39,24 @@
 'Mit navn det er Rasmus og jeg kommer fra firmaet Alvenir. Det er mig som har trænet denne lækre model.'
 
 >>> example_text = "en dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning det fungerer da meget godt ikke"
 >>> print(fixer.punctuate(example_text)) 
 'En dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning. Det fungerer da meget godt, ikke?' 
 ```
 
+Note that, per default, the input text will be normalied. See next section for more details.
 
 ## Parameters for PunctFixer
 * Pass `device="cuda"` or `device="cpu"` to indicate where to run inference. Default is `device="cpu"`
 * To handle long sequences, we use a chunk size and an overlap. These can be modified. For higher speed but 
 lower acuracy use a chunk size of 150-200 and very little overlap i.e. 5-10. These parameters are set with 
 default values `word_chunk_size=100`, `word_overlap=70` which makes it run a bit slow. The default parameters
 will be updated when we have some results on variations. 
 * Supported languages are "en" for English, "da" for Danish and "de" for German. Default is `language="da"`.
-
+* Note that the fixer has been trained on normalized text (lowercase letters and numbers) and will per default normalize input text. You can instantiate the model with `skip_normalization=True` to disable this but this might yield errors on some input text.
+* To raise warnings every time the input is normalied, set `warn_on_normalization=True`.
 
 ## Contribute
 If you encounter issues, feel free to open issues in the repo and then we will fix. Even better, create issue and 
 then a PR that fixes the issue! ;-)
 
 Happy punctuating!
```

### Comparing `punctfix-0.10.0/punctfix/inference.py` & `punctfix-0.10.1/punctfix/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,17 @@
             if not word:
                 to_warn.append("Additional whitespace was removed.")
             norm_word = WORD_NORMALIZATION_PATTERN.sub("", word)
             if not word:
                 continue
             if len(norm_word) < len(word):
                 to_warn.append(r"Non-word (r'\W') characters were removed.")
+            # We might have removed the entire word
+            if not norm_word:
+                continue
             if not norm_word.islower():
                 norm_word = norm_word.lower()
                 to_warn.append("Text was lowercased.")
             normalized_words.append(norm_word)
 
         # Warn once for each type of normalization
         if self.warn_on_normalization and to_warn:
```

### Comparing `punctfix-0.10.0/punctfix/models.py` & `punctfix-0.10.1/punctfix/models.py`

 * *Files identical despite different names*

### Comparing `punctfix-0.10.0/punctfix.egg-info/PKG-INFO` & `punctfix-0.10.1/punctfix.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punctfix
-Version: 0.10.0
+Version: 0.10.1
 Summary: Punctuation restoration library
 Home-page: https://github.com/danspeech/punctfix
 Author: Martin Carsten Nielsen
 Author-email: martin@alvenir.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -39,22 +39,24 @@
 'Mit navn det er Rasmus og jeg kommer fra firmaet Alvenir. Det er mig som har trænet denne lækre model.'
 
 >>> example_text = "en dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning det fungerer da meget godt ikke"
 >>> print(fixer.punctuate(example_text)) 
 'En dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning. Det fungerer da meget godt, ikke?' 
 ```
 
+Note that, per default, the input text will be normalied. See next section for more details.
 
 ## Parameters for PunctFixer
 * Pass `device="cuda"` or `device="cpu"` to indicate where to run inference. Default is `device="cpu"`
 * To handle long sequences, we use a chunk size and an overlap. These can be modified. For higher speed but 
 lower acuracy use a chunk size of 150-200 and very little overlap i.e. 5-10. These parameters are set with 
 default values `word_chunk_size=100`, `word_overlap=70` which makes it run a bit slow. The default parameters
 will be updated when we have some results on variations. 
 * Supported languages are "en" for English, "da" for Danish and "de" for German. Default is `language="da"`.
-
+* Note that the fixer has been trained on normalized text (lowercase letters and numbers) and will per default normalize input text. You can instantiate the model with `skip_normalization=True` to disable this but this might yield errors on some input text.
+* To raise warnings every time the input is normalied, set `warn_on_normalization=True`.
 
 ## Contribute
 If you encounter issues, feel free to open issues in the repo and then we will fix. Even better, create issue and 
 then a PR that fixes the issue! ;-)
 
 Happy punctuating!
```

### Comparing `punctfix-0.10.0/setup.py` & `punctfix-0.10.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="punctfix",
-    version="0.10.0",
+    version="0.10.1",
     author="Martin Carsten Nielsen",
     author_email="martin@alvenir.ai",
     description="Punctuation restoration library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

### Comparing `punctfix-0.10.0/tests/test_punctuation.py` & `punctfix-0.10.1/tests/test_punctuation.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,16 @@
         super().tearDown()
         self.model = None
 
     def test_do_normalize(self):
         self.model.warn_on_normalization = False
         expected_output = ["hejsa", "mand"]
         for model_input in ("hejsa, mand", " hejsa mand", "hejsa mand",
-                "Hejsa mand", "hejsa  mand", "  hejsa mand", "  hejsa, Mand"):
+                "Hejsa mand", "hejsa  mand", "  hejsa mand", "  hejsa, Mand",
+                "hejsa % mand ! % "):
             actual_output = self.model._split_input_text(model_input)
             self.assertEqual(actual_output, expected_output)
 
     def test_warnings(self):
         self.model.warn_on_normalization = True
         with self.assertWarns(NonNormalizedTextWarning):
             model_input = "hejsa, mand"
```


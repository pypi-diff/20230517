# Comparing `tmp/wordview-0.1.0.tar.gz` & `tmp/wordview-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.1.0.tar", max compression
+gzip compressed data, was "wordview-0.2.0.tar", max compression
```

## Comparing `wordview-0.1.0.tar` & `wordview-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,21 @@
--rw-r--r--   0        0        0     1074 2022-06-16 16:46:04.846999 wordview-0.1.0/LICENSE
--rw-r--r--   0        0        0    13150 2023-01-04 13:08:18.633408 wordview-0.1.0/README.md
--rw-r--r--   0        0        0      660 2023-01-04 14:07:32.254929 wordview-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      151 2022-06-16 16:46:04.892361 wordview-0.1.0/wordview/__init__.py
--rw-r--r--   0        0        0     5297 2022-12-31 16:48:35.202643 wordview-0.1.0/wordview/dashapp/assets/random-logo.png
--rw-r--r--   0        0        0    12891 2022-12-31 16:48:35.202998 wordview-0.1.0/wordview/dashapp/assets/s1.css
--rw-r--r--   0        0        0     2047 2022-12-31 16:48:35.203336 wordview-0.1.0/wordview/dashapp/assets/style.css
--rw-r--r--   0        0        0    17052 2023-01-04 12:59:11.985844 wordview-0.1.0/wordview/dashapp/index.py
--rw-r--r--   0        0        0        0 2022-06-16 16:46:04.892502 wordview-0.1.0/wordview/evaluation/__init__.py
--rw-r--r--   0        0        0      332 2022-06-16 16:46:04.892650 wordview-0.1.0/wordview/evaluation/functions.py
--rw-r--r--   0        0        0     3278 2022-06-16 16:46:04.892803 wordview-0.1.0/wordview/evaluation/metrics.py
--rw-r--r--   0        0        0    11892 2022-06-16 16:46:04.893003 wordview-0.1.0/wordview/gaussianize.py
--rw-r--r--   0        0        0       82 2023-01-04 12:59:19.930728 wordview-0.1.0/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     3053 2022-06-16 16:46:04.893499 wordview-0.1.0/wordview/mwes/am.py
--rw-r--r--   0        0        0     6220 2023-01-04 13:01:16.102043 wordview-0.1.0/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     6319 2023-01-04 13:01:13.153475 wordview-0.1.0/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0      111 2023-01-04 13:01:10.636489 wordview-0.1.0/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     1743 2022-06-16 16:46:04.894278 wordview-0.1.0/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0     7488 2023-01-04 13:01:07.901142 wordview-0.1.0/wordview/preprocessing/filtering.py
--rw-r--r--   0        0        0       63 2023-01-04 13:01:00.667260 wordview-0.1.0/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0   938013 2022-12-31 16:48:35.212911 wordview-0.1.0/wordview/text_analysis/lid.176.ftz
--rw-r--r--   0        0        0    20140 2023-01-04 13:00:54.471181 wordview-0.1.0/wordview/text_analysis/visual_analysis.py
--rw-r--r--   0        0        0    14551 2023-01-04 14:07:35.815270 wordview-0.1.0/setup.py
--rw-r--r--   0        0        0    13935 2023-01-04 14:07:35.816084 wordview-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      339 2023-05-17 09:03:13.609346 wordview-0.2.0/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2022-06-16 16:46:04.846999 wordview-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4613 2023-04-20 12:24:54.126503 wordview-0.2.0/README.rst
+-rw-r--r--   0        0        0      871 2023-05-17 09:14:47.935996 wordview-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      151 2022-06-16 16:46:04.892361 wordview-0.2.0/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-03-30 15:57:29.123003 wordview-0.2.0/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-02-19 17:09:47.466124 wordview-0.2.0/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4788 2023-03-31 14:18:45.152428 wordview-0.2.0/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-02-24 14:54:27.524967 wordview-0.2.0/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-03-02 08:17:36.835194 wordview-0.2.0/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0       84 2023-01-11 13:24:40.126952 wordview-0.2.0/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-01-24 17:56:38.022613 wordview-0.2.0/wordview/mwes/am.py
+-rw-r--r--   0        0        0     5305 2023-05-10 15:53:47.791178 wordview-0.2.0/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     6711 2023-05-10 15:53:47.792472 wordview-0.2.0/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0       55 2023-03-08 15:49:42.676986 wordview-0.2.0/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-04-20 12:24:54.167225 wordview-0.2.0/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0       75 2023-03-27 11:57:05.780678 wordview-0.2.0/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    11825 2023-02-09 12:17:50.008926 wordview-0.2.0/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0   938013 2022-12-31 16:48:35.212911 wordview-0.2.0/wordview/text_analysis/lid.176.ftz
+-rw-r--r--   0        0        0     7345 2023-05-01 15:17:11.759292 wordview-0.2.0/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5499 1970-01-01 00:00:00.000000 wordview-0.2.0/PKG-INFO
```

### Comparing `wordview-0.1.0/LICENSE` & `wordview-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.1.0/pyproject.toml` & `wordview-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 [tool.poetry]
 name = "wordview"
-version = "0.1.0"
-description = "WORDVIEW is a Python package for text analysis."
+version = "0.2.0"
+description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
-readme = "README.md"
+readme = "README.rst"
+include = ["CHANGES.rst"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.12"
 fasttext = "0.9.2"
 pandas = "1.3.5"
 scikit-learn = "1.0.1"
-scipy = "1.7.3"
+scipy = "1.10.0"
 nltk = "3.6.6"
 tqdm = "4.62.3"
 wordcloud = "1.8.1"
 plotly = "5.5.0"
-dash = "2.0.0"
+tabulate = "0.9.0"
+sentence-transformers = "2.2.2"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pre-commit = ">=3.0.0"
+pytest = ">=7.1"
+pytest-cov = ">=3.0.0"
+ipython = ">=8.4.0"
+sphinx = ">=v6.1.3"
+sphinx-rtd-theme= "1.2.0"
 
 [tool.poetry.scripts]
-script_download = "wordview.bin.downloads:download_req"
+script_download = "wordview.bin.downloads:download_nltk_req"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wordview-0.1.0/wordview/mwes/am.py` & `wordview-0.2.0/wordview/mwes/am.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Dict, List
 import math
 
 
 def calculate_pmi(
-    compound_dict: dict, word_dic: dict, num_compound: int, num_words: int, normalize: bool = False
+    compound_dict: dict,
+    word_dic: dict,
+    num_words: int,
+    normalize: bool = False,
 ) -> Dict[str, float]:
     """Calculate Pointwise Mutual Information between the two words of every word pair in nn_dict.
 
     Args:
         compound_dict: Dictionary of compounds and their count.
         word_dic: Dictionary of words and their count.
-        num_compound: Number of compounds.
         num_words: Number of words.
         normalize: Whether or not normalize the pmi score. Normalized pmi is referred to as npmi.
 
     Returns:
         sorted_compound_dict: Dictionary of compounds and their pmi/npmi values, sorted wrt their pmi/npmi.
     """
     tmp_compound_dict = compound_dict
@@ -29,15 +31,17 @@
             if not normalize:
                 tmp_compound_dict[compound] = round(pmi, 2)
             else:
                 npmi = pmi / float(-math.log(p_of_c))
                 tmp_compound_dict[compound] = round(npmi, 2)
         else:
             tmp_compound_dict[compound] = 0.0
-    sorted_compound_dict = dict(sorted(tmp_compound_dict.items(), key=lambda e: e[1], reverse=True))
+    sorted_compound_dict = dict(
+        sorted(tmp_compound_dict.items(), key=lambda e: e[1], reverse=True)
+    )
     return sorted_compound_dict
 
 
 def calculate_am(count_data: dict, am: str, mwe_types: List[str]) -> Dict[str, Dict]:
     """Read the counts from path_to_counts and for each compound calculates the measure specified by am.
 
     Args:
@@ -51,23 +55,21 @@
     res = {}
     num_words = sum(count_data["WORDS"].values())
     if am == "pmi":
         for mt in mwe_types:
             compound_dict_tmp = calculate_pmi(
                 compound_dict=count_data[mt],
                 word_dic=count_data["WORDS"],
-                num_compound=sum(count_data[mt].values()),
                 num_words=num_words,
                 normalize=False,
             )
             res[mt] = compound_dict_tmp
     elif am == "npmi":
         for mt in mwe_types:
             compound_dict_tmp = calculate_pmi(
                 compound_dict=count_data[mt],
                 word_dic=count_data["WORDS"],
-                num_compound=sum(count_data[mt].values()),
                 num_words=num_words,
                 normalize=True,
             )
             res[mt] = compound_dict_tmp
     return res
```

### Comparing `wordview-0.1.0/wordview/mwes/mwe.py` & `wordview-0.2.0/wordview/mwes/mwe.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,61 @@
-import os
-import sys
-import pandas
 import json
 from pathlib import Path
-from typing import List
+from typing import Dict, List, Union
+
+import pandas
 from nltk import word_tokenize
-from wordview.mwes.am import calculate_am
-from wordview.mwes.mwe_utils import replace_mwes, get_counts
+
 from wordview import logger
+from wordview.mwes.am import calculate_am
+from wordview.mwes.mwe_utils import get_counts
 
 
 class MWE(object):
+    """
+    Represents a Multiword Expression.
+    """
+
     def __init__(
         self,
         df: pandas.DataFrame,
         text_column: str,
         mwe_types: List[str] = ["NC"],
-        output_dir: str = "tmp",
         tokenize=False,
     ) -> None:
-        """Provide functionalities around MWEs, for unsupervised extraction of MWEs from text and replacing
-        them in the corpus.
+        """Initialize a new MWE object with the given df, text_column and mwe_types.
 
         Args:
-            df: DataFrame with a text_column that contains the corpus.
-            text_col: Specifies the column of DataFrame that contains the corpus. 'text_column' must contain tokenized text.
-            mwe_types: Types of MWEs. Can be a list containing any of ['NC', 'JNC'].
-            output_dir: Output directory where counts, MWEs and corpus with replaced MWEs are stored.
-            count_dir: Directory where count_file is sotred.
-            count_file: File in which counts are sotred.
-            mwe_dir: Directory where mwe_file is sotred.
-            mwe_file: File in which MWEs are sotred.
-            tokenize: Tokenize the content of 'text_column'.
+            df (pandas.DataFram): DataFrame with a text_column that contains the corpus.
+            text_column (str): Specifies the column of DataFrame where text data resides.
+            mwe_types (List): Types of MWEs to be extracted. Supports: NC for Noun-Noun and JNC for Adjective-Noun compounds. Example: ['NC', 'JNC'].
+            tokenize (bool): Tokenize the content of `df[text_column]`.
 
         Returns:
             None
         """
         self.df = df
-        self.text_col = text_column
+        self.text_column = text_column
         for mt in mwe_types:
             if mt not in ["NC", "JNC"]:
                 raise ValueError(f"{mt} type is not recognized.")
         self.mwe_types = mwe_types
-
-        self.output_dir = output_dir
-        self.count_dir = os.path.join(self.output_dir, "counts")
-        self.count_file = os.path.join(self.count_dir, "count_data.json")
-        self.mwe_dir = os.path.join(self.output_dir, "mwes")
-        self.mwe_file = os.path.join(self.mwe_dir, "mwe_data.json")
-        
-        Path(self.output_dir).mkdir(exist_ok=True)
-
         if tokenize:
-            logger.info('"tokenize" flag set to True. This might lead to a slow instantiation.')
+            logger.info(
+                '"tokenize" flag set to True. This might lead to a slow instantiation.'
+            )
             self.df[text_column] = self.df[text_column].apply(self._tokenize)
         else:
             self._check_tokenized()
 
     def _tokenize(self, x):
         """Helper function to tokenize and join the results with a space.
 
         Args:
-            None
+            x:
 
         Returns:
             None
         """
         return " ".join(word_tokenize(x))
 
     def _check_tokenized(self) -> None:
@@ -73,107 +63,94 @@
 
         Args:
             None
 
         Returns:
             None
         """
-        if self.df[self.text_col].shape[0] > 200:
-            tests = self.df[self.text_col].sample(n=200).tolist()
+        if self.df[self.text_column].shape[0] > 200:
+            tests = self.df[self.text_column].sample(n=200).tolist()
         else:
-            tests = self.df[self.text_col].sample(frac=0.8).tolist()
+            tests = self.df[self.text_column].sample(frac=0.8).tolist()
         num_pass = 0
         for t in tests:
             try:
                 if " ".join(word_tokenize(t)) == t:
                     num_pass += 1
             except Exception as E:
-                logger.error(f'Could not tokenize and join tokens in {t}: \n {E} ')
+                logger.error(f"Could not tokenize and join tokens in {t}: \n {E} ")
 
         if float(num_pass) / float(len(tests)) < 0.8:
             logger.warning(
-                f"It seems that the content of {self.text_col} in the input data frame is not (fully) tokenized.\nThis can lead to poor results. Consider re-instantiating your MWE instance with 'tokenize' flag set to True.\nNote that this might lead to a slower instantiation."
+                f"It seems that the content of {self.text_column} in the input data frame is not (fully) tokenized.\nThis can lead to poor results. Consider re-instantiating your MWE instance with 'tokenize' flag set to True.\nNote that this might lead to a slower instantiation."
             )
 
-    def build_counts(self, file_name: str=None) -> None:
-        """Create various count files to be used by downstream methods 
-        by calling snlp.mwes.counter.get_counts.
+    def build_counts(self, counts_filename: str = "") -> Union[None, Dict]:  # type: ignore
+        """Create various count files to be used by downstream methods
+        by calling wordview.mwes.mwe_utils.
 
         Args:
-            None
+            counts_filename (str): Filename for storing counts.
 
         Returns:
-            None
+            None when no counts_filename is provided, otherwise res which is a dictionary of counts.
         """
         logger.info("Creating counts...")
-        res = get_counts(df=self.df, text_column=self.text_col, mwe_types=self.mwe_types)
-        # Directory
-        try:
-            Path(self.count_dir).mkdir(exist_ok=True)
-        except Exception as e:
-            logger.error(e)
-            raise e
-        # File
-        if not file_name:
-            try:
-                with open(self.count_file, "w") as file:
-                    json.dump(res, file)
-            except Exception as e:
-                logger.error(e)
-                raise e
+        res = get_counts(
+            df=self.df, text_column=self.text_column, mwe_types=self.mwe_types
+        )
+        if not counts_filename:
+            return res
         else:
-            try:            
-                with open(file_name, "w") as file:
+            try:
+                with open(counts_filename, "w") as file:
                     json.dump(res, file)
             except Exception as e:
                 logger.error(e)
                 raise e
-            self.count_file = file_name
 
-    def extract_mwes(self, am: str = "pmi", file_name: str=None) -> None:
+    def extract_mwes(
+        self,
+        am: str = "pmi",
+        mwes_filename: str = "",
+        counts_filename: str = "",
+        counts: Dict = {},
+    ) -> Dict:
         """
+        Extract MWEs from counts_filename with respect to the association measure specified by `am`.
+
         Args:
-            mwe_types: Types of MWEs. Can be any of [NC, JNC]
-            am: The association measure to be used. Can be any of [pmi, npmi]
+            am (str): The association measure to be used. Can be any of [pmi, npmi]
+            mwes_filename (str): File for storing MWEs. Defaults to None.
+            counts_filename (str): File to read counts from.
 
         Returns:
-            None
+            Dictionary of MWEs.
         """
-        with open(self.count_file, "r") as file:
-            count_data = json.load(file)
-        logger.info(f"Extracting {self.mwe_types} based on {am}")
-        mwe_am_dict = calculate_am(count_data=count_data, am=am, mwe_types=self.mwe_types)
-        # Dir
-        try:
-            Path(self.mwe_dir).mkdir(exist_ok=True)
-        except Exception as e:
-            logger.error(e)
-            raise e
-        # File
-        if not file_name:
+        if counts:
+            count_data = counts
+        else:
             try:
-                with open(self.mwe_file, "w") as file:
-                    json.dump(mwe_am_dict, file)
+                with open(counts_filename, "r") as file:
+                    count_data = json.load(file)
             except Exception as e:
                 logger.error(e)
+                logger.error(
+                    "Counts must be provided either via input argument `counts` or `counts_filename`. Argument `counts` is not specified and it seems like there was an error reading the counts from `counts_filename`."
+                )
                 raise e
-        else:
+
+        logger.info(f"Extracting {self.mwe_types} based on {am}")
+        mwe_am_dict = calculate_am(
+            count_data=count_data, am=am, mwe_types=self.mwe_types
+        )
+        if mwes_filename:
             try:
-                with open(file_name, "w") as file:
+                with open(mwes_filename, "w") as file:
                     json.dump(mwe_am_dict, file)
             except Exception as e:
                 logger.error(e)
                 raise e
-
-
-if __name__ == "__main__":
-    import pandas as pd
-    from wordview.mwes.mwe_utils import replace_mwes
-
-    imdb_train = pd.read_csv("data/imdb_train_sample.tsv", sep="\t", names=["label", "text"])
-    mwe = MWE(df=imdb_train, mwe_types=["NC", "JNC"], text_column="text", tokenize=True)
-    mwe.build_counts()
-    mwe.extract_mwes(am="npmi")
-    new_df = replace_mwes(
-        path_to_mwes="tmp/mwes/mwe_data.json", mwe_types=["NC", "JNC"], df=imdb_train, text_column="text"
-    )
-    new_df.to_csv("tmp/new_df.csv", sep="\t")
+            finally:
+                return mwe_am_dict
+        else:
+            return mwe_am_dict
```

### Comparing `wordview-0.1.0/wordview/mwes/mwe_utils.py` & `wordview-0.2.0/wordview/mwes/mwe_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing import Dict, List
 import json
+import re
 import sys
+from collections import Counter
+from typing import Dict, List
+
+import nltk
 import pandas
-import re
 import tqdm
+
 from wordview import logger
-import nltk
-from collections import Counter
 
 
-def replace_mwes(
+def hyphenate_mwes(
     path_to_mwes: str,
     mwe_types: List[str],
     df: pandas.DataFrame,
     text_column: str,
     am_threshold: float = 0.7,
     only_mwes: bool = False,
     lower_case: bool = False,
@@ -36,26 +38,31 @@
     try:
         with open(path_to_mwes, "r") as file:
             mwe_type_mwe_am = json.load(file)
     except Exception as e:
         raise e
     good_mwes = set()
     for t in mwe_types:
-        logger.info(f'Replacing MWEs of type {t} in the corpus.')
+        logger.info(f"Replacing MWEs of type {t} in the corpus.")
         if t not in mwe_type_mwe_am:
-            logger.error(f'MWEs of type {t} do not exist. Make sure the file containing MWEs in {path_to_mwes} includes type {t}')
+            logger.error(
+                f"MWEs of type {t} do not exist. Make sure the file containing MWEs in {path_to_mwes} includes type {t}"
+            )
             sys.exit(1)
         pmi_sorted_dict = mwe_type_mwe_am[t]
         logger.info(f"Number of all MWEs of type {t}: {len(pmi_sorted_dict)}")
         for k, v in pmi_sorted_dict.items():
             if v >= am_threshold:
                 good_mwes.add(k)
             else:
                 break
-        logger.info("Number of MWEs to be replaced in corpus based on the association threshold: %d" % len(good_mwes))
+        logger.info(
+            "Number of MWEs to be replaced in corpus based on the association threshold: %d"
+            % len(good_mwes)
+        )
 
     logger.info("Replacing compounds in text")
     new_text = []
     for sent in tqdm.tqdm(df[text_column]):
         sent = sent.lower() if lower_case else sent
         bigrams = get_ngrams(sent, 2)
         if only_mwes:
@@ -70,50 +77,58 @@
                 if bg in good_mwes:
                     sent = re.sub(bg, bg.split(" ")[0] + "-" + bg.split(" ")[1], sent)
         new_text.append(sent)
     df[text_column] = new_text
     return df
 
 
-def get_ngrams(sentence: str, n: int) -> List:
+def get_ngrams(sentence: str, n: int) -> List[str]:
     """Extracts n-grams from sentence.
 
     Args:
         sentence: Input sentence from which n-grams are to be extracted.
         n: Size of n-grams.
 
     Returns:
         ngrams: List of extracted n-grams.
     """
-    ngrams = []
+    if not isinstance(sentence, str):
+        raise TypeError(
+            f"Input argument 'sentence' must be of type str. You have provided an input of type: {type(sentence)}."
+        )
+    ngrams: List[str] = []
     try:
         tokens = sentence.split(" ")
     except Exception as E:
         logger.error(E)
-        logger.error(f'Input "{sentence}" cannot be spilitted around space. No n-gram is extracted.')
+        logger.error(
+            f'Input "{sentence}" cannot be spilitted around space. No n-gram is extracted.'
+        )
         return ngrams
     for i in range(len(tokens) - n + 1):
         ngrams.append(" ".join(tokens[i : i + n]))
     return ngrams
 
 
-def get_counts(df: pandas.DataFrame, text_column: str, mwe_types: List[str]) -> dict:
+def get_counts(
+    df: pandas.DataFrame, text_column: str, mwe_types: List[str]
+) -> Dict[str, Dict[str, int]]:
     """Read a corpus in pandas.DataFrame format and generates all counts necessary for calculating AMs.
 
     Args:
         df (pandas.DataFrame): DataFrame with input data, which contains a column with text content
                                from which compounds and their counts are extracted.
         text_column: Name of the column the contains the text content.
         mwe_types: Types of MWEs. Can be any of [NC, JNC]
 
     Returns:
-        res: Dictionary of mwe_types to dictionary of individual mwe within that type and their count.
+        res which is a dictionary of mwe_types to dictionary of individual mwe within that type and their count.
             E.g. {'NC':{'climate change': 10, 'brain drain': 3}, 'JNC': {'black sheep': 3, 'red flag': 2}}
     """
-    res = {}
+    res: Dict[str, Dict[str, int]] = {}
     for mt in mwe_types:
         res[mt] = {}
     res["WORDS"] = {}
     for sent in tqdm.tqdm(df[text_column]):
         tokens = sent.split(" ")
         word_count_dict = Counter(tokens)
         for k, v in word_count_dict.items():
@@ -143,15 +158,15 @@
     """
     if not isinstance(tokens, list):
         raise TypeError(
             f'Input argument "tokens" must be a list of string. Currently it is of type {type(tokens)} \
             with a value of: {tokens}.'
         )
     if len(tokens) == 0:
-        return
+        return {}
     mwes = []
     postag_tokens = nltk.pos_tag(tokens)
     w1_pos_tags = []
     w2_pos_tags = []
     if mwe_type == "NC":
         w1_pos_tags = ["NN", "NNS"]
         w2_pos_tags = ["NN", "NNS"]
@@ -160,15 +175,17 @@
         w2_pos_tags = ["NN", "NNS"]
     for i in range(len(postag_tokens) - 1):
         w1 = postag_tokens[i]
         if w1[1] not in w1_pos_tags:
             continue
         else:
             w2 = postag_tokens[i + 1]
-            if not re.match("[a-zA-Z0-9]{2,}", w1[0]) or not re.match("[a-zA-Z0-9]{2,}", w2[0]):
+            if not re.match("[a-zA-Z0-9]{2,}", w1[0]) or not re.match(
+                "[a-zA-Z0-9]{2,}", w2[0]
+            ):
                 continue
             if w2[1] in w2_pos_tags:
                 if i + 2 < len(postag_tokens):
                     w3 = postag_tokens[i + 2]
                     if w3 not in ["NN", "NNS"]:
                         mwes.append(w1[0] + " " + w2[0])
                 else:
```

### Comparing `wordview-0.1.0/wordview/text_analysis/lid.176.ftz` & `wordview-0.2.0/wordview/text_analysis/lid.176.ftz`

 * *Files identical despite different names*


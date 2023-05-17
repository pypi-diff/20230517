# Comparing `tmp/algorithmadts-0.1.0.tar.gz` & `tmp/algorithmadts-0.1.1.tar.gz`

## Comparing `algorithmadts-0.1.0.tar` & `algorithmadts-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/.DS_Store
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/src/AlgorithmADTs/.DS_Store
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/src/AlgorithmADTs/AbstractDataTypes.py
--rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/src/AlgorithmADTs/GraphAlgorithms.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/src/AlgorithmADTs/__init__.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/tests/experimenting.ipynb
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/tests/test_GraphAlgorithms.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/LICENSE
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/README.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 algorithmadts-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.DS_Store
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/src/AlgorithmADTs/.DS_Store
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/src/AlgorithmADTs/AbstractDataTypes.py
+-rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/src/AlgorithmADTs/GraphAlgorithms.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/src/AlgorithmADTs/__init__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/tests/experimenting.ipynb
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/tests/test_GraphAlgorithms.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/README.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/PKG-INFO
```

### Comparing `algorithmadts-0.1.0/.DS_Store` & `algorithmadts-0.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.0/src/.DS_Store` & `algorithmadts-0.1.1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.0/src/AlgorithmADTs/.DS_Store` & `algorithmadts-0.1.1/src/AlgorithmADTs/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.0/src/AlgorithmADTs/AbstractDataTypes.py` & `algorithmadts-0.1.1/src/AlgorithmADTs/AbstractDataTypes.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.0/src/AlgorithmADTs/GraphAlgorithms.py` & `algorithmadts-0.1.1/src/AlgorithmADTs/GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.0/tests/experimenting.ipynb` & `algorithmadts-0.1.1/tests/experimenting.ipynb`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.0/tests/test_GraphAlgorithms.py` & `algorithmadts-0.1.1/tests/test_GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.0/LICENSE` & `algorithmadts-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.0/README.md` & `algorithmadts-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Algorithm Abstract Data Types
 Finlay's package for Abstract Data Types written for Algorithmics class
 
 ## Installation
 Run the following command in your terminal: 
-`pip install -i https://test.pypi.org/simple/ AlgorithmADTs`
+`pip install AlgorithmADTs`
 
 AlgorithmADTs can now be imported into your python scripts! 
 
 I recommend `from AlgorithmADTs import *` to include all functionality, but you can also import from `AlgorithmADTs.AbstractDataTypes` or `AlgorithmADTs.GraphAlgorithms` 
 
 ## ADTS:
 ```
```

### Comparing `algorithmadts-0.1.0/PKG-INFO` & `algorithmadts-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: AlgorithmADTs
-Version: 0.1.0
+Version: 0.1.1
 Summary: General purpose Abstract Data Types for Algorithmics
 Author-email: Finlay <finlay3.141@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Algorithm Abstract Data Types
 Finlay's package for Abstract Data Types written for Algorithmics class
 
 ## Installation
 Run the following command in your terminal: 
-`pip install -i https://test.pypi.org/simple/ AlgorithmADTs`
+`pip install AlgorithmADTs`
 
 AlgorithmADTs can now be imported into your python scripts! 
 
 I recommend `from AlgorithmADTs import *` to include all functionality, but you can also import from `AlgorithmADTs.AbstractDataTypes` or `AlgorithmADTs.GraphAlgorithms` 
 
 ## ADTS:
 ```
```


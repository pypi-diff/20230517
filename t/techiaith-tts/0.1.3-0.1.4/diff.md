# Comparing `tmp/techiaith-tts-0.1.3.tar.gz` & `tmp/techiaith-tts-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techiaith-tts-0.1.3.tar", last modified: Wed May 17 13:14:26 2023, max compression
+gzip compressed data, was "techiaith-tts-0.1.4.tar", last modified: Wed May 17 13:51:08 2023, max compression
```

## Comparing `techiaith-tts-0.1.3.tar` & `techiaith-tts-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:26.172718 techiaith-tts-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 13:14:26.172718 techiaith-tts-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:14:26.172718 techiaith-tts-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:26.168718 techiaith-tts-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:26.172718 techiaith-tts-0.1.3/src/techiaith/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/src/techiaith/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:26.168718 techiaith-tts-0.1.3/src/techiaith/tts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:26.172718 techiaith-tts-0.1.3/src/techiaith/tts/testun/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:26.172718 techiaith-tts-0.1.3/src/techiaith/tts/testun/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/src/techiaith/tts/testun/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/src/techiaith/tts/testun/date_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/src/techiaith/tts/testun/known_phrases.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/src/techiaith/tts/testun/lexicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/src/techiaith/tts/testun/lookups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/src/techiaith/tts/testun/number_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/src/techiaith/tts/testun/time_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/src/techiaith/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:26.172718 techiaith-tts-0.1.3/src/techiaith_tts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 13:14:26.000000 techiaith-tts-0.1.3/src/techiaith_tts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-17 13:14:26.000000 techiaith-tts-0.1.3/src/techiaith_tts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:14:26.000000 techiaith-tts-0.1.3/src/techiaith_tts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-17 13:14:26.000000 techiaith-tts-0.1.3/src/techiaith_tts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 13:14:26.000000 techiaith-tts-0.1.3/src/techiaith_tts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:26.172718 techiaith-tts-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/tests/test_date_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/tests/test_known_phrase.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/tests/test_lecsicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/tests/test_number_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-17 13:14:10.000000 techiaith-tts-0.1.3/tests/test_time_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:08.359551 techiaith-tts-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-17 13:50:49.000000 techiaith-tts-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 13:51:08.359551 techiaith-tts-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-17 13:50:49.000000 techiaith-tts-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-17 13:50:49.000000 techiaith-tts-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:51:08.359551 techiaith-tts-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-17 13:50:49.000000 techiaith-tts-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:08.351551 techiaith-tts-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:08.355551 techiaith-tts-0.1.4/src/techiaith/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:50:49.000000 techiaith-tts-0.1.4/src/techiaith/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:08.351551 techiaith-tts-0.1.4/src/techiaith/tts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:08.355551 techiaith-tts-0.1.4/src/techiaith/tts/testun/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:08.355551 techiaith-tts-0.1.4/src/techiaith/tts/testun/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:50:49.000000 techiaith-tts-0.1.4/src/techiaith/tts/testun/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/src/techiaith/tts/testun/date_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/src/techiaith/tts/testun/known_phrases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/src/techiaith/tts/testun/lexicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/src/techiaith/tts/testun/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/src/techiaith/tts/testun/number_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/src/techiaith/tts/testun/time_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/src/techiaith/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:08.355551 techiaith-tts-0.1.4/src/techiaith_tts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 13:51:08.000000 techiaith-tts-0.1.4/src/techiaith_tts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-17 13:51:08.000000 techiaith-tts-0.1.4/src/techiaith_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:51:08.000000 techiaith-tts-0.1.4/src/techiaith_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-17 13:51:08.000000 techiaith-tts-0.1.4/src/techiaith_tts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 13:51:08.000000 techiaith-tts-0.1.4/src/techiaith_tts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:08.359551 techiaith-tts-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/tests/test_date_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/tests/test_known_phrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/tests/test_lecsicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/tests/test_number_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-17 13:50:50.000000 techiaith-tts-0.1.4/tests/test_time_norm.py
```

### Comparing `techiaith-tts-0.1.3/LICENSE` & `techiaith-tts-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.3/PKG-INFO` & `techiaith-tts-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: techiaith-tts
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/techiaith/techiaith-tts
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `techiaith-tts-0.1.3/README.md` & `techiaith-tts-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.3/setup.py` & `techiaith-tts-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,12 +34,13 @@
     keywords="",
     url="https://github.com/techiaith/techiaith-tts",
     author="Allen Institute for Artificial Intelligence",
     author_email="contact@allenai.org",
     license="Apache",
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
-    package_data={"techiaith": ["py.typed", "*.txt"]},
+    include_package_data=True,
+    package_data={"techiaith": ["py.typed"]},
     install_requires=read_requirements("requirements.txt"),
     extras_require={"dev": read_requirements("dev-requirements.txt")},
     python_requires=">=3.8",
 )
```

### Comparing `techiaith-tts-0.1.3/src/techiaith/tts/testun/date_norm.py` & `techiaith-tts-0.1.4/src/techiaith/tts/testun/date_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.3/src/techiaith/tts/testun/lexicon.py` & `techiaith-tts-0.1.4/src/techiaith/tts/testun/lexicon.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.3/src/techiaith/tts/testun/lookups.py` & `techiaith-tts-0.1.4/src/techiaith/tts/testun/lookups.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.3/src/techiaith/tts/testun/number_norm.py` & `techiaith-tts-0.1.4/src/techiaith/tts/testun/number_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.3/src/techiaith/tts/testun/time_norm.py` & `techiaith-tts-0.1.4/src/techiaith/tts/testun/time_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.3/src/techiaith_tts.egg-info/PKG-INFO` & `techiaith-tts-0.1.4/src/techiaith_tts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: techiaith-tts
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/techiaith/techiaith-tts
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `techiaith-tts-0.1.3/src/techiaith_tts.egg-info/SOURCES.txt` & `techiaith-tts-0.1.4/src/techiaith_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.3/tests/test_date_norm.py` & `techiaith-tts-0.1.4/tests/test_date_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.3/tests/test_number_norm.py` & `techiaith-tts-0.1.4/tests/test_number_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.3/tests/test_time_norm.py` & `techiaith-tts-0.1.4/tests/test_time_norm.py`

 * *Files identical despite different names*


# Comparing `tmp/techiaith-tts-0.1.1.tar.gz` & `tmp/techiaith-tts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techiaith-tts-0.1.1.tar", last modified: Thu Mar 23 14:18:37 2023, max compression
+gzip compressed data, was "techiaith-tts-0.1.2.tar", last modified: Wed May 17 12:32:17 2023, max compression
```

## Comparing `techiaith-tts-0.1.1.tar` & `techiaith-tts-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:18:37.005167 techiaith-tts-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-23 14:18:37.005167 techiaith-tts-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 14:18:37.005167 techiaith-tts-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:18:37.001167 techiaith-tts-0.1.1/techiaith/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/techiaith/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/techiaith/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/techiaith/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:18:37.005167 techiaith-tts-0.1.1/techiaith_tts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-23 14:18:36.000000 techiaith-tts-0.1.1/techiaith_tts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-23 14:18:36.000000 techiaith-tts-0.1.1/techiaith_tts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:18:36.000000 techiaith-tts-0.1.1/techiaith_tts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-23 14:18:36.000000 techiaith-tts-0.1.1/techiaith_tts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-23 14:18:36.000000 techiaith-tts-0.1.1/techiaith_tts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:18:37.005167 techiaith-tts-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/tests/test_date_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/tests/test_known_phrase.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/tests/test_lecsicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/tests/test_number_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-23 14:18:22.000000 techiaith-tts-0.1.1/tests/test_time_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:17.410067 techiaith-tts-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-17 12:32:05.000000 techiaith-tts-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 12:32:17.410067 techiaith-tts-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-17 12:32:05.000000 techiaith-tts-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-17 12:32:05.000000 techiaith-tts-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:32:17.410067 techiaith-tts-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-17 12:32:05.000000 techiaith-tts-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:17.410067 techiaith-tts-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:17.410067 techiaith-tts-0.1.2/src/techiaith/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:05.000000 techiaith-tts-0.1.2/src/techiaith/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:17.406067 techiaith-tts-0.1.2/src/techiaith/tts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:17.410067 techiaith-tts-0.1.2/src/techiaith/tts/testun/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:17.410067 techiaith-tts-0.1.2/src/techiaith/tts/testun/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:05.000000 techiaith-tts-0.1.2/src/techiaith/tts/testun/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/src/techiaith/tts/testun/date_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/src/techiaith/tts/testun/known_phrases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/src/techiaith/tts/testun/lexicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/src/techiaith/tts/testun/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/src/techiaith/tts/testun/number_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/src/techiaith/tts/testun/time_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/src/techiaith/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:17.410067 techiaith-tts-0.1.2/src/techiaith_tts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 12:32:17.000000 techiaith-tts-0.1.2/src/techiaith_tts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-17 12:32:17.000000 techiaith-tts-0.1.2/src/techiaith_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:32:17.000000 techiaith-tts-0.1.2/src/techiaith_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-17 12:32:17.000000 techiaith-tts-0.1.2/src/techiaith_tts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 12:32:17.000000 techiaith-tts-0.1.2/src/techiaith_tts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:17.410067 techiaith-tts-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/tests/test_date_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/tests/test_known_phrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/tests/test_lecsicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/tests/test_number_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-17 12:32:06.000000 techiaith-tts-0.1.2/tests/test_time_norm.py
```

### Comparing `techiaith-tts-0.1.1/LICENSE` & `techiaith-tts-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.1/PKG-INFO` & `techiaith-tts-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: techiaith-tts
-Version: 0.1.1
-Home-page: https://github.com/str20tbl/techiaith-tts
+Version: 0.1.2
+Home-page: https://github.com/techiaith/techiaith-tts
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `techiaith-tts-0.1.1/README.md` & `techiaith-tts-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.1/setup.py` & `techiaith-tts-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import find_packages, setup
+from setuptools import find_namespace_packages, setup
 
 
 def read_requirements(filename: str):
     with open(filename) as requirements_file:
         requirements = []
         for line in requirements_file:
             line = line.strip()
@@ -11,15 +11,15 @@
             requirements.append(line)
     return requirements
 
 
 # version.py defines the VERSION and VERSION_SHORT variables.
 # We use exec here so we don't import cached_path whilst setting up.
 VERSION = {}  # type: ignore
-with open("techiaith/version.py", "r") as version_file:
+with open("src/techiaith/version.py", "r") as version_file:
     exec(version_file.read(), VERSION)
 
 setup(
     name="techiaith-tts",
     version=VERSION["VERSION"],
     description="",
     long_description=open("README.md").read(),
@@ -28,19 +28,18 @@
         "Intended Audience :: Science/Research",
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     keywords="",
-    url="https://github.com/str20tbl/techiaith-tts",
+    url="https://github.com/techiaith/techiaith-tts",
     author="Allen Institute for Artificial Intelligence",
     author_email="contact@allenai.org",
     license="Apache",
-    packages=find_packages(
-        exclude=["*.tests", "*.tests.*", "tests.*", "tests"],
-    ),
+    packages=find_namespace_packages(where="src"),
+    package_dir={"": "src"},
     package_data={"techiaith": ["py.typed"]},
     install_requires=read_requirements("requirements.txt"),
     extras_require={"dev": read_requirements("dev-requirements.txt")},
     python_requires=">=3.8",
 )
```

### Comparing `techiaith-tts-0.1.1/techiaith_tts.egg-info/PKG-INFO` & `techiaith-tts-0.1.2/src/techiaith_tts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: techiaith-tts
-Version: 0.1.1
-Home-page: https://github.com/str20tbl/techiaith-tts
+Version: 0.1.2
+Home-page: https://github.com/techiaith/techiaith-tts
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `techiaith-tts-0.1.1/tests/test_date_norm.py` & `techiaith-tts-0.1.2/tests/test_date_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.1/tests/test_number_norm.py` & `techiaith-tts-0.1.2/tests/test_number_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.1/tests/test_time_norm.py` & `techiaith-tts-0.1.2/tests/test_time_norm.py`

 * *Files identical despite different names*


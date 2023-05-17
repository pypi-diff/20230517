# Comparing `tmp/dctrackclient-0.3.0.tar.gz` & `tmp/dctrackclient-0.3.1.tar.gz`

## Comparing `dctrackclient-0.3.0.tar` & `dctrackclient-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/api.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/schema.json
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/.github/workflows/gen.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/LICENSE
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/LEGAL
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/api.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/schema.json
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/.github/workflows/gen.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/.gitignore
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/LICENSE
+-rw-r--r--   0        0        0     8447 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8964 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/PKG-INFO
```

### Comparing `dctrackclient-0.3.0/api.json` & `dctrackclient-0.3.1/api.json`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.0/schema.json` & `dctrackclient-0.3.1/schema.json`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.0/.github/workflows/gen.py` & `dctrackclient-0.3.1/.github/workflows/gen.py`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.0/.github/workflows/python-publish.yml` & `dctrackclient-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.0/src/dcTrackClient/__init__.py` & `dctrackclient-0.3.1/src/dcTrackClient/__init__.py`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.0/README.md` & `dctrackclient-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+**WARNING: this project is still under development and may not be stable!**
+
 # dcTrackClient ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/nicfv/dcTrackClient/python-publish.yml?label=publish&logo=pypi) ![PyPI](https://img.shields.io/pypi/v/dcTrackClient) ![PyPI - Downloads](https://img.shields.io/pypi/dm/dcTrackClient)
 
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API client in Python
 
 ## Initialize a connection to the dcTrack API
 
 Import the class:
```

### Comparing `dctrackclient-0.3.0/pyproject.toml` & `dctrackclient-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.3.0/PKG-INFO` & `dctrackclient-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.3.0
+Version: 0.3.1
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+**WARNING: this project is still under development and may not be stable!**
+
 # dcTrackClient ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/nicfv/dcTrackClient/python-publish.yml?label=publish&logo=pypi) ![PyPI](https://img.shields.io/pypi/v/dcTrackClient) ![PyPI - Downloads](https://img.shields.io/pypi/dm/dcTrackClient)
 
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API client in Python
 
 ## Initialize a connection to the dcTrack API
 
 Import the class:
```


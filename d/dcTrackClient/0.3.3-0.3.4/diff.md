# Comparing `tmp/dctrackclient-0.3.3.tar.gz` & `tmp/dctrackclient-0.3.4.tar.gz`

## Comparing `dctrackclient-0.3.3.tar` & `dctrackclient-0.3.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.3.3/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.3.3/.gitignore
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     8447 2020-02-02 00:00:00.000000 dctrackclient-0.3.3/../README.md
--rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 dctrackclient-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.3.4/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.3.4/.gitignore
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 dctrackclient-0.3.4/../README.md
+-rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 dctrackclient-0.3.4/PKG-INFO
```

### Comparing `dctrackclient-0.3.3/src/dcTrackClient/__init__.py` & `dctrackclient-0.3.4/src/dcTrackClient/__init__.py`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.3/pyproject.toml` & `dctrackclient-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.3.3/../README.md` & `dctrackclient-0.3.4/../README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 **WARNING: this project is still under development and may not be stable!**
 
-# dcTrackClient ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/nicfv/dcTrackClient/python-publish.yml?label=publish&logo=pypi) ![PyPI](https://img.shields.io/pypi/v/dcTrackClient) ![PyPI - Downloads](https://img.shields.io/pypi/dm/dcTrackClient)
+# dcTrackClient ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/nicfv/dcTrackClient/publish.yml?logo=github) ![PyPI](https://img.shields.io/pypi/v/dcTrackClient) ![PyPI - Downloads](https://img.shields.io/pypi/dm/dcTrackClient?logo=pypi)
 
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API client in Python
 
 ## Initialize a connection to the dcTrack API
 
 Import the class:
```

### Comparing `dctrackclient-0.3.3/PKG-INFO` & `dctrackclient-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.3.3
+Version: 0.3.4
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 **WARNING: this project is still under development and may not be stable!**
 
-# dcTrackClient ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/nicfv/dcTrackClient/python-publish.yml?label=publish&logo=pypi) ![PyPI](https://img.shields.io/pypi/v/dcTrackClient) ![PyPI - Downloads](https://img.shields.io/pypi/dm/dcTrackClient)
+# dcTrackClient ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/nicfv/dcTrackClient/publish.yml?logo=github) ![PyPI](https://img.shields.io/pypi/v/dcTrackClient) ![PyPI - Downloads](https://img.shields.io/pypi/dm/dcTrackClient?logo=pypi)
 
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API client in Python
 
 ## Initialize a connection to the dcTrack API
 
 Import the class:
```


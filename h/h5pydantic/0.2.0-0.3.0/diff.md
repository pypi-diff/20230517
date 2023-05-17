# Comparing `tmp/h5pydantic-0.2.0.tar.gz` & `tmp/h5pydantic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5pydantic-0.2.0.tar", max compression
+gzip compressed data, was "h5pydantic-0.3.0.tar", max compression
```

## Comparing `h5pydantic-0.2.0.tar` & `h5pydantic-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0      340 2023-05-13 03:54:48.206900 h5pydantic-0.2.0/README.md
--rw-r--r--   0        0        0      997 2023-05-13 04:30:16.241603 h5pydantic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4730 2023-05-13 01:47:30.188229 h5pydantic-0.2.0/src/h5pydantic/__init__.py
--rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 h5pydantic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-05-13 03:54:48.206900 h5pydantic-0.3.0/README.md
+-rw-r--r--   0        0        0     1219 2023-05-17 01:26:58.110102 h5pydantic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-05-17 00:29:12.901569 h5pydantic-0.3.0/src/h5pydantic/__init__.py
+-rw-r--r--   0        0        0     5726 2023-05-17 01:27:57.055075 h5pydantic-0.3.0/src/h5pydantic/model.py
+-rw-r--r--   0        0        0       12 2023-05-17 00:25:11.728066 h5pydantic-0.3.0/src/h5pydantic/newsfragments/.gitignore
+-rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 h5pydantic-0.3.0/PKG-INFO
```

### Comparing `h5pydantic-0.2.0/pyproject.toml` & `h5pydantic-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 [tool.poetry]
 name = "h5pydantic"
-version = "0.2.0"
+version = "0.3.0"
 description = "Pydantic models for HDF5 files."
 authors = ["Clinton Roy <clinton.roy@gmail.com>"]
-license = "PSF"
 readme = "README.md"
 repository = "https://gitlab.com/clinton.roy/h5pydantic"
 documentation = "https://h5pydantic.readthedocs.io/"
 packages = [{include = "h5pydantic", from = "src"}]
 classifiers = [
 	    "Development Status :: 3 - Alpha",
 	    "Framework :: Pydantic",
             "Natural Language :: English",
 	    "Topic :: File Formats",
             "Topic :: Scientific/Engineering :: Information Analysis",
             "Intended Audience :: Science/Research",
+            "License :: OSI Approved :: Python Software Foundation License",
 ]
 [tool.poetry.dependencies]
 python = "~3.9"
 h5py = "^3.8.0"
 pydantic = "^1.10.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 ruff = "^0.0.265"
+hypothesis = "^6.75.2"
 
 [tool.poetry.group.doc.dependencies]
-sphinx = "^7.0.0"
 sphinx-autodoc-typehints = "^1.23.0"
+sphinx-rtd-theme = "^1.2.0"
+sphinx = "6.2.1"
+towncrier = "^22.12.0"
 
 [tool.ruff]
 line-length = 120
 
+[tool.towncrier]
+package = "h5pydantic"
+package_dir = "src"
+filename = "docs/news.rst"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `h5pydantic-0.2.0/PKG-INFO` & `h5pydantic-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: h5pydantic
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pydantic models for HDF5 files.
 Home-page: https://gitlab.com/clinton.roy/h5pydantic
-License: PSF
 Author: Clinton Roy
 Author-email: clinton.roy@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pydantic
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: File Formats
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
```


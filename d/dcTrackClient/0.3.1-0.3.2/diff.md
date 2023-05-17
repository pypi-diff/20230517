# Comparing `tmp/dctrackclient-0.3.1.tar.gz` & `tmp/dctrackclient-0.3.2.tar.gz`

## Comparing `dctrackclient-0.3.1.tar` & `dctrackclient-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/LEGAL
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/api.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/schema.json
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/.github/workflows/gen.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/.gitignore
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/LICENSE
--rw-r--r--   0        0        0     8447 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8964 2020-02-02 00:00:00.000000 dctrackclient-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/LEGAL
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/api.json
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/package.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/schema.json
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/.github/workflows/gen.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/.gitignore
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8447 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/README.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 dctrackclient-0.3.2/PKG-INFO
```

### Comparing `dctrackclient-0.3.1/LEGAL` & `dctrackclient-0.3.2/LEGAL`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.1/api.json` & `dctrackclient-0.3.2/api.json`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.1/schema.json` & `dctrackclient-0.3.2/schema.json`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.1/.github/workflows/gen.py` & `dctrackclient-0.3.2/.github/workflows/gen.py`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.1/.github/workflows/python-publish.yml` & `dctrackclient-0.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.1/src/dcTrackClient/__init__.py` & `dctrackclient-0.3.2/src/dcTrackClient/__init__.py`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.1/LICENSE` & `dctrackclient-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.1/README.md` & `dctrackclient-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.3.1/pyproject.toml` & `dctrackclient-0.3.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
+license = {file = "LICENSE"}
 
 [project.urls]
 "Homepage" = "https://github.com/nicfv/dcTrackClient/"
 "Bug Tracker" = "https://github.com/nicfv/dcTrackClient/pulls"
```


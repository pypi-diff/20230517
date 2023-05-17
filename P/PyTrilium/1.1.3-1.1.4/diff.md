# Comparing `tmp/pytrilium-1.1.3.tar.gz` & `tmp/pytrilium-1.1.4.tar.gz`

## Comparing `pytrilium-1.1.3.tar` & `pytrilium-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pytrilium-1.1.3/.drone.yml
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 pytrilium-1.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pytrilium-1.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 pytrilium-1.1.3/.github/workflows/main.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytrilium-1.1.3/logs/.gitkeep
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pytrilium-1.1.3/pytrilium/PyTrilium.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 pytrilium-1.1.3/pytrilium/PyTriliumAttributeClient.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pytrilium-1.1.3/pytrilium/PyTriliumBranchClient.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 pytrilium-1.1.3/pytrilium/PyTriliumCalendarClient.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 pytrilium-1.1.3/pytrilium/PyTriliumClient.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pytrilium-1.1.3/pytrilium/PyTriliumCustomClient.py
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 pytrilium-1.1.3/pytrilium/PyTriliumNoteClient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytrilium-1.1.3/pytrilium/__init__.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 pytrilium-1.1.3/pytrilium/log.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pytrilium-1.1.3/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pytrilium-1.1.3/LICENSE
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 pytrilium-1.1.3/README.md
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pytrilium-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 pytrilium-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pytrilium-1.1.4/.drone.yml
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 pytrilium-1.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pytrilium-1.1.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 pytrilium-1.1.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytrilium-1.1.4/logs/.gitkeep
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pytrilium-1.1.4/pytrilium/PyTrilium.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 pytrilium-1.1.4/pytrilium/PyTriliumAttributeClient.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pytrilium-1.1.4/pytrilium/PyTriliumBranchClient.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 pytrilium-1.1.4/pytrilium/PyTriliumCalendarClient.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 pytrilium-1.1.4/pytrilium/PyTriliumClient.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pytrilium-1.1.4/pytrilium/PyTriliumCustomClient.py
+-rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 pytrilium-1.1.4/pytrilium/PyTriliumNoteClient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytrilium-1.1.4/pytrilium/__init__.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 pytrilium-1.1.4/pytrilium/log.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pytrilium-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pytrilium-1.1.4/LICENSE
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 pytrilium-1.1.4/README.md
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pytrilium-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 pytrilium-1.1.4/PKG-INFO
```

### Comparing `pytrilium-1.1.3/.drone.yml` & `pytrilium-1.1.4/.drone.yml`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/CODE_OF_CONDUCT.md` & `pytrilium-1.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/.github/workflows/main.yml` & `pytrilium-1.1.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/pytrilium/PyTrilium.py` & `pytrilium-1.1.4/pytrilium/PyTrilium.py`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/pytrilium/PyTriliumAttributeClient.py` & `pytrilium-1.1.4/pytrilium/PyTriliumAttributeClient.py`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/pytrilium/PyTriliumBranchClient.py` & `pytrilium-1.1.4/pytrilium/PyTriliumBranchClient.py`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/pytrilium/PyTriliumCalendarClient.py` & `pytrilium-1.1.4/pytrilium/PyTriliumCalendarClient.py`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/pytrilium/PyTriliumClient.py` & `pytrilium-1.1.4/pytrilium/PyTriliumClient.py`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/pytrilium/PyTriliumCustomClient.py` & `pytrilium-1.1.4/pytrilium/PyTriliumCustomClient.py`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/pytrilium/PyTriliumNoteClient.py` & `pytrilium-1.1.4/pytrilium/PyTriliumNoteClient.py`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/pytrilium/log.py` & `pytrilium-1.1.4/pytrilium/log.py`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/.gitignore` & `pytrilium-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/LICENSE` & `pytrilium-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/README.md` & `pytrilium-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pytrilium-1.1.3/pyproject.toml` & `pytrilium-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyTrilium"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="perfectra1n", email="perf3ctsec@gmail.com" },
 ]
 description = "A Python wrapper for the Trilium Notes API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pytrilium-1.1.3/PKG-INFO` & `pytrilium-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTrilium
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python wrapper for the Trilium Notes API
 Project-URL: Homepage, https://github.com/perfectra1n/pytrilium
 Project-URL: Bug Tracker, https://github.com/perfectra1n/pytrilium/issues
 Author-email: perfectra1n <perf3ctsec@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


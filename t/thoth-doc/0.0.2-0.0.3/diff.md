# Comparing `tmp/thoth_doc-0.0.2.tar.gz` & `tmp/thoth_doc-0.0.3.tar.gz`

## Comparing `thoth_doc-0.0.2.tar` & `thoth_doc-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    51725 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/Thoth.svg.png
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/src/thoth_doc/__init__.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/src/thoth_doc/main.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/LICENSE
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/README.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    51725 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/Thoth.svg.png
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/src/thoth_doc/__init__.py
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/src/thoth_doc/main.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/LICENSE
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/README.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/PKG-INFO
```

### Comparing `thoth_doc-0.0.2/Thoth.svg.png` & `thoth_doc-0.0.3/Thoth.svg.png`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.2/src/thoth_doc/main.py` & `thoth_doc-0.0.3/src/thoth_doc/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
     def __init__(self, docs_folder, compiled_docs_folder):
         self.docs_folder = docs_folder
         self.compiled_docs_folder = compiled_docs_folder
 
     def parse_file(self, filepath):
         compiled_markdown = ''
         cwd = os.getcwd()
-        print('cwd')
         base = filepath.replace(self.docs_folder, '')
 
         with open(filepath) as f:
             markdown = f.readlines()
 
         for line in markdown:
             matches = re.findall(RE_REFERENCE, line)
```

### Comparing `thoth_doc-0.0.2/LICENSE` & `thoth_doc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.2/pyproject.toml` & `thoth_doc-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thoth_doc"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Lev", email="smj510black@gmail.com" },
 ]
 description = "Dependency-free, lightweight docstring parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thoth_doc-0.0.2/PKG-INFO` & `thoth_doc-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoth_doc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dependency-free, lightweight docstring parser
 Project-URL: Homepage, https://github.com/mariownyou/thoth-doc
 Project-URL: Bug Tracker, https://github.com/mariownyou/thoth-doc/issues
 Author-email: Lev <smj510black@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


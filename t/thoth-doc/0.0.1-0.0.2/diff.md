# Comparing `tmp/thoth_doc-0.0.1.tar.gz` & `tmp/thoth_doc-0.0.2.tar.gz`

## Comparing `thoth_doc-0.0.1.tar` & `thoth_doc-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    51725 2020-02-02 00:00:00.000000 thoth_doc-0.0.1/Thoth.svg.png
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 thoth_doc-0.0.1/src/thoth_doc/__init__.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 thoth_doc-0.0.1/src/thoth_doc/main.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.1/LICENSE
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 thoth_doc-0.0.1/README.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 thoth_doc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 thoth_doc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    51725 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/Thoth.svg.png
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/src/thoth_doc/__init__.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/src/thoth_doc/main.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/LICENSE
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/README.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 thoth_doc-0.0.2/PKG-INFO
```

### Comparing `thoth_doc-0.0.1/Thoth.svg.png` & `thoth_doc-0.0.2/Thoth.svg.png`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.1/src/thoth_doc/main.py` & `thoth_doc-0.0.2/src/thoth_doc/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     def __init__(self, docs_folder, compiled_docs_folder):
         self.docs_folder = docs_folder
         self.compiled_docs_folder = compiled_docs_folder
 
     def parse_file(self, filepath):
         compiled_markdown = ''
         cwd = os.getcwd()
+        print('cwd')
         base = filepath.replace(self.docs_folder, '')
 
         with open(filepath) as f:
             markdown = f.readlines()
 
         for line in markdown:
             matches = re.findall(RE_REFERENCE, line)
@@ -114,15 +115,15 @@
             compiled_markdown += line
 
         with open(f'{cwd}/{self.compiled_docs_folder}{base}', 'w') as f:
             f.write(compiled_markdown)
 
     def create_folder_structure(self):
         cwd = os.getcwd()
-        os.makedirs(cwd + self.compiled_docs_folder, exist_ok=True)
+        os.makedirs(f'{cwd}/{self.compiled_docs_folder}', exist_ok=True)
 
         for root, dirs, files in os.walk(self.docs_folder):
             for dir in dirs:
                 path = f'{cwd}/{self.compiled_docs_folder}/{root.replace(self.docs_folder, "")}/{dir}'
                 os.makedirs(path, exist_ok=True)
 
     def generate(self):
```

### Comparing `thoth_doc-0.0.1/LICENSE` & `thoth_doc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.1/pyproject.toml` & `thoth_doc-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thoth_doc"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Lev", email="smj510black@gmail.com" },
 ]
 description = "Dependency-free, lightweight docstring parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thoth_doc-0.0.1/PKG-INFO` & `thoth_doc-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoth_doc
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dependency-free, lightweight docstring parser
 Project-URL: Homepage, https://github.com/mariownyou/thoth-doc
 Project-URL: Bug Tracker, https://github.com/mariownyou/thoth-doc/issues
 Author-email: Lev <smj510black@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


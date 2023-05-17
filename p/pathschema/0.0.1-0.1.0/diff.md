# Comparing `tmp/pathschema-0.0.1.tar.gz` & `tmp/pathschema-0.1.0.tar.gz`

## Comparing `pathschema-0.0.1.tar` & `pathschema-0.1.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pathschema-0.0.1/.pylintrc
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pathschema-0.0.1/requirements.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pathschema-0.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pathschema-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pathschema-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pathschema-0.0.1/pathschema/__init__.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 pathschema-0.0.1/pathschema/__main__.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pathschema-0.0.1/pathschema/exceptions.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 pathschema-0.0.1/pathschema/models.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 pathschema-0.0.1/pathschema/parser.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 pathschema-0.0.1/pathschema/utils.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 pathschema-0.0.1/pathschema/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/test_DirPathNode.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/test_FilePathNode.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/test_Parser.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/test_PathNode.py
--rw-r--r--   0        0        0    14023 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/test_Validator.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/.gitignore
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/generate_massive.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_invalid_schema.txt
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_schema.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_fail/Assets/CommunityAssets/sdfasdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_fail/Assets/Globals/Materials/brick.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_fail/Assets/Globals/Materials/water.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_fail/Assets/Globals/Textures/robot.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_fail/Assets/Notes.md/this should not be evaluated
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/not_allowed.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/Materials/solid_metal.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/Textures/body.jpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_fail/Assets/Scenes/test.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_fail/Assets/Scenes/level1/first.unity
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Notes.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/CommunityAssets/sdfasdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Globals/Materials/solid_brick.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Globals/Materials/trans_water.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Globals/Textures/robot.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/model.fbx
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/solid_material.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/texture.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/Materials/solid_metal.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/Textures/body.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.0.1/tests/experimentations/test_directory_ok/Assets/Scenes/level1/first.unity
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pathschema-0.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pathschema-0.0.1/LICENSE
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 pathschema-0.0.1/README.md
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 pathschema-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 pathschema-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pathschema-0.1.0/.pylintrc
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pathschema-0.1.0/requirements.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pathschema-0.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pathschema-0.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pathschema-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pathschema-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/__main__.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/exceptions.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/models.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/parser.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/utils.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/test_DirPathNode.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/test_FilePathNode.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/test_Parser.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/test_PathNode.py
+-rw-r--r--   0        0        0    14023 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/test_Validator.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/.gitignore
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/generate_massive.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_invalid_schema.txt
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_schema.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/CommunityAssets/sdfasdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Globals/Materials/brick.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Globals/Materials/water.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Globals/Textures/robot.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Notes.md/this should not be evaluated
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/not_allowed.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/Materials/solid_metal.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/Textures/body.jpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Scenes/test.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Scenes/level1/first.unity
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Notes.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/CommunityAssets/sdfasdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Globals/Materials/solid_brick.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Globals/Materials/trans_water.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Globals/Textures/robot.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/model.fbx
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/solid_material.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/texture.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/Materials/solid_metal.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/Textures/body.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Scenes/level1/first.unity
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pathschema-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pathschema-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pathschema-0.1.0/README.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pathschema-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 pathschema-0.1.0/PKG-INFO
```

### Comparing `pathschema-0.0.1/.github/workflows/build.yml` & `pathschema-0.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/.github/workflows/publish.yml` & `pathschema-0.1.0/.github/workflows/publish.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+name: Publish to PyPi
+
 on:
   workflow_dispatch:
 
 jobs:
   upload:
     name: Upload Package
     runs-on: ubuntu-latest
```

### Comparing `pathschema-0.0.1/pathschema/__main__.py` & `pathschema-0.1.0/pathschema/__main__.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/pathschema/models.py` & `pathschema-0.1.0/pathschema/models.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/pathschema/parser.py` & `pathschema-0.1.0/pathschema/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 	"""Parses the path schema definition"""
 
 	indentation_token = '\t'
 	directory_token = '/'
 	required_token = '+'
 	forbidden_token = '-'
 	any_token = '...'
+	comment_token = '#'
 
 	def _detect_indentation(self):
 		raise NotImplementedError()
 
 	def _indentation_count(self,  string: str):
 		num_of_indentation = 0
 		for character in string:
@@ -37,14 +38,18 @@
 
 		for line_num, line in enumerate(schema.split('\n')):
 			indentation = self._indentation_count(line)
 			name = line.strip()
 			if len(name) == 0:
 				continue
 
+			# comments get ignored
+			if name.startswith(self.comment_token):
+				continue
+
 			# add node
 			if indentation == node_depth:
 				pass
 
 			# dive in
 			elif indentation > node_depth:
```

### Comparing `pathschema-0.0.1/pathschema/utils.py` & `pathschema-0.1.0/pathschema/utils.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/pathschema/validator.py` & `pathschema-0.1.0/pathschema/validator.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/tests/test_DirPathNode.py` & `pathschema-0.1.0/tests/test_DirPathNode.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/tests/test_Parser.py` & `pathschema-0.1.0/tests/test_Parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,7 +133,24 @@
 				.add_child(FilePathNode(name='*.md', necessity=Necessity.REQUIRED))
 			)
 
 		print_node_tree(expected_tree)
 		print_node_tree(returned_tree)
 
 		self.assertEqual(expected_tree, returned_tree)
+
+	def test_schema_to_node_comment_ignored_pass(self):
+		schema =  'Assets/\n'
+		schema += '\t# comment!\n'
+		schema += '\t*.txt\n'
+		
+		returned_tree = Parser().schema_to_node_tree(schema)
+
+		expected_tree = DirPathNode(name='schema_root') \
+			.add_child(DirPathNode(name='Assets')
+				.add_child(FilePathNode(name='*.txt'))
+			)
+
+		print_node_tree(expected_tree)
+		print_node_tree(returned_tree)
+
+		self.assertEqual(expected_tree, returned_tree)
```

### Comparing `pathschema-0.0.1/tests/test_PathNode.py` & `pathschema-0.1.0/tests/test_PathNode.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/tests/test_Validator.py` & `pathschema-0.1.0/tests/test_Validator.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/tests/experimentations/generate_massive.py` & `pathschema-0.1.0/tests/experimentations/generate_massive.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/.gitignore` & `pathschema-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/LICENSE` & `pathschema-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathschema-0.0.1/README.md` & `pathschema-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # Path Schema
 
+![PyPi Version](https://img.shields.io/pypi/v/pathschema.svg) ![PyPI Python Version](https://img.shields.io/pypi/pyversions/pathschema.svg?logo=python&logoColor=gold) ![License MIT](https://img.shields.io/pypi/l/pathschema)
+
 ```bash
 pip install pathschema
 ```
 
 # How to use
 
 ```python
 from pathschema import validate
 
-schema = ""
+schema = ''
 
 path_to_validate = './path'
 
 with open('path/to/schema.txt', 'r') as f:
 	schema = f.read()
 
 result = validate(path_to_validate, schema)
```

### Comparing `pathschema-0.0.1/PKG-INFO` & `pathschema-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 Metadata-Version: 2.1
 Name: pathschema
-Version: 0.0.1
+Version: 0.1.0
 Summary: Standardize and plan out a file structure!
 Project-URL: Source, https://github.com/Apollo-Roboto/python-pathschema
 Author-email: Apollo-Roboto <Apollo_Roboto@outlook.com>
 License-Expression: MIT
 License-File: LICENSE
+Keywords: Directory,File,File System,Folder,Schema,Validation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: colorama==0.4.6
-Requires-Dist: pylint==2.17.4
 Description-Content-Type: text/markdown
 
 # Path Schema
 
+![PyPi Version](https://img.shields.io/pypi/v/pathschema.svg) ![PyPI Python Version](https://img.shields.io/pypi/pyversions/pathschema.svg?logo=python&logoColor=gold) ![License MIT](https://img.shields.io/pypi/l/pathschema)
+
 ```bash
 pip install pathschema
 ```
 
 # How to use
 
 ```python
 from pathschema import validate
 
-schema = ""
+schema = ''
 
 path_to_validate = './path'
 
 with open('path/to/schema.txt', 'r') as f:
 	schema = f.read()
 
 result = validate(path_to_validate, schema)
```


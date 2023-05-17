# Comparing `tmp/scale_json_binary-0.0.4.tar.gz` & `tmp/scale_json_binary-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_json_binary-0.0.4.tar", max compression
+gzip compressed data, was "scale_json_binary-0.0.5.tar", max compression
```

## Comparing `scale_json_binary-0.0.4.tar` & `scale_json_binary-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       71 2023-04-04 16:45:17.105041 scale_json_binary-0.0.4/README.md
--rw-r--r--   0        0        0      660 2023-04-04 16:47:55.828928 scale_json_binary-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       98 2023-03-29 20:56:32.931581 scale_json_binary-0.0.4/scale_json_binary/__init__.py
--rw-r--r--   0        0        0     3939 2023-03-29 20:56:32.931581 scale_json_binary-0.0.4/scale_json_binary/json_binary_codecs.py
--rw-r--r--   0        0        0        0 2023-03-29 20:56:32.931581 scale_json_binary-0.0.4/scale_json_binary/py.typed
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 scale_json_binary-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-04-04 17:04:54.683642 scale_json_binary-0.0.5/README.md
+-rw-r--r--   0        0        0      743 2023-04-04 17:09:36.647242 scale_json_binary-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-03-29 20:56:32.931581 scale_json_binary-0.0.5/scale_json_binary/__init__.py
+-rw-r--r--   0        0        0     3939 2023-03-29 20:56:32.931581 scale_json_binary-0.0.5/scale_json_binary/json_binary_codecs.py
+-rw-r--r--   0        0        0        0 2023-03-29 20:56:32.931581 scale_json_binary-0.0.5/scale_json_binary/py.typed
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 scale_json_binary-0.0.5/PKG-INFO
```

### Comparing `scale_json_binary-0.0.4/pyproject.toml` & `scale_json_binary-0.0.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [tool.poetry]
 name = "scale-json-binary"
-version = "0.0.4"
+version = "0.0.5"
 description = "Codecs for json binary spec"
-authors = ["Michael Choi <michael.choi@scale.com>"]
+authors = [
+    "Michael Choi <michael.choi@scale.com>",
+    "Rodrigo Belfiore <rodrigo.belfiore@scale.com>"
+]
 readme = "README.md"
 packages = [{include = "scale_json_binary"}]
+exclude = ["internal/"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = ">=1.22.4"
 ujson = ">=5.7.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `scale_json_binary-0.0.4/scale_json_binary/json_binary_codecs.py` & `scale_json_binary-0.0.5/scale_json_binary/json_binary_codecs.py`

 * *Files identical despite different names*

### Comparing `scale_json_binary-0.0.4/PKG-INFO` & `scale_json_binary-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-json-binary
-Version: 0.0.4
+Version: 0.0.5
 Summary: Codecs for json binary spec
 Author: Michael Choi
 Author-email: michael.choi@scale.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/piicli-0.0.2.tar.gz` & `tmp/piicli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piicli-0.0.2.tar", max compression
+gzip compressed data, was "piicli-0.0.3.tar", max compression
```

## Comparing `piicli-0.0.2.tar` & `piicli-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-16 09:44:17.758376 piicli-0.0.2/LICENSE
--rw-r--r--   0        0        0      170 2023-05-16 09:44:41.423465 piicli-0.0.2/README.md
--rw-r--r--   0        0        0      719 2023-05-17 12:26:00.167399 piicli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 11:11:21.834362 piicli-0.0.2/src/piicli/__init__.py
--rw-r--r--   0        0        0     4552 2023-05-17 12:22:45.339270 piicli-0.0.2/src/piicli/main.py
--rw-r--r--   0        0        0      331 2023-05-17 10:39:02.171793 piicli-0.0.2/src/piicli/utils.py
--rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 piicli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 09:44:17.758376 piicli-0.0.3/LICENSE
+-rw-r--r--   0        0        0      170 2023-05-16 09:44:41.423465 piicli-0.0.3/README.md
+-rw-r--r--   0        0        0      718 2023-05-17 12:38:00.283642 piicli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 11:11:21.834362 piicli-0.0.3/src/piicli/__init__.py
+-rw-r--r--   0        0        0     4552 2023-05-17 12:38:00.287681 piicli-0.0.3/src/piicli/main.py
+-rw-r--r--   0        0        0      331 2023-05-17 10:39:02.171793 piicli-0.0.3/src/piicli/utils.py
+-rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 piicli-0.0.3/PKG-INFO
```

### Comparing `piicli-0.0.2/LICENSE` & `piicli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `piicli-0.0.2/pyproject.toml` & `piicli-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "piicli"
-version = "0.0.2"
+version = "0.0.3"
 authors = ["Shubham Dogra <shubham.dogra@pingsafe.com>"]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -19,13 +19,13 @@
 [tool.poetry.dependencies]
 PyYAML = "^6.0"
 boto3 = "^1.26.135"
 requests = "^2.30.0"
 
 
 [tool.poetry.scripts]
-piicli = "piicli.main:execute_binary`"
+piicli = "piicli.main:execute_binary"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `piicli-0.0.2/src/piicli/main.py` & `piicli-0.0.3/src/piicli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 #         os.chmod(binary_path, 0o755)
 #         subprocess.run(binary_path)
 #
 #     except Exception as e:
 #         print(f"Something went wrong, err: {e}")
 
 def print_version():
-    print("running 0.0.1")
+    print("running 0.0.3")
 
 
 def execute_binary():
     try:
         home = os.getenv("HOME")
         metadata_dir = home + "/piicli_metadata"
         config_file = "conf.yaml"
```

### Comparing `piicli-0.0.2/PKG-INFO` & `piicli-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piicli
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author: Shubham Dogra
 Author-email: shubham.dogra@pingsafe.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```


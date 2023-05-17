# Comparing `tmp/piicli-0.0.8.tar.gz` & `tmp/piicli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piicli-0.0.8.tar", max compression
+gzip compressed data, was "piicli-0.0.9.tar", max compression
```

## Comparing `piicli-0.0.8.tar` & `piicli-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-16 09:44:17.758376 piicli-0.0.8/LICENSE
--rw-r--r--   0        0        0      170 2023-05-16 09:44:41.423465 piicli-0.0.8/README.md
--rw-r--r--   0        0        0      711 2023-05-17 13:55:05.625845 piicli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 11:11:21.834362 piicli-0.0.8/src/piicli/__init__.py
--rw-r--r--   0        0        0     4784 2023-05-17 13:55:05.629775 piicli-0.0.8/src/piicli/main.py
--rw-r--r--   0        0        0      331 2023-05-17 10:39:02.171793 piicli-0.0.8/src/piicli/utils.py
--rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 piicli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 09:44:17.758376 piicli-0.0.9/LICENSE
+-rw-r--r--   0        0        0      170 2023-05-16 09:44:41.423465 piicli-0.0.9/README.md
+-rw-r--r--   0        0        0      711 2023-05-17 13:59:49.375218 piicli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 11:11:21.834362 piicli-0.0.9/src/piicli/__init__.py
+-rw-r--r--   0        0        0     4784 2023-05-17 13:59:44.329423 piicli-0.0.9/src/piicli/main.py
+-rw-r--r--   0        0        0      331 2023-05-17 10:39:02.171793 piicli-0.0.9/src/piicli/utils.py
+-rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 piicli-0.0.9/PKG-INFO
```

### Comparing `piicli-0.0.8/LICENSE` & `piicli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `piicli-0.0.8/pyproject.toml` & `piicli-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "piicli"
-version = "0.0.8"
+version = "0.0.9"
 authors = ["Shubham Dogra <shubham.dogra@pingsafe.com>"]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `piicli-0.0.8/src/piicli/main.py` & `piicli-0.0.9/src/piicli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 
 def run_cli():
     try:
         package_name = "piicli"
         binary_name = "secrets"
         pre_execution_workflow(package_name, binary_name)
-        print("Running main cli, version: 0.0.8")
+        print("Running main cli, version: 0.0.9")
         execute_binary(package_name, binary_name)
     except Exception as e:
         print(e)
 
 
 if __name__ == '__main__':
     run_cli()
```

### Comparing `piicli-0.0.8/PKG-INFO` & `piicli-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piicli
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author: Shubham Dogra
 Author-email: shubham.dogra@pingsafe.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```


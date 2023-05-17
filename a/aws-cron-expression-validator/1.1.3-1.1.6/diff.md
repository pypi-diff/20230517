# Comparing `tmp/aws_cron_expression_validator-1.1.3.tar.gz` & `tmp/aws_cron_expression_validator-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/aws_cron_expression_validator/aws_cron_expression_validator/dist/.tmp-g0zfnplo/aws_cron_expression_validator-", last modified: Wed May 17 04:53:15 2023, max compression
+gzip compressed data, was "/home/runner/work/aws_cron_expression_validator/aws_cron_expression_validator/dist/.tmp-q3f1_72m/aws_cron_expression_validator-", last modified: Wed May 17 07:09:49 2023, max compression
```

## Comparing `aws_cron_expression_validator-1.1.3.tar` & `aws_cron_expression_validator-1.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:09:49.000000 aws_cron_expression_validator-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-17 07:09:21.000000 aws_cron_expression_validator-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-17 07:09:49.000000 aws_cron_expression_validator-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 07:09:21.000000 aws_cron_expression_validator-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-17 07:09:21.000000 aws_cron_expression_validator-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:09:49.000000 aws_cron_expression_validator-1.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:09:49.000000 aws_cron_expression_validator-1.1.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:09:21.000000 aws_cron_expression_validator-1.1.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:09:49.000000 aws_cron_expression_validator-1.1.6/src/aws_cron_expression_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:09:21.000000 aws_cron_expression_validator-1.1.6/src/aws_cron_expression_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-17 07:09:21.000000 aws_cron_expression_validator-1.1.6/src/aws_cron_expression_validator/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:09:49.000000 aws_cron_expression_validator-1.1.6/src/aws_cron_expression_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-17 07:09:49.000000 aws_cron_expression_validator-1.1.6/src/aws_cron_expression_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 07:09:49.000000 aws_cron_expression_validator-1.1.6/src/aws_cron_expression_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:09:49.000000 aws_cron_expression_validator-1.1.6/src/aws_cron_expression_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 07:09:49.000000 aws_cron_expression_validator-1.1.6/src/aws_cron_expression_validator.egg-info/top_level.txt
```

### Comparing `aws_cron_expression_validator-1.1.3/LICENSE` & `aws_cron_expression_validator-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_cron_expression_validator-1.1.3/PKG-INFO` & `aws_cron_expression_validator-1.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: aws_cron_expression_validator
-Version: 1.1.3
+Version: 1.1.6
 Summary: ValidatesAWS EventBridge cron expressions, which are similar to, but not compatible with Unix style cron expressions
 Author-email: Graham Coster <bitjugglers@gmail.com>
 Project-URL: Homepage, https://github.com/grumBit/aws_cron_expression_validator.git
 Project-URL: Bug Tracker, https://github.com/grumBit/aws_cron_expression_validator/issues
 Project-URL: Source, https://github.com/grumBit/aws_cron_expression_validator
 Project-URL: Security Policy, https://github.com/grumbit/aws_cron_expression_validator/blob/master/.github/SECURITY.md
+Project-URL: Release Notes, https://github.com/grumBit/aws_cron_expression_validator/blob/master/RELEASENOTES.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aws_cron_expression_validator-1.1.3/README.md` & `aws_cron_expression_validator-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aws_cron_expression_validator-1.1.3/pyproject.toml` & `aws_cron_expression_validator-1.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_cron_expression_validator"
-version = "1.1.3"
+version = "1.1.6"
 authors = [
   { name="Graham Coster", email="bitjugglers@gmail.com" },
 ]
 description = "ValidatesAWS EventBridge cron expressions, which are similar to, but not compatible with Unix style cron expressions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,14 +19,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/grumBit/aws_cron_expression_validator.git"
 "Bug Tracker" = "https://github.com/grumBit/aws_cron_expression_validator/issues"
 "Source" = "https://github.com/grumBit/aws_cron_expression_validator"
 "Security Policy" = "https://github.com/grumbit/aws_cron_expression_validator/blob/master/.github/SECURITY.md"
+"Release Notes" = "https://github.com/grumBit/aws_cron_expression_validator/blob/master/RELEASENOTES.md"
 
 [tool.pytest.ini_options]
 addopts = "--cov-report html --cov-report term-missing --cov-fail-under 95"
 
 [tool.coverage.run]
 source = ["src"]
```

### Comparing `aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator/validator.py` & `aws_cron_expression_validator-1.1.6/src/aws_cron_expression_validator/validator.py`

 * *Files identical despite different names*

### Comparing `aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/PKG-INFO` & `aws_cron_expression_validator-1.1.6/src/aws_cron_expression_validator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: aws-cron-expression-validator
-Version: 1.1.3
+Version: 1.1.6
 Summary: ValidatesAWS EventBridge cron expressions, which are similar to, but not compatible with Unix style cron expressions
 Author-email: Graham Coster <bitjugglers@gmail.com>
 Project-URL: Homepage, https://github.com/grumBit/aws_cron_expression_validator.git
 Project-URL: Bug Tracker, https://github.com/grumBit/aws_cron_expression_validator/issues
 Project-URL: Source, https://github.com/grumBit/aws_cron_expression_validator
 Project-URL: Security Policy, https://github.com/grumbit/aws_cron_expression_validator/blob/master/.github/SECURITY.md
+Project-URL: Release Notes, https://github.com/grumBit/aws_cron_expression_validator/blob/master/RELEASENOTES.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


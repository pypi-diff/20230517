# Comparing `tmp/aws_cron_expression_validator-1.1.2.tar.gz` & `tmp/aws_cron_expression_validator-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/aws_cron_expression_validator/aws_cron_expression_validator/dist/.tmp-_ohzvamu/aws_cron_expression_validator-", last modified: Sun May 14 23:42:02 2023, max compression
+gzip compressed data, was "/home/runner/work/aws_cron_expression_validator/aws_cron_expression_validator/dist/.tmp-g0zfnplo/aws_cron_expression_validator-", last modified: Wed May 17 04:53:15 2023, max compression
```

## Comparing `aws_cron_expression_validator-1.1.2.tar` & `aws_cron_expression_validator-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-17 04:52:57.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 04:53:15.000000 aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/top_level.txt
```

### Comparing `aws_cron_expression_validator-1.1.2/LICENSE` & `aws_cron_expression_validator-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_cron_expression_validator-1.1.2/PKG-INFO` & `aws_cron_expression_validator-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_cron_expression_validator
-Version: 1.1.2
+Version: 1.1.3
 Summary: ValidatesAWS EventBridge cron expressions, which are similar to, but not compatible with Unix style cron expressions
 Author-email: Graham Coster <bitjugglers@gmail.com>
 Project-URL: Homepage, https://github.com/grumBit/aws_cron_expression_validator.git
 Project-URL: Bug Tracker, https://github.com/grumBit/aws_cron_expression_validator/issues
 Project-URL: Source, https://github.com/grumBit/aws_cron_expression_validator
 Project-URL: Security Policy, https://github.com/grumbit/aws_cron_expression_validator/blob/master/.github/SECURITY.md
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aws_cron_expression_validator-1.1.2/README.md` & `aws_cron_expression_validator-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aws_cron_expression_validator-1.1.2/pyproject.toml` & `aws_cron_expression_validator-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_cron_expression_validator"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Graham Coster", email="bitjugglers@gmail.com" },
 ]
 description = "ValidatesAWS EventBridge cron expressions, which are similar to, but not compatible with Unix style cron expressions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator/validator.py` & `aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     minute_values = r"(0?[0-9]|[1-5][0-9])"  # [0]0-59
     hour_values = r"(0?[0-9]|1[0-9]|2[0-3])"  # [0]0-23
     month_of_day_values = r"(0?[1-9]|[1-2][0-9]|3[0-1])"  # [0]1-31
     month_values = r"(0?[1-9]|1[0-2]|JAN|FEB|MAR|APR|MAY|JUN|JUL|AUG|SEP|OCT|NOV|DEC)"  # [0]1-12 or JAN-DEC
     day_of_week_values = r"([1-7]|SUN|MON|TUE|WED|THU|FRI|SAT)"  # 1-7 or SAT-SUN
     day_of_week_hash = rf"({day_of_week_values}#[1-5])"  # Day of the week in the Nth week of the month
     year_values = r"((19[7-9][0-9])|(2[0-1][0-9][0-9]))"  # 1970-2199
+    natural_number = r"([0-9]*[1-9][0-9]*)"  # Integers greater than 0
 
     @classmethod
     def validate(cls, expression: str) -> str:
 
         value_count = len(expression.split(" "))
         if value_count != 6:
             raise AWSCronExpressionError(
@@ -96,16 +97,16 @@
     def list_regex(cls, values: str) -> str:
         range_ = cls.range_regex(values)
         return rf"({range_}(\,{range_})*)"  # One or more ranges separated by a comma
 
     @classmethod
     def slash_regex(cls, values: str) -> str:
         range_ = cls.range_regex(values)
-        return rf"((\*|{range_}|{values})\/[0-9]*[1-9][0-9]*)"
-        # Slash can be preceded by *, range, or a valid value and must be followed by an natural
+        return rf"((\*|{range_}|{values})\/{cls.natural_number})"
+        # Slash can be preceded by *, range, or a valid value and must be followed by a natural
         # number as the increment.
 
     @classmethod
     def common_regex(cls, values: str) -> str:
         return rf"({cls.list_regex(values)}|\*|{cls.slash_regex(values)})"  # values , - * /
 
     @classmethod
@@ -128,8 +129,8 @@
 
     @classmethod
     def day_of_week_regex(cls):
         return rf"^({cls.list_regex(cls.day_of_week_values)}|\*|\?|L|{cls.day_of_week_hash})$"  # values , - * ? L #
 
     @classmethod
     def year_regex(cls):
-        return rf"^({cls.common_regex(cls.year_values)}|\?|L)$"  # values , - * /
+        return rf"^({cls.common_regex(cls.year_values)})$"  # values , - * /
```

### Comparing `aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/PKG-INFO` & `aws_cron_expression_validator-1.1.3/src/aws_cron_expression_validator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cron-expression-validator
-Version: 1.1.2
+Version: 1.1.3
 Summary: ValidatesAWS EventBridge cron expressions, which are similar to, but not compatible with Unix style cron expressions
 Author-email: Graham Coster <bitjugglers@gmail.com>
 Project-URL: Homepage, https://github.com/grumBit/aws_cron_expression_validator.git
 Project-URL: Bug Tracker, https://github.com/grumBit/aws_cron_expression_validator/issues
 Project-URL: Source, https://github.com/grumBit/aws_cron_expression_validator
 Project-URL: Security Policy, https://github.com/grumbit/aws_cron_expression_validator/blob/master/.github/SECURITY.md
 Classifier: Development Status :: 5 - Production/Stable
```


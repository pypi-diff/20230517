# Comparing `tmp/dbt_coverage-0.3.3.tar.gz` & `tmp/dbt_coverage-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_coverage-0.3.3.tar", max compression
+gzip compressed data, was "dbt_coverage-0.3.4.tar", max compression
```

## Comparing `dbt_coverage-0.3.3.tar` & `dbt_coverage-0.3.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2021-11-22 15:44:35.000000 dbt_coverage-0.3.3/LICENSE.md
--rw-r--r--   0        0        0    11594 2022-11-21 18:01:55.219725 dbt_coverage-0.3.3/README.md
--rw-r--r--   0        0        0    32417 2023-04-20 11:34:06.923234 dbt_coverage-0.3.3/dbt_coverage/__init__.py
--rw-r--r--   0        0        0     1194 2023-04-20 11:48:46.212663 dbt_coverage-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    12968 1970-01-01 00:00:00.000000 dbt_coverage-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2021-11-22 15:44:35.000000 dbt_coverage-0.3.4/LICENSE.md
+-rw-r--r--   0        0        0    11594 2023-05-17 08:36:29.600016 dbt_coverage-0.3.4/README.md
+-rw-r--r--   0        0        0    32527 2023-05-17 08:36:29.600437 dbt_coverage-0.3.4/dbt_coverage/__init__.py
+-rw-r--r--   0        0        0     1194 2023-05-17 08:36:29.600709 dbt_coverage-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    12968 1970-01-01 00:00:00.000000 dbt_coverage-0.3.4/PKG-INFO
```

### Comparing `dbt_coverage-0.3.3/LICENSE.md` & `dbt_coverage-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt_coverage-0.3.3/README.md` & `dbt_coverage-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 Different version of `dbt-coverage` support different versions of `dbt`. Here is
 the support matrix.
 
 | `dbt`       | `dbt-coverage` |
 |-------------|----------------|
 | <0.20       | not tested     |
 | 0.20 - 0.21 | 0.1            |
-| 1.0 - 1.3   | 0.2, 0.3       |
+| 1.0 - 1.5   | 0.2, 0.3       |
 
 ## Related packages
 
 - https://github.com/mikaelene/dbt-test-coverage
 - [interrogate](https://interrogate.readthedocs.io/en/latest/) (docs coverage for Python)
 - [coverage.py](https://github.com/nedbat/coveragepy) (execution coverage for Python)
```

#### html2text {}

```diff
@@ -118,15 +118,15 @@
 changed models $ dbt docs generate # Generate catalog.json and manifest.json $
 dbt-coverage compute doc --cov-report after.json --cov-fail-compare before.json
 # Fail if the current coverage is lower than coverage in before.json $ dbt-
 coverage compare after.json before.json # Generate a detailed coverage delta
 report ``` ## Supported `dbt` versions Different version of `dbt-coverage`
 support different versions of `dbt`. Here is the support matrix. | `dbt` |
 `dbt-coverage` | |-------------|----------------| | <0.20 | not tested | | 0.20
-- 0.21 | 0.1 | | 1.0 - 1.3 | 0.2, 0.3 | ## Related packages - https://
+- 0.21 | 0.1 | | 1.0 - 1.5 | 0.2, 0.3 | ## Related packages - https://
 github.com/mikaelene/dbt-test-coverage - [interrogate](https://
 interrogate.readthedocs.io/en/latest/) (docs coverage for Python) -
 [coverage.py](https://github.com/nedbat/coveragepy) (execution coverage for
 Python) ## License Licensed under the MIT license (see [LICENSE.md](LICENSE.md)
 file for more details). [![FOSSA Status](https://app.fossa.com/api/projects/
 git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=large)](https://
 app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-
```

### Comparing `dbt_coverage-0.3.3/dbt_coverage/__init__.py` & `dbt_coverage-0.3.4/dbt_coverage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 
 SUPPORTED_MANIFEST_SCHEMA_VERSIONS = [
     "https://schemas.getdbt.com/dbt/manifest/v4.json",
     "https://schemas.getdbt.com/dbt/manifest/v5.json",
     "https://schemas.getdbt.com/dbt/manifest/v6.json",
     "https://schemas.getdbt.com/dbt/manifest/v7.json",
+    "https://schemas.getdbt.com/dbt/manifest/v8.json",
+    "https://schemas.getdbt.com/dbt/manifest/v9.json",
 ]
 
 app = typer.Typer(help="Compute coverage of dbt-managed data warehouses.")
 
 
 class CoverageType(Enum):
     DOC = "doc"
```

### Comparing `dbt_coverage-0.3.3/pyproject.toml` & `dbt_coverage-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-coverage"
-version = "0.3.3"
+version = "0.3.4"
 description = "One-stop-shop for docs and test coverage of dbt projects"
 authors = ["Andrej Švec <asvec@slido.com>"]
 readme = 'README.md'
 license = "MIT"
 repository = "https://github.com/slidoapp/dbt-coverage"
 homepage = "https://github.com/slidoapp/dbt-coverage"
 documentation = "https://github.com/slidoapp/dbt-coverage"
```

### Comparing `dbt_coverage-0.3.3/PKG-INFO` & `dbt_coverage-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-coverage
-Version: 0.3.3
+Version: 0.3.4
 Summary: One-stop-shop for docs and test coverage of dbt projects
 Home-page: https://github.com/slidoapp/dbt-coverage
 License: MIT
 Author: Andrej Švec
 Author-email: asvec@slido.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -255,15 +255,15 @@
 Different version of `dbt-coverage` support different versions of `dbt`. Here is
 the support matrix.
 
 | `dbt`       | `dbt-coverage` |
 |-------------|----------------|
 | <0.20       | not tested     |
 | 0.20 - 0.21 | 0.1            |
-| 1.0 - 1.3   | 0.2, 0.3       |
+| 1.0 - 1.5   | 0.2, 0.3       |
 
 ## Related packages
 
 - https://github.com/mikaelene/dbt-test-coverage
 - [interrogate](https://interrogate.readthedocs.io/en/latest/) (docs coverage for Python)
 - [coverage.py](https://github.com/nedbat/coveragepy) (execution coverage for Python)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-coverage Version: 0.3.3 Summary: One-stop-shop
+Metadata-Version: 2.1 Name: dbt-coverage Version: 0.3.4 Summary: One-stop-shop
 for docs and test coverage of dbt projects Home-page: https://github.com/
 slidoapp/dbt-coverage License: MIT Author: Andrej Å vec Author-email:
 asvec@slido.com Requires-Python: >=3.6,<4.0 Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
@@ -136,15 +136,15 @@
 changed models $ dbt docs generate # Generate catalog.json and manifest.json $
 dbt-coverage compute doc --cov-report after.json --cov-fail-compare before.json
 # Fail if the current coverage is lower than coverage in before.json $ dbt-
 coverage compare after.json before.json # Generate a detailed coverage delta
 report ``` ## Supported `dbt` versions Different version of `dbt-coverage`
 support different versions of `dbt`. Here is the support matrix. | `dbt` |
 `dbt-coverage` | |-------------|----------------| | <0.20 | not tested | | 0.20
-- 0.21 | 0.1 | | 1.0 - 1.3 | 0.2, 0.3 | ## Related packages - https://
+- 0.21 | 0.1 | | 1.0 - 1.5 | 0.2, 0.3 | ## Related packages - https://
 github.com/mikaelene/dbt-test-coverage - [interrogate](https://
 interrogate.readthedocs.io/en/latest/) (docs coverage for Python) -
 [coverage.py](https://github.com/nedbat/coveragepy) (execution coverage for
 Python) ## License Licensed under the MIT license (see [LICENSE.md](LICENSE.md)
 file for more details). [![FOSSA Status](https://app.fossa.com/api/projects/
 git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=large)](https://
 app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-
```


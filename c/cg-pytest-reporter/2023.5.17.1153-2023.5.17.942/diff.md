# Comparing `tmp/cg_pytest_reporter-2023.5.17.1153.tar.gz` & `tmp/cg_pytest_reporter-2023.5.17.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_pytest_reporter-2023.5.17.1153.tar", max compression
+gzip compressed data, was "cg_pytest_reporter-2023.5.17.942.tar", max compression
```

## Comparing `cg_pytest_reporter-2023.5.17.1153.tar` & `cg_pytest_reporter-2023.5.17.942.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       21 2023-05-17 11:53:07.524460 cg_pytest_reporter-2023.5.17.1153/README.md
--rw-r--r--   0        0        0      422 2023-05-17 11:53:07.524460 cg_pytest_reporter-2023.5.17.1153/cg_pytest_reporter/__init__.py
--rw-r--r--   0        0        0    17620 2023-05-17 11:53:07.524460 cg_pytest_reporter-2023.5.17.1153/cg_pytest_reporter/plugin.py
--rw-r--r--   0        0        0     1809 2023-05-17 11:53:30.873825 cg_pytest_reporter-2023.5.17.1153/pyproject.toml
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.17.1153/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-05-17 09:42:07.964449 cg_pytest_reporter-2023.5.17.942/README.md
+-rw-r--r--   0        0        0      422 2023-05-17 09:42:07.964449 cg_pytest_reporter-2023.5.17.942/cg_pytest_reporter/__init__.py
+-rw-r--r--   0        0        0    17620 2023-05-17 09:42:07.964449 cg_pytest_reporter-2023.5.17.942/cg_pytest_reporter/plugin.py
+-rw-r--r--   0        0        0     1810 2023-05-17 09:42:33.186790 cg_pytest_reporter-2023.5.17.942/pyproject.toml
+-rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.17.942/PKG-INFO
```

### Comparing `cg_pytest_reporter-2023.5.17.1153/cg_pytest_reporter/plugin.py` & `cg_pytest_reporter-2023.5.17.942/cg_pytest_reporter/plugin.py`

 * *Files identical despite different names*

### Comparing `cg_pytest_reporter-2023.5.17.1153/pyproject.toml` & `cg_pytest_reporter-2023.5.17.942/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "cg-pytest-reporter"
-version = "2023.05.17.1153"
+version = "2023.05.17.0942"
 description = ""
 authors = ["CodeGrade <info@codegrade.com>"]
 readme = "README.md"
 packages = [{include = "cg_pytest_reporter"}]
 
 [tool.poetry.plugins.pytest11]
 cg_pytest_reporter = "cg_pytest_reporter.plugin"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 pytest = ">=7.3.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 pylint = "^2.17.4"
 yapf = "^0.33.0"
 isort = "^5.12.0"
```


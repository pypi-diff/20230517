# Comparing `tmp/pyschlage-2023.4.2.tar.gz` & `tmp/pyschlage-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyschlage-2023.4.2.tar", last modified: Sun Apr 23 00:14:32 2023, max compression
+gzip compressed data, was "pyschlage-2023.5.0.tar", last modified: Wed May 17 12:58:16 2023, max compression
```

## Comparing `pyschlage-2023.4.2.tar` & `pyschlage-2023.5.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.064046 pyschlage-2023.4.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.064046 pyschlage-2023.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.064046 pyschlage-2023.4.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.064046 pyschlage-2023.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/pyschlage/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-23 00:14:31.000000 pyschlage-2023.4.2/pyschlage/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/code.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/pyschlage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-23 00:14:32.000000 pyschlage-2023.4.2/pyschlage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-23 00:14:32.000000 pyschlage-2023.4.2/pyschlage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:14:32.000000 pyschlage-2023.4.2/pyschlage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 00:14:32.000000 pyschlage-2023.4.2/pyschlage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 00:14:32.000000 pyschlage-2023.4.2/pyschlage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:14:31.000000 pyschlage-2023.4.2/pyschlage.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/scripts/setup
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:16.024805 pyschlage-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:16.020805 pyschlage-2023.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:16.020805 pyschlage-2023.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:16.020805 pyschlage-2023.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-17 12:58:16.024805 pyschlage-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:16.020805 pyschlage-2023.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:16.020805 pyschlage-2023.5.0/pyschlage/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyschlage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-17 12:58:15.000000 pyschlage-2023.5.0/pyschlage/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyschlage/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyschlage/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyschlage/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyschlage/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyschlage/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyschlage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyschlage/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyschlage/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/pyschlage/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:16.024805 pyschlage-2023.5.0/pyschlage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-17 12:58:15.000000 pyschlage-2023.5.0/pyschlage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-17 12:58:16.000000 pyschlage-2023.5.0/pyschlage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:58:15.000000 pyschlage-2023.5.0/pyschlage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 12:58:16.000000 pyschlage-2023.5.0/pyschlage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 12:58:16.000000 pyschlage-2023.5.0/pyschlage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:58:15.000000 pyschlage-2023.5.0/pyschlage.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:16.024805 pyschlage-2023.5.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/scripts/setup
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:58:16.024805 pyschlage-2023.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:16.024805 pyschlage-2023.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-17 12:57:59.000000 pyschlage-2023.5.0/tests/test_user.py
```

### Comparing `pyschlage-2023.4.2/.devcontainer.json` & `pyschlage-2023.5.0/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/.github/workflows/build-and-test.yml` & `pyschlage-2023.5.0/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/.github/workflows/publish-python.yml` & `pyschlage-2023.5.0/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/.gitignore` & `pyschlage-2023.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/.pre-commit-config.yaml` & `pyschlage-2023.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/LICENSE` & `pyschlage-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/PKG-INFO` & `pyschlage-2023.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschlage
-Version: 2023.4.2
+Version: 2023.5.0
 Summary: Python API for interacting with Schlage WiFi locks.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Project-URL: Documentation, https://pyschlage.readthedocs.io
```

### Comparing `pyschlage-2023.4.2/README.md` & `pyschlage-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/docs/Makefile` & `pyschlage-2023.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/docs/api.rst` & `pyschlage-2023.5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/docs/index.rst` & `pyschlage-2023.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/docs/make.bat` & `pyschlage-2023.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/pyproject.toml` & `pyschlage-2023.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/pyschlage/api.py` & `pyschlage-2023.5.0/pyschlage/api.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/pyschlage/auth.py` & `pyschlage-2023.5.0/pyschlage/auth.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/pyschlage/code.py` & `pyschlage-2023.5.0/pyschlage/code.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/pyschlage/common.py` & `pyschlage-2023.5.0/pyschlage/common.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/pyschlage/device.py` & `pyschlage-2023.5.0/pyschlage/device.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/pyschlage/lock.py` & `pyschlage-2023.5.0/pyschlage/lock.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/pyschlage/log.py` & `pyschlage-2023.5.0/pyschlage/log.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/pyschlage/user.py` & `pyschlage-2023.5.0/pyschlage/user.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/pyschlage.egg-info/PKG-INFO` & `pyschlage-2023.5.0/pyschlage.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschlage
-Version: 2023.4.2
+Version: 2023.5.0
 Summary: Python API for interacting with Schlage WiFi locks.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Project-URL: Documentation, https://pyschlage.readthedocs.io
```

### Comparing `pyschlage-2023.4.2/pyschlage.egg-info/SOURCES.txt` & `pyschlage-2023.5.0/pyschlage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/tests/conftest.py` & `pyschlage-2023.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/tests/test_auth.py` & `pyschlage-2023.5.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/tests/test_code.py` & `pyschlage-2023.5.0/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/tests/test_lock.py` & `pyschlage-2023.5.0/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.2/tests/test_log.py` & `pyschlage-2023.5.0/tests/test_log.py`

 * *Files identical despite different names*


# Comparing `tmp/pollination-honeybee-display-0.1.8.tar.gz` & `tmp/pollination-honeybee-display-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-honeybee-display-0.1.8.tar", last modified: Tue Jan 17 21:34:30 2023, max compression
+gzip compressed data, was "dist/pollination-honeybee-display-0.1.9.tar", last modified: Thu Jan 19 16:41:26 2023, max compression
```

## Comparing `pollination-honeybee-display-0.1.8.tar` & `pollination-honeybee-display-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 21:34:30.000000 pollination-honeybee-display-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 21:34:30.000000 pollination-honeybee-display-0.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 21:34:30.000000 pollination-honeybee-display-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-01-17 21:34:30.000000 pollination-honeybee-display-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 21:34:30.000000 pollination-honeybee-display-0.1.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 21:34:30.000000 pollination-honeybee-display-0.1.8/pollination/honeybee_display/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/pollination/honeybee_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/pollination/honeybee_display/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 21:34:30.000000 pollination-honeybee-display-0.1.8/pollination_honeybee_display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-01-17 21:34:29.000000 pollination-honeybee-display-0.1.8/pollination_honeybee_display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-17 21:34:29.000000 pollination-honeybee-display-0.1.8/pollination_honeybee_display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 21:34:29.000000 pollination-honeybee-display-0.1.8/pollination_honeybee_display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 21:33:41.000000 pollination-honeybee-display-0.1.8/pollination_honeybee_display.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-17 21:34:29.000000 pollination-honeybee-display-0.1.8/pollination_honeybee_display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-17 21:34:29.000000 pollination-honeybee-display-0.1.8/pollination_honeybee_display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-17 21:34:30.000000 pollination-honeybee-display-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 21:34:30.000000 pollination-honeybee-display-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-17 21:33:11.000000 pollination-honeybee-display-0.1.8/tests/translate_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/pollination/honeybee_display/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/pollination/honeybee_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/pollination/honeybee_display/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/pollination_honeybee_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/pollination_honeybee_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/pollination_honeybee_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/pollination_honeybee_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 16:40:33.000000 pollination-honeybee-display-0.1.9/pollination_honeybee_display.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/pollination_honeybee_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/pollination_honeybee_display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 16:41:26.000000 pollination-honeybee-display-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-19 16:39:48.000000 pollination-honeybee-display-0.1.9/tests/translate_test.py
```

### Comparing `pollination-honeybee-display-0.1.8/.github/workflows/ci.yaml` & `pollination-honeybee-display-0.1.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-display-0.1.8/.github/workflows/dependency-release.yaml` & `pollination-honeybee-display-0.1.9/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-display-0.1.8/LICENSE` & `pollination-honeybee-display-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-display-0.1.8/PKG-INFO` & `pollination-honeybee-display-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-display
-Version: 0.1.8
+Version: 0.1.9
 Summary: Plugin for Pollination with all honeybee extensions.
 Home-page: https://github.com/pollination/honeybee-display
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-honeybee-display-0.1.8/pollination/honeybee_display/translate.py` & `pollination-honeybee-display-0.1.9/pollination/honeybee_display/translate.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-display-0.1.8/pollination_honeybee_display.egg-info/PKG-INFO` & `pollination-honeybee-display-0.1.9/pollination_honeybee_display.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-display
-Version: 0.1.8
+Version: 0.1.9
 Summary: Plugin for Pollination with all honeybee extensions.
 Home-page: https://github.com/pollination/honeybee-display
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-honeybee-display-0.1.8/pollination_honeybee_display.egg-info/SOURCES.txt` & `pollination-honeybee-display-0.1.9/pollination_honeybee_display.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-display-0.1.8/setup.py` & `pollination-honeybee-display-0.1.9/setup.py`

 * *Files identical despite different names*


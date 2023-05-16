# Comparing `tmp/access_nri_intake-0.0.2.tar.gz` & `tmp/access_nri_intake-0.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_nri_intake-0.0.2.tar", last modified: Tue May 16 04:26:57 2023, max compression
+gzip compressed data, was "access_nri_intake-0.0.2.post1.tar", last modified: Tue May 16 04:41:18 2023, max compression
```

## Comparing `access_nri_intake-0.0.2.tar` & `access_nri_intake-0.0.2.post1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/access_nri_intake/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/access_nri_intake/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/access_nri_intake/esmcat/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/esmcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/esmcat/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/esmcat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/access_nri_intake/metacat/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/metacat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/metacat/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/metacat/translators.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/metacatalog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:18.616680 access_nri_intake-0.0.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-16 04:41:18.616680 access_nri_intake-0.0.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:41:18.616680 access_nri_intake-0.0.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:18.612680 access_nri_intake-0.0.2.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:18.616680 access_nri_intake-0.0.2.post1/src/access_nri_intake/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 04:41:18.616680 access_nri_intake-0.0.2.post1/src/access_nri_intake/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:18.616680 access_nri_intake-0.0.2.post1/src/access_nri_intake/esmcat/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake/esmcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake/esmcat/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake/esmcat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:18.616680 access_nri_intake-0.0.2.post1/src/access_nri_intake/metacat/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake/metacat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake/metacat/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake/metacat/translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake/metacatalog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:18.616680 access_nri_intake-0.0.2.post1/src/access_nri_intake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-16 04:41:18.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-16 04:41:18.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:41:18.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 04:41:18.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-16 04:41:18.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 04:41:18.000000 access_nri_intake-0.0.2.post1/src/access_nri_intake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-16 04:41:05.000000 access_nri_intake-0.0.2.post1/versioneer.py
```

### Comparing `access_nri_intake-0.0.2/LICENSE` & `access_nri_intake-0.0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/PKG-INFO` & `access_nri_intake-0.0.2.post1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access_nri_intake
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `access_nri_intake-0.0.2/pyproject.toml` & `access_nri_intake-0.0.2.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/src/access_nri_intake/cli.py` & `access_nri_intake-0.0.2.post1/src/access_nri_intake/cli.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/src/access_nri_intake/esmcat/__init__.py` & `access_nri_intake-0.0.2.post1/src/access_nri_intake/esmcat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/src/access_nri_intake/esmcat/builders.py` & `access_nri_intake-0.0.2.post1/src/access_nri_intake/esmcat/builders.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/src/access_nri_intake/esmcat/utils.py` & `access_nri_intake-0.0.2.post1/src/access_nri_intake/esmcat/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/src/access_nri_intake/metacat/__init__.py` & `access_nri_intake-0.0.2.post1/src/access_nri_intake/metacat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/src/access_nri_intake/metacat/manager.py` & `access_nri_intake-0.0.2.post1/src/access_nri_intake/metacat/manager.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/src/access_nri_intake/metacat/translators.py` & `access_nri_intake-0.0.2.post1/src/access_nri_intake/metacat/translators.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/src/access_nri_intake/utils.py` & `access_nri_intake-0.0.2.post1/src/access_nri_intake/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/src/access_nri_intake.egg-info/PKG-INFO` & `access_nri_intake-0.0.2.post1/src/access_nri_intake.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access-nri-intake
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `access_nri_intake-0.0.2/src/access_nri_intake.egg-info/SOURCES.txt` & `access_nri_intake-0.0.2.post1/src/access_nri_intake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.2/versioneer.py` & `access_nri_intake-0.0.2.post1/versioneer.py`

 * *Files identical despite different names*


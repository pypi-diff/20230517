# Comparing `tmp/access_nri_intake-0.0.3.tar.gz` & `tmp/access_nri_intake-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_nri_intake-0.0.3.tar", last modified: Tue May 16 22:21:12 2023, max compression
+gzip compressed data, was "access_nri_intake-0.0.4.tar", last modified: Wed May 17 00:45:07 2023, max compression
```

## Comparing `access_nri_intake-0.0.3.tar` & `access_nri_intake-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:21:12.639320 access_nri_intake-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-16 22:21:12.639320 access_nri_intake-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:21:12.639320 access_nri_intake-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:21:12.631320 access_nri_intake-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:21:12.639320 access_nri_intake-0.0.3/src/access_nri_intake/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/src/access_nri_intake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 22:21:12.639320 access_nri_intake-0.0.3/src/access_nri_intake/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:21:12.635320 access_nri_intake-0.0.3/src/access_nri_intake/cat/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/src/access_nri_intake/cat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/src/access_nri_intake/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:21:12.635320 access_nri_intake-0.0.3/src/access_nri_intake/esmcat/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/src/access_nri_intake/esmcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/src/access_nri_intake/esmcat/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/src/access_nri_intake/esmcat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:21:12.639320 access_nri_intake-0.0.3/src/access_nri_intake/metacat/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/src/access_nri_intake/metacat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/src/access_nri_intake/metacat/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/src/access_nri_intake/metacat/translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/src/access_nri_intake/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:21:12.635320 access_nri_intake-0.0.3/src/access_nri_intake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-16 22:21:12.000000 access_nri_intake-0.0.3/src/access_nri_intake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-16 22:21:12.000000 access_nri_intake-0.0.3/src/access_nri_intake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:21:12.000000 access_nri_intake-0.0.3/src/access_nri_intake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-16 22:21:12.000000 access_nri_intake-0.0.3/src/access_nri_intake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-16 22:21:12.000000 access_nri_intake-0.0.3/src/access_nri_intake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 22:21:12.000000 access_nri_intake-0.0.3/src/access_nri_intake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-16 22:20:47.000000 access_nri_intake-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.148981 access_nri_intake-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake/cat/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/cat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/cat/metacatalog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake/esmcat/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/esmcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/esmcat/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/esmcat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake/metacat/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/metacat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/metacat/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/metacat/translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/versioneer.py
```

### Comparing `access_nri_intake-0.0.3/LICENSE` & `access_nri_intake-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.3/README.rst` & `access_nri_intake-0.0.4/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 =========================
 ACCESS-NRI Intake Catalog
 =========================
 
 **Tools and configuration info used to manage ACCESS-NRI's intake catalog**
 
-Note, this is under development. Things might change/break frequently and without warning.
+Note, this project is under development. Things might change/break frequently and without warning.
 
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
 | Package       | |pypi| |conda|       |
```

### Comparing `access_nri_intake-0.0.3/pyproject.toml` & `access_nri_intake-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "access_nri_intake"
 authors = [
     { name = "ACCESS-NRI" },
 ]
 description = "Intake catalog managed by ACCESS-NRI and associated tools"
-readme = "README.md"
+readme = "README.rst"
 requires-python = ">=3.9"
 license = { text = "Apache-2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
@@ -37,15 +37,15 @@
   "versioneer[toml]",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-access_nri_intake = ["*.yaml"]
+access_nri_intake = ["cat/metacatalog.yaml"]
 
 [tool.versioneer]
 VCS = "git"
 style = "pep440"
 versionfile_source = "src/access_nri_intake/_version.py"
 versionfile_build = "access_nri_intake/_version.py"
 tag_prefix = "v"
```

### Comparing `access_nri_intake-0.0.3/src/access_nri_intake/cli.py` & `access_nri_intake-0.0.4/src/access_nri_intake/cli.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.3/src/access_nri_intake/esmcat/__init__.py` & `access_nri_intake-0.0.4/src/access_nri_intake/esmcat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.3/src/access_nri_intake/esmcat/builders.py` & `access_nri_intake-0.0.4/src/access_nri_intake/esmcat/builders.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.3/src/access_nri_intake/esmcat/utils.py` & `access_nri_intake-0.0.4/src/access_nri_intake/esmcat/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.3/src/access_nri_intake/metacat/__init__.py` & `access_nri_intake-0.0.4/src/access_nri_intake/metacat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.3/src/access_nri_intake/metacat/manager.py` & `access_nri_intake-0.0.4/src/access_nri_intake/metacat/manager.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.3/src/access_nri_intake/metacat/translators.py` & `access_nri_intake-0.0.4/src/access_nri_intake/metacat/translators.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.3/src/access_nri_intake/utils.py` & `access_nri_intake-0.0.4/src/access_nri_intake/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.3/src/access_nri_intake.egg-info/SOURCES.txt` & `access_nri_intake-0.0.4/src/access_nri_intake.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 src/access_nri_intake.egg-info/PKG-INFO
 src/access_nri_intake.egg-info/SOURCES.txt
 src/access_nri_intake.egg-info/dependency_links.txt
 src/access_nri_intake.egg-info/entry_points.txt
 src/access_nri_intake.egg-info/requires.txt
 src/access_nri_intake.egg-info/top_level.txt
 src/access_nri_intake/cat/__init__.py
+src/access_nri_intake/cat/metacatalog.yaml
 src/access_nri_intake/esmcat/__init__.py
 src/access_nri_intake/esmcat/builders.py
 src/access_nri_intake/esmcat/utils.py
 src/access_nri_intake/metacat/__init__.py
 src/access_nri_intake/metacat/manager.py
 src/access_nri_intake/metacat/translators.py
```

### Comparing `access_nri_intake-0.0.3/versioneer.py` & `access_nri_intake-0.0.4/versioneer.py`

 * *Files identical despite different names*


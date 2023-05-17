# Comparing `tmp/cici.tools-0.1.0.tar.gz` & `tmp/cici.tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cici.tools-0.1.0.tar", last modified: Wed May 17 08:00:03 2023, max compression
+gzip compressed data, was "cici.tools-0.1.1.tar", last modified: Wed May 17 08:06:27 2023, max compression
```

## Comparing `cici.tools-0.1.0.tar` & `cici.tools-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:00:03.446613 cici.tools-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-17 07:59:59.000000 cici.tools-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 08:00:03.446613 cici.tools-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-05-17 07:59:59.000000 cici.tools-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:00:03.442946 cici.tools-0.1.0/cici/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:59:59.000000 cici.tools-0.1.0/cici/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-17 07:59:59.000000 cici.tools-0.1.0/cici/__main__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 08:00:00.000000 cici.tools-0.1.0/cici/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:00:03.446613 cici.tools-0.1.0/cici/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:59:59.000000 cici.tools-0.1.0/cici/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6752 2023-05-17 07:59:59.000000 cici.tools-0.1.0/cici/cli/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     2918 2023-05-17 07:59:59.000000 cici.tools-0.1.0/cici/cli/update.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-17 07:59:59.000000 cici.tools-0.1.0/cici/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-17 07:59:59.000000 cici.tools-0.1.0/cici/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:00:03.446613 cici.tools-0.1.0/cici/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:59:59.000000 cici.tools-0.1.0/cici/schema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:00:03.445696 cici.tools-0.1.0/cici.tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 08:00:03.000000 cici.tools-0.1.0/cici.tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      411 2023-05-17 08:00:03.000000 cici.tools-0.1.0/cici.tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 08:00:03.000000 cici.tools-0.1.0/cici.tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-17 08:00:03.000000 cici.tools-0.1.0/cici.tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-17 08:00:03.000000 cici.tools-0.1.0/cici.tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-17 08:00:03.000000 cici.tools-0.1.0/cici.tools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-17 08:00:03.447530 cici.tools-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-17 08:00:00.000000 cici.tools-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:06:27.173720 cici.tools-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 08:06:23.000000 cici.tools-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 08:06:27.173720 cici.tools-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-05-17 08:06:23.000000 cici.tools-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:06:27.169720 cici.tools-0.1.1/cici/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 08:06:23.000000 cici.tools-0.1.1/cici/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-17 08:06:23.000000 cici.tools-0.1.1/cici/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 08:06:24.000000 cici.tools-0.1.1/cici/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:06:27.172720 cici.tools-0.1.1/cici/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 08:06:23.000000 cici.tools-0.1.1/cici/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6752 2023-05-17 08:06:23.000000 cici.tools-0.1.1/cici/cli/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     2918 2023-05-17 08:06:23.000000 cici.tools-0.1.1/cici/cli/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-17 08:06:23.000000 cici.tools-0.1.1/cici/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-17 08:06:23.000000 cici.tools-0.1.1/cici/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:06:27.173720 cici.tools-0.1.1/cici/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-05-17 08:06:23.000000 cici.tools-0.1.1/cici/schema/LICENSE.gitlab
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 08:06:23.000000 cici.tools-0.1.1/cici/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70638 2023-05-17 08:06:23.000000 cici.tools-0.1.1/cici/schema/gitlab-ci.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:06:27.171720 cici.tools-0.1.1/cici.tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 08:06:27.000000 cici.tools-0.1.1/cici.tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-17 08:06:27.000000 cici.tools-0.1.1/cici.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 08:06:27.000000 cici.tools-0.1.1/cici.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-17 08:06:27.000000 cici.tools-0.1.1/cici.tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-17 08:06:27.000000 cici.tools-0.1.1/cici.tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-17 08:06:27.000000 cici.tools-0.1.1/cici.tools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-17 08:06:27.174720 cici.tools-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-17 08:06:24.000000 cici.tools-0.1.1/setup.py
```

### Comparing `cici.tools-0.1.0/PKG-INFO` & `cici.tools-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici.tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: CI pipeline toolkit.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
```

### Comparing `cici.tools-0.1.0/README.md` & `cici.tools-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.0/cici/cli/bundle.py` & `cici.tools-0.1.1/cici/cli/bundle.py`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.0/cici/cli/update.py` & `cici.tools-0.1.1/cici/cli/update.py`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.0/cici/main.py` & `cici.tools-0.1.1/cici/main.py`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.0/cici.tools.egg-info/PKG-INFO` & `cici.tools-0.1.1/cici.tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici.tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: CI pipeline toolkit.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
```

### Comparing `cici.tools-0.1.0/setup.py` & `cici.tools-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```


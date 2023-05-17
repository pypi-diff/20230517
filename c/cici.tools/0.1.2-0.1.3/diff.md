# Comparing `tmp/cici.tools-0.1.2.tar.gz` & `tmp/cici.tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cici.tools-0.1.2.tar", last modified: Wed May 17 08:38:57 2023, max compression
+gzip compressed data, was "cici.tools-0.1.3.tar", last modified: Wed May 17 09:08:12 2023, max compression
```

## Comparing `cici.tools-0.1.2.tar` & `cici.tools-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:38:57.120410 cici.tools-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 08:38:53.000000 cici.tools-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 08:38:57.120410 cici.tools-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-05-17 08:38:53.000000 cici.tools-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:38:57.116409 cici.tools-0.1.2/cici/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 08:38:53.000000 cici.tools-0.1.2/cici/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-17 08:38:53.000000 cici.tools-0.1.2/cici/__main__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 08:38:54.000000 cici.tools-0.1.2/cici/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:38:57.119410 cici.tools-0.1.2/cici/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 08:38:53.000000 cici.tools-0.1.2/cici/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6752 2023-05-17 08:38:53.000000 cici.tools-0.1.2/cici/cli/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     2918 2023-05-17 08:38:53.000000 cici.tools-0.1.2/cici/cli/update.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-17 08:38:53.000000 cici.tools-0.1.2/cici/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-05-17 08:38:53.000000 cici.tools-0.1.2/cici/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:38:57.120410 cici.tools-0.1.2/cici/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-05-17 08:38:53.000000 cici.tools-0.1.2/cici/schema/LICENSE.gitlab
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 08:38:53.000000 cici.tools-0.1.2/cici/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    70638 2023-05-17 08:38:53.000000 cici.tools-0.1.2/cici/schema/gitlab-ci.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:38:57.118410 cici.tools-0.1.2/cici.tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 08:38:57.000000 cici.tools-0.1.2/cici.tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-17 08:38:57.000000 cici.tools-0.1.2/cici.tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 08:38:57.000000 cici.tools-0.1.2/cici.tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-17 08:38:57.000000 cici.tools-0.1.2/cici.tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-17 08:38:57.000000 cici.tools-0.1.2/cici.tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-17 08:38:57.000000 cici.tools-0.1.2/cici.tools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-17 08:38:57.121410 cici.tools-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-17 08:38:54.000000 cici.tools-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:08:12.450373 cici.tools-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 09:08:08.000000 cici.tools-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 09:08:12.450373 cici.tools-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-05-17 09:08:08.000000 cici.tools-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:08:12.446372 cici.tools-0.1.3/cici/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 09:08:09.000000 cici.tools-0.1.3/cici/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:08:12.449373 cici.tools-0.1.3/cici/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6752 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/cli/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     2918 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/cli/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:08:12.449373 cici.tools-0.1.3/cici/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/schema/LICENSE.gitlab
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70638 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/schema/gitlab-ci.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:08:12.448372 cici.tools-0.1.3/cici.tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-17 09:08:12.450373 cici.tools-0.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-17 09:08:09.000000 cici.tools-0.1.3/setup.py
```

### Comparing `cici.tools-0.1.2/PKG-INFO` & `cici.tools-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici.tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: CI pipeline toolkit.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
```

### Comparing `cici.tools-0.1.2/README.md` & `cici.tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.2/cici/cli/bundle.py` & `cici.tools-0.1.3/cici/cli/bundle.py`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.2/cici/cli/update.py` & `cici.tools-0.1.3/cici/cli/update.py`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.2/cici/main.py` & `cici.tools-0.1.3/cici/main.py`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.2/cici/schema/LICENSE.gitlab` & `cici.tools-0.1.3/cici/schema/LICENSE.gitlab`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.2/cici/schema/gitlab-ci.json` & `cici.tools-0.1.3/cici/schema/gitlab-ci.json`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.2/cici.tools.egg-info/PKG-INFO` & `cici.tools-0.1.3/cici.tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici.tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: CI pipeline toolkit.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
```

### Comparing `cici.tools-0.1.2/setup.py` & `cici.tools-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```


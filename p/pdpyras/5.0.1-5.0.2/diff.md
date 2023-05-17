# Comparing `tmp/pdpyras-5.0.1.tar.gz` & `tmp/pdpyras-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpyras-5.0.1.tar", last modified: Mon May  1 19:52:54 2023, max compression
+gzip compressed data, was "pdpyras-5.0.2.tar", last modified: Wed May 17 20:39:44 2023, max compression
```

## Comparing `pdpyras-5.0.1.tar` & `pdpyras-5.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-01 19:52:54.548575 pdpyras-5.0.1/
--rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.0.1/LICENSE
--rw-r--r--   0 demitri    (503) staff       (20)      393 2023-05-01 19:52:54.548441 pdpyras-5.0.1/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-01 18:31:04.000000 pdpyras-5.0.1/README.rst
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-01 19:52:54.548263 pdpyras-5.0.1/pdpyras.egg-info/
--rw-r--r--   0 demitri    (503) staff       (20)      393 2023-05-01 19:52:54.000000 pdpyras-5.0.1/pdpyras.egg-info/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)      192 2023-05-01 19:52:54.000000 pdpyras-5.0.1/pdpyras.egg-info/SOURCES.txt
--rw-r--r--   0 demitri    (503) staff       (20)        1 2023-05-01 19:52:54.000000 pdpyras-5.0.1/pdpyras.egg-info/dependency_links.txt
--rw-r--r--   0 demitri    (503) staff       (20)       29 2023-05-01 19:52:54.000000 pdpyras-5.0.1/pdpyras.egg-info/requires.txt
--rw-r--r--   0 demitri    (503) staff       (20)        8 2023-05-01 19:52:54.000000 pdpyras-5.0.1/pdpyras.egg-info/top_level.txt
--rw-r--r--   0 demitri    (503) staff       (20)    86705 2023-05-01 19:52:37.000000 pdpyras-5.0.1/pdpyras.py
--rw-r--r--   0 demitri    (503) staff       (20)       38 2023-05-01 19:52:54.548626 pdpyras-5.0.1/setup.cfg
--rw-r--r--   0 demitri    (503) staff       (20)      657 2023-05-01 19:52:37.000000 pdpyras-5.0.1/setup.py
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-17 20:39:44.019305 pdpyras-5.0.2/
+-rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.0.2/LICENSE
+-rw-r--r--   0 demitri    (503) staff       (20)      374 2023-05-17 20:39:44.019184 pdpyras-5.0.2/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-01 18:31:04.000000 pdpyras-5.0.2/README.rst
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-17 20:39:44.019018 pdpyras-5.0.2/pdpyras.egg-info/
+-rw-r--r--   0 demitri    (503) staff       (20)      374 2023-05-17 20:39:43.000000 pdpyras-5.0.2/pdpyras.egg-info/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)      192 2023-05-17 20:39:43.000000 pdpyras-5.0.2/pdpyras.egg-info/SOURCES.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        1 2023-05-17 20:39:43.000000 pdpyras-5.0.2/pdpyras.egg-info/dependency_links.txt
+-rw-r--r--   0 demitri    (503) staff       (20)       29 2023-05-17 20:39:43.000000 pdpyras-5.0.2/pdpyras.egg-info/requires.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        8 2023-05-17 20:39:43.000000 pdpyras-5.0.2/pdpyras.egg-info/top_level.txt
+-rw-r--r--   0 demitri    (503) staff       (20)    86702 2023-05-17 20:39:30.000000 pdpyras-5.0.2/pdpyras.py
+-rw-r--r--   0 demitri    (503) staff       (20)       38 2023-05-17 20:39:44.019345 pdpyras-5.0.2/setup.cfg
+-rw-r--r--   0 demitri    (503) staff       (20)      657 2023-05-17 20:01:06.000000 pdpyras-5.0.2/setup.py
```

### Comparing `pdpyras-5.0.1/LICENSE` & `pdpyras-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdpyras-5.0.1/README.rst` & `pdpyras-5.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pdpyras-5.0.1/pdpyras.py` & `pdpyras-5.0.2/pdpyras.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Libraries from PyPI
 import requests
 from deprecation import deprecated, DeprecatedWarning
 from urllib3.exceptions import HTTPError, PoolError
 from requests.exceptions import RequestException
 
-__version__ = '5.0.1'
+__version__ = '5.0.2'
 
 #######################
 ### CLIENT DEFAULTS ###
 #######################
 ITERATION_LIMIT = 1e4
 """
 The maximum position of a result in classic pagination.
@@ -781,17 +781,17 @@
             f"{endpoint}: API responded with {err_type} error (status %d)" \
             f"{context_msg}: %s"
         ) % (r.status_code, truncate_text(r.text))
     elif not received_http_response:
         return f"{endpoint}: Network or other unknown error{context_msg}"
     else:
         return (
-            f"{endpoint}: Success (status %d) but an expectation still " \
+            f"{endpoint}: Success (status {r.status_code}) but an expectation still " \
             f"failed{context_msg}"
-        )%(r.status_code)
+        )
 
 def last_4(secret: str):
     """Returns an abbreviation of the input"""
     return '*'+str(secret)[-4:]
 
 @deprecated(deprecated_in='5.0.0', removed_in='5.1.0',
         current_version=__version__, details='Use singular_name instead.')
```

### Comparing `pdpyras-5.0.1/setup.py` & `pdpyras-5.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '5.0.1'
+__version__ = '5.0.2'
 
 if __name__ == '__main__':
     setup(
         name='pdpyras',
         description="PagerDuty Python REST API Sessions",
         long_description="A basic REST API client for PagerDuty based on Requests' Session class",
         py_modules=['pdpyras'],
```


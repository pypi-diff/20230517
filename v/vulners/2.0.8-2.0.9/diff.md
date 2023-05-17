# Comparing `tmp/vulners-2.0.8.tar.gz` & `tmp/vulners-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulners-2.0.8.tar", last modified: Wed Feb  8 10:22:01 2023, max compression
+gzip compressed data, was "vulners-2.0.9.tar", last modified: Wed Feb 22 09:23:29 2023, max compression
```

## Comparing `vulners-2.0.8.tar` & `vulners-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 deploy    (1003) deploy    (1003)        0 2023-02-08 10:22:01.192549 vulners-2.0.8/
--rw-r--r--   0 deploy    (1003) deploy    (1003)       91 2023-02-08 10:21:56.000000 vulners-2.0.8/AUTHORS
--rw-r--r--   0 deploy    (1003) deploy    (1003)    35141 2023-02-08 10:21:56.000000 vulners-2.0.8/LICENSE
--rw-r--r--   0 deploy    (1003) deploy    (1003)       80 2023-02-08 10:21:56.000000 vulners-2.0.8/MANIFEST.in
--rw-r--r--   0 deploy    (1003) deploy    (1003)     8210 2023-02-08 10:22:01.192549 vulners-2.0.8/PKG-INFO
--rw-r--r--   0 deploy    (1003) deploy    (1003)     5904 2023-02-08 10:21:56.000000 vulners-2.0.8/README.md
--rw-r--r--   0 deploy    (1003) deploy    (1003)       38 2023-02-08 10:22:01.192549 vulners-2.0.8/setup.cfg
--rw-r--r--   0 deploy    (1003) deploy    (1003)     1486 2023-02-08 10:21:56.000000 vulners-2.0.8/setup.py
-drwxr-xr-x   0 deploy    (1003) deploy    (1003)        0 2023-02-08 10:22:01.192549 vulners-2.0.8/vulners/
--rw-r--r--   0 deploy    (1003) deploy    (1003)      227 2023-02-08 10:21:56.000000 vulners-2.0.8/vulners/__init__.py
--rw-r--r--   0 deploy    (1003) deploy    (1003)    19211 2023-02-08 10:21:56.000000 vulners-2.0.8/vulners/base.py
--rw-r--r--   0 deploy    (1003) deploy    (1003)    11287 2023-02-08 10:21:56.000000 vulners-2.0.8/vulners/vscanner.py
--rw-r--r--   0 deploy    (1003) deploy    (1003)    29595 2023-02-08 10:21:56.000000 vulners-2.0.8/vulners/vulners.py
-drwxr-xr-x   0 deploy    (1003) deploy    (1003)        0 2023-02-08 10:22:01.192549 vulners-2.0.8/vulners.egg-info/
--rw-r--r--   0 deploy    (1003) deploy    (1003)     8210 2023-02-08 10:22:00.000000 vulners-2.0.8/vulners.egg-info/PKG-INFO
--rw-r--r--   0 deploy    (1003) deploy    (1003)      275 2023-02-08 10:22:00.000000 vulners-2.0.8/vulners.egg-info/SOURCES.txt
--rw-r--r--   0 deploy    (1003) deploy    (1003)        1 2023-02-08 10:22:00.000000 vulners-2.0.8/vulners.egg-info/dependency_links.txt
--rw-r--r--   0 deploy    (1003) deploy    (1003)       21 2023-02-08 10:22:00.000000 vulners-2.0.8/vulners.egg-info/requires.txt
--rw-r--r--   0 deploy    (1003) deploy    (1003)        8 2023-02-08 10:22:00.000000 vulners-2.0.8/vulners.egg-info/top_level.txt
+drwxr-xr-x   0 deploy    (1003) deploy    (1003)        0 2023-02-22 09:23:29.430987 vulners-2.0.9/
+-rw-r--r--   0 deploy    (1003) deploy    (1003)       91 2023-02-22 09:23:24.000000 vulners-2.0.9/AUTHORS
+-rw-r--r--   0 deploy    (1003) deploy    (1003)    35141 2023-02-22 09:23:24.000000 vulners-2.0.9/LICENSE
+-rw-r--r--   0 deploy    (1003) deploy    (1003)       80 2023-02-22 09:23:24.000000 vulners-2.0.9/MANIFEST.in
+-rw-r--r--   0 deploy    (1003) deploy    (1003)     8210 2023-02-22 09:23:29.430987 vulners-2.0.9/PKG-INFO
+-rw-r--r--   0 deploy    (1003) deploy    (1003)     5904 2023-02-22 09:23:24.000000 vulners-2.0.9/README.md
+-rw-r--r--   0 deploy    (1003) deploy    (1003)       38 2023-02-22 09:23:29.430987 vulners-2.0.9/setup.cfg
+-rw-r--r--   0 deploy    (1003) deploy    (1003)     1486 2023-02-22 09:23:24.000000 vulners-2.0.9/setup.py
+drwxr-xr-x   0 deploy    (1003) deploy    (1003)        0 2023-02-22 09:23:29.430987 vulners-2.0.9/vulners/
+-rw-r--r--   0 deploy    (1003) deploy    (1003)      227 2023-02-22 09:23:24.000000 vulners-2.0.9/vulners/__init__.py
+-rw-r--r--   0 deploy    (1003) deploy    (1003)    19211 2023-02-22 09:23:24.000000 vulners-2.0.9/vulners/base.py
+-rw-r--r--   0 deploy    (1003) deploy    (1003)    11287 2023-02-22 09:23:24.000000 vulners-2.0.9/vulners/vscanner.py
+-rw-r--r--   0 deploy    (1003) deploy    (1003)    30551 2023-02-22 09:23:24.000000 vulners-2.0.9/vulners/vulners.py
+drwxr-xr-x   0 deploy    (1003) deploy    (1003)        0 2023-02-22 09:23:29.430987 vulners-2.0.9/vulners.egg-info/
+-rw-r--r--   0 deploy    (1003) deploy    (1003)     8210 2023-02-22 09:23:28.000000 vulners-2.0.9/vulners.egg-info/PKG-INFO
+-rw-r--r--   0 deploy    (1003) deploy    (1003)      275 2023-02-22 09:23:28.000000 vulners-2.0.9/vulners.egg-info/SOURCES.txt
+-rw-r--r--   0 deploy    (1003) deploy    (1003)        1 2023-02-22 09:23:28.000000 vulners-2.0.9/vulners.egg-info/dependency_links.txt
+-rw-r--r--   0 deploy    (1003) deploy    (1003)       21 2023-02-22 09:23:28.000000 vulners-2.0.9/vulners.egg-info/requires.txt
+-rw-r--r--   0 deploy    (1003) deploy    (1003)        8 2023-02-22 09:23:28.000000 vulners-2.0.9/vulners.egg-info/top_level.txt
```

### Comparing `vulners-2.0.8/LICENSE` & `vulners-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vulners-2.0.8/PKG-INFO` & `vulners-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulners
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python library and command-line utility for Vulners (https://vulners.com)
 Home-page: https://github.com/vulnersCom/api
 Author: Kirill Ermakov, Andrei Churin
 Author-email: isox@vulners.com, aachurin@gmail.com
 License: UNKNOWN
 Description: # [Vulners API v3](https://vulners.com) Python wrapper
```

### Comparing `vulners-2.0.8/README.md` & `vulners-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vulners-2.0.8/setup.py` & `vulners-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `vulners-2.0.8/vulners/base.py` & `vulners-2.0.9/vulners/base.py`

 * *Files identical despite different names*

### Comparing `vulners-2.0.8/vulners/vscanner.py` & `vulners-2.0.9/vulners/vscanner.py`

 * *Files identical despite different names*

### Comparing `vulners-2.0.8/vulners/vulners.py` & `vulners-2.0.9/vulners/vulners.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,14 +426,21 @@
         method="get",
         url="/api/v3/archive/distributive/",
         params=[("os", String()), ("version", String())],
         result_type="zipjson",
         content_handler=_unpack_json_file,
     )
 
+    getsploit = Endpoint(
+        method="get",
+        url="/api/v3/archive/getsploit/",
+        params=[],
+        result_type="zip",
+    )
+
     del _unpack_json_file
 
     @validate_params(collection=String(), start_date=String(), end_date=String())
     def get_collection(
         self, collection, start_date="1950-01-01", end_date="2199-01-01"
     ):
         """
@@ -592,14 +599,33 @@
         url="/api/v3/subscriptions/webhook",
         params=[
             ("subscriptionid", String()),
             ("newest_only", String(default="true"))
         ]
     )
 
+    @validate_params(
+        limit=Integer(minimum=1, maximum=10000),
+        offset=Integer(minimum=0, maximum=10000),
+        filter=Dict(),
+        sort=String()
+    )
+    def hostvulns_report(self, limit=30, offset=0, filter=None, sort=''):
+        """
+        Get Linux Audit results. Return list of hosts and host vulnerabilities:
+           host ip and fqdn, os name and version, cumulative fix, vulnerability ids
+
+        limit: The maximum number of items to return. 10000 is the hard limit.
+        offset: Skip this amount of items. 10000 is the hard limit.
+        filter: Dict of fields to filter, eg { 'OS': 'Centos', 'OSVersion': '7'}
+        sort: Field to sort, eg 'modified' or '-modified' to sort desc
+        """
+
+        return self.__report("hostvulns", offset, limit, filter or {}, sort)
+
 
 _Unset = object()
 
 
 # noinspection PyPep8Naming
 class DeprecatedVulnersApi(VulnersApi):
     def __init__(self, *args, **kwargs):
```

### Comparing `vulners-2.0.8/vulners.egg-info/PKG-INFO` & `vulners-2.0.9/vulners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulners
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python library and command-line utility for Vulners (https://vulners.com)
 Home-page: https://github.com/vulnersCom/api
 Author: Kirill Ermakov, Andrei Churin
 Author-email: isox@vulners.com, aachurin@gmail.com
 License: UNKNOWN
 Description: # [Vulners API v3](https://vulners.com) Python wrapper
```


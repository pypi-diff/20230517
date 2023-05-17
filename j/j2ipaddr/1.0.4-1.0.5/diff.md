# Comparing `tmp/j2ipaddr-1.0.4.tar.gz` & `tmp/j2ipaddr-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "j2ipaddr-1.0.4.tar", last modified: Tue Oct 18 20:43:45 2022, max compression
+gzip compressed data, was "j2ipaddr-1.0.5.tar", last modified: Wed May 17 15:03:06 2023, max compression
```

## Comparing `j2ipaddr-1.0.4.tar` & `j2ipaddr-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:43:45.175268 j2ipaddr-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-18 20:43:32.000000 j2ipaddr-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4956 2022-10-18 20:43:45.175268 j2ipaddr-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4415 2022-10-18 20:43:32.000000 j2ipaddr-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:43:45.171268 j2ipaddr-1.0.4/j2ipaddr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 20:43:32.000000 j2ipaddr-1.0.4/j2ipaddr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-10-18 20:43:32.000000 j2ipaddr-1.0.4/j2ipaddr/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:43:45.171268 j2ipaddr-1.0.4/j2ipaddr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4956 2022-10-18 20:43:45.000000 j2ipaddr-1.0.4/j2ipaddr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-10-18 20:43:45.000000 j2ipaddr-1.0.4/j2ipaddr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 20:43:45.000000 j2ipaddr-1.0.4/j2ipaddr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-18 20:43:45.000000 j2ipaddr-1.0.4/j2ipaddr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-18 20:43:45.000000 j2ipaddr-1.0.4/j2ipaddr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-10-18 20:43:32.000000 j2ipaddr-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-18 20:43:45.175268 j2ipaddr-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:03:06.042248 j2ipaddr-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 15:02:50.000000 j2ipaddr-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-17 15:03:06.042248 j2ipaddr-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-17 15:02:50.000000 j2ipaddr-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:03:06.042248 j2ipaddr-1.0.5/j2ipaddr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:02:50.000000 j2ipaddr-1.0.5/j2ipaddr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-17 15:02:50.000000 j2ipaddr-1.0.5/j2ipaddr/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:03:06.042248 j2ipaddr-1.0.5/j2ipaddr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-17 15:03:06.000000 j2ipaddr-1.0.5/j2ipaddr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-17 15:03:06.000000 j2ipaddr-1.0.5/j2ipaddr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:03:06.000000 j2ipaddr-1.0.5/j2ipaddr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 15:03:06.000000 j2ipaddr-1.0.5/j2ipaddr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 15:03:06.000000 j2ipaddr-1.0.5/j2ipaddr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 15:02:50.000000 j2ipaddr-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:03:06.042248 j2ipaddr-1.0.5/setup.cfg
```

### Comparing `j2ipaddr-1.0.4/LICENSE` & `j2ipaddr-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `j2ipaddr-1.0.4/PKG-INFO` & `j2ipaddr-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: j2ipaddr
-Version: 1.0.4
+Version: 1.0.5
 Summary: Jinja2 filters for IP addresses, the easy way
 Author-email: Arturo Baldo <baldoarturo@mail.com>
 Project-URL: Homepage, https://github.com/baldoarturo/j2ipaddr
 Keywords: jinja2,jinja,filters,netaddr,ipaddr,networking
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `j2ipaddr-1.0.4/README.md` & `j2ipaddr-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `j2ipaddr-1.0.4/j2ipaddr/filters.py` & `j2ipaddr-1.0.5/j2ipaddr/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from inspect import isfunction
-from netaddr import IPNetwork
+from netaddr import IPNetwork, IPAddress
 
 import j2ipaddr
 
 
 def ip_address(addr):
     """
     Returns an IP address for a combination of IP address and subnet mask
@@ -92,26 +92,26 @@
     """
     Returns the first usable address in network address for a combination of IP address and subnet mask
 
     Example:
     ip_network('10.10.10.5/24')
     > 10.10.10.1
     """
-    return IPNetwork(addr).first
+    return IPAddress(IPNetwork(addr).first).__str__()
 
 
 def ip_network_last(addr):
     """
     Returns the last usable address in network address for a combination of IP address and subnet mask
 
     Example:
     ip_network('10.10.10.5/24')
     > 10.10.10.254
     """
-    return IPNetwork(addr).last
+    return IPAddress(IPNetwork(addr).last).__str__()
 
 
 def load_all():
     """
     Returns a dict will all the functions inside filters, except load_all
     """
     import inspect
```

### Comparing `j2ipaddr-1.0.4/j2ipaddr.egg-info/PKG-INFO` & `j2ipaddr-1.0.5/j2ipaddr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: j2ipaddr
-Version: 1.0.4
+Version: 1.0.5
 Summary: Jinja2 filters for IP addresses, the easy way
 Author-email: Arturo Baldo <baldoarturo@mail.com>
 Project-URL: Homepage, https://github.com/baldoarturo/j2ipaddr
 Keywords: jinja2,jinja,filters,netaddr,ipaddr,networking
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `j2ipaddr-1.0.4/pyproject.toml` & `j2ipaddr-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "j2ipaddr"
-version = "1.0.4"
+version = "1.0.5"
 description = "Jinja2 filters for IP addresses, the easy way"
 readme = "README.md"
 authors = [{ name = "Arturo Baldo", email = "baldoarturo@mail.com" }]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```


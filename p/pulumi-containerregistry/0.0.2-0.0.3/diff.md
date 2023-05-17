# Comparing `tmp/pulumi_containerregistry-0.0.2.tar.gz` & `tmp/pulumi_containerregistry-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_containerregistry-0.0.2.tar", last modified: Wed May 17 12:39:04 2023, max compression
+gzip compressed data, was "pulumi_containerregistry-0.0.3.tar", last modified: Wed May 17 12:57:33 2023, max compression
```

## Comparing `pulumi_containerregistry-0.0.2.tar` & `pulumi_containerregistry-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:39:04.914126 pulumi_containerregistry-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 12:39:04.914126 pulumi_containerregistry-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:39:04.914126 pulumi_containerregistry-0.0.2/pulumi_containerregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:39:04.914126 pulumi_containerregistry-0.0.2/pulumi_containerregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/pulumi_containerregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:39:04.914126 pulumi_containerregistry-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-17 12:39:04.000000 pulumi_containerregistry-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:33.612567 pulumi_containerregistry-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 12:57:33.612567 pulumi_containerregistry-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:33.608567 pulumi_containerregistry-0.0.3/pulumi_containerregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:33.612567 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:57:33.612567 pulumi_containerregistry-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/setup.py
```

### Comparing `pulumi_containerregistry-0.0.2/PKG-INFO` & `pulumi_containerregistry-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_containerregistry
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Pulumi package for creating and managing containerregistry cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/rhysmdnz/pulumi-containerregistry
 Keywords: pulumi containerregistry category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_containerregistry-0.0.2/README.md` & `pulumi_containerregistry-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.2/pulumi_containerregistry/__init__.py` & `pulumi_containerregistry-0.0.3/pulumi_containerregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.2/pulumi_containerregistry/_utilities.py` & `pulumi_containerregistry-0.0.3/pulumi_containerregistry/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.2/pulumi_containerregistry/provider.py` & `pulumi_containerregistry-0.0.3/pulumi_containerregistry/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.2/pulumi_containerregistry/resource.py` & `pulumi_containerregistry-0.0.3/pulumi_containerregistry/resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.2/pulumi_containerregistry.egg-info/PKG-INFO` & `pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-containerregistry
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Pulumi package for creating and managing containerregistry cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/rhysmdnz/pulumi-containerregistry
 Keywords: pulumi containerregistry category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_containerregistry-0.0.2/pulumi_containerregistry.egg-info/SOURCES.txt` & `pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.2/setup.py` & `pulumi_containerregistry-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.2"
-PLUGIN_VERSION = "0.0.2"
+VERSION = "0.0.3"
+PLUGIN_VERSION = "0.0.3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'containerregistry', PLUGIN_VERSION])
         except OSError as error:
```


# Comparing `tmp/MySerializator-0.1.2.tar.gz` & `tmp/MySerializator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MySerializator-0.1.2.tar", last modified: Wed May 17 13:24:41 2023, max compression
+gzip compressed data, was "MySerializator-0.1.7.tar", last modified: Wed May 17 13:53:24 2023, max compression
```

## Comparing `MySerializator-0.1.2.tar` & `MySerializator-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-17 13:24:41.385442 MySerializator-0.1.2/
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-17 13:24:41.385442 MySerializator-0.1.2/MySerializator.egg-info/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      301 2023-05-17 13:24:41.000000 MySerializator-0.1.2/MySerializator.egg-info/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      207 2023-05-17 13:24:41.000000 MySerializator-0.1.2/MySerializator.egg-info/SOURCES.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-17 13:24:41.000000 MySerializator-0.1.2/MySerializator.egg-info/dependency_links.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       12 2023-05-17 13:24:41.000000 MySerializator-0.1.2/MySerializator.egg-info/top_level.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      301 2023-05-17 13:24:41.385442 MySerializator-0.1.2/PKG-INFO
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-17 13:24:41.385442 MySerializator-0.1.2/serializers/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        0 2023-05-14 17:02:08.000000 MySerializator-0.1.2/serializers/__init__.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      595 2023-05-16 21:32:12.000000 MySerializator-0.1.2/serializers/factory.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-17 13:24:41.385442 MySerializator-0.1.2/setup.cfg
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      433 2023-05-17 13:24:30.000000 MySerializator-0.1.2/setup.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-17 13:53:24.009594 MySerializator-0.1.7/
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-17 13:53:24.009594 MySerializator-0.1.7/MySerializator.egg-info/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      301 2023-05-17 13:53:23.000000 MySerializator-0.1.7/MySerializator.egg-info/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      207 2023-05-17 13:53:23.000000 MySerializator-0.1.7/MySerializator.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-17 13:53:23.000000 MySerializator-0.1.7/MySerializator.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       12 2023-05-17 13:53:23.000000 MySerializator-0.1.7/MySerializator.egg-info/top_level.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      301 2023-05-17 13:53:24.009594 MySerializator-0.1.7/PKG-INFO
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-17 13:53:24.009594 MySerializator-0.1.7/serializers/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        0 2023-05-14 17:02:08.000000 MySerializator-0.1.7/serializers/__init__.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      595 2023-05-16 21:32:12.000000 MySerializator-0.1.7/serializers/factory.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-17 13:53:24.009594 MySerializator-0.1.7/setup.cfg
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      433 2023-05-17 13:53:18.000000 MySerializator-0.1.7/setup.py
```

### Comparing `MySerializator-0.1.2/serializers/factory.py` & `MySerializator-0.1.7/serializers/factory.py`

 * *Files identical despite different names*


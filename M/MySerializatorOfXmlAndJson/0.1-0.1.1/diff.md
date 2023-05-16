# Comparing `tmp/MySerializatorOfXmlAndJson-0.1.tar.gz` & `tmp/MySerializatorOfXmlAndJson-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MySerializatorOfXmlAndJson-0.1.tar", last modified: Tue May 16 22:02:58 2023, max compression
+gzip compressed data, was "MySerializatorOfXmlAndJson-0.1.1.tar", last modified: Tue May 16 22:04:15 2023, max compression
```

## Comparing `MySerializatorOfXmlAndJson-0.1.tar` & `MySerializatorOfXmlAndJson-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-16 22:02:58.867731 MySerializatorOfXmlAndJson-0.1/
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-16 22:02:58.863731 MySerializatorOfXmlAndJson-0.1/MySerializatorOfXmlAndJson.egg-info/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      308 2023-05-16 22:02:58.000000 MySerializatorOfXmlAndJson-0.1/MySerializatorOfXmlAndJson.egg-info/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      304 2023-05-16 22:02:58.000000 MySerializatorOfXmlAndJson-0.1/MySerializatorOfXmlAndJson.egg-info/SOURCES.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-16 22:02:58.000000 MySerializatorOfXmlAndJson-0.1/MySerializatorOfXmlAndJson.egg-info/dependency_links.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        6 2023-05-16 22:02:58.000000 MySerializatorOfXmlAndJson-0.1/MySerializatorOfXmlAndJson.egg-info/requires.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       12 2023-05-16 22:02:58.000000 MySerializatorOfXmlAndJson-0.1/MySerializatorOfXmlAndJson.egg-info/top_level.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      308 2023-05-16 22:02:58.863731 MySerializatorOfXmlAndJson-0.1/PKG-INFO
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-16 22:02:58.863731 MySerializatorOfXmlAndJson-0.1/serializers/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        0 2023-05-14 17:02:08.000000 MySerializatorOfXmlAndJson-0.1/serializers/__init__.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      595 2023-05-16 21:32:12.000000 MySerializatorOfXmlAndJson-0.1/serializers/factory.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-16 22:02:58.867731 MySerializatorOfXmlAndJson-0.1/setup.cfg
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      471 2023-05-16 22:02:03.000000 MySerializatorOfXmlAndJson-0.1/setup.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-16 22:04:15.727777 MySerializatorOfXmlAndJson-0.1.1/
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-16 22:04:15.723777 MySerializatorOfXmlAndJson-0.1.1/MySerializatorOfXmlAndJson.egg-info/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      310 2023-05-16 22:04:15.000000 MySerializatorOfXmlAndJson-0.1.1/MySerializatorOfXmlAndJson.egg-info/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      304 2023-05-16 22:04:15.000000 MySerializatorOfXmlAndJson-0.1.1/MySerializatorOfXmlAndJson.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-16 22:04:15.000000 MySerializatorOfXmlAndJson-0.1.1/MySerializatorOfXmlAndJson.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        6 2023-05-16 22:04:15.000000 MySerializatorOfXmlAndJson-0.1.1/MySerializatorOfXmlAndJson.egg-info/requires.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       12 2023-05-16 22:04:15.000000 MySerializatorOfXmlAndJson-0.1.1/MySerializatorOfXmlAndJson.egg-info/top_level.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      310 2023-05-16 22:04:15.723777 MySerializatorOfXmlAndJson-0.1.1/PKG-INFO
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-16 22:04:15.723777 MySerializatorOfXmlAndJson-0.1.1/serializers/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        0 2023-05-14 17:02:08.000000 MySerializatorOfXmlAndJson-0.1.1/serializers/__init__.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      595 2023-05-16 21:32:12.000000 MySerializatorOfXmlAndJson-0.1.1/serializers/factory.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-16 22:04:15.727777 MySerializatorOfXmlAndJson-0.1.1/setup.cfg
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      473 2023-05-16 22:03:54.000000 MySerializatorOfXmlAndJson-0.1.1/setup.py
```

### Comparing `MySerializatorOfXmlAndJson-0.1/serializers/factory.py` & `MySerializatorOfXmlAndJson-0.1.1/serializers/factory.py`

 * *Files identical despite different names*


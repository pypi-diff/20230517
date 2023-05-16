# Comparing `tmp/CactusSerializer-2.0.0.tar.gz` & `tmp/CactusSerializer-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CactusSerializer-2.0.0.tar", last modified: Tue May 16 22:06:21 2023, max compression
+gzip compressed data, was "CactusSerializer-3.0.0.tar", last modified: Tue May 16 22:33:37 2023, max compression
```

## Comparing `CactusSerializer-2.0.0.tar` & `CactusSerializer-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-16 22:06:21.989162 CactusSerializer-2.0.0/
-drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-16 22:06:21.801163 CactusSerializer-2.0.0/CactusSerializer.egg-info/
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      405 2023-05-16 22:06:21.000000 CactusSerializer-2.0.0/CactusSerializer.egg-info/PKG-INFO
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      414 2023-05-16 22:06:21.000000 CactusSerializer-2.0.0/CactusSerializer.egg-info/SOURCES.txt
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        1 2023-05-16 22:06:21.000000 CactusSerializer-2.0.0/CactusSerializer.egg-info/dependency_links.txt
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)       11 2023-05-16 22:06:21.000000 CactusSerializer-2.0.0/CactusSerializer.egg-info/top_level.txt
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      405 2023-05-16 22:06:21.989162 CactusSerializer-2.0.0/PKG-INFO
-drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-16 22:06:21.969162 CactusSerializer-2.0.0/Serializer/
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     6100 2023-05-16 22:03:41.000000 CactusSerializer-2.0.0/Serializer/JsonDeserializer.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      721 2023-05-14 09:54:29.000000 CactusSerializer-2.0.0/Serializer/JsonParser.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     8117 2023-05-16 22:03:41.000000 CactusSerializer-2.0.0/Serializer/JsonSerializer.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      388 2023-05-13 14:17:01.000000 CactusSerializer-2.0.0/Serializer/SerializerFactory.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     6245 2023-05-16 22:03:41.000000 CactusSerializer-2.0.0/Serializer/XmlDeserializer.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      750 2023-05-14 09:54:29.000000 CactusSerializer-2.0.0/Serializer/XmlParser.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     8163 2023-05-16 22:03:41.000000 CactusSerializer-2.0.0/Serializer/XmlSerializer.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-14 10:15:55.000000 CactusSerializer-2.0.0/Serializer/__init__.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      306 2023-05-13 11:12:37.000000 CactusSerializer-2.0.0/Serializer/constants.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)       38 2023-05-16 22:06:21.989162 CactusSerializer-2.0.0/setup.cfg
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      551 2023-05-16 22:03:51.000000 CactusSerializer-2.0.0/setup.py
+drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-16 22:33:36.975784 CactusSerializer-3.0.0/
+drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-16 22:33:36.899784 CactusSerializer-3.0.0/CactusSerializer.egg-info/
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      405 2023-05-16 22:33:36.000000 CactusSerializer-3.0.0/CactusSerializer.egg-info/PKG-INFO
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      414 2023-05-16 22:33:36.000000 CactusSerializer-3.0.0/CactusSerializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        1 2023-05-16 22:33:36.000000 CactusSerializer-3.0.0/CactusSerializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)       11 2023-05-16 22:33:36.000000 CactusSerializer-3.0.0/CactusSerializer.egg-info/top_level.txt
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      405 2023-05-16 22:33:36.975784 CactusSerializer-3.0.0/PKG-INFO
+drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-16 22:33:36.971784 CactusSerializer-3.0.0/Serializer/
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     6100 2023-05-16 22:03:41.000000 CactusSerializer-3.0.0/Serializer/JsonDeserializer.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      721 2023-05-14 09:54:29.000000 CactusSerializer-3.0.0/Serializer/JsonParser.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     8117 2023-05-16 22:03:41.000000 CactusSerializer-3.0.0/Serializer/JsonSerializer.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      388 2023-05-13 14:17:01.000000 CactusSerializer-3.0.0/Serializer/SerializerFactory.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     6245 2023-05-16 22:03:41.000000 CactusSerializer-3.0.0/Serializer/XmlDeserializer.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      750 2023-05-14 09:54:29.000000 CactusSerializer-3.0.0/Serializer/XmlParser.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     8200 2023-05-16 22:31:14.000000 CactusSerializer-3.0.0/Serializer/XmlSerializer.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-14 10:15:55.000000 CactusSerializer-3.0.0/Serializer/__init__.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      306 2023-05-13 11:12:37.000000 CactusSerializer-3.0.0/Serializer/constants.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)       38 2023-05-16 22:33:36.975784 CactusSerializer-3.0.0/setup.cfg
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      551 2023-05-16 22:32:23.000000 CactusSerializer-3.0.0/setup.py
```

### Comparing `CactusSerializer-2.0.0/Serializer/JsonDeserializer.py` & `CactusSerializer-3.0.0/Serializer/JsonDeserializer.py`

 * *Files identical despite different names*

### Comparing `CactusSerializer-2.0.0/Serializer/JsonParser.py` & `CactusSerializer-3.0.0/Serializer/JsonParser.py`

 * *Files identical despite different names*

### Comparing `CactusSerializer-2.0.0/Serializer/JsonSerializer.py` & `CactusSerializer-3.0.0/Serializer/JsonSerializer.py`

 * *Files identical despite different names*

### Comparing `CactusSerializer-2.0.0/Serializer/XmlDeserializer.py` & `CactusSerializer-3.0.0/Serializer/XmlDeserializer.py`

 * *Files identical despite different names*

### Comparing `CactusSerializer-2.0.0/Serializer/XmlParser.py` & `CactusSerializer-3.0.0/Serializer/XmlParser.py`

 * *Files identical despite different names*

### Comparing `CactusSerializer-2.0.0/Serializer/XmlSerializer.py` & `CactusSerializer-3.0.0/Serializer/XmlSerializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,20 +139,22 @@
 
 
 def serialize_property(obj, indent, new_indent):
     property_dict = {"property_type": obj.fget}
     result = serialize_dict(property_dict, indent, new_indent)
     return result
 
+
 def get_code_class(obj):
     if obj.__name__ != 'object':
         temp = dict(obj.__dict__)
         for key in list(temp)[:len(temp)-1]:
             if key in EXTRA_ATTRIBUTE_CLASS_CODE:
-                temp.pop(key)
+                if key in temp:
+                    temp.pop(key)
                 continue
             if list(temp)[len(temp)-1] in EXTRA_ATTRIBUTE_CLASS_CODE:
                 temp.pop(list(temp)[len(temp)-1])
         result = temp
     else:
         result = {}
     return result
```

### Comparing `CactusSerializer-2.0.0/setup.py` & `CactusSerializer-3.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CactusSerializer",
-    version="2.0.0",
+    version="3.0.0",
     description="module for serialization/deserialization(JSON, XML)",
     url="https://github.com/Antilevskaya-Ksenia-153501/Python-labs/tree/lab3",
     author="Ksenia Antilevskaya",
     author_email="antikevkun@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
```


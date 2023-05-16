# Comparing `tmp/CactusSerializer-1.0.0.tar.gz` & `tmp/CactusSerializer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CactusSerializer-1.0.0.tar", last modified: Mon May 15 07:07:42 2023, max compression
+gzip compressed data, was "CactusSerializer-2.0.0.tar", last modified: Tue May 16 22:06:21 2023, max compression
```

## Comparing `CactusSerializer-1.0.0.tar` & `CactusSerializer-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-15 07:07:42.270759 CactusSerializer-1.0.0/
-drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-15 07:07:42.198760 CactusSerializer-1.0.0/CactusSerializer.egg-info/
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      405 2023-05-15 07:07:41.000000 CactusSerializer-1.0.0/CactusSerializer.egg-info/PKG-INFO
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      414 2023-05-15 07:07:42.000000 CactusSerializer-1.0.0/CactusSerializer.egg-info/SOURCES.txt
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        1 2023-05-15 07:07:41.000000 CactusSerializer-1.0.0/CactusSerializer.egg-info/dependency_links.txt
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)       11 2023-05-15 07:07:41.000000 CactusSerializer-1.0.0/CactusSerializer.egg-info/top_level.txt
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      405 2023-05-15 07:07:42.270759 CactusSerializer-1.0.0/PKG-INFO
-drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-15 07:07:42.262759 CactusSerializer-1.0.0/Serializer/
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     6013 2023-05-15 06:41:46.000000 CactusSerializer-1.0.0/Serializer/JsonDeserializer.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      721 2023-05-14 09:54:29.000000 CactusSerializer-1.0.0/Serializer/JsonParser.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     7806 2023-05-14 10:20:24.000000 CactusSerializer-1.0.0/Serializer/JsonSerializer.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      388 2023-05-13 14:17:01.000000 CactusSerializer-1.0.0/Serializer/SerializerFactory.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     6158 2023-05-15 06:41:46.000000 CactusSerializer-1.0.0/Serializer/XmlDeserializer.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      750 2023-05-14 09:54:29.000000 CactusSerializer-1.0.0/Serializer/XmlParser.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     7889 2023-05-14 10:20:24.000000 CactusSerializer-1.0.0/Serializer/XmlSerializer.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-14 10:15:55.000000 CactusSerializer-1.0.0/Serializer/__init__.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      306 2023-05-13 11:12:37.000000 CactusSerializer-1.0.0/Serializer/constants.py
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)       38 2023-05-15 07:07:42.270759 CactusSerializer-1.0.0/setup.cfg
--rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      551 2023-05-15 07:07:18.000000 CactusSerializer-1.0.0/setup.py
+drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-16 22:06:21.989162 CactusSerializer-2.0.0/
+drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-16 22:06:21.801163 CactusSerializer-2.0.0/CactusSerializer.egg-info/
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      405 2023-05-16 22:06:21.000000 CactusSerializer-2.0.0/CactusSerializer.egg-info/PKG-INFO
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      414 2023-05-16 22:06:21.000000 CactusSerializer-2.0.0/CactusSerializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        1 2023-05-16 22:06:21.000000 CactusSerializer-2.0.0/CactusSerializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)       11 2023-05-16 22:06:21.000000 CactusSerializer-2.0.0/CactusSerializer.egg-info/top_level.txt
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      405 2023-05-16 22:06:21.989162 CactusSerializer-2.0.0/PKG-INFO
+drwxrwxr-x   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-16 22:06:21.969162 CactusSerializer-2.0.0/Serializer/
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     6100 2023-05-16 22:03:41.000000 CactusSerializer-2.0.0/Serializer/JsonDeserializer.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      721 2023-05-14 09:54:29.000000 CactusSerializer-2.0.0/Serializer/JsonParser.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     8117 2023-05-16 22:03:41.000000 CactusSerializer-2.0.0/Serializer/JsonSerializer.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      388 2023-05-13 14:17:01.000000 CactusSerializer-2.0.0/Serializer/SerializerFactory.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     6245 2023-05-16 22:03:41.000000 CactusSerializer-2.0.0/Serializer/XmlDeserializer.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      750 2023-05-14 09:54:29.000000 CactusSerializer-2.0.0/Serializer/XmlParser.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)     8163 2023-05-16 22:03:41.000000 CactusSerializer-2.0.0/Serializer/XmlSerializer.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)        0 2023-05-14 10:15:55.000000 CactusSerializer-2.0.0/Serializer/__init__.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      306 2023-05-13 11:12:37.000000 CactusSerializer-2.0.0/Serializer/constants.py
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)       38 2023-05-16 22:06:21.989162 CactusSerializer-2.0.0/setup.cfg
+-rw-rw-r--   0 pythonsurvivor  (1000) pythonsurvivor  (1000)      551 2023-05-16 22:03:51.000000 CactusSerializer-2.0.0/setup.py
```

### Comparing `CactusSerializer-1.0.0/Serializer/JsonDeserializer.py` & `CactusSerializer-2.0.0/Serializer/JsonDeserializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,16 @@
             key = True
     if 'function_type' in result:
         result = deserialize_func(result)
     elif 'staticmethod_type' in result:
         result = staticmethod(result['staticmethod_type'])
     elif 'classmethod_type' in result:
         result = classmethod(result['classmethod_type'])
+    elif 'property_type' in result:
+        result = property(result['property_type'])
     elif 'class_type' in result:
         result = deserialize_class(result)
     elif 'type_code' in result:
         result = deserialize_code(result)
     elif 'iter_type' in result:
         result = deserialize_iter(result)
     elif 'builtin_type' in result:
```

### Comparing `CactusSerializer-1.0.0/Serializer/JsonParser.py` & `CactusSerializer-2.0.0/Serializer/JsonParser.py`

 * *Files identical despite different names*

### Comparing `CactusSerializer-1.0.0/Serializer/JsonSerializer.py` & `CactusSerializer-2.0.0/Serializer/JsonSerializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         return serialize_class(obj, indent, new_indent)
     elif inspect.isfunction(obj) or inspect.ismethod(obj):
         return serialize_func(obj, indent, new_indent)
     elif isinstance(obj, staticmethod):
         return serialize_staticmethod(obj, indent, new_indent)
     elif isinstance(obj, classmethod):
         return serialize_classmethod(obj, indent, new_indent)
+    elif isinstance(obj, property):
+        return serialize_property(obj, indent, new_indent)
     elif inspect.isbuiltin(obj):
         return serialize_builtin(obj, indent, new_indent)
     elif isinstance(obj, types.GeneratorType):
         return serialize_iter(obj, indent, new_indent)
     elif inspect.ismodule(obj):
         return serialize_module(obj, indent, new_indent)
     elif hasattr(obj, '__iter__') and hasattr(obj, '__next__'):
@@ -131,20 +133,27 @@
 
 def serialize_classmethod(obj, indent, new_indent):
     classmethod_dict = {"classmethod_type": obj.__func__}
     result = serialize_dict(classmethod_dict, indent, new_indent)
     return result
 
 
+def serialize_property(obj, indent, new_indent):
+    property_dict = {"property_type": obj.fget}
+    result = serialize_dict(property_dict, indent, new_indent)
+    return result
+
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

### Comparing `CactusSerializer-1.0.0/Serializer/XmlDeserializer.py` & `CactusSerializer-2.0.0/Serializer/XmlDeserializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,16 @@
             key = True
     if 'function_type' in result:
         result = deserialize_func(result)
     elif 'staticmethod_type' in result:
         result = staticmethod(result['staticmethod_type'])
     elif 'classmethod_type' in result:
         result = classmethod(result['classmethod_type'])
+    elif 'property_type' in result:
+        result = property(result['property_type'])
     elif 'class_type' in result:
         result = deserialize_class(result)
     elif 'type_code' in result:
         result = deserialize_code(result)
     elif 'iter_type' in result:
         result = deserialize_iter(result)
     elif 'builtin_type' in result:
```

### Comparing `CactusSerializer-1.0.0/Serializer/XmlParser.py` & `CactusSerializer-2.0.0/Serializer/XmlParser.py`

 * *Files identical despite different names*

### Comparing `CactusSerializer-1.0.0/Serializer/XmlSerializer.py` & `CactusSerializer-2.0.0/Serializer/XmlSerializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         return serialize_class(obj, indent, new_indent)
     elif inspect.isfunction(obj) or inspect.ismethod(obj):
         return serialize_func(obj, indent, new_indent)
     elif isinstance(obj, staticmethod):
         return serialize_staticmethod(obj, indent, new_indent)
     elif isinstance(obj, classmethod):
         return serialize_classmethod(obj, indent, new_indent)
+    elif isinstance(obj, property):
+        return serialize_property(obj, indent, new_indent)
     elif inspect.isbuiltin(obj):
         return serialize_builtin(obj, indent, new_indent)
     elif isinstance(obj, types.GeneratorType):
         return serialize_iter(obj, indent, new_indent)
     elif inspect.ismodule(obj):
         return serialize_module(obj, indent, new_indent)
     elif hasattr(obj, '__iter__') and hasattr(obj, '__next__'):
@@ -132,14 +134,19 @@
 
 def serialize_classmethod(obj, indent, new_indent):
     classmethod_dict = {"classmethod_type": obj.__func__}
     result = serialize_dict(classmethod_dict, indent, new_indent)
     return result
 
 
+def serialize_property(obj, indent, new_indent):
+    property_dict = {"property_type": obj.fget}
+    result = serialize_dict(property_dict, indent, new_indent)
+    return result
+
 def get_code_class(obj):
     if obj.__name__ != 'object':
         temp = dict(obj.__dict__)
         for key in list(temp)[:len(temp)-1]:
             if key in EXTRA_ATTRIBUTE_CLASS_CODE:
                 temp.pop(key)
                 continue
```

### Comparing `CactusSerializer-1.0.0/setup.py` & `CactusSerializer-2.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CactusSerializer",
-    version="1.0.0",
+    version="2.0.0",
     description="module for serialization/deserialization(JSON, XML)",
     url="https://github.com/Antilevskaya-Ksenia-153501/Python-labs/tree/lab3",
     author="Ksenia Antilevskaya",
     author_email="antikevkun@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
```


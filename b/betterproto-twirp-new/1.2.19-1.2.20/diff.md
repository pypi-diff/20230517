# Comparing `tmp/betterproto-twirp-new-1.2.19.tar.gz` & `tmp/betterproto-twirp-new-1.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterproto-twirp-new-1.2.19.tar", last modified: Wed May 17 06:57:40 2023, max compression
+gzip compressed data, was "betterproto-twirp-new-1.2.20.tar", last modified: Wed May 17 07:19:45 2023, max compression
```

## Comparing `betterproto-twirp-new-1.2.19.tar` & `betterproto-twirp-new-1.2.20.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:57:40.188923 betterproto-twirp-new-1.2.19/
--rw-r--r--   0 zhouluying   (503) staff       (20)       41 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.19/MANIFEST.in
--rw-r--r--   0 zhouluying   (503) staff       (20)     1062 2023-05-17 06:57:40.188705 betterproto-twirp-new-1.2.19/PKG-INFO
--rw-r--r--   0 zhouluying   (503) staff       (20)      685 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.19/README.md
-drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:57:40.186966 betterproto-twirp-new-1.2.19/betterproto/
--rw-r--r--   0 zhouluying   (503) staff       (20)    40385 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.19/betterproto/__init__.py
--rw-r--r--   0 zhouluying   (503) staff       (20)      322 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.19/betterproto/casing.py
--rwxr-xr-x   0 zhouluying   (503) staff       (20)    17048 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.19/betterproto/plugin.py
--rw-r--r--   0 zhouluying   (503) staff       (20)        0 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.19/betterproto/py.typed
-drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:57:40.187221 betterproto-twirp-new-1.2.19/betterproto/templates/
--rw-r--r--   0 zhouluying   (503) staff       (20)     2656 2023-05-17 06:57:05.000000 betterproto-twirp-new-1.2.19/betterproto/templates/template.py
--rw-r--r--   0 zhouluying   (503) staff       (20)     3265 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.19/betterproto/utils.py
-drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:57:40.188455 betterproto-twirp-new-1.2.19/betterproto_twirp_new.egg-info/
--rw-r--r--   0 zhouluying   (503) staff       (20)     1062 2023-05-17 06:57:40.000000 betterproto-twirp-new-1.2.19/betterproto_twirp_new.egg-info/PKG-INFO
--rw-r--r--   0 zhouluying   (503) staff       (20)      505 2023-05-17 06:57:40.000000 betterproto-twirp-new-1.2.19/betterproto_twirp_new.egg-info/SOURCES.txt
--rw-r--r--   0 zhouluying   (503) staff       (20)        1 2023-05-17 06:57:40.000000 betterproto-twirp-new-1.2.19/betterproto_twirp_new.egg-info/dependency_links.txt
--rw-r--r--   0 zhouluying   (503) staff       (20)       75 2023-05-17 06:57:40.000000 betterproto-twirp-new-1.2.19/betterproto_twirp_new.egg-info/entry_points.txt
--rw-r--r--   0 zhouluying   (503) staff       (20)        1 2023-05-17 06:41:50.000000 betterproto-twirp-new-1.2.19/betterproto_twirp_new.egg-info/not-zip-safe
--rw-r--r--   0 zhouluying   (503) staff       (20)      185 2023-05-17 06:57:40.000000 betterproto-twirp-new-1.2.19/betterproto_twirp_new.egg-info/requires.txt
--rw-r--r--   0 zhouluying   (503) staff       (20)       12 2023-05-17 06:57:40.000000 betterproto-twirp-new-1.2.19/betterproto_twirp_new.egg-info/top_level.txt
--rw-r--r--   0 zhouluying   (503) staff       (20)      165 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.19/pyproject.toml
--rw-r--r--   0 zhouluying   (503) staff       (20)       38 2023-05-17 06:57:40.188973 betterproto-twirp-new-1.2.19/setup.cfg
--rw-r--r--   0 zhouluying   (503) staff       (20)     1134 2023-05-17 06:57:34.000000 betterproto-twirp-new-1.2.19/setup.py
+drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 07:19:45.652183 betterproto-twirp-new-1.2.20/
+-rw-r--r--   0 zhouluying   (503) staff       (20)       41 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.20/MANIFEST.in
+-rw-r--r--   0 zhouluying   (503) staff       (20)     1062 2023-05-17 07:19:45.651863 betterproto-twirp-new-1.2.20/PKG-INFO
+-rw-r--r--   0 zhouluying   (503) staff       (20)      685 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.20/README.md
+drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 07:19:45.643663 betterproto-twirp-new-1.2.20/betterproto/
+-rw-r--r--   0 zhouluying   (503) staff       (20)    40385 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.20/betterproto/__init__.py
+-rw-r--r--   0 zhouluying   (503) staff       (20)      322 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.20/betterproto/casing.py
+-rwxr-xr-x   0 zhouluying   (503) staff       (20)    17048 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.20/betterproto/plugin.py
+-rw-r--r--   0 zhouluying   (503) staff       (20)        0 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.20/betterproto/py.typed
+drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 07:19:45.643929 betterproto-twirp-new-1.2.20/betterproto/templates/
+-rw-r--r--   0 zhouluying   (503) staff       (20)     2649 2023-05-17 07:19:05.000000 betterproto-twirp-new-1.2.20/betterproto/templates/template.py
+-rw-r--r--   0 zhouluying   (503) staff       (20)     3265 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.20/betterproto/utils.py
+drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 07:19:45.651493 betterproto-twirp-new-1.2.20/betterproto_twirp_new.egg-info/
+-rw-r--r--   0 zhouluying   (503) staff       (20)     1062 2023-05-17 07:19:45.000000 betterproto-twirp-new-1.2.20/betterproto_twirp_new.egg-info/PKG-INFO
+-rw-r--r--   0 zhouluying   (503) staff       (20)      505 2023-05-17 07:19:45.000000 betterproto-twirp-new-1.2.20/betterproto_twirp_new.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouluying   (503) staff       (20)        1 2023-05-17 07:19:45.000000 betterproto-twirp-new-1.2.20/betterproto_twirp_new.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouluying   (503) staff       (20)       75 2023-05-17 07:19:45.000000 betterproto-twirp-new-1.2.20/betterproto_twirp_new.egg-info/entry_points.txt
+-rw-r--r--   0 zhouluying   (503) staff       (20)        1 2023-05-17 06:41:50.000000 betterproto-twirp-new-1.2.20/betterproto_twirp_new.egg-info/not-zip-safe
+-rw-r--r--   0 zhouluying   (503) staff       (20)      185 2023-05-17 07:19:45.000000 betterproto-twirp-new-1.2.20/betterproto_twirp_new.egg-info/requires.txt
+-rw-r--r--   0 zhouluying   (503) staff       (20)       12 2023-05-17 07:19:45.000000 betterproto-twirp-new-1.2.20/betterproto_twirp_new.egg-info/top_level.txt
+-rw-r--r--   0 zhouluying   (503) staff       (20)      165 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.20/pyproject.toml
+-rw-r--r--   0 zhouluying   (503) staff       (20)       38 2023-05-17 07:19:45.652240 betterproto-twirp-new-1.2.20/setup.cfg
+-rw-r--r--   0 zhouluying   (503) staff       (20)     1134 2023-05-17 07:19:38.000000 betterproto-twirp-new-1.2.20/setup.py
```

### Comparing `betterproto-twirp-new-1.2.19/PKG-INFO` & `betterproto-twirp-new-1.2.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterproto-twirp-new
-Version: 1.2.19
+Version: 1.2.20
 Summary: A better Protobuf / Twirp generator & library
 Home-page: http://github.com/danielgtaylor/python-betterproto
 Author: lvhaitao, yunshu, fengzhi
 Author-email: zhouluying@bilibili.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `betterproto-twirp-new-1.2.19/README.md` & `betterproto-twirp-new-1.2.20/README.md`

 * *Files identical despite different names*

### Comparing `betterproto-twirp-new-1.2.19/betterproto/__init__.py` & `betterproto-twirp-new-1.2.20/betterproto/__init__.py`

 * *Files identical despite different names*

### Comparing `betterproto-twirp-new-1.2.19/betterproto/plugin.py` & `betterproto-twirp-new-1.2.20/betterproto/plugin.py`

 * *Files identical despite different names*

### Comparing `betterproto-twirp-new-1.2.19/betterproto/templates/template.py` & `betterproto-twirp-new-1.2.20/betterproto/templates/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 {% for service in description.services %}
 class {{ service.py_name }}Stub(betterproto.ServiceStub):
     {% if service.comment %}
 {{ service.comment }}
 
     {% endif %}
     {% for method in service.methods %}
-    @allure.step( {{ method.comment | default_if_none:"no method comment" }} )
+    @allure.step( {{ method.comment | default('no_method_comment') }} )
     def {{ method.py_name }}(self, request: {{ method.input }}) -> {{ method.output }}:
         {% if method.comment %}
 {{ method.comment }}
         {% endif %}
 {% if method.comment %}
         logging.getLogger(__name__).info( "start call "+"[{{ method.py_name }}]"+" api"+"=>"+{{ method.comment }} )
 {% else %}
```

### Comparing `betterproto-twirp-new-1.2.19/betterproto/utils.py` & `betterproto-twirp-new-1.2.20/betterproto/utils.py`

 * *Files identical despite different names*

### Comparing `betterproto-twirp-new-1.2.19/betterproto_twirp_new.egg-info/PKG-INFO` & `betterproto-twirp-new-1.2.20/betterproto_twirp_new.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterproto-twirp-new
-Version: 1.2.19
+Version: 1.2.20
 Summary: A better Protobuf / Twirp generator & library
 Home-page: http://github.com/danielgtaylor/python-betterproto
 Author: lvhaitao, yunshu, fengzhi
 Author-email: zhouluying@bilibili.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `betterproto-twirp-new-1.2.19/setup.py` & `betterproto-twirp-new-1.2.20/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="betterproto-twirp-new",
-    version="1.2.19",
+    version="1.2.20",
     description="A better Protobuf / Twirp generator & library",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/danielgtaylor/python-betterproto",
     author="lvhaitao, yunshu, fengzhi",
     author_email="zhouluying@bilibili.com",
     license="MIT",
```


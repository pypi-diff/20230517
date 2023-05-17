# Comparing `tmp/betterproto-twirp-new-1.2.17.tar.gz` & `tmp/betterproto-twirp-new-1.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterproto-twirp-new-1.2.17.tar", last modified: Wed May 17 06:41:50 2023, max compression
+gzip compressed data, was "betterproto-twirp-new-1.2.18.tar", last modified: Wed May 17 06:54:48 2023, max compression
```

## Comparing `betterproto-twirp-new-1.2.17.tar` & `betterproto-twirp-new-1.2.18.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:41:50.296609 betterproto-twirp-new-1.2.17/
--rw-r--r--   0 zhouluying   (503) staff       (20)       41 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.17/MANIFEST.in
--rw-r--r--   0 zhouluying   (503) staff       (20)     1062 2023-05-17 06:41:50.296434 betterproto-twirp-new-1.2.17/PKG-INFO
--rw-r--r--   0 zhouluying   (503) staff       (20)      685 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.17/README.md
-drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:41:50.294898 betterproto-twirp-new-1.2.17/betterproto/
--rw-r--r--   0 zhouluying   (503) staff       (20)    40385 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.17/betterproto/__init__.py
--rw-r--r--   0 zhouluying   (503) staff       (20)      322 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.17/betterproto/casing.py
--rwxr-xr-x   0 zhouluying   (503) staff       (20)    17048 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.17/betterproto/plugin.py
--rw-r--r--   0 zhouluying   (503) staff       (20)        0 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.17/betterproto/py.typed
-drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:41:50.295186 betterproto-twirp-new-1.2.17/betterproto/templates/
--rw-r--r--   0 zhouluying   (503) staff       (20)     2732 2023-05-17 06:32:33.000000 betterproto-twirp-new-1.2.17/betterproto/templates/template.py
--rw-r--r--   0 zhouluying   (503) staff       (20)     3265 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.17/betterproto/utils.py
-drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:41:50.296236 betterproto-twirp-new-1.2.17/betterproto_twirp_new.egg-info/
--rw-r--r--   0 zhouluying   (503) staff       (20)     1062 2023-05-17 06:41:50.000000 betterproto-twirp-new-1.2.17/betterproto_twirp_new.egg-info/PKG-INFO
--rw-r--r--   0 zhouluying   (503) staff       (20)      505 2023-05-17 06:41:50.000000 betterproto-twirp-new-1.2.17/betterproto_twirp_new.egg-info/SOURCES.txt
--rw-r--r--   0 zhouluying   (503) staff       (20)        1 2023-05-17 06:41:50.000000 betterproto-twirp-new-1.2.17/betterproto_twirp_new.egg-info/dependency_links.txt
--rw-r--r--   0 zhouluying   (503) staff       (20)       75 2023-05-17 06:41:50.000000 betterproto-twirp-new-1.2.17/betterproto_twirp_new.egg-info/entry_points.txt
--rw-r--r--   0 zhouluying   (503) staff       (20)        1 2023-05-17 06:41:50.000000 betterproto-twirp-new-1.2.17/betterproto_twirp_new.egg-info/not-zip-safe
--rw-r--r--   0 zhouluying   (503) staff       (20)      185 2023-05-17 06:41:50.000000 betterproto-twirp-new-1.2.17/betterproto_twirp_new.egg-info/requires.txt
--rw-r--r--   0 zhouluying   (503) staff       (20)       12 2023-05-17 06:41:50.000000 betterproto-twirp-new-1.2.17/betterproto_twirp_new.egg-info/top_level.txt
--rw-r--r--   0 zhouluying   (503) staff       (20)      165 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.17/pyproject.toml
--rw-r--r--   0 zhouluying   (503) staff       (20)       38 2023-05-17 06:41:50.296658 betterproto-twirp-new-1.2.17/setup.cfg
--rw-r--r--   0 zhouluying   (503) staff       (20)     1134 2023-05-17 06:41:41.000000 betterproto-twirp-new-1.2.17/setup.py
+drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:54:48.377633 betterproto-twirp-new-1.2.18/
+-rw-r--r--   0 zhouluying   (503) staff       (20)       41 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.18/MANIFEST.in
+-rw-r--r--   0 zhouluying   (503) staff       (20)     1062 2023-05-17 06:54:48.377439 betterproto-twirp-new-1.2.18/PKG-INFO
+-rw-r--r--   0 zhouluying   (503) staff       (20)      685 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.18/README.md
+drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:54:48.375681 betterproto-twirp-new-1.2.18/betterproto/
+-rw-r--r--   0 zhouluying   (503) staff       (20)    40385 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.18/betterproto/__init__.py
+-rw-r--r--   0 zhouluying   (503) staff       (20)      322 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.18/betterproto/casing.py
+-rwxr-xr-x   0 zhouluying   (503) staff       (20)    17048 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.18/betterproto/plugin.py
+-rw-r--r--   0 zhouluying   (503) staff       (20)        0 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.18/betterproto/py.typed
+drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:54:48.375919 betterproto-twirp-new-1.2.18/betterproto/templates/
+-rw-r--r--   0 zhouluying   (503) staff       (20)     2650 2023-05-17 06:54:26.000000 betterproto-twirp-new-1.2.18/betterproto/templates/template.py
+-rw-r--r--   0 zhouluying   (503) staff       (20)     3265 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.18/betterproto/utils.py
+drwxr-xr-x   0 zhouluying   (503) staff       (20)        0 2023-05-17 06:54:48.377222 betterproto-twirp-new-1.2.18/betterproto_twirp_new.egg-info/
+-rw-r--r--   0 zhouluying   (503) staff       (20)     1062 2023-05-17 06:54:48.000000 betterproto-twirp-new-1.2.18/betterproto_twirp_new.egg-info/PKG-INFO
+-rw-r--r--   0 zhouluying   (503) staff       (20)      505 2023-05-17 06:54:48.000000 betterproto-twirp-new-1.2.18/betterproto_twirp_new.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouluying   (503) staff       (20)        1 2023-05-17 06:54:48.000000 betterproto-twirp-new-1.2.18/betterproto_twirp_new.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouluying   (503) staff       (20)       75 2023-05-17 06:54:48.000000 betterproto-twirp-new-1.2.18/betterproto_twirp_new.egg-info/entry_points.txt
+-rw-r--r--   0 zhouluying   (503) staff       (20)        1 2023-05-17 06:41:50.000000 betterproto-twirp-new-1.2.18/betterproto_twirp_new.egg-info/not-zip-safe
+-rw-r--r--   0 zhouluying   (503) staff       (20)      185 2023-05-17 06:54:48.000000 betterproto-twirp-new-1.2.18/betterproto_twirp_new.egg-info/requires.txt
+-rw-r--r--   0 zhouluying   (503) staff       (20)       12 2023-05-17 06:54:48.000000 betterproto-twirp-new-1.2.18/betterproto_twirp_new.egg-info/top_level.txt
+-rw-r--r--   0 zhouluying   (503) staff       (20)      165 2021-12-12 02:02:31.000000 betterproto-twirp-new-1.2.18/pyproject.toml
+-rw-r--r--   0 zhouluying   (503) staff       (20)       38 2023-05-17 06:54:48.377688 betterproto-twirp-new-1.2.18/setup.cfg
+-rw-r--r--   0 zhouluying   (503) staff       (20)     1134 2023-05-17 06:54:43.000000 betterproto-twirp-new-1.2.18/setup.py
```

### Comparing `betterproto-twirp-new-1.2.17/PKG-INFO` & `betterproto-twirp-new-1.2.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterproto-twirp-new
-Version: 1.2.17
+Version: 1.2.18
 Summary: A better Protobuf / Twirp generator & library
 Home-page: http://github.com/danielgtaylor/python-betterproto
 Author: lvhaitao, yunshu, fengzhi
 Author-email: zhouluying@bilibili.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `betterproto-twirp-new-1.2.17/README.md` & `betterproto-twirp-new-1.2.18/README.md`

 * *Files identical despite different names*

### Comparing `betterproto-twirp-new-1.2.17/betterproto/__init__.py` & `betterproto-twirp-new-1.2.18/betterproto/__init__.py`

 * *Files identical despite different names*

### Comparing `betterproto-twirp-new-1.2.17/betterproto/plugin.py` & `betterproto-twirp-new-1.2.18/betterproto/plugin.py`

 * *Files identical despite different names*

### Comparing `betterproto-twirp-new-1.2.17/betterproto/templates/template.py` & `betterproto-twirp-new-1.2.18/betterproto/templates/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,15 @@
 {% for service in description.services %}
 class {{ service.py_name }}Stub(betterproto.ServiceStub):
     {% if service.comment %}
 {{ service.comment }}
 
     {% endif %}
     {% for method in service.methods %}
-        {% if method.comment is None %}
-            method.comment = "no method comment info"
-        {% endif %}
-    @allure.step( {{ method.comment }} )
+    @allure.step( {{ method.comment  | default: "no method comment" }} )
     def {{ method.py_name }}(self, request: {{ method.input }}) -> {{ method.output }}:
         {% if method.comment %}
 {{ method.comment }}
         {% endif %}
 {% if method.comment %}
         logging.getLogger(__name__).info( "start call "+"[{{ method.py_name }}]"+" api"+"=>"+{{ method.comment }} )
 {% else %}
```

### Comparing `betterproto-twirp-new-1.2.17/betterproto/utils.py` & `betterproto-twirp-new-1.2.18/betterproto/utils.py`

 * *Files identical despite different names*

### Comparing `betterproto-twirp-new-1.2.17/betterproto_twirp_new.egg-info/PKG-INFO` & `betterproto-twirp-new-1.2.18/betterproto_twirp_new.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterproto-twirp-new
-Version: 1.2.17
+Version: 1.2.18
 Summary: A better Protobuf / Twirp generator & library
 Home-page: http://github.com/danielgtaylor/python-betterproto
 Author: lvhaitao, yunshu, fengzhi
 Author-email: zhouluying@bilibili.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `betterproto-twirp-new-1.2.17/setup.py` & `betterproto-twirp-new-1.2.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="betterproto-twirp-new",
-    version="1.2.17",
+    version="1.2.18",
     description="A better Protobuf / Twirp generator & library",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/danielgtaylor/python-betterproto",
     author="lvhaitao, yunshu, fengzhi",
     author_email="zhouluying@bilibili.com",
     license="MIT",
```


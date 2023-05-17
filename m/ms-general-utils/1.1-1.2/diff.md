# Comparing `tmp/ms_general_utils-1.1.tar.gz` & `tmp/ms_general_utils-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_general_utils-1.1.tar", last modified: Tue Apr  4 10:47:38 2023, max compression
+gzip compressed data, was "ms_general_utils-1.2.tar", last modified: Wed May 17 10:40:40 2023, max compression
```

## Comparing `ms_general_utils-1.1.tar` & `ms_general_utils-1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 10:47:38.977857 ms_general_utils-1.1/
--rw-rw-rw-   0        0        0     1073 2023-03-14 11:56:37.000000 ms_general_utils-1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      352 2023-04-04 10:47:38.971863 ms_general_utils-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-03-14 15:40:50.000000 ms_general_utils-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 10:47:38.882679 ms_general_utils-1.1/ms_general_utils.egg-info/
--rw-rw-rw-   0        0        0      352 2023-04-04 10:47:38.000000 ms_general_utils-1.1/ms_general_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-04 10:47:38.000000 ms_general_utils-1.1/ms_general_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 10:47:38.000000 ms_general_utils-1.1/ms_general_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-04 10:47:38.000000 ms_general_utils-1.1/ms_general_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-04 10:47:38.968862 ms_general_utils-1.1/ms_utils/
--rw-rw-rw-   0        0        0      555 2023-03-27 15:14:21.000000 ms_general_utils-1.1/ms_utils/__init__.py
--rw-rw-rw-   0        0        0      386 2023-03-17 12:23:38.000000 ms_general_utils-1.1/ms_utils/abstract_model.py
--rw-rw-rw-   0        0        0     1034 2023-03-17 11:27:17.000000 ms_general_utils-1.1/ms_utils/binary_uuid.py
--rw-rw-rw-   0        0        0      695 2023-03-17 08:52:55.000000 ms_general_utils-1.1/ms_utils/func_date.py
--rw-rw-rw-   0        0        0     2570 2023-04-03 15:04:19.000000 ms_general_utils-1.1/ms_utils/generic_crud_class.py
--rw-rw-rw-   0        0        0      706 2023-03-17 08:52:56.000000 ms_general_utils-1.1/ms_utils/generic_pagination.py
--rw-rw-rw-   0        0        0     1527 2023-04-03 17:16:10.000000 ms_general_utils-1.1/ms_utils/model_utils.py
--rw-rw-rw-   0        0        0      341 2023-03-17 08:52:56.000000 ms_general_utils-1.1/ms_utils/prepare_json_response.py
--rw-rw-rw-   0        0        0      466 2023-04-03 14:47:57.000000 ms_general_utils-1.1/ms_utils/validation_utils.py
--rw-rw-rw-   0        0        0     4253 2023-04-04 10:46:53.000000 ms_general_utils-1.1/ms_utils/view_utils.py
--rw-rw-rw-   0        0        0       42 2023-04-04 10:47:38.978857 ms_general_utils-1.1/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-04-04 10:47:13.000000 ms_general_utils-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:40:40.806660 ms_general_utils-1.2/
+-rw-rw-rw-   0        0        0     1073 2023-03-14 11:56:37.000000 ms_general_utils-1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      352 2023-05-17 10:40:40.805649 ms_general_utils-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-03-14 15:40:50.000000 ms_general_utils-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 10:40:40.764645 ms_general_utils-1.2/ms_general_utils.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-05-17 10:40:40.000000 ms_general_utils-1.2/ms_general_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-05-17 10:40:40.000000 ms_general_utils-1.2/ms_general_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:40:40.000000 ms_general_utils-1.2/ms_general_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 10:40:40.000000 ms_general_utils-1.2/ms_general_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 10:40:40.803652 ms_general_utils-1.2/ms_utils/
+-rw-rw-rw-   0        0        0      555 2023-03-27 15:14:21.000000 ms_general_utils-1.2/ms_utils/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-03-17 12:23:38.000000 ms_general_utils-1.2/ms_utils/abstract_model.py
+-rw-rw-rw-   0        0        0     1034 2023-03-17 11:27:17.000000 ms_general_utils-1.2/ms_utils/binary_uuid.py
+-rw-rw-rw-   0        0        0      695 2023-03-17 08:52:55.000000 ms_general_utils-1.2/ms_utils/func_date.py
+-rw-rw-rw-   0        0        0     2570 2023-04-03 15:04:19.000000 ms_general_utils-1.2/ms_utils/generic_crud_class.py
+-rw-rw-rw-   0        0        0      706 2023-03-17 08:52:56.000000 ms_general_utils-1.2/ms_utils/generic_pagination.py
+-rw-rw-rw-   0        0        0     1527 2023-04-03 17:16:10.000000 ms_general_utils-1.2/ms_utils/model_utils.py
+-rw-rw-rw-   0        0        0      341 2023-03-17 08:52:56.000000 ms_general_utils-1.2/ms_utils/prepare_json_response.py
+-rw-rw-rw-   0        0        0      466 2023-04-03 14:47:57.000000 ms_general_utils-1.2/ms_utils/validation_utils.py
+-rw-rw-rw-   0        0        0     4232 2023-05-17 10:37:49.000000 ms_general_utils-1.2/ms_utils/view_utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 10:40:40.807651 ms_general_utils-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      674 2023-05-17 10:40:15.000000 ms_general_utils-1.2/setup.py
```

### Comparing `ms_general_utils-1.1/LICENSE.txt` & `ms_general_utils-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.1/ms_utils/__init__.py` & `ms_general_utils-1.2/ms_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.1/ms_utils/binary_uuid.py` & `ms_general_utils-1.2/ms_utils/binary_uuid.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.1/ms_utils/func_date.py` & `ms_general_utils-1.2/ms_utils/func_date.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.1/ms_utils/generic_crud_class.py` & `ms_general_utils-1.2/ms_utils/generic_crud_class.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.1/ms_utils/generic_pagination.py` & `ms_general_utils-1.2/ms_utils/generic_pagination.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.1/ms_utils/model_utils.py` & `ms_general_utils-1.2/ms_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.1/ms_utils/view_utils.py` & `ms_general_utils-1.2/ms_utils/view_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,23 @@
     db = None
 
     def __int__(self, ma, app, db):
         self.db = db
         self.ma = ma
         self.ma.init_app(app)
 
-    def generic_list(self, model, schema):
+    def generic_list(self, model, schema, **kwargs):
         """
         Generic list
         :return: jsonify
         """
         page = int(request.args.get('page')) if request.args.get('page') else 1
         per_page = int(request.args.get('per_page')) if request.args.get('per_page') else 10
 
-        query = model.query.filter(model.name.contains(request.args.get('q'))) \
+        query = model.query.filter_by(**kwargs) \
             .paginate(page=page, per_page=per_page) if request.args.get(
             'q') else model.query.paginate(page=page, per_page=per_page)
         query.items = generic_get_serialize_data(schema(many=True), query.items)
         data = generic_get_serialize_data(
             PaginationSchema(self.ma, current_app, schema(many=True)).pagination_sub_class, query)
 
         return prepare_json_response(f'{model.__name__} get successfully', data=data)
```

### Comparing `ms_general_utils-1.1/setup.py` & `ms_general_utils-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ms_general_utils',
     packages=find_packages(),
     include_package_data=True,
-    version='1.1',
+    version='1.2',
     description='General functions for the implementation of microservices.',
     authors=[
         {"name": "Alejandro A. Serrano Correa", "email": "alejandroasc93@gmail.com"},
         {"name": "Rene Gonzalez Ramos", "email": "rgramos9310@gmail.com"}
     ],
     license="GPLv3",
     url="https://github.com/rgramos/ms-utils.git",
```


# Comparing `tmp/django-excel-importer-0.1.1.tar.gz` & `tmp/django-excel-importer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-excel-importer-0.1.1.tar", last modified: Mon May 15 09:24:30 2023, max compression
+gzip compressed data, was "django-excel-importer-0.1.2.tar", last modified: Wed May 17 05:19:59 2023, max compression
```

## Comparing `django-excel-importer-0.1.1.tar` & `django-excel-importer-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hubertshelley   (501) staff       (20)        0 2023-05-15 09:24:30.922539 django-excel-importer-0.1.1/
--rw-r--r--   0 hubertshelley   (501) staff       (20)      644 2023-05-15 09:24:30.922401 django-excel-importer-0.1.1/PKG-INFO
-drwxr-xr-x   0 hubertshelley   (501) staff       (20)        0 2023-05-15 09:24:30.920964 django-excel-importer-0.1.1/django_excel_importer.egg-info/
--rw-r--r--   0 hubertshelley   (501) staff       (20)      644 2023-05-15 09:24:30.000000 django-excel-importer-0.1.1/django_excel_importer.egg-info/PKG-INFO
--rw-r--r--   0 hubertshelley   (501) staff       (20)      319 2023-05-15 09:24:30.000000 django-excel-importer-0.1.1/django_excel_importer.egg-info/SOURCES.txt
--rw-r--r--   0 hubertshelley   (501) staff       (20)        1 2023-05-15 09:24:30.000000 django-excel-importer-0.1.1/django_excel_importer.egg-info/dependency_links.txt
--rw-r--r--   0 hubertshelley   (501) staff       (20)       36 2023-05-15 09:24:30.000000 django-excel-importer-0.1.1/django_excel_importer.egg-info/requires.txt
--rw-r--r--   0 hubertshelley   (501) staff       (20)        9 2023-05-15 09:24:30.000000 django-excel-importer-0.1.1/django_excel_importer.egg-info/top_level.txt
-drwxr-xr-x   0 hubertshelley   (501) staff       (20)        0 2023-05-15 09:24:30.921978 django-excel-importer-0.1.1/importer/
--rw-r--r--   0 hubertshelley   (501) staff       (20)      203 2023-04-17 08:10:13.000000 django-excel-importer-0.1.1/importer/__init__.py
--rw-r--r--   0 hubertshelley   (501) staff       (20)     1648 2023-05-15 05:31:03.000000 django-excel-importer-0.1.1/importer/exception.py
--rw-r--r--   0 hubertshelley   (501) staff       (20)    11794 2023-05-15 06:42:40.000000 django-excel-importer-0.1.1/importer/importer.py
--rw-r--r--   0 hubertshelley   (501) staff       (20)      372 2023-04-17 05:27:34.000000 django-excel-importer-0.1.1/importer/serializer.py
--rw-r--r--   0 hubertshelley   (501) staff       (20)       38 2023-05-15 09:24:30.922675 django-excel-importer-0.1.1/setup.cfg
--rw-r--r--   0 hubertshelley   (501) staff       (20)     4016 2023-05-15 09:24:03.000000 django-excel-importer-0.1.1/setup.py
+drwxr-xr-x   0 hubertshelley   (501) staff       (20)        0 2023-05-17 05:19:59.179935 django-excel-importer-0.1.2/
+-rw-r--r--   0 hubertshelley   (501) staff       (20)      644 2023-05-17 05:19:59.179814 django-excel-importer-0.1.2/PKG-INFO
+drwxr-xr-x   0 hubertshelley   (501) staff       (20)        0 2023-05-17 05:19:59.178492 django-excel-importer-0.1.2/django_excel_importer.egg-info/
+-rw-r--r--   0 hubertshelley   (501) staff       (20)      644 2023-05-17 05:19:59.000000 django-excel-importer-0.1.2/django_excel_importer.egg-info/PKG-INFO
+-rw-r--r--   0 hubertshelley   (501) staff       (20)      319 2023-05-17 05:19:59.000000 django-excel-importer-0.1.2/django_excel_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 hubertshelley   (501) staff       (20)        1 2023-05-17 05:19:59.000000 django-excel-importer-0.1.2/django_excel_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 hubertshelley   (501) staff       (20)       36 2023-05-17 05:19:59.000000 django-excel-importer-0.1.2/django_excel_importer.egg-info/requires.txt
+-rw-r--r--   0 hubertshelley   (501) staff       (20)        9 2023-05-17 05:19:59.000000 django-excel-importer-0.1.2/django_excel_importer.egg-info/top_level.txt
+drwxr-xr-x   0 hubertshelley   (501) staff       (20)        0 2023-05-17 05:19:59.179414 django-excel-importer-0.1.2/importer/
+-rw-r--r--   0 hubertshelley   (501) staff       (20)      203 2023-04-17 08:10:13.000000 django-excel-importer-0.1.2/importer/__init__.py
+-rw-r--r--   0 hubertshelley   (501) staff       (20)     1648 2023-05-15 05:31:03.000000 django-excel-importer-0.1.2/importer/exception.py
+-rw-r--r--   0 hubertshelley   (501) staff       (20)    11975 2023-05-17 05:18:26.000000 django-excel-importer-0.1.2/importer/importer.py
+-rw-r--r--   0 hubertshelley   (501) staff       (20)      372 2023-04-17 05:27:34.000000 django-excel-importer-0.1.2/importer/serializer.py
+-rw-r--r--   0 hubertshelley   (501) staff       (20)       38 2023-05-17 05:19:59.180064 django-excel-importer-0.1.2/setup.cfg
+-rw-r--r--   0 hubertshelley   (501) staff       (20)     4016 2023-05-17 05:18:35.000000 django-excel-importer-0.1.2/setup.py
```

### Comparing `django-excel-importer-0.1.1/PKG-INFO` & `django-excel-importer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-excel-importer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django Excel 导入到项目.
 Home-page: https://github.com/hubertshelley
 Author: Hubert Shelley
 Author-email: hubertshelley@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `django-excel-importer-0.1.1/django_excel_importer.egg-info/PKG-INFO` & `django-excel-importer-0.1.2/django_excel_importer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-excel-importer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django Excel 导入到项目.
 Home-page: https://github.com/hubertshelley
 Author: Hubert Shelley
 Author-email: hubertshelley@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `django-excel-importer-0.1.1/importer/exception.py` & `django-excel-importer-0.1.2/importer/exception.py`

 * *Files identical despite different names*

### Comparing `django-excel-importer-0.1.1/importer/importer.py` & `django-excel-importer-0.1.2/importer/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,18 @@
                 if custom_head_dict[key] in self.model_fields_dict.keys():
                     self.model_fields_dict[custom_head_dict[key]] = key
                     continue
                 field_name = key.split('.')[0]
                 if field_name in self.model_fields_dict.values():
                     for k, v in self.model_fields_dict.items():
                         if v == field_name:
-                            self.model_fields_dict[k] = key
+                            if custom_head_dict[key] == k:
+                                self.model_fields_dict[k] = key
+                            else:
+                                self.model_fields_dict[custom_head_dict[key]] = key
                             break
         self.model_fields_dict_index = {v: k for k, v in self.model_fields_dict.items()}
 
     def clean_data(self, data):
         """
         清洗数据
         :param data:
```

### Comparing `django-excel-importer-0.1.1/setup.py` & `django-excel-importer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # Package meta-data.
 NAME = 'django-excel-importer'
 DESCRIPTION = 'Django Excel 导入到项目.'
 URL = 'https://github.com/hubertshelley'
 EMAIL = 'hubertshelley@163.com'
 AUTHOR = 'Hubert Shelley'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'Django',
     'djangorestframework',
     'openpyxl',
 ]
```


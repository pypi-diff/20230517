# Comparing `tmp/spswarehouse_airflow-0.2.0.tar.gz` & `tmp/spswarehouse_airflow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spswarehouse_airflow-0.2.0.tar", last modified: Tue May  9 16:15:05 2023, max compression
+gzip compressed data, was "spswarehouse_airflow-0.2.1.tar", last modified: Wed May 17 18:28:18 2023, max compression
```

## Comparing `spswarehouse_airflow-0.2.0.tar` & `spswarehouse_airflow-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 16:15:05.909099 spswarehouse_airflow-0.2.0/
--rw-rw-rw-   0        0        0    35823 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      448 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2034 2023-05-09 16:15:05.907088 spswarehouse_airflow-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1634 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 16:15:05.909099 spswarehouse_airflow-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-05-09 16:12:13.000000 spswarehouse_airflow-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:15:05.888659 spswarehouse_airflow-0.2.0/spswarehouse_airflow/
--rw-rw-rw-   0        0        0      548 2022-12-20 21:53:23.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-05-09 15:37:21.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/calpads.py
--rw-rw-rw-   0        0        0     2326 2022-12-23 15:26:09.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/googledrive.py
--rw-rw-rw-   0        0        0     1556 2022-12-23 15:26:16.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/googlesheets.py
--rw-rw-rw-   0        0        0     1374 2022-12-23 15:26:22.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/googleslides.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:15:05.904087 spswarehouse_airflow-0.2.0/spswarehouse_airflow/powerschool/
--rw-rw-rw-   0        0        0        0 2023-05-09 15:51:57.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/powerschool/__init__.py
--rw-rw-rw-   0        0        0     1112 2023-05-08 21:52:17.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/powerschool/powerschool.py
--rw-rw-rw-   0        0        0      989 2023-05-09 15:56:21.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/powerschool/powerschool_calpads.py
--rw-rw-rw-   0        0        0     1271 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/table_names.py
--rw-rw-rw-   0        0        0     7195 2023-01-05 16:34:44.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/table_utils.py
--rw-rw-rw-   0        0        0     4978 2022-12-23 15:33:36.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/warehouse.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:15:05.897739 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/
--rw-rw-rw-   0        0        0     2034 2023-05-09 16:15:05.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      687 2023-05-09 16:15:05.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 16:15:05.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      225 2023-05-09 16:15:05.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-09 16:15:05.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 18:28:18.980305 spswarehouse_airflow-0.2.1/
+-rw-rw-rw-   0        0        0    35823 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      448 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2034 2023-05-17 18:28:18.979640 spswarehouse_airflow-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1634 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 18:28:18.980824 spswarehouse_airflow-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-05-17 18:24:26.000000 spswarehouse_airflow-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:28:18.964550 spswarehouse_airflow-0.2.1/spswarehouse_airflow/
+-rw-rw-rw-   0        0        0      548 2022-12-20 21:53:23.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-05-17 17:34:00.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/calpads.py
+-rw-rw-rw-   0        0        0     2326 2022-12-23 15:26:09.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/googledrive.py
+-rw-rw-rw-   0        0        0     1556 2022-12-23 15:26:16.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/googlesheets.py
+-rw-rw-rw-   0        0        0     1374 2022-12-23 15:26:22.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/googleslides.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:28:18.976889 spswarehouse_airflow-0.2.1/spswarehouse_airflow/powerschool/
+-rw-rw-rw-   0        0        0        0 2023-05-09 15:51:57.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/powerschool/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-05-08 21:52:17.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/powerschool/powerschool.py
+-rw-rw-rw-   0        0        0      989 2023-05-09 15:56:21.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/powerschool/powerschool_calpads.py
+-rw-rw-rw-   0        0        0     1271 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/table_names.py
+-rw-rw-rw-   0        0        0     7195 2023-01-05 16:34:44.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/table_utils.py
+-rw-rw-rw-   0        0        0     4978 2022-12-23 15:33:36.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow/warehouse.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:28:18.972888 spswarehouse_airflow-0.2.1/spswarehouse_airflow.egg-info/
+-rw-rw-rw-   0        0        0     2034 2023-05-17 18:28:18.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      687 2023-05-17 18:28:18.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 18:28:18.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      243 2023-05-17 18:28:18.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-17 18:28:18.000000 spswarehouse_airflow-0.2.1/spswarehouse_airflow.egg-info/top_level.txt
```

### Comparing `spswarehouse_airflow-0.2.0/LICENSE` & `spswarehouse_airflow-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/PKG-INFO` & `spswarehouse_airflow-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse_airflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Summit Public Schools Snowflake warehouse for use in Airflow
 Home-page: https://github.com/SummitPublicSchools/spswarehouse_airflow
 Author: Harry Li Consulting, LLC
 Author-email: hcli.consulting@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse_airflow-0.2.0/README.md` & `spswarehouse_airflow-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/setup.py` & `spswarehouse_airflow-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spswarehouse_airflow",
-    version="0.2.0",
+    version="0.2.1",
     author="Harry Li Consulting, LLC",
     author_email="hcli.consulting@gmail.com",
     description="Summit Public Schools Snowflake warehouse for use in Airflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SummitPublicSchools/spswarehouse_airflow",
     packages=setuptools.find_packages(),
@@ -24,11 +24,12 @@
         'SQLAlchemy==1.4.44',
         'snowflake-sqlalchemy==1.4.4',
         'google-api-python-client==1.12.11',
         'google-auth-httplib2==0.1.0',
         'google-auth-oauthlib==0.7.1',
         'gspread==5.7.2',
         'PyDrive2==1.15.0',
-        'spswarehouse>=0.1.1',
+        'spswarehouse>=0.2.0',
+        'duct-tape>=0.26.0',
         'apache-airflow<=2.5.0',
     ]
 )
```

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow/__init__.py` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow/calpads.py` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow/calpads.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from airflow.hooks.base_hook import BaseHook
-from spswarehouse.calpads import CALPADS as BaseCalpads
+from spswarehouse.calpads.calpads import CALPADS as BaseCalpads
 
 default_conn_id = 'calpads_ui'
 
 class CALPADS(BaseCalpads):
     """
     Wrapper class for the spswarehouse CALPADS class that
     handles retrieving credentials from Airflow connection
```

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow/googledrive.py` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow/googledrive.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow/googlesheets.py` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow/googlesheets.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow/googleslides.py` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow/googleslides.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow/powerschool/powerschool.py` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow/powerschool/powerschool.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow/powerschool/powerschool_calpads.py` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow/powerschool/powerschool_calpads.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow/table_names.py` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow/table_names.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow/table_utils.py` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow/table_utils.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow/warehouse.py` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow/warehouse.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/PKG-INFO` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse-airflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Summit Public Schools Snowflake warehouse for use in Airflow
 Home-page: https://github.com/SummitPublicSchools/spswarehouse_airflow
 Author: Harry Li Consulting, LLC
 Author-email: hcli.consulting@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/SOURCES.txt` & `spswarehouse_airflow-0.2.1/spswarehouse_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*


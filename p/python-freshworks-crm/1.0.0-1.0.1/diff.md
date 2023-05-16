# Comparing `tmp/python-freshworks-crm-1.0.0.tar.gz` & `tmp/python-freshworks-crm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-freshworks-crm-1.0.0.tar", last modified: Tue May 16 21:02:11 2023, max compression
+gzip compressed data, was "dist\python-freshworks-crm-1.0.1.tar", last modified: Tue May 16 21:16:58 2023, max compression
```

## Comparing `python-freshworks-crm-1.0.0.tar` & `python-freshworks-crm-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/freshsales/
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:26.000000 python-freshworks-crm-1.0.0/freshsales/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/freshsales/v2/
--rw-rw-rw-   0        0        0    36110 2023-05-16 20:10:47.000000 python-freshworks-crm-1.0.0/freshsales/v2/api.py
--rw-rw-rw-   0        0        0      672 2023-05-06 14:43:54.000000 python-freshworks-crm-1.0.0/freshsales/v2/errors.py
--rw-rw-rw-   0        0        0     6751 2023-05-16 19:48:06.000000 python-freshworks-crm-1.0.0/freshsales/v2/models.py
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:11.000000 python-freshworks-crm-1.0.0/freshsales/v2/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-16 20:02:39.000000 python-freshworks-crm-1.0.0/freshsales/__init__.py
--rw-rw-rw-   0        0        0      842 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/python_freshworks_crm.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/python_freshworks_crm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      842 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/python_freshworks_crm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       40 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/python_freshworks_crm.egg-info/requires.txt
--rw-rw-rw-   0        0        0      666 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/python_freshworks_crm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/python_freshworks_crm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1128 2023-05-16 20:57:21.000000 python-freshworks-crm-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:02:11.000000 python-freshworks-crm-1.0.0/tests/
--rw-rw-rw-   0        0        0     7914 2023-05-16 19:03:28.000000 python-freshworks-crm-1.0.0/tests/conftest.py
--rw-rw-rw-   0        0        0     3549 2023-05-13 23:26:20.000000 python-freshworks-crm-1.0.0/tests/test_accounts.py
--rw-rw-rw-   0        0        0     2711 2023-05-16 11:24:32.000000 python-freshworks-crm-1.0.0/tests/test_appointments.py
--rw-rw-rw-   0        0        0     3567 2023-05-13 23:26:09.000000 python-freshworks-crm-1.0.0/tests/test_contacts.py
--rw-rw-rw-   0        0        0     3368 2023-05-16 15:02:47.000000 python-freshworks-crm-1.0.0/tests/test_deals.py
--rw-rw-rw-   0        0        0     3344 2023-05-16 19:06:03.000000 python-freshworks-crm-1.0.0/tests/test_documents.py
--rw-rw-rw-   0        0        0     2422 2023-05-14 12:53:28.000000 python-freshworks-crm-1.0.0/tests/test_lists.py
--rw-rw-rw-   0        0        0     1727 2023-05-14 13:16:40.000000 python-freshworks-crm-1.0.0/tests/test_notes.py
--rw-rw-rw-   0        0        0     4032 2023-05-16 15:03:28.000000 python-freshworks-crm-1.0.0/tests/test_products.py
--rw-rw-rw-   0        0        0     2907 2023-05-16 19:05:03.000000 python-freshworks-crm-1.0.0/tests/test_sales_activities.py
--rw-rw-rw-   0        0        0     6561 2023-05-14 20:08:32.000000 python-freshworks-crm-1.0.0/tests/test_selectors.py
--rw-rw-rw-   0        0        0     3241 2023-05-15 01:49:25.000000 python-freshworks-crm-1.0.0/tests/test_tasks.py
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:43.000000 python-freshworks-crm-1.0.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:16:58.000000 python-freshworks-crm-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:16:58.000000 python-freshworks-crm-1.0.1/freshsales/
+-rw-rw-rw-   0        0        0        0 2023-05-06 00:00:26.000000 python-freshworks-crm-1.0.1/freshsales/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:16:58.000000 python-freshworks-crm-1.0.1/freshsales/v2/
+-rw-rw-rw-   0        0        0    36110 2023-05-16 20:10:47.000000 python-freshworks-crm-1.0.1/freshsales/v2/api.py
+-rw-rw-rw-   0        0        0      672 2023-05-06 14:43:54.000000 python-freshworks-crm-1.0.1/freshsales/v2/errors.py
+-rw-rw-rw-   0        0        0     6751 2023-05-16 19:48:06.000000 python-freshworks-crm-1.0.1/freshsales/v2/models.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 00:00:11.000000 python-freshworks-crm-1.0.1/freshsales/v2/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-16 21:16:06.000000 python-freshworks-crm-1.0.1/freshsales/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 20:08:52.000000 python-freshworks-crm-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      878 2023-05-16 21:16:58.000000 python-freshworks-crm-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 21:16:58.000000 python-freshworks-crm-1.0.1/python_freshworks_crm.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-16 21:16:57.000000 python-freshworks-crm-1.0.1/python_freshworks_crm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      878 2023-05-16 21:16:57.000000 python-freshworks-crm-1.0.1/python_freshworks_crm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2023-05-16 21:16:57.000000 python-freshworks-crm-1.0.1/python_freshworks_crm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      684 2023-05-16 21:16:58.000000 python-freshworks-crm-1.0.1/python_freshworks_crm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-05-16 21:16:58.000000 python-freshworks-crm-1.0.1/python_freshworks_crm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      443 2023-05-16 19:56:20.000000 python-freshworks-crm-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 21:16:58.000000 python-freshworks-crm-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2023-05-16 21:11:52.000000 python-freshworks-crm-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:16:58.000000 python-freshworks-crm-1.0.1/tests/
+-rw-rw-rw-   0        0        0     7914 2023-05-16 19:03:28.000000 python-freshworks-crm-1.0.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     3549 2023-05-13 23:26:20.000000 python-freshworks-crm-1.0.1/tests/test_accounts.py
+-rw-rw-rw-   0        0        0     2711 2023-05-16 11:24:32.000000 python-freshworks-crm-1.0.1/tests/test_appointments.py
+-rw-rw-rw-   0        0        0     3567 2023-05-13 23:26:09.000000 python-freshworks-crm-1.0.1/tests/test_contacts.py
+-rw-rw-rw-   0        0        0     3368 2023-05-16 15:02:47.000000 python-freshworks-crm-1.0.1/tests/test_deals.py
+-rw-rw-rw-   0        0        0     3344 2023-05-16 19:06:03.000000 python-freshworks-crm-1.0.1/tests/test_documents.py
+-rw-rw-rw-   0        0        0     2422 2023-05-14 12:53:28.000000 python-freshworks-crm-1.0.1/tests/test_lists.py
+-rw-rw-rw-   0        0        0     1727 2023-05-14 13:16:40.000000 python-freshworks-crm-1.0.1/tests/test_notes.py
+-rw-rw-rw-   0        0        0     4032 2023-05-16 15:03:28.000000 python-freshworks-crm-1.0.1/tests/test_products.py
+-rw-rw-rw-   0        0        0     2907 2023-05-16 19:05:03.000000 python-freshworks-crm-1.0.1/tests/test_sales_activities.py
+-rw-rw-rw-   0        0        0     6561 2023-05-14 20:08:32.000000 python-freshworks-crm-1.0.1/tests/test_selectors.py
+-rw-rw-rw-   0        0        0     3241 2023-05-15 01:49:25.000000 python-freshworks-crm-1.0.1/tests/test_tasks.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 00:00:43.000000 python-freshworks-crm-1.0.1/tests/__init__.py
```

### Comparing `python-freshworks-crm-1.0.0/freshsales/v2/api.py` & `python-freshworks-crm-1.0.1/freshsales/v2/api.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/freshsales/v2/errors.py` & `python-freshworks-crm-1.0.1/freshsales/v2/errors.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/freshsales/v2/models.py` & `python-freshworks-crm-1.0.1/freshsales/v2/models.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/PKG-INFO` & `python-freshworks-crm-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: python-freshworks-crm
-Version: 1.0.0
+Version: 1.0.1
 Summary: An API wrapper for the Freshsales CRM
 Home-page: https://github.com/robertvy/python-freshworksCRM
 Author: Robert Van Ysendyck
 Author-email: rvy@vyp-consulting.com
 License: BSD
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `python-freshworks-crm-1.0.0/python_freshworks_crm.egg-info/PKG-INFO` & `python-freshworks-crm-1.0.1/python_freshworks_crm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: python-freshworks-crm
-Version: 1.0.0
+Version: 1.0.1
 Summary: An API wrapper for the Freshsales CRM
 Home-page: https://github.com/robertvy/python-freshworksCRM
 Author: Robert Van Ysendyck
 Author-email: rvy@vyp-consulting.com
 License: BSD
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `python-freshworks-crm-1.0.0/python_freshworks_crm.egg-info/SOURCES.txt` & `python-freshworks-crm-1.0.1/python_freshworks_crm.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+README.md
 setup.py
 freshsales/__init__.py
 freshsales/exceptions.py
 freshsales/v2/__init__.py
 freshsales/v2/api.py
 freshsales/v2/errors.py
 freshsales/v2/models.py
```

### Comparing `python-freshworks-crm-1.0.0/setup.py` & `python-freshworks-crm-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/conftest.py` & `python-freshworks-crm-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_accounts.py` & `python-freshworks-crm-1.0.1/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_appointments.py` & `python-freshworks-crm-1.0.1/tests/test_appointments.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_contacts.py` & `python-freshworks-crm-1.0.1/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_deals.py` & `python-freshworks-crm-1.0.1/tests/test_deals.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_documents.py` & `python-freshworks-crm-1.0.1/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_lists.py` & `python-freshworks-crm-1.0.1/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_notes.py` & `python-freshworks-crm-1.0.1/tests/test_notes.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_products.py` & `python-freshworks-crm-1.0.1/tests/test_products.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_sales_activities.py` & `python-freshworks-crm-1.0.1/tests/test_sales_activities.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_selectors.py` & `python-freshworks-crm-1.0.1/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.0/tests/test_tasks.py` & `python-freshworks-crm-1.0.1/tests/test_tasks.py`

 * *Files identical despite different names*


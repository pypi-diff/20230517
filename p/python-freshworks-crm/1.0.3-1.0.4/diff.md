# Comparing `tmp/python-freshworks-crm-1.0.3.tar.gz` & `tmp/python-freshworks-crm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-freshworks-crm-1.0.3.tar", last modified: Tue May 16 22:42:10 2023, max compression
+gzip compressed data, was "dist\python-freshworks-crm-1.0.4.tar", last modified: Wed May 17 17:51:13 2023, max compression
```

## Comparing `python-freshworks-crm-1.0.3.tar` & `python-freshworks-crm-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 22:42:10.000000 python-freshworks-crm-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-16 22:42:09.000000 python-freshworks-crm-1.0.3/freshsales/
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:26.000000 python-freshworks-crm-1.0.3/freshsales/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:42:09.000000 python-freshworks-crm-1.0.3/freshsales/v2/
--rw-rw-rw-   0        0        0    36110 2023-05-16 22:21:19.000000 python-freshworks-crm-1.0.3/freshsales/v2/api.py
--rw-rw-rw-   0        0        0      672 2023-05-06 14:43:54.000000 python-freshworks-crm-1.0.3/freshsales/v2/errors.py
--rw-rw-rw-   0        0        0     6751 2023-05-16 19:48:06.000000 python-freshworks-crm-1.0.3/freshsales/v2/models.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:42:10.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/
--rw-rw-rw-   0        0        0     7914 2023-05-16 19:03:28.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/conftest.py
--rw-rw-rw-   0        0        0     3549 2023-05-13 23:26:20.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_accounts.py
--rw-rw-rw-   0        0        0     2711 2023-05-16 11:24:32.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_appointments.py
--rw-rw-rw-   0        0        0     3567 2023-05-13 23:26:09.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_contacts.py
--rw-rw-rw-   0        0        0     3368 2023-05-16 15:02:47.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_deals.py
--rw-rw-rw-   0        0        0     3344 2023-05-16 19:06:03.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_documents.py
--rw-rw-rw-   0        0        0     2422 2023-05-14 12:53:28.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_lists.py
--rw-rw-rw-   0        0        0     1727 2023-05-14 13:16:40.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_notes.py
--rw-rw-rw-   0        0        0     4032 2023-05-16 15:03:28.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_products.py
--rw-rw-rw-   0        0        0     2907 2023-05-16 19:05:03.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_sales_activities.py
--rw-rw-rw-   0        0        0     6561 2023-05-14 20:08:32.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_selectors.py
--rw-rw-rw-   0        0        0     3241 2023-05-15 01:49:25.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/test_tasks.py
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:43.000000 python-freshworks-crm-1.0.3/freshsales/v2/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:11.000000 python-freshworks-crm-1.0.3/freshsales/v2/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-16 22:41:36.000000 python-freshworks-crm-1.0.3/freshsales/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-05-16 20:08:52.000000 python-freshworks-crm-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      878 2023-05-16 22:42:10.000000 python-freshworks-crm-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 22:42:10.000000 python-freshworks-crm-1.0.3/python_freshworks_crm.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-16 22:42:09.000000 python-freshworks-crm-1.0.3/python_freshworks_crm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      878 2023-05-16 22:42:09.000000 python-freshworks-crm-1.0.3/python_freshworks_crm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-05-16 22:42:09.000000 python-freshworks-crm-1.0.3/python_freshworks_crm.egg-info/requires.txt
--rw-rw-rw-   0        0        0      866 2023-05-16 22:42:09.000000 python-freshworks-crm-1.0.3/python_freshworks_crm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 22:42:09.000000 python-freshworks-crm-1.0.3/python_freshworks_crm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      443 2023-05-16 19:56:20.000000 python-freshworks-crm-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 22:42:10.000000 python-freshworks-crm-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-05-16 22:04:30.000000 python-freshworks-crm-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/freshsales/
+-rw-rw-rw-   0        0        0        0 2023-05-06 00:00:26.000000 python-freshworks-crm-1.0.4/freshsales/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/freshsales/v2/
+-rw-rw-rw-   0        0        0    36122 2023-05-17 17:15:40.000000 python-freshworks-crm-1.0.4/freshsales/v2/api.py
+-rw-rw-rw-   0        0        0      672 2023-05-06 14:43:54.000000 python-freshworks-crm-1.0.4/freshsales/v2/errors.py
+-rw-rw-rw-   0        0        0     6751 2023-05-16 19:48:06.000000 python-freshworks-crm-1.0.4/freshsales/v2/models.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/
+-rw-rw-rw-   0        0        0     7914 2023-05-16 19:03:28.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/conftest.py
+-rw-rw-rw-   0        0        0     3549 2023-05-13 23:26:20.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_accounts.py
+-rw-rw-rw-   0        0        0     2711 2023-05-16 11:24:32.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_appointments.py
+-rw-rw-rw-   0        0        0     3567 2023-05-13 23:26:09.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_contacts.py
+-rw-rw-rw-   0        0        0     3368 2023-05-16 15:02:47.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_deals.py
+-rw-rw-rw-   0        0        0     3344 2023-05-16 19:06:03.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_documents.py
+-rw-rw-rw-   0        0        0     2422 2023-05-14 12:53:28.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_lists.py
+-rw-rw-rw-   0        0        0     1727 2023-05-14 13:16:40.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_notes.py
+-rw-rw-rw-   0        0        0     4032 2023-05-16 15:03:28.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_products.py
+-rw-rw-rw-   0        0        0     2907 2023-05-16 19:05:03.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_sales_activities.py
+-rw-rw-rw-   0        0        0     6561 2023-05-14 20:08:32.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_selectors.py
+-rw-rw-rw-   0        0        0     3241 2023-05-15 01:49:25.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_tasks.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 00:00:43.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 00:00:11.000000 python-freshworks-crm-1.0.4/freshsales/v2/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-17 17:50:50.000000 python-freshworks-crm-1.0.4/freshsales/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 20:08:52.000000 python-freshworks-crm-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      878 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-17 17:51:12.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      878 2023-05-17 17:51:12.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-05-17 17:51:12.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      866 2023-05-17 17:51:12.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2023-05-17 17:51:12.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      443 2023-05-16 19:56:20.000000 python-freshworks-crm-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-05-16 22:04:30.000000 python-freshworks-crm-1.0.4/setup.py
```

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/api.py` & `python-freshworks-crm-1.0.4/freshsales/v2/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,22 +210,22 @@
 
     def upsert_account(self, unique_identifier, **account_properties):
         url = '/sales_accounts/upsert'
         unique_field_name, unique_field_value = unique_identifier
         unique_identifier = {unique_field_name: unique_field_value}
         data = {
             'unique_identifier': unique_identifier,
-            'account': account_properties
+            'sales_account': account_properties
         }
         response = self._api._post(url, data=json.dumps(data))
         return Account(**response.get('sales_account', {}))
 
     def clone_account(self, account_id, **data):
         url = f'/sales_accounts/{account_id}/clone'
-        payload = {'account': data} if data else {}
+        payload = {'sales_account': data} if data else {}
         response = self._api._post(url, data=json.dumps(payload))
         return Account(**response.get('sales_account', {}))
 
     def delete_account(self, account_id):
         url = f'/sales_accounts/{account_id}'
         return self._api._delete(url)
```

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/errors.py` & `python-freshworks-crm-1.0.4/freshsales/v2/errors.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/models.py` & `python-freshworks-crm-1.0.4/freshsales/v2/models.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/conftest.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_accounts.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_appointments.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_appointments.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_contacts.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_deals.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_deals.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_documents.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_lists.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_notes.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_notes.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_products.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_products.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_sales_activities.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_sales_activities.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_selectors.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/freshsales/v2/tests/test_tasks.py` & `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/LICENSE` & `python-freshworks-crm-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/PKG-INFO` & `python-freshworks-crm-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-freshworks-crm
-Version: 1.0.3
+Version: 1.0.4
 Summary: An API wrapper for the Freshsales CRM
 Home-page: https://github.com/robertvy/python-freshworksCRM
 Author: Robert Van Ysendyck
 Author-email: rvy@vyp-consulting.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-freshworks-crm-1.0.3/python_freshworks_crm.egg-info/PKG-INFO` & `python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-freshworks-crm
-Version: 1.0.3
+Version: 1.0.4
 Summary: An API wrapper for the Freshsales CRM
 Home-page: https://github.com/robertvy/python-freshworksCRM
 Author: Robert Van Ysendyck
 Author-email: rvy@vyp-consulting.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-freshworks-crm-1.0.3/python_freshworks_crm.egg-info/SOURCES.txt` & `python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.3/setup.py` & `python-freshworks-crm-1.0.4/setup.py`

 * *Files identical despite different names*


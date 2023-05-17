# Comparing `tmp/py-bigquery-mock-0.1.9.tar.gz` & `tmp/py-bigquery-mock-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-bigquery-mock-0.1.9.tar", last modified: Tue May 16 19:51:55 2023, max compression
+gzip compressed data, was "py-bigquery-mock-0.2.0.tar", last modified: Tue May 16 20:53:07 2023, max compression
```

## Comparing `py-bigquery-mock-0.1.9.tar` & `py-bigquery-mock-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 19:51:55.118710 py-bigquery-mock-0.1.9/
--rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.1.9/LICENSE
--rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-16 19:51:55.118582 py-bigquery-mock-0.1.9/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305      458 2023-05-16 19:44:40.000000 py-bigquery-mock-0.1.9/README.md
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 19:51:55.117942 py-bigquery-mock-0.1.9/bigquery_mock/
--rw-r--r--   0 phtremblay (2028354092) 932231305       52 2023-05-16 19:46:21.000000 py-bigquery-mock-0.1.9/bigquery_mock/__init__.py
--rw-r--r--   0 phtremblay (2028354092) 932231305     2495 2023-05-16 19:24:07.000000 py-bigquery-mock-0.1.9/bigquery_mock/bigquery_mock.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 19:51:55.118419 py-bigquery-mock-0.1.9/py_bigquery_mock.egg-info/
--rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-16 19:51:55.000000 py-bigquery-mock-0.1.9/py_bigquery_mock.egg-info/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305      243 2023-05-16 19:51:55.000000 py-bigquery-mock-0.1.9/py_bigquery_mock.egg-info/SOURCES.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-16 19:51:55.000000 py-bigquery-mock-0.1.9/py_bigquery_mock.egg-info/dependency_links.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       14 2023-05-16 19:51:55.000000 py-bigquery-mock-0.1.9/py_bigquery_mock.egg-info/top_level.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-16 19:51:55.118753 py-bigquery-mock-0.1.9/setup.cfg
--rw-r--r--   0 phtremblay (2028354092) 932231305      407 2023-05-16 19:49:28.000000 py-bigquery-mock-0.1.9/setup.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 20:53:07.513156 py-bigquery-mock-0.2.0/
+-rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.2.0/LICENSE
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-16 20:53:07.513038 py-bigquery-mock-0.2.0/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305      464 2023-05-16 19:55:28.000000 py-bigquery-mock-0.2.0/README.md
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 20:53:07.512416 py-bigquery-mock-0.2.0/bigquery_mock/
+-rw-r--r--   0 phtremblay (2028354092) 932231305       52 2023-05-16 20:45:36.000000 py-bigquery-mock-0.2.0/bigquery_mock/__init__.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305     3195 2023-05-16 20:40:11.000000 py-bigquery-mock-0.2.0/bigquery_mock/bigquery_mock.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 20:53:07.512881 py-bigquery-mock-0.2.0/py_bigquery_mock.egg-info/
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-16 20:53:07.000000 py-bigquery-mock-0.2.0/py_bigquery_mock.egg-info/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305      243 2023-05-16 20:53:07.000000 py-bigquery-mock-0.2.0/py_bigquery_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-16 20:53:07.000000 py-bigquery-mock-0.2.0/py_bigquery_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       14 2023-05-16 20:53:07.000000 py-bigquery-mock-0.2.0/py_bigquery_mock.egg-info/top_level.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-16 20:53:07.513198 py-bigquery-mock-0.2.0/setup.cfg
+-rw-r--r--   0 phtremblay (2028354092) 932231305      407 2023-05-16 20:46:41.000000 py-bigquery-mock-0.2.0/setup.py
```

### Comparing `py-bigquery-mock-0.1.9/LICENSE` & `py-bigquery-mock-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-bigquery-mock-0.1.9/bigquery_mock/bigquery_mock.py` & `py-bigquery-mock-0.2.0/bigquery_mock/bigquery_mock.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,32 +51,52 @@
 
     def values(self, *args, **kwargs):
         return self._values
 
     def keys(self, *args, **kwargs):
         return self.info.keys()
 
+def get_sql_key(query):
+    for line in query.split('\n'):
+        if 'py-bigquery-mock-register:' in line:
+            fields = line.split(':')
+            if len(fields) != 2:
+                raise InvalidData('hint  should be in format "py-bigquery-mock-register: key"')
+            return fields[1].strip()
+
 class Client:
 
-    def _test_valid_data(self):
-        if not isinstance(self.data, list):
-            raise InvalidData(f'{self.data} is not a list')
+    def _test_valid_data(self, data):
+        if not isinstance(data, list):
+            raise InvalidData(f'{data} is not a list')
         errors = []
-        for n, i in enumerate(self.data):
+        for n, i in enumerate(data):
             if not isinstance(i, list):
                 errors.append((n, i, 'not a list'))
         if len(errors) != 0:
             raise InvalidData(errors)
 
     def __init__(self, data = []):
+        self._test_valid_data(data)
         self.data = data
-        self._test_valid_data()
+        self.registered_data = {}
 
-    def query(self, *args, **kwargs):
-        return RowIterator(data = self.data)
+    def register_data(self, key, data):
+        self._test_valid_data(data)
+        self.registered_data[key] = data
+
+    def query(self, query, *args, **kwargs):
+        key = get_sql_key(query)
+        if key:
+            data = self.registered_data.get(key)
+            if not data:
+                raise InvalidData(f'{key} not found in registered_data')
+        else:
+            data = self.data
+        return RowIterator(data = data)
 
     def create_table(self, table):
         return table
 
     def delete_table(self, table_id, not_found_ok=False):
         pass
```


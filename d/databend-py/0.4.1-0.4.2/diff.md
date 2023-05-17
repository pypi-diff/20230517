# Comparing `tmp/databend_py-0.4.1-py3-none-any.whl.zip` & `tmp/databend_py-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 17442 bytes, number of entries: 18
--rw-r--r--  2.0 unx      227 b- defN 23-May-13 08:52 databend_py/__init__.py
--rw-r--r--  2.0 unx    10797 b- defN 23-May-13 23:39 databend_py/client.py
+Zip file size: 17796 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      227 b- defN 23-May-17 12:48 databend_py/__init__.py
+-rw-r--r--  2.0 unx    12673 b- defN 23-May-17 12:48 databend_py/client.py
 -rw-r--r--  2.0 unx     6927 b- defN 23-May-13 23:39 databend_py/connection.py
 -rw-r--r--  2.0 unx      909 b- defN 22-Nov-07 03:45 databend_py/context.py
 -rw-r--r--  2.0 unx      931 b- defN 23-Jan-12 08:08 databend_py/datetypes.py
 -rw-r--r--  2.0 unx      184 b- defN 22-Nov-16 02:52 databend_py/defines.py
 -rw-r--r--  2.0 unx      884 b- defN 23-May-13 23:39 databend_py/errors.py
 -rw-r--r--  2.0 unx      206 b- defN 22-Nov-07 03:45 databend_py/log.py
--rw-r--r--  2.0 unx     2128 b- defN 23-Feb-13 02:21 databend_py/result.py
+-rw-r--r--  2.0 unx     2117 b- defN 23-May-17 12:48 databend_py/result.py
 -rw-r--r--  2.0 unx     1133 b- defN 23-May-13 23:39 databend_py/retry.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Nov-07 03:45 databend_py/util/__init__.py
 -rw-r--r--  2.0 unx     1452 b- defN 22-Nov-07 03:45 databend_py/util/escape.py
 -rw-r--r--  2.0 unx     2254 b- defN 22-Nov-12 09:37 databend_py/util/helper.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-13 23:39 databend_py-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3531 b- defN 23-May-13 23:39 databend_py-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-13 23:39 databend_py-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-13 23:39 databend_py-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1437 b- defN 23-May-13 23:39 databend_py-0.4.1.dist-info/RECORD
-18 files, 44461 bytes uncompressed, 15100 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-17 12:48 databend_py-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3531 b- defN 23-May-17 12:48 databend_py-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 12:48 databend_py-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-17 12:48 databend_py-0.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1437 b- defN 23-May-17 12:48 databend_py-0.4.2.dist-info/RECORD
+18 files, 46326 bytes uncompressed, 15454 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: databend_py/util/escape.py
 Comment: 
 
 Filename: databend_py/util/helper.py
 Comment: 
 
-Filename: databend_py-0.4.1.dist-info/LICENSE
+Filename: databend_py-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: databend_py-0.4.1.dist-info/METADATA
+Filename: databend_py-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: databend_py-0.4.1.dist-info/WHEEL
+Filename: databend_py-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: databend_py-0.4.1.dist-info/top_level.txt
+Filename: databend_py-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: databend_py-0.4.1.dist-info/RECORD
+Filename: databend_py-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databend_py/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .client import Client
 from .connection import Connection
 from .datetypes import DatabendDataType
 
-VERSION = (0, 4, 1)
+VERSION = (0, 4, 2)
 __version__ = '.'.join(str(x) for x in VERSION)
 
 __all__ = ['Client', 'Connection', 'DatabendDataType']
```

## databend_py/client.py

```diff
@@ -1,71 +1,77 @@
-import io
+import csv
+import json
+import os
 import re
+import requests
+import time
+import uuid
 from urllib.parse import urlparse, parse_qs, unquote
+
 from .connection import Connection
-from .util.helper import asbool, Helper
-from .util.escape import escape_params
 from .result import QueryResult
-import json, operator, csv, uuid, requests, time, os
+from .util.escape import escape_params
+from .util.helper import asbool, Helper
 
 
 class Client(object):
     """
     Client for communication with the databend http server.
     Single connection is established per each connected instance of the client.
     """
 
     def __init__(self, *args, **kwargs):
         self.settings = (kwargs.pop('settings', None) or {}).copy()
         self.connection = Connection(*args, **kwargs)
         self.query_result_cls = QueryResult
         self.helper = Helper
+        self._debug = asbool(self.settings.get('debug', False))
 
     def __enter__(self):
         return self
 
     def disconnect(self):
         self.disconnect_connection()
 
     def disconnect_connection(self):
         self.connection.disconnect()
 
-    def data_generator(self, raw_data):
+    def _data_generator(self, raw_data):
         while raw_data['next_uri'] is not None:
             try:
-                raw_data = self.receive_data(raw_data['next_uri'])
+                raw_data = self._receive_data(raw_data['next_uri'])
                 yield raw_data
             except (Exception, KeyboardInterrupt):
                 self.disconnect()
                 raise
 
-    def receive_data(self, next_uri: str):
+    def _receive_data(self, next_uri: str):
         resp = self.connection.next_page(next_uri)
         raw_data = json.loads(resp.content)
         helper = self.helper()
         helper.response = raw_data
         helper.check_error()
         return raw_data
 
-    def receive_result(self, query, query_id=None, with_column_types=False):
+    def _receive_result(self, query, query_id=None, with_column_types=False):
         raw_data = self.connection.query(query)
         helper = self.helper()
         helper.response = raw_data
         helper.check_error()
-        gen = self.data_generator(raw_data)
+        gen = self._data_generator(raw_data)
         result = self.query_result_cls(
             gen, raw_data, with_column_types=with_column_types)
         return result.get_result()
 
-    def iter_receive_result(self, query, query_id=None, with_column_types=False):
+    def _iter_receive_result(self, query, query_id=None, with_column_types=False):
         raw_data = self.connection.query(query)
         helper = self.helper()
         helper.response = raw_data
         helper.check_error()
-        gen = self.data_generator(raw_data)
+        gen = self._data_generator(raw_data)
         result = self.query_result_cls(
             gen, raw_data, with_column_types=with_column_types)
         _, rows = result.get_result()
         for row in rows:
             for r in row:
                 yield r
 
@@ -100,65 +106,66 @@
         # INSERT queries can use list/tuple/generator of list/tuples/dicts.
         # For SELECT parameters can be passed in only in dict right now.
         is_insert = isinstance(params, (list, tuple))
 
         if is_insert:
             # remove the `\n` '\s' `\t` in the SQL
             query = " ".join([s.strip() for s in query.splitlines()]).strip()
-            rv = self.process_insert_query(query, params)
+            rv = self._process_insert_query(query, params)
             return [], rv
 
-        column_types, rv = self.process_ordinary_query(
+        column_types, rv = self._process_ordinary_query(
             query, params=params, with_column_types=with_column_types,
             query_id=query_id)
         return column_types, rv
 
     # params = [(1,),(2,)] or params = [(1,2),(2,3)]
-    def process_insert_query(self, query, params):
+    def _process_insert_query(self, query, params):
         insert_rows = 0
         if "values" in query:
             query = query.split("values")[0] + 'values'
         elif "VALUES" in query:
             query = query.split("VALUES")[0] + 'VALUES'
         insert_re = re.compile("(?i)^INSERT INTO\s+\x60?([\w.^\(]+)\x60?\s*(\([^\)]*\))?")
         match = insert_re.match(query.strip())
         if len(match.group().split(' ')) < 2:
             raise Exception("Not standard insert statement")
         table_name = match[1]
 
         batch_size = query.count(',') + 1
         if params is not None:
             tuple_ls = [tuple(params[i:i + batch_size]) for i in range(0, len(params), batch_size)]
-            filename = self.generate_csv(tuple_ls)
-            csv_data = self.get_csv_data(filename)
-            self.sync_csv_file_into_table(filename, csv_data, table_name)
+            filename = self._generate_csv(tuple_ls)
+            with open(filename, "rb") as f:
+                self._sync_csv_file_into_table(f, filename, table_name, "CSV")
             insert_rows = len(tuple_ls)
+            os.remove(filename)
 
         return insert_rows
 
-    def process_ordinary_query(self, query, params=None, with_column_types=False,
-                               query_id=None):
+    def _process_ordinary_query(self, query, params=None, with_column_types=False,
+                                query_id=None):
         if params is not None:
-            query = self.substitute_params(
+            query = self._substitute_params(
                 query, params, self.connection.context
             )
-        return self.receive_result(query, query_id=query_id, with_column_types=with_column_types, )
+        return self._receive_result(query, query_id=query_id, with_column_types=with_column_types, )
 
     def execute_iter(self, query, params=None, with_column_types=False,
                      query_id=None, settings=None):
         if params is not None:
-            query = self.substitute_params(
+            query = self._substitute_params(
                 query, params, self.connection.context
             )
-        return self.iter_receive_result(query, query_id=query_id, with_column_types=with_column_types)
+        return self._iter_receive_result(query, query_id=query_id, with_column_types=with_column_types)
 
-    def iter_process_ordinary_query(self, query, with_column_types=False, query_id=None):
-        return self.iter_receive_result(query, query_id=query_id, with_column_types=with_column_types)
+    def _iter_process_ordinary_query(self, query, with_column_types=False, query_id=None):
+        return self._iter_receive_result(query, query_id=query_id, with_column_types=with_column_types)
 
-    def substitute_params(self, query, params, context):
+    def _substitute_params(self, query, params, context):
         if not isinstance(params, dict):
             raise ValueError('Parameters are expected in dict form')
 
         escaped = escape_params(params, context)
         return query % escaped
 
     @classmethod
@@ -194,14 +201,16 @@
             if name == 'client_name':
                 kwargs[name] = value
             elif name == 'secure':
                 kwargs[name] = asbool(value)
             elif name == 'copy_purge':
                 kwargs[name] = asbool(value)
                 settings[name] = asbool(value)
+            elif name == 'debug':
+                settings[name] = asbool(value)
             elif name in timeouts:
                 kwargs[name] = float(value)
             else:
                 settings[name] = value  # settings={'copy_purge':False}
         secure = kwargs.get("secure", False)
         kwargs['secure'] = secure
 
@@ -221,47 +230,86 @@
             kwargs['password'] = unquote(parsed_url.password)
 
         if settings:
             kwargs['settings'] = settings
 
         return cls(host, **kwargs)
 
-    def generate_csv(self, bindings):
-        file_name = f'{uuid.uuid4()}.csv'
+    def _generate_csv(self, bindings):
+        file_name = f'/tmp/{uuid.uuid4()}.csv'
         with open(file_name, "w+") as csvfile:
             spamwriter = csv.writer(csvfile, delimiter=',', quoting=csv.QUOTE_MINIMAL)
             spamwriter.writerows(bindings)
 
         return file_name
 
-    def get_csv_data(self, filename):
-        with open(filename, "r") as csvfile:
-            return io.StringIO(csvfile.read())
-
-    def stage_csv_file(self, filename, data):
-        stage_path = "@~/%s" % filename
+    def stage_csv_file(self, file_descriptor, file_name):
+        stage_path = "@~/%s" % file_name
+        start_presign_time = time.time()
         _, row = self.execute('presign upload %s' % stage_path)
+        if self._debug:
+            print("upload: presign file:%s duration:%ss" % (file_name, time.time() - start_presign_time))
+
         presigned_url = row[0][2]
         headers = json.loads(row[0][1])
-        resp = requests.put(presigned_url, headers=headers, data=data)
-        resp.raise_for_status()
+        start_upload_time = time.time()
+        try:
+            resp = requests.put(presigned_url, headers=headers, data=file_descriptor)
+            resp.raise_for_status()
+        finally:
+            if self._debug:
+                print("upload: put file:%s duration:%ss" % (file_name, time.time() - start_upload_time))
         return stage_path
 
-    def sync_csv_file_into_table(self, filename, data, table):
+    def _sync_csv_file_into_table(self, file_descriptor, file_name, table, file_type):
         start = time.time()
-        stage_path = self.stage_csv_file(filename, data)
-        copy_options = self.generate_copy_options()
+        stage_path = self.stage_csv_file(file_descriptor, file_name)
+        copy_options = self._generate_copy_options()
         _, _ = self.execute(
-            f"COPY INTO {table} FROM {stage_path} FILE_FORMAT = (type = CSV)\
+            f"COPY INTO {table} FROM {stage_path} FILE_FORMAT = (type = {file_type} RECORD_DELIMITER = '\r\n')\
              PURGE = {copy_options['PURGE']} FORCE = {copy_options['FORCE']}\
               SIZE_LIMIT={copy_options['SIZE_LIMIT']} ON_ERROR = {copy_options['ON_ERROR']}")
-        print("sync %s duration:%ss" % (filename, int(time.time() - start)))
-        os.remove(filename)
+        if self._debug:
+            print("upload: copy %s duration:%ss" % (file_name, int(time.time() - start)))
+
+    def upload(self, file_descriptor, file_name, table_name, file_type=None):
+        """
+        upload the file to database.table according to the file
+        filename: the filename
+        table_name: the table which write into
+        file_type: the file type, default CSV
+        """
+        if not file_type:
+            if len(file_name.split(".")) > 0:
+                file_type = file_name.split(".")[1].upper()
+            else:
+                file_type = "CSV"
+        self._sync_csv_file_into_table(file_descriptor, file_name, table_name, file_type)
+
+    def upload_to_stage(self, file_descriptor, stage_path=None, file_name=None):
+        """
+        upload the file to user stage
+        :param stage_path: target stage path
+        :param file_descriptor: open file handler
+        :param file_name:
+        :return:
+        """
+        if stage_path is None:
+            stage_path = "~"
+        if file_name is None:
+            file_name = f'{uuid.uuid4()}'
+        stage_path = f"@{stage_path}/{file_name}"
+        _, row = self.execute('presign upload %s' % stage_path)
+        presigned_url = row[0][2]
+        headers = json.loads(row[0][1])
+        resp = requests.put(presigned_url, headers=headers, data=file_descriptor)
+        resp.raise_for_status()
+        return stage_path
 
-    def generate_copy_options(self):
+    def _generate_copy_options(self):
         # copy options docs: https://databend.rs/doc/sql-commands/dml/dml-copy-into-table#copyoptions
         copy_options = {}
         if "copy_purge" in self.settings:
             copy_options["PURGE"] = self.settings["copy_purge"]
         else:
             copy_options["PURGE"] = False
```

## databend_py/result.py

```diff
@@ -1,8 +1,7 @@
-import ast
 from .datetypes import DatabendDataType
 import re
 
 
 class QueryResult(object):
     """
     Stores query result from multiple response data.
```

## Comparing `databend_py-0.4.1.dist-info/LICENSE` & `databend_py-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `databend_py-0.4.1.dist-info/METADATA` & `databend_py-0.4.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-py
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python driver with native interface for Databend
 Home-page: https://github.com/databendcloud/databend-py
 Author: Databend Cloud Team
 Author-email: hantmac@outlook.com
 License: Apache License
 Keywords: databend db database cloud analytics
 Classifier: Development Status :: 4 - Beta
```

## Comparing `databend_py-0.4.1.dist-info/RECORD` & `databend_py-0.4.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-databend_py/__init__.py,sha256=_ZDovDFCdkUaFcLPcadXt6q2yvljnXGmNQY_XZ7G4t0,227
-databend_py/client.py,sha256=DlNZcI5jUjV5KOlx5kF9DjQ4NNT_qd40pGw8zxIYYDQ,10797
+databend_py/__init__.py,sha256=bgTD6P2OftE-qz5KI3x3q7KcZFKugu-Vp4fmxgTvtcM,227
+databend_py/client.py,sha256=mt7_9Z8F1dkuM_CwYjT37aoJsTWRFm-K2dhefZ-nmwI,12673
 databend_py/connection.py,sha256=90u06LUJS8216pWVqX2UcHAT24f7Dx_aOKlh_7fhPF4,6927
 databend_py/context.py,sha256=yPkJ_BN4LGODvKCOjNlDGqABwxAMQTQl7w1vIGRPBDg,909
 databend_py/datetypes.py,sha256=Yl5ZS_C5oPfyOcE2xTQNtxgPZnxnMKIc_lYSmEnFJdg,931
 databend_py/defines.py,sha256=eQOK22KSKfcBukcD4oHsmlgpXFms92ew0ORxWNnxxH0,184
 databend_py/errors.py,sha256=-4WBvTF0OvggCa9pJEWeU02BDX-IVDx6e5hGZWjH2GI,884
 databend_py/log.py,sha256=dMuMaWptI_nexWDZMtZaAnoEOluIfYWNdoR9OSAhgKM,206
-databend_py/result.py,sha256=Ru1FwwMtbbT5E2Iesv9d6fGZeL8pFJ0lG0vA3bLN3m8,2128
+databend_py/result.py,sha256=Zx6f_bz7CS0HDOx-wpi5GY-HQwLRkenpobnw0bkzNqo,2117
 databend_py/retry.py,sha256=c-kNYxqgnD30U23Xy-yHVeBp0wItsatkxql2O1rkWNE,1133
 databend_py/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databend_py/util/escape.py,sha256=DE7PaShERoOw285fkg3pu7T_oMU4_2dMkHbjXEqPcn4,1452
 databend_py/util/helper.py,sha256=0r1d3CeNtMLdTPN_v8yW-GjjpjHVneIJJKKGdTioOoE,2254
-databend_py-0.4.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-databend_py-0.4.1.dist-info/METADATA,sha256=BuJD3cgEL7pmLwmN5N_nNdafaktJpJGsw4HHNbuDVws,3531
-databend_py-0.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-databend_py-0.4.1.dist-info/top_level.txt,sha256=t0rUVwHfEpXcuMreSkL69rc5DWv6FmzB4AfEGcc4_7U,12
-databend_py-0.4.1.dist-info/RECORD,,
+databend_py-0.4.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+databend_py-0.4.2.dist-info/METADATA,sha256=fEZwHCIt0fwFaTwg6qKSvKdsXsG5R3jx2RkbkTY7rZM,3531
+databend_py-0.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+databend_py-0.4.2.dist-info/top_level.txt,sha256=t0rUVwHfEpXcuMreSkL69rc5DWv6FmzB4AfEGcc4_7U,12
+databend_py-0.4.2.dist-info/RECORD,,
```


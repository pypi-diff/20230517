# Comparing `tmp/pg_bulk_ingest-0.0.6.tar.gz` & `tmp/pg_bulk_ingest-0.0.7.tar.gz`

## Comparing `pg_bulk_ingest-0.0.6.tar` & `pg_bulk_ingest-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/pg_bulk_ingest.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/LICENSE
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/pg_bulk_ingest.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/PKG-INFO
```

### Comparing `pg_bulk_ingest-0.0.6/pg_bulk_ingest.py` & `pg_bulk_ingest-0.0.7/pg_bulk_ingest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import uuid
 
 import sqlalchemy as sa
 import json
 from io import IOBase
 
+
 try:
     from psycopg2 import sql as sql2
 except ImportError:
     sql2 = None
 
 try:
     from psycopg import sql as sql3
@@ -186,7 +187,24 @@
             CREATE SCHEMA IF NOT EXISTS {}
         ''', table.schema))
     metadata.create_all(conn)
 
     # Insert rows into just the first table
     csv_copy(sql, conn, first_table, rows, copy_from_stdin)
 
+
+def replace(conn, metadata, rows):
+    sql, copy_from_stdin = _sql_and_copy_from_stdin(conn.engine.driver)
+
+    first_table = next(iter(metadata.tables.values()))
+
+    # Create the tables
+    for table in metadata.tables.values():
+        conn.execute(_bind_identifiers(sql, conn, '''
+            CREATE SCHEMA IF NOT EXISTS {}
+        ''', table.schema))
+    metadata.create_all(conn)
+    conn.execute(sa.delete(first_table))
+
+
+    # Insert rows into just the first table
+    csv_copy(sql, conn, first_table, rows, copy_from_stdin)
```

### Comparing `pg_bulk_ingest-0.0.6/.gitignore` & `pg_bulk_ingest-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.6/LICENSE` & `pg_bulk_ingest-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.6/README.md` & `pg_bulk_ingest-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.6/pyproject.toml` & `pg_bulk_ingest-0.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-bulk-ingest"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_bulk_ingest-0.0.6/PKG-INFO` & `pg_bulk_ingest-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-bulk-ingest
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking
 Project-URL: Source, https://github.com/uktrade/pg-bulk-ingest
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

